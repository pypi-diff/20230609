# Comparing `tmp/philbot_voice-1.8.6.tar.gz` & `tmp/philbot_voice-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.8.6.tar", max compression
+gzip compressed data, was "philbot_voice-1.8.7.tar", max compression
```

## Comparing `philbot_voice-1.8.6.tar` & `philbot_voice-1.8.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-09 11:52:54.471182 philbot_voice-1.8.6/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-09 11:52:54.471182 philbot_voice-1.8.6/philbot-voice/__main__.py
--rw-r--r--   0        0        0    37928 2023-06-09 11:52:54.471182 philbot_voice-1.8.6/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-09 11:52:54.471182 philbot_voice-1.8.6/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.8.6/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-09 17:17:48.917405 philbot_voice-1.8.7/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-09 17:17:48.917405 philbot_voice-1.8.7/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    38014 2023-06-09 17:17:48.917405 philbot_voice-1.8.7/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-09 17:17:48.917405 philbot_voice-1.8.7/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.8.7/PKG-INFO
```

### Comparing `philbot_voice-1.8.6/philbot-voice/voice.py` & `philbot_voice-1.8.7/philbot-voice/voice.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,19 +253,19 @@
     def __listen(self):
         print('VOICE CONNECTION ' + self.guild_id + ' listening')
         frame_duration = 20
         frame_rate = 48000
         sample_width = 2
         channels = 2
         desired_frame_size = int(frame_rate * frame_duration / 1000)
-        buffer = b"\x00" * 1024 * 1024
+        buffer = b"\x00" * desired_frame_size * desired_frame_size * channels * sample_width
         secret_box = nacl.secret.SecretBox(bytes(self.secret_key))
         error = ctypes.c_int(0)
         decoder = pyogg.opus.opus_decoder_create(pyogg.opus.opus_int32(frame_rate), ctypes.c_int(channels), ctypes.byref(error))
-        file = wave.open(STORAGE_DIRECTORY + './output.' + self.guild_id + '.wav', 'wb')
+        file = wave.open(STORAGE_DIRECTORY + '/output.' + self.guild_id + '.wav', 'wb')
         file.setnchannels(channels)
         file.setsampwidth(sample_width)
         file.setframerate(frame_rate)
         last_sequence = -1
         while True:
             with self.lock:
                 if not self.listener:
@@ -310,15 +310,15 @@
         print('VOICE CONNECTION ' + self.guild_id + ' streaming')
 
         frame_duration = 20
         frame_rate = 48000
         sample_width = 2
         channels = 2
         desired_frame_size = int(frame_rate * frame_duration / 1000)
-        buffer = b"\x00" * 1024 * 1024
+        buffer = b"\x00" * desired_frame_size * channels * sample_width
         secret_box = nacl.secret.SecretBox(bytes(self.secret_key))
         error = ctypes.c_int(0)
         encoder = pyogg.opus.opus_encoder_create(pyogg.opus.opus_int32(frame_rate), ctypes.c_int(channels), ctypes.c_int(pyogg.opus.OPUS_APPLICATION_AUDIO), ctypes.byref(error))
         if error.value != 0:
             raise RuntimeError(str(error.value))
         if self.mode != "xsalsa20_poly1305":
             raise RuntimeError('unexpected mode: ' + self.mode)
```

### Comparing `philbot_voice-1.8.6/pyproject.toml` & `philbot_voice-1.8.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.8.6"
+version = "1.8.7"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.8.6/PKG-INFO` & `philbot_voice-1.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.8.6
+Version: 1.8.7
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

