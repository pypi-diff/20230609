# Comparing `tmp/openvalidators-1.0.2.tar.gz` & `tmp/openvalidators-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvalidators-1.0.2.tar", last modified: Wed Jun  7 20:01:13 2023, max compression
+gzip compressed data, was "openvalidators-1.0.4.tar", last modified: Fri Jun  9 16:20:48 2023, max compression
```

## Comparing `openvalidators-1.0.2.tar` & `openvalidators-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-07 20:01:13.358997 openvalidators-1.0.2/
--rw-r--r--   0 pedroferreira   (501) staff       (20)     1087 2023-06-05 21:08:43.000000 openvalidators-1.0.2/LICENSE
--rw-r--r--   0 pedroferreira   (501) staff       (20)     8971 2023-06-07 20:01:13.358866 openvalidators-1.0.2/PKG-INFO
--rw-r--r--   0 pedroferreira   (501) staff       (20)     7757 2023-06-06 18:34:54.000000 openvalidators-1.0.2/README.md
-drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-07 20:01:13.357876 openvalidators-1.0.2/openvalidators/
--rw-r--r--   0 pedroferreira   (501) staff       (20)     1403 2023-06-07 20:00:55.000000 openvalidators-1.0.2/openvalidators/__init__.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     8831 2023-06-07 17:58:23.000000 openvalidators-1.0.2/openvalidators/config.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     4366 2023-06-06 18:32:40.000000 openvalidators-1.0.2/openvalidators/dendrite.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)    16781 2023-06-07 20:00:41.000000 openvalidators-1.0.2/openvalidators/forward.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)    13620 2023-06-06 18:32:40.000000 openvalidators-1.0.2/openvalidators/gating.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     2029 2023-06-05 21:08:43.000000 openvalidators-1.0.2/openvalidators/misc.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     3557 2023-06-06 18:32:40.000000 openvalidators-1.0.2/openvalidators/mock.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     6977 2023-06-07 13:42:52.000000 openvalidators-1.0.2/openvalidators/neuron.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)    10885 2023-06-06 18:32:40.000000 openvalidators-1.0.2/openvalidators/prompts.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     7927 2023-06-06 18:32:40.000000 openvalidators-1.0.2/openvalidators/reward.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     2547 2023-06-07 13:42:52.000000 openvalidators-1.0.2/openvalidators/run.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     9418 2023-06-07 20:00:41.000000 openvalidators-1.0.2/openvalidators/utils.py
--rw-r--r--   0 pedroferreira   (501) staff       (20)     2912 2023-06-07 17:58:23.000000 openvalidators-1.0.2/openvalidators/weights.py
-drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-07 20:01:13.358692 openvalidators-1.0.2/openvalidators.egg-info/
--rw-r--r--   0 pedroferreira   (501) staff       (20)     8971 2023-06-07 20:01:13.000000 openvalidators-1.0.2/openvalidators.egg-info/PKG-INFO
--rw-r--r--   0 pedroferreira   (501) staff       (20)      580 2023-06-07 20:01:13.000000 openvalidators-1.0.2/openvalidators.egg-info/SOURCES.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)        1 2023-06-07 20:01:13.000000 openvalidators-1.0.2/openvalidators.egg-info/dependency_links.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)       69 2023-06-07 20:01:13.000000 openvalidators-1.0.2/openvalidators.egg-info/entry_points.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)      143 2023-06-07 20:01:13.000000 openvalidators-1.0.2/openvalidators.egg-info/requires.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)       15 2023-06-07 20:01:13.000000 openvalidators-1.0.2/openvalidators.egg-info/top_level.txt
--rw-r--r--   0 pedroferreira   (501) staff       (20)       38 2023-06-07 20:01:13.359037 openvalidators-1.0.2/setup.cfg
--rw-r--r--   0 pedroferreira   (501) staff       (20)     3496 2023-06-06 18:47:52.000000 openvalidators-1.0.2/setup.py
+drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-09 16:20:48.831678 openvalidators-1.0.4/
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     1087 2023-06-05 21:08:43.000000 openvalidators-1.0.4/LICENSE
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     8951 2023-06-09 16:20:48.831221 openvalidators-1.0.4/PKG-INFO
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     7757 2023-06-06 18:34:54.000000 openvalidators-1.0.4/README.md
+drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-09 16:20:48.829804 openvalidators-1.0.4/openvalidators/
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     1529 2023-06-09 16:19:51.000000 openvalidators-1.0.4/openvalidators/__init__.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     8831 2023-06-07 17:58:23.000000 openvalidators-1.0.4/openvalidators/config.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     4366 2023-06-06 18:32:40.000000 openvalidators-1.0.4/openvalidators/dendrite.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)    16764 2023-06-09 16:19:51.000000 openvalidators-1.0.4/openvalidators/forward.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)    13620 2023-06-06 18:32:40.000000 openvalidators-1.0.4/openvalidators/gating.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     2029 2023-06-05 21:08:43.000000 openvalidators-1.0.4/openvalidators/misc.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     3557 2023-06-06 18:32:40.000000 openvalidators-1.0.4/openvalidators/mock.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     6977 2023-06-07 13:42:52.000000 openvalidators-1.0.4/openvalidators/neuron.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)    10885 2023-06-06 18:32:40.000000 openvalidators-1.0.4/openvalidators/prompts.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     7927 2023-06-06 18:32:40.000000 openvalidators-1.0.4/openvalidators/reward.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     2547 2023-06-07 13:42:52.000000 openvalidators-1.0.4/openvalidators/run.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     9418 2023-06-07 21:15:53.000000 openvalidators-1.0.4/openvalidators/utils.py
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     2912 2023-06-07 17:58:23.000000 openvalidators-1.0.4/openvalidators/weights.py
+drwxr-xr-x   0 pedroferreira   (501) staff       (20)        0 2023-06-09 16:20:48.830882 openvalidators-1.0.4/openvalidators.egg-info/
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     8951 2023-06-09 16:20:48.000000 openvalidators-1.0.4/openvalidators.egg-info/PKG-INFO
+-rw-r--r--   0 pedroferreira   (501) staff       (20)      580 2023-06-09 16:20:48.000000 openvalidators-1.0.4/openvalidators.egg-info/SOURCES.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)        1 2023-06-09 16:20:48.000000 openvalidators-1.0.4/openvalidators.egg-info/dependency_links.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)       68 2023-06-09 16:20:48.000000 openvalidators-1.0.4/openvalidators.egg-info/entry_points.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)      143 2023-06-09 16:20:48.000000 openvalidators-1.0.4/openvalidators.egg-info/requires.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)       15 2023-06-09 16:20:48.000000 openvalidators-1.0.4/openvalidators.egg-info/top_level.txt
+-rw-r--r--   0 pedroferreira   (501) staff       (20)       38 2023-06-09 16:20:48.831757 openvalidators-1.0.4/setup.cfg
+-rw-r--r--   0 pedroferreira   (501) staff       (20)     3496 2023-06-06 18:47:52.000000 openvalidators-1.0.4/setup.py
```

### Comparing `openvalidators-1.0.2/LICENSE` & `openvalidators-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.2/PKG-INFO` & `openvalidators-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: openvalidators
-Version: 1.0.2
+Version: 1.0.4
 Summary: Openvalidators is a collection of open source validators for the Bittensor Network.
 Home-page: https://github.com/opentensor/validators
 Author: bittensor.com
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: MIT
 Keywords: bittensor,validator,ai,machine-learning,deep-learning,blockchain,pytorch,torch,neural-networks,cryptocurrency
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -159,9 +158,7 @@
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
```

### Comparing `openvalidators-1.0.2/README.md` & `openvalidators-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.2/openvalidators/__init__.py` & `openvalidators-1.0.4/openvalidators/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 from . import neuron
 from . import prompts
 from . import reward
 from . import run
 from . import utils
 from . import weights
 
