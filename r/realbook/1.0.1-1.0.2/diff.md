# Comparing `tmp/realbook-1.0.1.tar.gz` & `tmp/realbook-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realbook-1.0.1.tar", last modified: Thu Dec 15 22:52:13 2022, max compression
+gzip compressed data, was "realbook-1.0.2.tar", last modified: Fri Jun  9 18:34:35 2023, max compression
```

## Comparing `realbook-1.0.1.tar` & `realbook-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2022-12-15 22:52:13.699515 realbook-1.0.1/
--rw-r--r--   0 drubinstein   (501) staff       (20)     7364 2022-12-14 16:22:31.000000 realbook-1.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 drubinstein   (501) staff       (20)    11357 2022-12-14 16:22:31.000000 realbook-1.0.1/LICENSE
--rw-r--r--   0 drubinstein   (501) staff       (20)      312 2022-12-14 16:47:24.000000 realbook-1.0.1/MANIFEST.in
--rw-r--r--   0 drubinstein   (501) staff       (20)      820 2022-12-14 16:22:31.000000 realbook-1.0.1/NOTICE
--rw-r--r--   0 drubinstein   (501) staff       (20)      354 2022-12-14 16:22:31.000000 realbook-1.0.1/OWNERS.md
--rw-r--r--   0 drubinstein   (501) staff       (20)     1023 2022-12-15 22:52:13.699619 realbook-1.0.1/PKG-INFO
--rw-r--r--   0 drubinstein   (501) staff       (20)     7679 2022-12-15 01:57:04.000000 realbook-1.0.1/README.md
--rw-r--r--   0 drubinstein   (501) staff       (20)      969 2022-12-14 16:22:31.000000 realbook-1.0.1/SECURITY.md
--rw-r--r--   0 drubinstein   (501) staff       (20)      189 2022-12-15 01:31:49.000000 realbook-1.0.1/pyproject.toml
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2022-12-15 22:52:13.682042 realbook-1.0.1/realbook/
--rw-r--r--   0 drubinstein   (501) staff       (20)      819 2022-12-15 22:51:56.000000 realbook-1.0.1/realbook/__init__.py
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2022-12-15 22:52:13.690063 realbook-1.0.1/realbook/callbacks/
--rw-r--r--   0 drubinstein   (501) staff       (20)      616 2022-12-14 16:22:31.000000 realbook-1.0.1/realbook/callbacks/__init__.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     5684 2022-12-15 01:08:02.000000 realbook-1.0.1/realbook/callbacks/debugging.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     7782 2022-12-15 01:08:13.000000 realbook-1.0.1/realbook/callbacks/spectrogram_visualization.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     2983 2022-12-15 00:53:42.000000 realbook-1.0.1/realbook/callbacks/speed.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     7226 2022-12-15 01:32:02.000000 realbook-1.0.1/realbook/callbacks/utilization.py
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2022-12-15 22:52:13.694856 realbook-1.0.1/realbook/layers/
--rw-r--r--   0 drubinstein   (501) staff       (20)      616 2022-12-14 16:22:31.000000 realbook-1.0.1/realbook/layers/__init__.py
--rw-r--r--   0 drubinstein   (501) staff       (20)    12504 2022-12-15 00:53:42.000000 realbook-1.0.1/realbook/layers/compatibility.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     2437 2022-12-15 00:53:42.000000 realbook-1.0.1/realbook/layers/math.py
--rw-r--r--   0 drubinstein   (501) staff       (20)    26605 2022-12-14 23:39:45.000000 realbook-1.0.1/realbook/layers/nnaudio.py
--rw-r--r--   0 drubinstein   (501) staff       (20)    15284 2022-12-15 00:53:42.000000 realbook-1.0.1/realbook/layers/signal.py
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2022-12-15 22:52:13.686264 realbook-1.0.1/realbook.egg-info/
--rw-r--r--   0 drubinstein   (501) staff       (20)     1023 2022-12-15 22:52:13.000000 realbook-1.0.1/realbook.egg-info/PKG-INFO
--rw-r--r--   0 drubinstein   (501) staff       (20)      927 2022-12-15 22:52:13.000000 realbook-1.0.1/realbook.egg-info/SOURCES.txt
--rw-r--r--   0 drubinstein   (501) staff       (20)        1 2022-12-15 22:52:13.000000 realbook-1.0.1/realbook.egg-info/dependency_links.txt
--rw-r--r--   0 drubinstein   (501) staff       (20)        1 2022-12-14 16:20:49.000000 realbook-1.0.1/realbook.egg-info/not-zip-safe
--rw-r--r--   0 drubinstein   (501) staff       (20)      409 2022-12-15 22:52:13.000000 realbook-1.0.1/realbook.egg-info/requires.txt
--rw-r--r--   0 drubinstein   (501) staff       (20)       15 2022-12-15 22:52:13.000000 realbook-1.0.1/realbook.egg-info/top_level.txt
--rw-r--r--   0 drubinstein   (501) staff       (20)     1579 2022-12-15 22:52:13.700242 realbook-1.0.1/setup.cfg
--rw-r--r--   0 drubinstein   (501) staff       (20)      686 2022-12-14 16:40:48.000000 realbook-1.0.1/setup.py
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2022-12-15 22:52:13.695278 realbook-1.0.1/tests/
--rw-r--r--   0 drubinstein   (501) staff       (20)      616 2022-12-14 16:22:31.000000 realbook-1.0.1/tests/__init__.py
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2022-12-15 22:52:13.696934 realbook-1.0.1/tests/callbacks/
--rw-r--r--   0 drubinstein   (501) staff       (20)     4411 2022-12-15 00:53:42.000000 realbook-1.0.1/tests/callbacks/test_debugging.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     6020 2022-12-15 01:08:28.000000 realbook-1.0.1/tests/callbacks/test_spectrogram_visualization.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     2218 2022-12-14 19:14:20.000000 realbook-1.0.1/tests/callbacks/test_speed.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     2762 2022-12-14 19:14:43.000000 realbook-1.0.1/tests/callbacks/test_utilization.py
-drwxr-xr-x   0 drubinstein   (501) staff       (20)        0 2022-12-15 22:52:13.699195 realbook-1.0.1/tests/layers/
--rw-r--r--   0 drubinstein   (501) staff       (20)    10656 2022-12-15 01:09:32.000000 realbook-1.0.1/tests/layers/test_compatibility.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     2539 2022-12-15 01:09:47.000000 realbook-1.0.1/tests/layers/test_math.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     4545 2022-12-14 23:26:21.000000 realbook-1.0.1/tests/layers/test_nnaudio.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     7059 2022-12-14 23:26:21.000000 realbook-1.0.1/tests/layers/test_signal.py
--rw-r--r--   0 drubinstein   (501) staff       (20)     1144 2022-12-15 01:31:57.000000 realbook-1.0.1/tox.ini
+drwxr-xr-x   0 psobot     (501) staff       (20)        0 2023-06-09 18:34:35.295424 realbook-1.0.2/
+-rw-r--r--   0 psobot     (501) staff       (20)     7364 2023-05-11 15:30:26.000000 realbook-1.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 psobot     (501) staff       (20)    11357 2023-05-11 15:30:26.000000 realbook-1.0.2/LICENSE
+-rw-r--r--   0 psobot     (501) staff       (20)      312 2023-05-11 15:30:26.000000 realbook-1.0.2/MANIFEST.in
+-rw-r--r--   0 psobot     (501) staff       (20)      820 2023-05-11 15:30:26.000000 realbook-1.0.2/NOTICE
+-rw-r--r--   0 psobot     (501) staff       (20)      354 2023-05-11 15:30:26.000000 realbook-1.0.2/OWNERS.md
+-rw-r--r--   0 psobot     (501) staff       (20)     1036 2023-06-09 18:34:35.295575 realbook-1.0.2/PKG-INFO
+-rw-r--r--   0 psobot     (501) staff       (20)     7991 2023-05-11 15:30:26.000000 realbook-1.0.2/README.md
+-rw-r--r--   0 psobot     (501) staff       (20)      969 2023-05-11 15:30:26.000000 realbook-1.0.2/SECURITY.md
+-rw-r--r--   0 psobot     (501) staff       (20)      189 2023-05-11 15:30:26.000000 realbook-1.0.2/pyproject.toml
+drwxr-xr-x   0 psobot     (501) staff       (20)        0 2023-06-09 18:34:35.239749 realbook-1.0.2/realbook/
+-rw-r--r--   0 psobot     (501) staff       (20)      819 2023-06-09 18:33:55.000000 realbook-1.0.2/realbook/__init__.py
+drwxr-xr-x   0 psobot     (501) staff       (20)        0 2023-06-09 18:34:35.263729 realbook-1.0.2/realbook/callbacks/
+-rw-r--r--   0 psobot     (501) staff       (20)      616 2023-05-11 15:30:26.000000 realbook-1.0.2/realbook/callbacks/__init__.py
+-rw-r--r--   0 psobot     (501) staff       (20)     5684 2023-05-11 15:30:26.000000 realbook-1.0.2/realbook/callbacks/debugging.py
+-rw-r--r--   0 psobot     (501) staff       (20)     7780 2023-06-09 18:33:55.000000 realbook-1.0.2/realbook/callbacks/spectrogram_visualization.py
+-rw-r--r--   0 psobot     (501) staff       (20)     2983 2023-05-11 15:30:26.000000 realbook-1.0.2/realbook/callbacks/speed.py
+-rw-r--r--   0 psobot     (501) staff       (20)     7226 2023-05-11 15:30:26.000000 realbook-1.0.2/realbook/callbacks/utilization.py
+drwxr-xr-x   0 psobot     (501) staff       (20)        0 2023-06-09 18:34:35.277786 realbook-1.0.2/realbook/layers/
+-rw-r--r--   0 psobot     (501) staff       (20)      616 2023-05-11 15:30:26.000000 realbook-1.0.2/realbook/layers/__init__.py
+-rw-r--r--   0 psobot     (501) staff       (20)    12504 2023-05-11 15:30:26.000000 realbook-1.0.2/realbook/layers/compatibility.py
+-rw-r--r--   0 psobot     (501) staff       (20)     2439 2023-05-11 15:30:26.000000 realbook-1.0.2/realbook/layers/math.py
+-rw-r--r--   0 psobot     (501) staff       (20)    26605 2023-05-11 15:30:26.000000 realbook-1.0.2/realbook/layers/nnaudio.py
+-rw-r--r--   0 psobot     (501) staff       (20)    18160 2023-06-09 18:33:55.000000 realbook-1.0.2/realbook/layers/signal.py
+drwxr-xr-x   0 psobot     (501) staff       (20)        0 2023-06-09 18:34:35.279260 realbook-1.0.2/realbook/vendor/
+-rw-r--r--   0 psobot     (501) staff       (20)      616 2023-06-09 18:33:55.000000 realbook-1.0.2/realbook/vendor/__init__.py
+-rw-r--r--   0 psobot     (501) staff       (20)    28685 2023-06-09 18:33:56.000000 realbook-1.0.2/realbook/vendor/librosa_filters.py
+drwxr-xr-x   0 psobot     (501) staff       (20)        0 2023-06-09 18:34:35.247017 realbook-1.0.2/realbook.egg-info/
+-rw-r--r--   0 psobot     (501) staff       (20)     1036 2023-06-09 18:34:34.000000 realbook-1.0.2/realbook.egg-info/PKG-INFO
+-rw-r--r--   0 psobot     (501) staff       (20)      990 2023-06-09 18:34:35.000000 realbook-1.0.2/realbook.egg-info/SOURCES.txt
+-rw-r--r--   0 psobot     (501) staff       (20)        1 2023-06-09 18:34:34.000000 realbook-1.0.2/realbook.egg-info/dependency_links.txt
+-rw-r--r--   0 psobot     (501) staff       (20)        1 2023-05-11 15:55:41.000000 realbook-1.0.2/realbook.egg-info/not-zip-safe
+-rw-r--r--   0 psobot     (501) staff       (20)      627 2023-06-09 18:34:34.000000 realbook-1.0.2/realbook.egg-info/requires.txt
+-rw-r--r--   0 psobot     (501) staff       (20)       15 2023-06-09 18:34:34.000000 realbook-1.0.2/realbook.egg-info/top_level.txt
+-rw-r--r--   0 psobot     (501) staff       (20)     1787 2023-06-09 18:34:35.297854 realbook-1.0.2/setup.cfg
+-rw-r--r--   0 psobot     (501) staff       (20)      686 2023-05-11 15:30:26.000000 realbook-1.0.2/setup.py
+drwxr-xr-x   0 psobot     (501) staff       (20)        0 2023-06-09 18:34:35.281417 realbook-1.0.2/tests/
+-rw-r--r--   0 psobot     (501) staff       (20)      616 2023-05-11 15:30:26.000000 realbook-1.0.2/tests/__init__.py
+drwxr-xr-x   0 psobot     (501) staff       (20)        0 2023-06-09 18:34:35.292032 realbook-1.0.2/tests/callbacks/
+-rw-r--r--   0 psobot     (501) staff       (20)     4411 2023-05-11 15:30:26.000000 realbook-1.0.2/tests/callbacks/test_debugging.py
+-rw-r--r--   0 psobot     (501) staff       (20)     7129 2023-06-09 18:33:56.000000 realbook-1.0.2/tests/callbacks/test_spectrogram_visualization.py
+-rw-r--r--   0 psobot     (501) staff       (20)     2218 2023-05-11 15:30:26.000000 realbook-1.0.2/tests/callbacks/test_speed.py
+-rw-r--r--   0 psobot     (501) staff       (20)     2762 2023-05-11 15:30:26.000000 realbook-1.0.2/tests/callbacks/test_utilization.py
+drwxr-xr-x   0 psobot     (501) staff       (20)        0 2023-06-09 18:34:35.294797 realbook-1.0.2/tests/layers/
+-rw-r--r--   0 psobot     (501) staff       (20)    10656 2023-06-09 18:33:49.000000 realbook-1.0.2/tests/layers/test_compatibility.py
+-rw-r--r--   0 psobot     (501) staff       (20)     2539 2023-06-09 18:33:49.000000 realbook-1.0.2/tests/layers/test_math.py
+-rw-r--r--   0 psobot     (501) staff       (20)     4046 2023-06-09 18:33:56.000000 realbook-1.0.2/tests/layers/test_nnaudio.py
+-rw-r--r--   0 psobot     (501) staff       (20)    10586 2023-06-09 18:33:56.000000 realbook-1.0.2/tests/layers/test_signal.py
+-rw-r--r--   0 psobot     (501) staff       (20)     1144 2023-05-11 15:30:26.000000 realbook-1.0.2/tox.ini
```

### Comparing `realbook-1.0.1/CODE_OF_CONDUCT.md` & `realbook-1.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/LICENSE` & `realbook-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/NOTICE` & `realbook-1.0.2/NOTICE`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/PKG-INFO` & `realbook-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: realbook
-Version: 1.0.1
+Version: 1.0.2
 Summary: Realbook, a library to make using audio on TensorFlow easier.
 Home-page: https://github.com/spotify/realbook
 Author: Spotify
 Author-email: realbook@spotify.com
 Maintainer: Spotify
 Maintainer-email: realbook@spotify.com
 License: Apache 2.0
-Description: Realbook, a library to make using audio on TensorFlow easier.
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Provides-Extra: dev
 Provides-Extra: tensorboard
 Provides-Extra: test
+License-File: LICENSE
+License-File: NOTICE
+
+Realbook, a library to make using audio on TensorFlow easier.
```

