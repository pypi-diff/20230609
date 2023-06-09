# Comparing `tmp/philbot_voice-1.8.5.tar.gz` & `tmp/philbot_voice-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.8.5.tar", max compression
+gzip compressed data, was "philbot_voice-1.8.6.tar", max compression
```

## Comparing `philbot_voice-1.8.5.tar` & `philbot_voice-1.8.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-08 10:45:43.747449 philbot_voice-1.8.5/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-08 10:45:43.747449 philbot_voice-1.8.5/philbot-voice/__main__.py
--rw-r--r--   0        0        0    34459 2023-06-08 10:45:43.751450 philbot_voice-1.8.5/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-08 10:45:43.751450 philbot_voice-1.8.5/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.8.5/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-09 11:52:54.471182 philbot_voice-1.8.6/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-09 11:52:54.471182 philbot_voice-1.8.6/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    37928 2023-06-09 11:52:54.471182 philbot_voice-1.8.6/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-09 11:52:54.471182 philbot_voice-1.8.6/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.8.6/PKG-INFO
```

### Comparing `philbot_voice-1.8.5/philbot-voice/voice.py` & `philbot_voice-1.8.6/philbot-voice/voice.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,14 +83,21 @@
 
 def create_voice_package(sequence, timestamp, ssrc, secret_box, voice_chunk):
     header = create_voice_package_header(sequence, timestamp, ssrc)
     nonce = bytearray(24)
     nonce[:12] = header
     return header + secret_box.encrypt(voice_chunk, bytes(nonce)).ciphertext
 
+def unwrap_voice_package(package, secret_box):
+    header = package[:12]
+    nonce = bytearray(24)
+    nonce[:12] = header
+    voice_chunk = secret_box.decrypt(package[12:], bytes(nonce))
+    return voice_chunk, struct.unpack_from('>H', header, 2)[0], struct.unpack_from('>I', header, 4)[0]
+
 download_lock = threading.Lock()
 downloads = {}
 
 def download_from_youtube(guild_id, url):
     codec = 'wav'
     filename = url[url.index('v=') + 2:]
     if '&' in filename:
@@ -220,27 +227,14 @@
                         'paused': self.paused
                     }))
             else:
                 try:
                     os.remove(filename)
                 except:
                     pass
-
-    def __listen(self):
-        print('VOICE CONNECTION ' + self.guild_id + ' listening')
-        while True:
-            with self.lock:
-                if not self.listener:
-                    break
-            try:
-                data, address = self.socket.recvfrom(UDP_MAX_PAYLOAD)
-                # print('VOICE CONNECTION received voice data package from ' + address[0] + ':' + str(address[1]) + ': ' + str(len(data)) + 'b')
-            except: # TODO limit to socket closed exceptions only
-                pass
-        print('VOICE CONNECTION ' + self.guild_id + ' listener terminated')
     
     def __callback(self, reason):
         delay = 1
         while True:
             if delay > 60 * 60:
                 break
             try:
@@ -252,33 +246,82 @@
 
     def __callback_playback_finished(self):
         self.__callback('voice_playback_finished')
 
     def __callback_reconnect(self):
         self.__callback('voice_reconnect')
 