-__version__ = "1.0.2"
-__spec_version__ = 1003
+__version__ = "1.0.4"
+version_split = __version__.split(".")
+__spec_version__ = (1000 * int(version_split[0])) + (10 * int(version_split[1])) + (1 * int(version_split[2]))
```

### Comparing `openvalidators-1.0.2/openvalidators/config.py` & `openvalidators-1.0.4/openvalidators/config.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.2/openvalidators/dendrite.py` & `openvalidators-1.0.4/openvalidators/dendrite.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.2/openvalidators/forward.py` & `openvalidators-1.0.4/openvalidators/forward.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,20 +40,22 @@
         k (int): Number of uids to return.
         exclude (List[int]): List of uids to exclude from the random sampling.
     Returns:
         uids (torch.LongTensor): Randomly sampled available uids.
     Notes:
         If `k` is larger than the number of available `uids`, set `k` to the number of available `uids`.
     """
-    candidate_uids = [
-        uid
-        for uid in range(self.metagraph.n.item())
-        if check_uid_availability(self.metagraph, uid, self.config.neuron.vpermit_tao_limit)
-        and (exclude is None or uid not in exclude)
-    ]
+    candidate_uids = []
+
+    for uid in range(self.metagraph.n.item()):
+        uid_is_available = check_uid_availability(self.metagraph, uid, self.config.neuron.vpermit_tao_limit)
+        uid_is_not_excluded = (exclude is None or uid not in exclude)
+
+        if uid_is_available and uid_is_not_excluded:
+            candidate_uids.append(uid)
 
     available_uids = torch.tensor(candidate_uids, dtype=torch.int64).to(self.device)
     uids = torch.tensor(random.sample(available_uids.tolist(), k), dtype=torch.int64)
     return uids
 
 
 def is_successful_completion(self, response: bt.DendriteCall, min_len: int = 10, nsfw_bound_score: float = 0.5) -> bool:
@@ -335,22 +337,19 @@
         uids=answer_uids,
         roles=["user"],
         messages=[answer_prompt],
         completions=answer_completions,
         rewards=answer_rewards,
     )
 
-    # Compute forward pass rewards.
-    scattered_followup_rewards = (
-        torch.zeros((self.metagraph.n), dtype=torch.float32).to(self.device).scatter(0, followup_uids, followup_rewards)
-    )
-    scattered_answer_rewards = (
-        torch.zeros((self.metagraph.n), dtype=torch.float32).to(self.device).scatter(0, answer_uids, answer_rewards)
-    )
-    rewards = scattered_followup_rewards + scattered_answer_rewards
+    # Compute forward pass rewards, assumes followup_uids and answer_uids are mutually exclusive.
+    rewards = self.moving_averaged_scores.scatter(0, followup_uids, followup_rewards)
+    rewards = rewards.scatter(0, answer_uids, answer_rewards)
+
+    # Update moving_averaged_scores with rewards.
     self.moving_averaged_scores = self.config.neuron.moving_average_alpha * rewards.to(self.device) + (
         1 - self.config.neuron.moving_average_alpha
     ) * self.moving_averaged_scores.to(self.device)
 
     # Train the gating layer.
     scores = self.gating_model(answer_prompt).to(self.device)
     gating_loss = self.gating_model.backward(scores=scores[answer_uids], rewards=answer_rewards)
```

### Comparing `openvalidators-1.0.2/openvalidators/gating.py` & `openvalidators-1.0.4/openvalidators/gating.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.2/openvalidators/misc.py` & `openvalidators-1.0.4/openvalidators/misc.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.2/openvalidators/mock.py` & `openvalidators-1.0.4/openvalidators/mock.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.2/openvalidators/neuron.py` & `openvalidators-1.0.4/openvalidators/neuron.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.2/openvalidators/prompts.py` & `openvalidators-1.0.4/openvalidators/prompts.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.2/openvalidators/reward.py` & `openvalidators-1.0.4/openvalidators/reward.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.2/openvalidators/run.py` & `openvalidators-1.0.4/openvalidators/run.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.2/openvalidators/utils.py` & `openvalidators-1.0.4/openvalidators/utils.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.2/openvalidators/weights.py` & `openvalidators-1.0.4/openvalidators/weights.py`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.2/openvalidators.egg-info/PKG-INFO` & `openvalidators-1.0.4/openvalidators.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: openvalidators
-Version: 1.0.2
+Version: 1.0.4
 Summary: Openvalidators is a collection of open source validators for the Bittensor Network.
 Home-page: https://github.com/opentensor/validators
 Author: bittensor.com
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: MIT
 Keywords: bittensor,validator,ai,machine-learning,deep-learning,blockchain,pytorch,torch,neural-networks,cryptocurrency
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -159,9 +158,7 @@
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
```

### Comparing `openvalidators-1.0.2/openvalidators.egg-info/SOURCES.txt` & `openvalidators-1.0.4/openvalidators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openvalidators-1.0.2/setup.py` & `openvalidators-1.0.4/setup.py`

 * *Files identical despite different names*