### Comparing `realbook-1.0.1/README.md` & `realbook-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Below are a few highlights of what we have written so far.
 
 ## Keras Layers
 
 - `FrozenGraphLayer` - Allows you to use a TF V1 graph as a Keras layer.
 - `CQT` - Constant-Q transform layers ported from [nnAudio](https://kinwaicheuk.github.io/nnAudio/index.html).
-- `STFT`, `ISTFT`, `MelSpectrogram` and `Spectrogram` - Layers that perform common audio feature preprocessing. All checked for correctness against [librosa](https://librosa.org/).
+- `Stft`, `Istft`, `MelSpectrogram`, `Spectrogram`, `Magnitude`, `Phase` and `MagnitudeToDecibel` - Layers that perform common audio feature preprocessing. All checked for correctness against [librosa](https://librosa.org/).
 
 ## Callbacks
 
 - `Spectrogram visualization` - Allows you to write spectrogram output layers to TensorBoard.
 - `Training Speed` - Allows you to visualize on TensorBoard how fast each epoch of training is taking.
 - `Utilization` - Allows you to plot on TensorBoard CPU, CPU Memory, GPU and GPU Memory utilization as you train.
 
@@ -44,15 +44,15 @@
 ## A Binary Classifier With Audio Input
 
 Let's use realbook to train a binary classifier that takes in audio, converts the audio to a spectrogram and then 
 runs the spectorgram output through two trainable Dense layers.
 
 ```python3
 import tensorflow as tf
-from realbook.signal import STFT
+from realbook.layers.signal import STFT
 
 train_ds = tf.data.TFRecordDataset(training_filenames)
 val_ds = tf.data.TFRecordDataset(validation_filenames)
 
 # Create a sequential model
 model = tf.keras.Sequential([
     tf.keras.layers.InputLayer((22050,)),
@@ -77,15 +77,15 @@
 ## A Binary Classifier With Audio Input and CPU Memory Utilization Measurement
 
 Below is the previous binary classifier example, but we're now going to add a realbook
 callback to the model's callback list.
 
 ```python3
 import tensorflow as tf
-from realbook.signal import STFT
+from realbook.layers.signal import STFT
 from realbook.callbacks.utilization import MemoryUtilizationCallback
 
 train_ds = tf.data.TFRecordDataset(training_filenames)
 val_ds = tf.data.TFRecordDataset(validation_filenames)
 
 # Create a sequential model
 model = tf.keras.Sequential([
@@ -179,19 +179,27 @@
 $ tox
 
 # run a specific environment
 $ tox -e check-formatting
 $ tox -e py38
 ```
 
+### Formatting files
+
+Before committing PR's please format your files using tox as some of the formatting options realboook uses is different than the defaults of the [Black](https://black.readthedocs.io/en/stable/) formatter:
+
+```sh
+tox -e format
+```
+
 See [tox's documentation](https://tox.readthedocs.io/en/latest/) for more information.
 
 ## Copyright and License
 realbook is Copyright 2022 Spotify AB.
 
 This software is licensed under the Apache License, Version 2.0 (the "Apache License"). You may choose either license to govern your use of this software only upon the condition that you accept all of the terms of either the Apache License.
 
 You may obtain a copy of the Apache License at:
 
 http://www.apache.org/licenses/LICENSE-2.0
 
-Unless required by applicable law or agreed to in writing, software distributed under the Apache License or the GPL License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the Apache License for the specific language governing permissions and limitations under the Apache License
+Unless required by applicable law or agreed to in writing, software distributed under the Apache License or the GPL License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the Apache License for the specific language governing permissions and limitations under the Apache License
```

### Comparing `realbook-1.0.1/SECURITY.md` & `realbook-1.0.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/realbook/__init__.py` & `realbook-1.0.2/realbook/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 __author__ = "Spotify"
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __email__ = "realbook@spotify.com"
 __description__ = "Python libraries for easier machine learning on audio"
 __url__ = "https://github.com/spotify/realbook"
```

### Comparing `realbook-1.0.1/realbook/callbacks/__init__.py` & `realbook-1.0.2/realbook/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/realbook/callbacks/debugging.py` & `realbook-1.0.2/realbook/callbacks/debugging.py`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/realbook/callbacks/spectrogram_visualization.py` & `realbook-1.0.2/realbook/callbacks/spectrogram_visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             # (Yes, you'd think that self.model.layers returns all layers - but that doesn't seem to be the case.)
             input_to_image = tf.keras.models.Model(
                 inputs=non_trainable_input_layers[0].input, outputs=non_trainable_input_layers[-1].output
             )
 
             with self.tensorboard_writer.as_default():
                 # Pull n random batches from the dataset and send them to TensorBoard.
-                for (data, _) in self.example_batches:
+                for data, _ in self.example_batches:
                     assert tf.rank(data) == 2, "Expected input data to be of rank 2, with shape (batch, audio)."
                     assert tf.shape(data)[0] < tf.shape(data)[1], (
                         "Expected input data to be of rank 2, with shape (batch, audio), but got shape"
                         f" {tf.shape(data)}."
                     )
 
                     spectrograms = input_to_image(data)
```

### Comparing `realbook-1.0.1/realbook/callbacks/speed.py` & `realbook-1.0.2/realbook/callbacks/speed.py`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/realbook/callbacks/utilization.py` & `realbook-1.0.2/realbook/callbacks/utilization.py`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/realbook/layers/__init__.py` & `realbook-1.0.2/realbook/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/realbook/layers/compatibility.py` & `realbook-1.0.2/realbook/layers/compatibility.py`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/realbook/layers/math.py` & `realbook-1.0.2/realbook/layers/math.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 
 
-def log_base_b(x: tf.Tensor, base: int) -> tf.Tensor:
+def log_base_b(x: tf.Tensor, base: float) -> tf.Tensor:
     """
     Compute log_b(x)
     Args:
         x : input
         base : log base. E.g. for log10 base=10
     Returns:
         log_base(x)
```

### Comparing `realbook-1.0.1/realbook/layers/nnaudio.py` & `realbook-1.0.2/realbook/layers/nnaudio.py`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/realbook/layers/signal.py` & `realbook-1.0.2/realbook/layers/signal.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import warnings
 from typing import Any, Callable, Dict, Optional, Union
 
-import librosa
 import tensorflow as tf
 import numpy as np
 
+from realbook.layers.math import log_base_b
+from realbook.vendor import librosa_filters
+
 
 def _create_padded_window(
     window_fn: Callable[[int, tf.dtypes.DType], tf.Tensor],
     unpadded_window_length: int,
     fft_length: int,
 ) -> Callable[[int, tf.dtypes.DType], tf.Tensor]:
     lpad = (fft_length - unpadded_window_length) // 2
@@ -203,15 +205,15 @@
                 "like (num_frames, num_bins) or (num_batches, num_frames, num_bins)."
             )
 
         self.window = _create_padded_window(self.window_fn, self.window_length, self.fft_length)(
             self.fft_length
         )  # type: ignore
 
-        self.window_sum = librosa.filters.window_sumsquare(
+        self.window_sum = librosa_filters.window_sumsquare(  # type: ignore
             window=self.window.numpy(),
             n_frames=input_shape[0] if input_shape.rank == 2 else input_shape[1],
             win_length=self.window_length,
             n_fft=self.fft_length,
             hop_length=self.hop_length,
             dtype=self.dtypes_type.as_numpy_dtype,
         )
@@ -347,15 +349,15 @@
         self.sample_rate = sample_rate
         self.normalization = normalization
 
     def build(self, input_shape: tf.TensorShape) -> None:
         super().build(input_shape)
 
         self.mel_weight_matrix = tf.constant(
-            librosa.filters.mel(
+            librosa_filters.mel(  # type: ignore
                 sr=self.sample_rate,
                 n_fft=self.fft_length,
                 n_mels=self.n_mels,
                 fmin=self.lower_edge_hertz,
                 fmax=self.upper_edge_hertz,
                 htk=self.htk,
                 norm=self.normalization,
@@ -376,7 +378,102 @@
                 "upper_edge_hertz": self.upper_edge_hertz,
                 "htk": self.htk,
                 "sample_rate": self.sample_rate,
                 "normalization": self.normalization,
             }
         )
         return config
+
+
+class Magnitude(tf.keras.layers.Layer):
+    def __init__(
+        self,
+        name: Optional[str] = None,
+        dtype: tf.dtypes.DType = tf.float32,
+        *args: Any,
+        **kwargs: Any,
+    ):
+        """
+        A Tensorflow Keras layer that calculates the magnitude of a complex tensor.
+
+        Args:
+            name: Name of the layer.
+            dtype: Type used in calculation.
+        """
+        super().__init__(name=name, dtype=dtype, *args, **kwargs)
+
+    def call(self, inputs: tf.Tensor) -> tf.Tensor:
+        return tf.math.abs(inputs)
+
+    def get_config(self) -> Dict[str, Any]:
+        config: Dict[str, Any] = super().get_config().copy()
+        return config
+
+
+class Phase(tf.keras.layers.Layer):
+    def __init__(
+        self,
+        name: Optional[str] = None,
+        dtype: tf.dtypes.DType = tf.float32,
+        *args: Any,
+        **kwargs: Any,
+    ):
+        """
+        A Tensorflow Keras layer that calculates the phase of a complex tensor.
+
+        Args:
+            name: Name of the layer.
+            dtype: Type used in calculation.
+        """
+        super().__init__(name=name, dtype=dtype, *args, **kwargs)
+
+    def call(self, inputs: tf.Tensor) -> tf.Tensor:
+        return tf.math.angle(inputs)
+
+    def get_config(self) -> Dict[str, Any]:
+        config: Dict[str, Any] = super().get_config().copy()
+        return config
+
+
+class MagnitudeToDecibel(tf.keras.layers.Layer):
+    def __init__(
+        self,
+        ref: float = 1.0,
+        amin: float = 1e-10,
+        top_db: float = 80.0,
+        name: Optional[str] = None,
+        dtype: tf.dtypes.DType = tf.float32,
+    ):
+        """
+        A Keras layer that converts a real-valued tensor to decibel scale.
+
+        Args:
+            ref: Reference power that would be scaled to 0 dB.
+            amin: Minimum power threshold.
+            top_db: Minimum negative cut-off in decibels.
+            name: Name of the layer.
+            dtype: Type used in calculation.
+        """
+        super().__init__(name=name, dtype=dtype)
+        self.ref = ref
+        self.amin = amin
+        self.top_db = top_db
+
+    def call(self, inputs: tf.Tensor) -> tf.Tensor:
+        log_spec = 10.0 * (
+            log_base_b(tf.math.maximum(inputs, self.amin), 10.0)
+            - log_base_b(tf.math.maximum(self.amin, self.ref), 10.0)
+        )
+        log_spec = tf.math.maximum(log_spec, tf.math.reduce_max(log_spec, keepdims=True) - self.top_db)
+
+        return log_spec
+
+    def get_config(self) -> Dict[str, Any]:
+        config: Dict[str, Any] = super().get_config().copy()
+        config.update(
+            {
+                "ref": self.ref,
+                "amin": self.amin,
+                "top_db": self.top_db,
+            }
+        )
+        return config
```

### Comparing `realbook-1.0.1/realbook.egg-info/PKG-INFO` & `realbook-1.0.2/realbook.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: realbook
-Version: 1.0.1
+Version: 1.0.2
 Summary: Realbook, a library to make using audio on TensorFlow easier.
 Home-page: https://github.com/spotify/realbook
 Author: Spotify
 Author-email: realbook@spotify.com
 Maintainer: Spotify
 Maintainer-email: realbook@spotify.com
 License: Apache 2.0
-Description: Realbook, a library to make using audio on TensorFlow easier.
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Provides-Extra: dev
 Provides-Extra: tensorboard
 Provides-Extra: test
+License-File: LICENSE
+License-File: NOTICE
+
+Realbook, a library to make using audio on TensorFlow easier.
```

### Comparing `realbook-1.0.1/realbook.egg-info/SOURCES.txt` & `realbook-1.0.2/realbook.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 realbook/callbacks/speed.py
 realbook/callbacks/utilization.py
 realbook/layers/__init__.py
 realbook/layers/compatibility.py
 realbook/layers/math.py
 realbook/layers/nnaudio.py
 realbook/layers/signal.py
+realbook/vendor/__init__.py
+realbook/vendor/librosa_filters.py
 tests/__init__.py
 tests/callbacks/test_debugging.py
 tests/callbacks/test_spectrogram_visualization.py
 tests/callbacks/test_speed.py
 tests/callbacks/test_utilization.py
 tests/layers/test_compatibility.py
 tests/layers/test_math.py
```

### Comparing `realbook-1.0.1/setup.cfg` & `realbook-1.0.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.1
+current_version = 1.0.2
 commit = True
 tag = True
 
 [metadata]
 name = realbook
 version = attr: realbook.__version__
 description = Realbook, a library to make using audio on TensorFlow easier.
@@ -31,36 +31,40 @@
 [options]
 zip_safe = False
 packages = find:
 include_package_data = True
 install_requires = 
 	tensorflow>=2.4; sys_platform != 'darwin' or platform.machine != 'arm64'
 	tensorflow-macos>=2.4; sys_platform == 'darwin' and platform.machine == 'arm64'
-	tensorboard>=2.4
-	librosa>=0.9,<0.10
+	tensorboard
 	types-protobuf
+	numpy
+	typing_extensions
 
 [options.extras_require]
 dev = 
 	realbook[tensorboard,test]
 	bumpversion>=0.5.3
-	ipython
-	ipdb
 tensorboard = 
 	matplotlib
 	psutil
 	nvsmi
+	librosa>=0.9,<0.10
 test = 
 	coverage>=5.0.2
 	pytest>=7.1.1
 	pytest-cov>=4.0.0
 	pytest-mock>=3.10.0
 	tox
 	torch
 	nnaudio
+	numpy==1.21.6
+	librosa>=0.9,<0.10
+	tensorflow>=2.4,<2.11; sys_platform != 'darwin' or platform.machine != 'arm64'
+	tensorflow-macos>=2.4,<2.11; sys_platform == 'darwin' and platform.machine == 'arm64'
 
 [bumpversion:file:realbook/__init__.py]
 
 [bdist_wheel]
 universal = 1
 
 [egg_info]
```

### Comparing `realbook-1.0.1/setup.py` & `realbook-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/tests/__init__.py` & `realbook-1.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/tests/callbacks/test_debugging.py` & `realbook-1.0.2/tests/callbacks/test_debugging.py`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/tests/callbacks/test_spectrogram_visualization.py` & `realbook-1.0.2/tests/callbacks/test_spectrogram_visualization.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,19 +13,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License
 
 from typing import Any
 
+import platform
 import pytest
 import numpy as np
 import tensorflow as tf
 
-from realbook.callbacks.spectrogram_visualization import SpectrogramVisualizationCallback
+try:
+    from realbook.callbacks.spectrogram_visualization import SpectrogramVisualizationCallback
+except ImportError as e:
+    if "numpy.core.multiarray failed to import" in str(e) and platform.system() == "Windows":
+        SpectrogramVisualizationCallback = None  # type: ignore
+    else:
+        raise
+
 from realbook.layers.signal import Spectrogram
 
 
 try:
     from contextlib import nullcontext
 except ImportError:
 
@@ -48,14 +56,18 @@
         pass
 
 
 DEFAULT_SAMPLE_RATE = 22050
 TEST_AUDIO = np.linspace(0, 1, num=DEFAULT_SAMPLE_RATE * 10)
 
 
+@pytest.mark.skipif(
+    SpectrogramVisualizationCallback is None,
+    reason="SpectrogramVisualizationCallback import fails on this platform",
+)
 def test_spectrogram_visualization_callback() -> None:
     fake_data = tf.data.Dataset.zip(
         (
             tf.data.Dataset.from_tensor_slices([TEST_AUDIO]),
             tf.data.Dataset.from_tensor_slices([1]),
         )
     ).batch(1)
@@ -76,14 +88,18 @@
         raise_on_error=True,
     )
 
     model.fit(fake_data, callbacks=[cb])
     assert True
 
 
+@pytest.mark.skipif(
+    SpectrogramVisualizationCallback is None,
+    reason="SpectrogramVisualizationCallback import fails on this platform",
+)
 def test_callback_fails_on_unbatched_input() -> None:
     fake_data = tf.data.Dataset.zip(
         (
             tf.data.Dataset.from_tensor_slices([TEST_AUDIO]),
             tf.data.Dataset.from_tensor_slices([1]),
         )
     )
@@ -106,14 +122,18 @@
     )
 
     with pytest.raises(AssertionError) as excinfo:
         model.fit(fake_data.batch(1), callbacks=[cb])
     assert "shape" in str(excinfo.value)
 
 
+@pytest.mark.skipif(
+    SpectrogramVisualizationCallback is None,
+    reason="SpectrogramVisualizationCallback import fails on this platform",
+)
 def test_callback_logs_but_doesnt_throw_by_default(caplog: pytest.LogCaptureFixture) -> None:
     fake_data = tf.data.Dataset.zip(
         (
             tf.data.Dataset.from_tensor_slices([TEST_AUDIO]),
             tf.data.Dataset.from_tensor_slices([1]),
         )
     )
@@ -129,14 +149,18 @@
     # Cause the callback to error by passing in unbatched data.
     cb = SpectrogramVisualizationCallback(FakeWriter(), fake_data, sample_rate=DEFAULT_SAMPLE_RATE)
     model.fit(fake_data.batch(1), callbacks=[cb])
     assert "AssertionError" in caplog.text
     assert "shape" in caplog.text
 
 
+@pytest.mark.skipif(
+    SpectrogramVisualizationCallback is None,
+    reason="SpectrogramVisualizationCallback import fails on this platform",
+)
 def test_fails_on_no_image_like_layers() -> None:
     fake_data = tf.data.Dataset.zip(
         (
             tf.data.Dataset.from_tensor_slices([TEST_AUDIO]),
             tf.data.Dataset.from_tensor_slices([1]),
         )
     ).batch(1)
@@ -158,14 +182,18 @@
 
     with pytest.raises(ValueError) as excinfo:
         model.fit(fake_data, callbacks=[cb])
     assert isinstance(excinfo.value, ValueError)
     assert "spectrogram" in str(excinfo.value)
 
 
+@pytest.mark.skipif(
+    SpectrogramVisualizationCallback is None,
+    reason="SpectrogramVisualizationCallback import fails on this platform",
+)
 def test_flexible_with_input_shapes() -> None:
     fake_data = tf.data.Dataset.zip(
         (
             tf.data.Dataset.from_tensor_slices([TEST_AUDIO]),
             tf.data.Dataset.from_tensor_slices([1]),
         )
     ).batch(1)
@@ -188,14 +216,18 @@
         raise_on_error=True,
     )
 
     model.fit(fake_data, callbacks=[cb])
     assert True
 
 
+@pytest.mark.skipif(
+    SpectrogramVisualizationCallback is None,
+    reason="SpectrogramVisualizationCallback import fails on this platform",
+)
 def test_keras_functional_api_with_tfop_lambda() -> None:
     fake_data = tf.data.Dataset.zip(
         (
             tf.data.Dataset.from_tensor_slices([TEST_AUDIO]),
             tf.data.Dataset.from_tensor_slices([1]),
         )
     ).batch(1)
```

### Comparing `realbook-1.0.1/tests/callbacks/test_speed.py` & `realbook-1.0.2/tests/callbacks/test_speed.py`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/tests/callbacks/test_utilization.py` & `realbook-1.0.2/tests/callbacks/test_utilization.py`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/tests/layers/test_compatibility.py` & `realbook-1.0.2/tests/layers/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/tests/layers/test_math.py` & `realbook-1.0.2/tests/layers/test_math.py`

 * *Files identical despite different names*

### Comparing `realbook-1.0.1/tests/layers/test_nnaudio.py` & `realbook-1.0.2/tests/layers/test_nnaudio.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,58 +15,35 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 import torch
 import numpy as np
 import pytest
-import librosa
-import librosa.display
+import platform
 
-from typing import List, Tuple, Union
+try:
+    import librosa
+    from realbook.layers import nnaudio as our_nnaudio
+    from nnAudio.Spectrogram import CQT2010v2
+except ImportError as e:
+    if "numpy.core.multiarray failed to import" in str(e) and platform.system() == "Windows":
+        librosa = None
+        our_nnaudio = None  # type: ignore
+        CQT2010v2 = None
+    else:
+        raise
 
-from realbook.layers import nnaudio as our_nnaudio
-from nnAudio.Spectrogram import CQT2010v2
-
-TEST_SAMPLE_RATE = 22050
+from typing import Tuple, Union
 
 
-# Test using this model directly, as well as wrapping it in a Lambda layer.
-def get_parameterized_model_variants(
-    match_torch_exactly_values: Tuple[bool, bool] = (True, False)
-) -> List[tf.keras.layers.Layer]:
-    possible_models = [
-        our_nnaudio.CQT(match_torch_exactly=v, trainable=trainable)
-        for v in match_torch_exactly_values
-        for trainable in (True, False)
-    ]
-
-    return [
-        item
-        for models in [
-            [tf.keras.Sequential([tf.keras.layers.InputLayer((TEST_SAMPLE_RATE,)), model])]
-            + (
-                [
-                    tf.keras.Sequential(
-                        [
-                            tf.keras.layers.InputLayer((TEST_SAMPLE_RATE,)),
-                            tf.keras.layers.Lambda(lambda x: model(x)),
-                        ]
-                    )
-                ]
-                # Using a layer with trainable weights inside a Lambda layer isn't supported.
-                if not model.trainable
-                else []
-            )
-            for model in possible_models
-        ]
-        for item in models
-    ]
+TEST_SAMPLE_RATE = 22050
 
 
+@pytest.mark.skipif(librosa is None, reason="Librosa failed to import on this platform.")
 @pytest.mark.parametrize(
     "match_torch_exactly,threshold,trainable",
     (
         (True, 0.0001, False),
         (False, 4, False),
         (True, 0.0001, True),
         (False, 4, True),
@@ -79,29 +56,33 @@
     actual = our_nnaudio.CQT(match_torch_exactly=match_torch_exactly, trainable=trainable)(signal).numpy()
 
     assert expected.shape == actual.shape
     assert np.allclose(expected, actual, rtol=threshold, atol=threshold)
 
 
 def build_layer(
-    layer: tf.keras.layers.Layer, input_shape: Union[Tuple[int], Tuple[int, int]] = (1, TEST_SAMPLE_RATE)
+    layer: tf.keras.layers.Layer,
+    input_shape: Union[Tuple[int], Tuple[int, int]] = (1, TEST_SAMPLE_RATE),
 ) -> tf.keras.layers.Layer:
     layer.build(input_shape)
     return layer
 
 
+@pytest.mark.skipif(our_nnaudio is None, reason="nnaudio failed to import on this platform.")
 def test_cqt_trainable_weights() -> None:
     assert not build_layer(our_nnaudio.CQT(trainable=False)).trainable
     assert not build_layer(our_nnaudio.CQT(trainable=False)).trainable_weights
 
     assert build_layer(our_nnaudio.CQT(trainable=True)).trainable
     assert len(build_layer(our_nnaudio.CQT(trainable=True)).trainable_variables) == 2
     assert len(build_layer(our_nnaudio.CQT(trainable=True)).trainable_weights) == 2
 
 
+@pytest.mark.skipif(librosa is None, reason="Librosa failed to import on this platform.")
+@pytest.mark.skipif(our_nnaudio is None, reason="nnaudio failed to import on this platform.")
 @pytest.mark.parametrize("train", (True, False))
 def test_cqt_trainable_layers_change_on_training(train: bool) -> None:
     # Make a model that's trainable, then train it and ensure the weights change from the default.
     trainable_cqt = our_nnaudio.CQT(trainable=True)
     untrained_cqt = build_layer(our_nnaudio.CQT(trainable=True), (TEST_SAMPLE_RATE * 10,))
 
     model = tf.keras.Sequential(
```

### Comparing `realbook-1.0.1/tox.ini` & `realbook-1.0.2/tox.ini`

 * *Files identical despite different names*

