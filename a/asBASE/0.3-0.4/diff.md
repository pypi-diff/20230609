# Comparing `tmp/asBASE-0.3.tar.gz` & `tmp/asBASE-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asBASE-0.3.tar", last modified: Sat May 27 12:56:47 2023, max compression
+gzip compressed data, was "asBASE-0.4.tar", last modified: Thu Jun  8 23:35:50 2023, max compression
```

## Comparing `asBASE-0.3.tar` & `asBASE-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-27 12:56:47.759232 asBASE-0.3/
--rw-rw----   0 root         (0) everybody  (9997)       20 2023-05-26 23:55:19.000000 asBASE-0.3/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)      320 2023-05-27 12:56:47.735232 asBASE-0.3/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      818 2023-05-27 00:54:02.000000 asBASE-0.3/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-27 12:56:47.595232 asBASE-0.3/asBASE/
--rw-rw----   0 root         (0) everybody  (9997)     2183 2023-05-27 12:55:57.000000 asBASE-0.3/asBASE/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-27 12:56:47.711232 asBASE-0.3/asBASE.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      320 2023-05-27 12:56:47.000000 asBASE-0.3/asBASE.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      169 2023-05-27 12:56:47.000000 asBASE-0.3/asBASE.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-27 12:56:47.000000 asBASE-0.3/asBASE.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        7 2023-05-27 12:56:47.000000 asBASE-0.3/asBASE.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-27 12:56:47.763232 asBASE-0.3/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      361 2023-05-27 12:56:33.000000 asBASE-0.3/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 23:35:50.681495 asBASE-0.4/
+-rw-rw----   0 root         (0) everybody  (9997)       20 2023-05-26 23:55:19.000000 asBASE-0.4/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)      320 2023-06-08 23:35:50.669495 asBASE-0.4/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      818 2023-05-27 00:54:02.000000 asBASE-0.4/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 23:35:50.581495 asBASE-0.4/asBASE/
+-rw-rw----   0 root         (0) everybody  (9997)     2611 2023-06-08 23:34:26.000000 asBASE-0.4/asBASE/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 23:35:50.649495 asBASE-0.4/asBASE.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      320 2023-06-08 23:35:50.000000 asBASE-0.4/asBASE.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      169 2023-06-08 23:35:50.000000 asBASE-0.4/asBASE.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-08 23:35:50.000000 asBASE-0.4/asBASE.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        7 2023-06-08 23:35:50.000000 asBASE-0.4/asBASE.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-08 23:35:50.681495 asBASE-0.4/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      361 2023-06-08 23:35:35.000000 asBASE-0.4/setup.py
```

### Comparing `asBASE-0.3/README.md` & `asBASE-0.4/README.md`

 * *Files identical despite different names*

### Comparing `asBASE-0.3/asBASE/__init__.py` & `asBASE-0.4/asBASE/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 		json_dict = self.read_json()
 		json_dict[key] = value
 		self.write_json(json_dict)
 	def get(self, key):
 		json_dict = self.read_json()
 		if key in json_dict:
 			if "time" in json_dict and "expire" in json_dict["time"] and key in json_dict["time"]["expire"]:
-				if json_dict["time"]["expire"][key] < time.time():
+				if json_dict["time"]["expire"][key] <= time.time():
 					del json_dict["time"]["expire"][key]
 					del json_dict[key]
 					self.write_json(json_dict)
 					return None
 			return json_dict[key]
 	def sismember(self, key, member):
 		json_dict = self.read_json()
@@ -28,20 +28,28 @@
 			json_dict["time"]["expire"][key] = time.time() + ttl
 			self.write_json(json_dict)
 			return True
 		return False
 	def sadd(self, key, *values):
 		json_dict = self.read_json()
 		if "set" in json_dict.get(key, {}):
-			json_dict[key]["set"].extend(values)
+			for value in values:
+				if value not in json_dict[key]["set"]:
+					json_dict[key]["set"].append(value)
 		else:
 			json_dict[key] = {"set": list(values)}
 		self.write_json(json_dict)
 	def smembers(self, key):
 		json_dict = self.read_json()
+		if "time" in json_dict and "expire" in json_dict["time"] and key in json_dict["time"]["expire"]:
+			if json_dict["time"]["expire"][key] <= time.time():
+				del json_dict["time"]["expire"][key]
+				del json_dict[key]
+				self.write_json(json_dict)
+				return None
 		return json_dict.get(key, {}).get("set", [])
 	def srem(self, key, value):
 		json_dict = self.read_json()
 		if "set" in json_dict.get(key, {}):
 			if value in json_dict[key]["set"]:
 				json_dict[key]["set"].remove(value)
 				self.write_json(json_dict)
@@ -54,14 +62,19 @@
 		return False
 	def ttl(self, key):
 		json_dict = self.read_json()
 		if "time" in json_dict and "expire" in json_dict["time"] and key in json_dict["time"]["expire"]:
 			ttl = json_dict["time"]["expire"][key] - time.time()
 			return max(0, int(ttl))
 		return None
+	def scard(self, key):
+		try:
+			return int(len(self.smembers(key)))
+		except:
+			return None
 	def read_json(self):
 		try:
 			with open(self.filename, "r") as f:
 				json_str = f.read()
 				return json.loads(json_str)
 		except:
 			return {}
```