+    def __listen(self):
+        print('VOICE CONNECTION ' + self.guild_id + ' listening')
+        frame_duration = 20
+        frame_rate = 48000
+        sample_width = 2
+        channels = 2
+        desired_frame_size = int(frame_rate * frame_duration / 1000)
+        buffer = b"\x00" * 1024 * 1024
+        secret_box = nacl.secret.SecretBox(bytes(self.secret_key))
+        error = ctypes.c_int(0)
+        decoder = pyogg.opus.opus_decoder_create(pyogg.opus.opus_int32(frame_rate), ctypes.c_int(channels), ctypes.byref(error))
+        file = wave.open(STORAGE_DIRECTORY + './output.' + self.guild_id + '.wav', 'wb')
+        file.setnchannels(channels)
+        file.setsampwidth(sample_width)
+        file.setframerate(frame_rate)
+        last_sequence = -1
+        while True:
+            with self.lock:
+                if not self.listener:
+                    break
+            package = None
+            try:
+                package, address = self.socket.recvfrom(UDP_MAX_PAYLOAD)
+            except: # TODO limit to socket closed exceptions only
+                continue
+            # print('VOICE CONNECTION received voice data package from ' + address[0] + ':' + str(address[1]) + ': ' + str(len(data)) + 'b')
+            voice_chunk = None
+            sequence = None
+            timestamp = None
+            try:
+                voice_chunk, sequence, timestamp = unwrap_voice_package(package, secret_box)
+            except: # TODO limit to wrong encryption (received random package)
+                continue
+            # TODO in all the following cases, handle and resort properly
+            if last_sequence < 0:
+                last_sequence = sequence - 1
+            if last_sequence + 1 < sequence:
+                while last_sequence + 1 != sequence:
+                    file.writeframes(b"\x00" * desired_frame_size * sample_width * channels)
+                    last_sequence += 1
+            elif last_sequence > sequence:
+                continue
+            last_sequence = sequence
+            effective_frame_size = pyogg.opus.opus_decode(decoder, ctypes.cast(voice_chunk, pyogg.opus.c_uchar_p), pyogg.opus.opus_int32(len(voice_chunk)), ctypes.cast(buffer, pyogg.opus.opus_int16_p), ctypes.c_int(len(buffer) // channels // sample_width), ctypes.c_int(0))
+            if effective_frame_size < 0:
+                effective_frame_size = 0
+            pcm = buffer[:effective_frame_size * sample_width * channels]
+            if effective_frame_size < desired_frame_size:
+                pcm += b"\x00" * (desired_frame_size - effective_frame_size) * sample_width * channels
+            file.writeframes(pcm)
+        file.close()
+        pyogg.opus.opus_decoder_destroy(decoder)
+        print('VOICE CONNECTION ' + self.guild_id + ' listener terminated')
+
     def __stream(self):
         # https://discord.com/developers/docs/topics/voice-connections#encrypting-and-sending-voice
         # https://github.com/Rapptz/discord.py/blob/master/discord/voice_client.py
         print('VOICE CONNECTION ' + self.guild_id + ' streaming')
 
         frame_duration = 20
         frame_rate = 48000
         sample_width = 2
         channels = 2
         desired_frame_size = int(frame_rate * frame_duration / 1000)
         buffer = b"\x00" * 1024 * 1024
         secret_box = nacl.secret.SecretBox(bytes(self.secret_key))
         error = ctypes.c_int(0)
-        encoder = pyogg.opus.opus_encoder_create(
-            pyogg.opus.opus_int32(frame_rate),
-            ctypes.c_int(channels),
-            ctypes.c_int(pyogg.opus.OPUS_APPLICATION_AUDIO),
-            ctypes.byref(error)
-        )
+        encoder = pyogg.opus.opus_encoder_create(pyogg.opus.opus_int32(frame_rate), ctypes.c_int(channels), ctypes.c_int(pyogg.opus.OPUS_APPLICATION_AUDIO), ctypes.byref(error))
         if error.value != 0:
             raise RuntimeError(str(error.value))
         if self.mode != "xsalsa20_poly1305":
             raise RuntimeError('unexpected mode: ' + self.mode)
 
         sequence = 0
         filename = None
@@ -343,18 +386,26 @@
                 pcm = file.readframes(desired_frame_size)
                 if len(pcm) == 0:
                     with self.lock:
                         self.url = None
                 effective_frame_size = len(pcm) // sample_width // channels
                 if effective_frame_size < desired_frame_size:
                     pcm += b"\x00" * (desired_frame_size - effective_frame_size) * sample_width * channels
-                encoded_bytes = pyogg.opus.opus_encode(encoder, ctypes.cast(pcm, pyogg.opus.opus_int16_p), ctypes.c_int(effective_frame_size), ctypes.cast(buffer, pyogg.opus.c_uchar_p), pyogg.opus.opus_int32(len(buffer)))
+                encoded_bytes = pyogg.opus.opus_encode(encoder, ctypes.cast(pcm, pyogg.opus.opus_int16_p), ctypes.c_int(desired_frame_size), ctypes.cast(buffer, pyogg.opus.c_uchar_p), pyogg.opus.opus_int32(len(buffer)))
                 opus_frame = bytes(buffer[:encoded_bytes])
+                ####################
+                #decoder = pyogg.opus.opus_decoder_create(pyogg.opus.opus_int32(frame_rate), ctypes.c_int(channels), ctypes.byref(error))
+                #effective_frame_size = pyogg.opus.opus_decode(decoder, ctypes.cast(opus_frame, pyogg.opus.c_uchar_p), pyogg.opus.opus_int32(len(opus_frame)), ctypes.cast(buffer, pyogg.opus.opus_int16_p), ctypes.c_int(len(buffer) // channels // sample_width), ctypes.c_int(0))
+                #pcm_reconstructed = buffer[:effective_frame_size]
+                #pyogg.opus.opus_decoder_destroy(decoder)
+                #encoded_bytes = pyogg.opus.opus_encode(encoder, ctypes.cast(pcm_reconstructed, pyogg.opus.opus_int16_p), ctypes.c_int(desired_frame_size), ctypes.cast(buffer, pyogg.opus.c_uchar_p), pyogg.opus.opus_int32(len(buffer)))
+                #opus_frame = bytes(buffer[:encoded_bytes])
+                ####################
             else:
-                opus_frame = b"\x00" * desired_frame_size * sample_width * channels
+                opus_frame = b"\xF8\xFF\xFE"
             # send a frame
             package = create_voice_package(sequence, sequence * desired_frame_size, self.ssrc, secret_box, opus_frame)
             sequence += 1
             try:
                 self.socket.sendto(package, (self.ip, self.port))
             except: # TODO limit to socket close exceptions only
                 pass
@@ -380,14 +431,15 @@
             if sleep_time < 0:
                 # we are behind, what to do?
                 pass
             elif sleep_time == 0:
                 pass
             else:
                 time.sleep(sleep_time / 1000.0 * 2) # I have no fucking idea why multiplying this by two results in a clean audio stream!!! (times two is actually just a tad too slow, but not noticable by humans)
+                # current theory is that above when calculating effective and desired frame rates, we miss in some places a "divide by 2", reason is that we seem to pass the length in bytes, but as a short pointer. thats inconcistent
             timestamp = new_timestamp
 
         if filename:
             file.close()
             try:
                 os.remove(filename)
             except:
@@ -438,17 +490,14 @@
                     while not my_port:
                         try:
                             my_port = random.randint(UDP_PORT_MIN, UDP_PORT_MAX)
                             self.socket.bind(('0.0.0.0', my_port))
                             break
                         except:
                             my_port = None
-                    print('VOICE CONNECTION ' + self.guild_id + ' server ready at ' + my_ip + ':' + str(my_port))
-                    self.listener = threading.Thread(target=self.__listen)
-                    self.listener.start()
                     print('VOICE GATEWAY ' + self.guild_id + ' sending select protocol')
                     ws.send(json.dumps({
                         "op": 1,
                         "d": {
                             "protocol": "udp",
                             "data": {
                                 "address": my_ip,
@@ -457,14 +506,17 @@
                             }
                         }
                     }))
                 case 4:
                     print('VOICE GATEWAY ' + self.guild_id + ' received session description')
                     self.mode = payload['d']['mode']
                     self.secret_key = payload['d']['secret_key']
+                    print('VOICE CONNECTION ' + self.guild_id + ' server ready')
+                    self.listener = threading.Thread(target=self.__listen)
+                    self.listener.start()
                     print('VOICE GATEWAY ' + self.guild_id + ' sending speaking')
                     ws.send(json.dumps({
                         "op": 5,
                         "d": {
                             "speaking": 1,
                             "delay": 0,
                             "ssrc": self.ssrc
@@ -569,15 +621,15 @@
             case _: # something else
                 self.__stop()
                 time.sleep(5)
                 self.__try_start()
     
     def __try_start(self):
         with self.lock:
-            if self.ws or not self.channel_id or not self.session_id or not self.endpoint or not self.token or not self.url:
+            if self.ws or not self.channel_id or not self.session_id or not self.endpoint or not self.token:
                 return
             print('VOICE GATEWAY ' + self.guild_id + ' connection starting')
             self.ws = websocket.WebSocketApp(self.endpoint + '?v=4', on_open=self.__ws_on_open, on_message=self.__ws_on_message, on_error=self.__ws_on_error, on_close=self.__ws_on_close)
             threading.Thread(target=self.ws.run_forever).start()
     
     def __stop(self):
         listener = None
```

### Comparing `philbot_voice-1.8.5/pyproject.toml` & `philbot_voice-1.8.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.8.5"
+version = "1.8.6"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.8.5/PKG-INFO` & `philbot_voice-1.8.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.8.5
+Version: 1.8.6
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

