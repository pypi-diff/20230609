# Comparing `tmp/djitellopy-2.4.0.tar.gz` & `tmp/djitellopy-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djitellopy-2.4.0.tar", last modified: Sun Sep  5 12:30:29 2021, max compression
+gzip compressed data, was "djitellopy-2.5.0.tar", last modified: Fri Jun  9 16:29:13 2023, max compression
```

## Comparing `djitellopy-2.4.0.tar` & `djitellopy-2.5.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2021-09-05 12:30:29.000000 djitellopy-2.4.0/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     4472 2021-09-05 12:30:29.000000 djitellopy-2.4.0/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2581 2021-06-06 21:28:41.000000 djitellopy-2.4.0/README.md
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2021-09-05 12:30:29.000000 djitellopy-2.4.0/djitellopy/
--rw-r--r--   0 jakob     (1000) jakob     (1000)       75 2020-03-31 10:03:36.000000 djitellopy-2.4.0/djitellopy/__init__.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2255 2021-02-28 10:42:06.000000 djitellopy-2.4.0/djitellopy/enforce_types.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     4255 2021-01-30 00:10:23.000000 djitellopy-2.4.0/djitellopy/swarm.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    35999 2021-09-05 12:20:13.000000 djitellopy-2.4.0/djitellopy/tello.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2021-09-05 12:30:29.000000 djitellopy-2.4.0/djitellopy.egg-info/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     4472 2021-09-05 12:30:29.000000 djitellopy-2.4.0/djitellopy.egg-info/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)      288 2021-09-05 12:30:29.000000 djitellopy-2.4.0/djitellopy.egg-info/SOURCES.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2021-09-05 12:30:29.000000 djitellopy-2.4.0/djitellopy.egg-info/dependency_links.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       20 2021-09-05 12:30:29.000000 djitellopy-2.4.0/djitellopy.egg-info/requires.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       11 2021-09-05 12:30:29.000000 djitellopy-2.4.0/djitellopy.egg-info/top_level.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       79 2021-09-05 12:30:29.000000 djitellopy-2.4.0/setup.cfg
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1464 2021-09-05 12:26:11.000000 djitellopy-2.4.0/setup.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-06-09 16:29:13.160699 djitellopy-2.5.0/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1079 2021-11-13 16:10:23.000000 djitellopy-2.5.0/LICENSE.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     5146 2023-06-09 16:29:13.160699 djitellopy-2.5.0/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3766 2022-09-23 23:41:09.000000 djitellopy-2.5.0/README.md
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-06-09 16:29:13.160699 djitellopy-2.5.0/djitellopy/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       91 2021-12-27 00:26:55.000000 djitellopy-2.5.0/djitellopy/__init__.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2255 2021-11-13 16:10:23.000000 djitellopy-2.5.0/djitellopy/enforce_types.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     4275 2021-12-27 00:27:43.000000 djitellopy-2.5.0/djitellopy/swarm.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    37008 2023-06-09 16:10:22.000000 djitellopy-2.5.0/djitellopy/tello.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-06-09 16:29:13.160699 djitellopy-2.5.0/djitellopy.egg-info/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     5146 2023-06-09 16:29:13.000000 djitellopy-2.5.0/djitellopy.egg-info/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      300 2023-06-09 16:29:13.000000 djitellopy-2.5.0/djitellopy.egg-info/SOURCES.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-06-09 16:29:13.000000 djitellopy-2.5.0/djitellopy.egg-info/dependency_links.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       30 2023-06-09 16:29:13.000000 djitellopy-2.5.0/djitellopy.egg-info/requires.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       11 2023-06-09 16:29:13.000000 djitellopy-2.5.0/djitellopy.egg-info/top_level.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       79 2023-06-09 16:29:13.160699 djitellopy-2.5.0/setup.cfg
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1595 2023-06-09 16:27:02.000000 djitellopy-2.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djitellopy-2.4.0/djitellopy/enforce_types.py` & `djitellopy-2.5.0/djitellopy/enforce_types.py`

 * *Files identical despite different names*

### Comparing `djitellopy-2.4.0/djitellopy/swarm.py` & `djitellopy-2.5.0/djitellopy/swarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Library for controlling multiple DJI Ryze Tello drones.
 """
 
 from threading import Thread, Barrier
 from queue import Queue
 from typing import List, Callable
 
-from .tello import Tello
+from .tello import Tello, TelloException
 from .enforce_types import enforce_types
 
 
 @enforce_types
 class TelloSwarm:
     """Swarm library for controlling multiple Tellos simultaneously
     """
@@ -36,15 +36,15 @@
     def fromIps(ips: list):
         """Create TelloSwarm from a list of IP addresses.
 
         Arguments:
             ips: list of IP Addresses
         """
         if not ips:
-            raise ValueError("No ips provided")
+            raise TelloException("No ips provided")
 
         tellos = []
         for ip in ips:
             tellos.append(Tello(ip.strip()))
 
         return TelloSwarm(tellos)
```

### Comparing `djitellopy-2.4.0/djitellopy/tello.py` & `djitellopy-2.5.0/djitellopy/tello.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 """Library for interacting with DJI Ryze Tello drones.
 """
 
 # coding=utf-8
 import logging
 import socket
 import time
-from threading import Thread
+from collections import deque
+from threading import Thread, Lock
 from typing import Optional, Union, Type, Dict
 
-import cv2 # type: ignore
 from .enforce_types import enforce_types
 
+import av
+import numpy as np
+
 
 threads_initialized = False
 drones: Optional[dict] = {}
 client_socket: socket.socket
 
 
+class TelloException(Exception):
+    pass
+
+
 @enforce_types
 class Tello:
     """Python wrapper to interact with the Ryze Tello drone using the official Tello api.
     Tello API documentation:
     [1.3](https://dl-cdn.ryzerobotics.com/downloads/tello/20180910/Tello%20SDK%20Documentation%20EN_1.3.pdf),
     [2.0 with EDU-only commands](https://dl-cdn.ryzerobotics.com/downloads/Tello/Tello%20SDK%202.0%20User%20Guide.pdf)
     """
     # Send and receive commands, client socket
     RESPONSE_TIMEOUT = 7  # in seconds
     TAKEOFF_TIMEOUT = 20  # in seconds
-    FRAME_GRAB_TIMEOUT = 3
+    FRAME_GRAB_TIMEOUT = 5
     TIME_BTW_COMMANDS = 0.1  # in seconds
     TIME_BTW_RC_CONTROL_COMMANDS = 0.001  # in seconds
     RETRY_COUNT = 3  # number of retries after a failed command
     TELLO_IP = '192.168.10.1'  # Tello IP address
 
     # Video stream, server socket
     VS_UDP_IP = '0.0.0.0'
@@ -80,36 +87,36 @@
     FLOAT_STATE_FIELDS = ('baro', 'agx', 'agy', 'agz')
 
     state_field_converters: Dict[str, Union[Type[int], Type[float]]]
     state_field_converters = {key : int for key in INT_STATE_FIELDS}
     state_field_converters.update({key : float for key in FLOAT_STATE_FIELDS})
 
     # VideoCapture object
-    cap: Optional[cv2.VideoCapture] = None
     background_frame_read: Optional['BackgroundFrameRead'] = None
 
     stream_on = False
     is_flying = False
 
     def __init__(self,
                  host=TELLO_IP,
-                 retry_count=RETRY_COUNT):
+                 retry_count=RETRY_COUNT,
+                 vs_udp=VS_UDP_PORT):
 
         global threads_initialized, client_socket, drones
 
         self.address = (host, Tello.CONTROL_UDP_PORT)
         self.stream_on = False
         self.retry_count = retry_count
         self.last_received_command_timestamp = time.time()
         self.last_rc_control_timestamp = time.time()
 
         if not threads_initialized:
             # Run Tello command responses UDP receiver on background
             client_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-            client_socket.bind(('', Tello.CONTROL_UDP_PORT))
+            client_socket.bind(("", Tello.CONTROL_UDP_PORT))
             response_receiver_thread = Thread(target=Tello.udp_response_receiver)
             response_receiver_thread.daemon = True
             response_receiver_thread.start()
 
             # Run state UDP receiver on background
             state_receiver_thread = Thread(target=Tello.udp_state_receiver)
             state_receiver_thread.daemon = True
@@ -117,14 +124,23 @@
 
             threads_initialized = True
 
         drones[host] = {'responses': [], 'state': {}}
 
         self.LOGGER.info("Tello instance was initialized. Host: '{}'. Port: '{}'.".format(host, Tello.CONTROL_UDP_PORT))
 
+        self.vs_udp_port = vs_udp
+
+
+    def change_vs_udp(self, udp_port):
+        """Change the UDP Port for sending video feed from the drone.
+        """
+        self.vs_udp_port = udp_port
+        self.send_control_command(f'port 8890 {self.vs_udp_port}')
+
     def get_own_udp_object(self):
         """Get own object from the global drones dict. This object is filled
         with responses and state information by the receiver threads.
         Internal method, you normally wouldn't call this yourself.
         """
         global drones
 
@@ -226,15 +242,15 @@
         Internal method, you normally wouldn't call this yourself.
         """
         state = self.get_current_state()
 
         if key in state:
             return state[key]
         else:
-            raise Exception('Could not get state property: {}'.format(key))
+            raise TelloException('Could not get state property: {}'.format(key))
 
     def get_mission_pad_id(self) -> int:
         """Mission pad ID of the currently detected mission pad
         Only available on Tello EDUs after calling enable_mission_pads
         Returns:
             int: -1 if none is detected, else 1-8
         """
@@ -387,41 +403,26 @@
         """
         return self.get_state_field('bat')
 
     def get_udp_video_address(self) -> str:
         """Internal method, you normally wouldn't call this youself.
         """
         address_schema = 'udp://@{ip}:{port}'  # + '?overrun_nonfatal=1&fifo_size=5000'
-        address = address_schema.format(ip=self.VS_UDP_IP, port=self.VS_UDP_PORT)
+        address = address_schema.format(ip=self.VS_UDP_IP, port=self.vs_udp_port)
         return address
 
-    def get_video_capture(self):
-        """Get the VideoCapture object from the camera drone.
-        Users usually want to use get_frame_read instead.
-        Returns:
-            VideoCapture
-        """
-
-        if self.cap is None:
-            self.cap = cv2.VideoCapture(self.get_udp_video_address())
-
-        if not self.cap.isOpened():
-            self.cap.open(self.get_udp_video_address())
-
-        return self.cap
-
-    def get_frame_read(self) -> 'BackgroundFrameRead':
+    def get_frame_read(self, with_queue = False, max_queue_len = 32) -> 'BackgroundFrameRead':
         """Get the BackgroundFrameRead object from the camera drone. Then, you just need to call
         backgroundFrameRead.frame to get the actual frame received by the drone.
         Returns:
             BackgroundFrameRead
         """
         if self.background_frame_read is None:
             address = self.get_udp_video_address()
-            self.background_frame_read = BackgroundFrameRead(self, address)  # also sets self.cap
+            self.background_frame_read = BackgroundFrameRead(self, address, with_queue, max_queue_len)
             self.background_frame_read.start()
         return self.background_frame_read
 
     def send_command_with_return(self, command: str, timeout: int = RESPONSE_TIMEOUT) -> str:
         """Send command to Tello and wait for its response.
         Internal method, you normally wouldn't call this yourself.
         Return:
@@ -521,16 +522,16 @@
         return float(response)
 
     def raise_result_error(self, command: str, response: str) -> bool:
         """Used to reaise an error after an unsuccessful command
         Internal method, you normally wouldn't call this yourself.
         """
         tries = 1 + self.retry_count
-        raise Exception("Command '{}' was unsuccessful for {} tries. Latest response:\t'{}'"
-                        .format(command, tries, response))
+        raise TelloException("Command '{}' was unsuccessful for {} tries. Latest response:\t'{}'"
+                             .format(command, tries, response))
 
     def connect(self, wait_for_state=True):
         """Enter SDK mode. Call this before any of the control functions.
         """
         self.send_control_command("command")
 
         if wait_for_state:
@@ -539,15 +540,15 @@
                 if self.get_current_state():
                     t = i / REPS  # in seconds
                     Tello.LOGGER.debug("'.connect()' received first state packet after {} seconds".format(t))
                     break
                 time.sleep(1 / REPS)
 
             if not self.get_current_state():
-                raise Exception('Did not receive a state packet from the Tello')
+                raise TelloException('Did not receive a state packet from the Tello')
 
     def send_keepalive(self):
         """Send a keepalive packet to prevent the drone from landing after 15s
         """
         self.send_control_command("keepalive")
 
     def turn_motor_on(self):
@@ -560,14 +561,15 @@
         """
         self.send_control_command("motoroff")
 
     def initiate_throw_takeoff(self):
         """Allows you to take off by throwing your drone within 5 seconds of this command
         """
         self.send_control_command("throwfly")
+        self.is_flying = True
 
     def takeoff(self):
         """Automatic takeoff.
         """
         # Something it takes a looooot of time to take off and return a succesful takeoff.
         # So we better wait. Otherwise, it would give us an error on the following calls.
         self.send_control_command("takeoff", timeout=Tello.TAKEOFF_TIMEOUT)
@@ -595,18 +597,23 @@
 
     def streamoff(self):
         """Turn off video streaming.
         """
         self.send_control_command("streamoff")
         self.stream_on = False
 
+        if self.background_frame_read is not None:
+            self.background_frame_read.stop()
+            self.background_frame_read = None
+
     def emergency(self):
         """Stop all motors immediately.
         """
-        self.send_control_command("emergency")
+        self.send_command_without_return("emergency")
+        self.is_flying = False
 
     def move(self, direction: str, x: int):
         """Tello fly up, down, left, right, forward or back with distance x cm.
         Users would normally call one of the move_x functions instead.
         Arguments:
             direction: up, down, left, right, forward or back
             x: 20-500
@@ -998,77 +1005,105 @@
             str
         """
         return self.send_read_command('active?')
 
     def end(self):
         """Call this method when you want to end the tello object
         """
-        if self.is_flying:
-            self.land()
-        if self.stream_on:
-            self.streamoff()
+        try:
+            if self.is_flying:
+                self.land()
+            if self.stream_on:
+                self.streamoff()
+        except TelloException:
+            pass
+
         if self.background_frame_read is not None:
             self.background_frame_read.stop()
-        if self.cap is not None:
-            self.cap.release()
 
         host = self.address[0]
         if host in drones:
             del drones[host]
 
     def __del__(self):
         self.end()
 
 
 class BackgroundFrameRead:
     """
-    This class read frames from a VideoCapture in background. Use
+    This class read frames using PyAV in background. Use
     backgroundFrameRead.frame to get the current frame.
     """
 
-    def __init__(self, tello, address):
-        tello.cap = cv2.VideoCapture(address)
-
-        self.cap = tello.cap
+    def __init__(self, tello, address, with_queue = False, maxsize = 32):
+        self.address = address
+        self.lock = Lock()
+        self.frame = np.zeros([300, 400, 3], dtype=np.uint8)
+        self.frames = deque([], maxsize)
+        self.with_queue = with_queue
 
-        if not self.cap.isOpened():
-            self.cap.open(address)
-
-        # Try grabbing a frame multiple times
+        # Try grabbing frame with PyAV
         # According to issue #90 the decoder might need some time
         # https://github.com/damiafuentes/DJITelloPy/issues/90#issuecomment-855458905
-        start = time.time()
-        while time.time() - start < Tello.FRAME_GRAB_TIMEOUT:
-            Tello.LOGGER.debug('trying to grab a frame...')
-            self.grabbed, self.frame = self.cap.read()
-            if self.frame is not None:
-                break
-            time.sleep(0.05)
-
-        if not self.grabbed or self.frame is None:
-            raise Exception('Failed to grab first frame from video stream')
+        try:
+            Tello.LOGGER.debug('trying to grab video frames...')
+            self.container = av.open(self.address, timeout=(Tello.FRAME_GRAB_TIMEOUT, None))
+        except av.error.ExitError:
+            raise TelloException('Failed to grab video frames from video stream')
 
         self.stopped = False
         self.worker = Thread(target=self.update_frame, args=(), daemon=True)
 
     def start(self):
         """Start the frame update worker
         Internal method, you normally wouldn't call this yourself.
         """
         self.worker.start()
 
     def update_frame(self):
-        """Thread worker function to retrieve frames from a VideoCapture
+        """Thread worker function to retrieve frames using PyAV
         Internal method, you normally wouldn't call this yourself.
         """
-        while not self.stopped:
-            if not self.grabbed or not self.cap.isOpened():
-                self.stop()
-            else:
-                self.grabbed, self.frame = self.cap.read()
+        try:
+            for frame in self.container.decode(video=0):
+                if self.with_queue:
+                    self.frames.append(np.array(frame.to_image()))
+                else:
+                    self.frame = np.array(frame.to_image())
+
+                if self.stopped:
+                    self.container.close()
+                    break
+        except av.error.ExitError:
+            raise TelloException('Do not have enough frames for decoding, please try again or increase video fps before get_frame_read()')
+    
+    def get_queued_frame(self):
+        """
+        Get a frame from the queue
+        """
+        with self.lock:
+            try:
+                return self.frames.popleft()
+            except IndexError:
+                return None
+
+    @property
+    def frame(self):
+        """
+        Access the frame variable directly
+        """
+        if self.with_queue:
+            return self.get_queued_frame()
+
+        with self.lock:
+            return self._frame
+
+    @frame.setter
+    def frame(self, value):
+        with self.lock:
+            self._frame = value
 
     def stop(self):
         """Stop the frame update worker
         Internal method, you normally wouldn't call this yourself.
         """
         self.stopped = True
-        self.worker.join()
```

### Comparing `djitellopy-2.4.0/setup.py` & `djitellopy-2.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,33 +6,37 @@
 # replace relative urls to example files with absolute urls to the main git repo
 repo_code_url = "https://github.com/damiafuentes/DJITelloPy/tree/master"
 long_description = long_description.replace("](examples/", "]({}/examples/".format(repo_code_url))
 
 setuptools.setup(
     name='djitellopy',
     packages=['djitellopy'],
-    version='2.4.0',
+    version='2.5.0',
     license='MIT',
     description='Tello drone library including support for video streaming, swarms, state packets and more',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jakob Löw',
     author_email='djitellopy@m4gnus.de',
     url='https://github.com/damiafuentes/DJITelloPy',
-    download_url='https://github.com/damiafuentes/DJITelloPy/archive/2.4.0.tar.gz',
+    download_url='https://github.com/damiafuentes/DJITelloPy/archive/2.5.0.tar.gz',
     keywords=['tello', 'dji', 'drone', 'sdk', 'official sdk'],
     install_requires=[
         'numpy',
         'opencv-python',
+        'av',
+        'pillow'
     ],
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

