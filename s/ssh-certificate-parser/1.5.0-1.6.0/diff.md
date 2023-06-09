# Comparing `tmp/ssh_certificate_parser-1.5.0.tar.gz` & `tmp/ssh_certificate_parser-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_certificate_parser-1.5.0.tar", last modified: Wed May 24 15:24:45 2023, max compression
+gzip compressed data, was "ssh_certificate_parser-1.6.0.tar", last modified: Fri Jun  9 17:46:22 2023, max compression
```

## Comparing `ssh_certificate_parser-1.5.0.tar` & `ssh_certificate_parser-1.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-05-24 15:24:44.999946 ssh_certificate_parser-1.5.0/
--rw-r--r--   0 jhammond   (502) staff       (20)     1049 2023-05-24 15:20:42.000000 ssh_certificate_parser-1.5.0/CHANGES.md
--rw-r--r--   0 jhammond   (502) staff       (20)      754 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.5.0/LICENSE.txt
--rw-r--r--   0 jhammond   (502) staff       (20)       27 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.5.0/MANIFEST.in
--rw-r--r--   0 jhammond   (502) staff       (20)     2289 2023-05-24 15:24:44.999780 ssh_certificate_parser-1.5.0/PKG-INFO
--rw-r--r--   0 jhammond   (502) staff       (20)     1179 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.5.0/README.md
--rw-r--r--   0 jhammond   (502) staff       (20)       38 2023-05-24 15:24:44.999995 ssh_certificate_parser-1.5.0/setup.cfg
--rwxr-xr-x   0 jhammond   (502) staff       (20)     1378 2023-05-24 15:20:42.000000 ssh_certificate_parser-1.5.0/setup.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-05-24 15:24:44.998197 ssh_certificate_parser-1.5.0/ssh_certificate_parser/
--rw-r--r--   0 jhammond   (502) staff       (20)     6334 2023-05-24 14:36:25.000000 ssh_certificate_parser-1.5.0/ssh_certificate_parser/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)      335 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.5.0/ssh_certificate_parser/__main__.py
--rw-r--r--   0 jhammond   (502) staff       (20)      548 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.5.0/ssh_certificate_parser/errors.py
--rw-r--r--   0 jhammond   (502) staff       (20)      946 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.5.0/ssh_certificate_parser/parser_helpers.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-05-24 15:24:44.999015 ssh_certificate_parser-1.5.0/ssh_certificate_parser.egg-info/
--rw-r--r--   0 jhammond   (502) staff       (20)     2289 2023-05-24 15:24:44.000000 ssh_certificate_parser-1.5.0/ssh_certificate_parser.egg-info/PKG-INFO
--rw-r--r--   0 jhammond   (502) staff       (20)      499 2023-05-24 15:24:44.000000 ssh_certificate_parser-1.5.0/ssh_certificate_parser.egg-info/SOURCES.txt
--rw-r--r--   0 jhammond   (502) staff       (20)        1 2023-05-24 15:24:44.000000 ssh_certificate_parser-1.5.0/ssh_certificate_parser.egg-info/dependency_links.txt
--rw-r--r--   0 jhammond   (502) staff       (20)       10 2023-05-24 15:24:44.000000 ssh_certificate_parser-1.5.0/ssh_certificate_parser.egg-info/requires.txt
--rw-r--r--   0 jhammond   (502) staff       (20)       23 2023-05-24 15:24:44.000000 ssh_certificate_parser-1.5.0/ssh_certificate_parser.egg-info/top_level.txt
--rw-r--r--   0 jhammond   (502) staff       (20)       80 2023-03-14 17:09:46.000000 ssh_certificate_parser-1.5.0/test_requirements.txt
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-05-24 15:24:44.999446 ssh_certificate_parser-1.5.0/tests/
--rw-r--r--   0 jhammond   (502) staff       (20)     3943 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.5.0/tests/test_basic.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1540 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.5.0/tests/test_parser_functions.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-09 17:46:22.099721 ssh_certificate_parser-1.6.0/
+-rw-r--r--   0 jhammond   (502) staff       (20)     1145 2023-06-09 17:45:41.000000 ssh_certificate_parser-1.6.0/CHANGES.md
+-rw-r--r--   0 jhammond   (502) staff       (20)      754 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.6.0/LICENSE.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)       27 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.6.0/MANIFEST.in
+-rw-r--r--   0 jhammond   (502) staff       (20)     2418 2023-06-09 17:46:22.099575 ssh_certificate_parser-1.6.0/PKG-INFO
+-rw-r--r--   0 jhammond   (502) staff       (20)     1308 2023-06-09 17:45:41.000000 ssh_certificate_parser-1.6.0/README.md
+-rw-r--r--   0 jhammond   (502) staff       (20)       38 2023-06-09 17:46:22.099765 ssh_certificate_parser-1.6.0/setup.cfg
+-rwxr-xr-x   0 jhammond   (502) staff       (20)     1378 2023-06-09 17:45:41.000000 ssh_certificate_parser-1.6.0/setup.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-09 17:46:22.098278 ssh_certificate_parser-1.6.0/ssh_certificate_parser/
+-rw-r--r--   0 jhammond   (502) staff       (20)     6794 2023-06-09 17:04:41.000000 ssh_certificate_parser-1.6.0/ssh_certificate_parser/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      335 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.6.0/ssh_certificate_parser/__main__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      548 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.6.0/ssh_certificate_parser/errors.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      946 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.6.0/ssh_certificate_parser/parser_helpers.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-09 17:46:22.099077 ssh_certificate_parser-1.6.0/ssh_certificate_parser.egg-info/
+-rw-r--r--   0 jhammond   (502) staff       (20)     2418 2023-06-09 17:46:22.000000 ssh_certificate_parser-1.6.0/ssh_certificate_parser.egg-info/PKG-INFO
+-rw-r--r--   0 jhammond   (502) staff       (20)      499 2023-06-09 17:46:22.000000 ssh_certificate_parser-1.6.0/ssh_certificate_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)        1 2023-06-09 17:46:22.000000 ssh_certificate_parser-1.6.0/ssh_certificate_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)       10 2023-06-09 17:46:22.000000 ssh_certificate_parser-1.6.0/ssh_certificate_parser.egg-info/requires.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)       23 2023-06-09 17:46:22.000000 ssh_certificate_parser-1.6.0/ssh_certificate_parser.egg-info/top_level.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)      119 2023-06-09 17:45:41.000000 ssh_certificate_parser-1.6.0/test_requirements.txt
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-09 17:46:22.099362 ssh_certificate_parser-1.6.0/tests/
+-rw-r--r--   0 jhammond   (502) staff       (20)     4985 2023-06-09 17:04:41.000000 ssh_certificate_parser-1.6.0/tests/test_basic.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1540 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.6.0/tests/test_parser_functions.py
```

### Comparing `ssh_certificate_parser-1.5.0/CHANGES.md` & `ssh_certificate_parser-1.6.0/CHANGES.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-ChangeLog
-=========
+# CHANGELOG
 
-1.5.0
------
+## v1.6.0
+
+- Adds support for certs that last forever
+- Adds support for `ed25519` certs
+
+## v1.5.0
 
 - Adds proper support for `ecdsa-sha2-nistp256`
 
-1.4.0
------
+## v1.4.0
 
 - Adds proper support for `ecdsa-sha2-nistp384`
 
-1.3.3
------
+## v1.3.3
 
 - Fix RtD link issue
 
-1.3.2
------
+## v1.3.2
 
 - Fix PyPI project URLs
 
-1.3.1
------
+## v1.3.1
 
 - Fix `setup.py` issues
 
-1.3.0
------
+## v1.3.0
 
 - Can now parse ECDSA keys (if they're signed with an RSA CA)
 - Add `.from_file` constructor on `SSHCertificate`
 - Add a bunch of type hints
 - Improve documentation a bit
 
-1.2.0
------
+## v1.2.0
 
 - Can now parse DSA and Ed25519 keys (although they still have to have been signed by an RSA CA)
 - Unit tests
 - `key_type` is now in the `SSHCertificate` object
 - `pubkey_parts` is a dictionary containing the appropriate parts for that key (e.g., `n` and `e` for RSA)
 - Now raises subclasses of `ssh_certificate_parser.errors.SSHCertificateParserError` instead of just `ValueError` with a string description
 
-1.1.0
------
+## v1.1.0
 
 - CA certificate fingerprint (equivalent to `ssh-keygen -l -f /path/to/key.pub`) is now parsed for ssh-rsa CAs. I don't have any ECDSA/Ed25519 CAs so I haven't tested them!
+
+## v1.0.0
+
+- Initial release
```

### Comparing `ssh_certificate_parser-1.5.0/LICENSE.txt` & `ssh_certificate_parser-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssh_certificate_parser-1.5.0/PKG-INFO` & `ssh_certificate_parser-1.6.0/ssh_certificate_parser.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ssh_certificate_parser
-Version: 1.5.0
+Name: ssh-certificate-parser
+Version: 1.6.0
 Summary: Python library for interacting with OpenSSH Certificates
 Home-page: https://github.com/easypost/ssh_certificate_parser
 Author: James Brown
 Author-email: jbrown@easypost.com
 License: ISC
 Project-URL: Docs, https://ssh-certificate-parser.readthedocs.io/
 Project-URL: Tracker, https://github.com/EasyPost/ssh_certificate_parser/issues
@@ -40,7 +40,21 @@
 
 cert = SSHCertificate.from_file('/etc/ssh/ssh_host_rsa_key-cert.pub')
 
 remaining_seconds_of_validity = cert.remaining_validity
 ```
 
 Full documentation is at <https://ssh-certificate-parser.readthedocs.io/en/latest/>.
+
+## Development
+
+```sh
+# Install dependencies
+make install
+
+# Lint project
+make lint
+
+# Test project
+make test
+make coverage
+```
```

### Comparing `ssh_certificate_parser-1.5.0/README.md` & `ssh_certificate_parser-1.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,7 +14,21 @@
 
 cert = SSHCertificate.from_file('/etc/ssh/ssh_host_rsa_key-cert.pub')
 
 remaining_seconds_of_validity = cert.remaining_validity
 ```
 
 Full documentation is at <https://ssh-certificate-parser.readthedocs.io/en/latest/>.
+
+## Development
+
+```sh
+# Install dependencies
+make install
+
+# Lint project
+make lint
+
+# Test project
+make test
+make coverage
+```
```

### Comparing `ssh_certificate_parser-1.5.0/setup.py` & `ssh_certificate_parser-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="ssh_certificate_parser",
-    version="1.5.0",
+    version="1.6.0",
     author="James Brown",
     author_email="jbrown@easypost.com",
     url="https://github.com/easypost/ssh_certificate_parser",
     license="ISC",
     packages=find_packages(exclude=["tests"]),
     description="Python library for interacting with OpenSSH Certificates",
     long_description=open("README.md", "r").read(),
```

### Comparing `ssh_certificate_parser-1.5.0/ssh_certificate_parser/__init__.py` & `ssh_certificate_parser-1.6.0/ssh_certificate_parser/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,14 +44,18 @@
     modulus = byte_array[:modulus_len]
     byte_array = byte_array[modulus_len:]
     exponent_len, byte_array = take_u32(byte_array)
     exponent = byte_array[:exponent_len]
     return RSAPublicKey(modulus=modulus, exponent=exponent, raw=raw_pubkey)
 
 
+def take_ed25519_cert(raw_pubkey):
+    return PublicKey(raw=raw_pubkey)
+
+
 def utcnow():
     return datetime.datetime.utcnow()  # pragma: no cover
 
 
 @attr.s
 class SSHCertificate(object):
     """Representation of a signed SSH certificate"""
@@ -140,22 +144,29 @@
         cert_type, blob = take_u32(blob)
         cert_type = CertType(cert_type)
         key_id, blob = take_pascal_string(blob)
         principals, blob = take_list(blob, take_pascal_string)
         valid_after, blob = take_u64(blob)
         valid_after = datetime.datetime.utcfromtimestamp(valid_after)
         valid_before, blob = take_u64(blob)
-        valid_before = datetime.datetime.utcfromtimestamp(valid_before)
+        # Forever certificate may be large, change to a value that can be handled by CPython
+        max_python_datetime = datetime.datetime(year=9999, month=12, day=31)
+        if valid_before > max_python_datetime.timestamp():
+            valid_before = max_python_datetime
+        else:
+            valid_before = datetime.datetime.utcfromtimestamp(valid_before)
         crits, blob = take_list(blob, take_pascal_string)
         exts, blob = take_list(blob, take_pascal_string)
         unknown, blob = take_pascal_bytestring(blob)
         raw_ca, blob = take_pascal_bytestring(blob)
         ca_cert_type, raw_ca_rest = take_pascal_string(raw_ca)
         if ca_cert_type in ('ssh-rsa', 'ecdsa-sha2-nistp256', 'ecdsa-sha2-nistp384'):
             ca_cert = take_rsa_cert(raw_ca, raw_ca_rest)
+        elif ca_cert_type == 'ssh-ed25519':
+            ca_cert = take_ed25519_cert(raw_ca)
         else:
             raise UnsupportedCertificateTypeError(ca_cert_type)
         signature = blob
         return SSHCertificate(
             serial, cert_type, key_id, principals, valid_after, valid_before,
             crits, exts, ca_cert, signature, key_type, pubkey_parts
         )
```

### Comparing `ssh_certificate_parser-1.5.0/ssh_certificate_parser/errors.py` & `ssh_certificate_parser-1.6.0/ssh_certificate_parser/errors.py`

 * *Files identical despite different names*

### Comparing `ssh_certificate_parser-1.5.0/ssh_certificate_parser/parser_helpers.py` & `ssh_certificate_parser-1.6.0/ssh_certificate_parser/parser_helpers.py`

 * *Files identical despite different names*

### Comparing `ssh_certificate_parser-1.5.0/ssh_certificate_parser.egg-info/PKG-INFO` & `ssh_certificate_parser-1.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ssh-certificate-parser
-Version: 1.5.0
+Name: ssh_certificate_parser
+Version: 1.6.0
 Summary: Python library for interacting with OpenSSH Certificates
 Home-page: https://github.com/easypost/ssh_certificate_parser
 Author: James Brown
 Author-email: jbrown@easypost.com
 License: ISC
 Project-URL: Docs, https://ssh-certificate-parser.readthedocs.io/
 Project-URL: Tracker, https://github.com/EasyPost/ssh_certificate_parser/issues
@@ -40,7 +40,21 @@
 
 cert = SSHCertificate.from_file('/etc/ssh/ssh_host_rsa_key-cert.pub')
 
 remaining_seconds_of_validity = cert.remaining_validity
 ```
 
 Full documentation is at <https://ssh-certificate-parser.readthedocs.io/en/latest/>.
+
+## Development
+
+```sh
+# Install dependencies
+make install
+
+# Lint project
+make lint
+
+# Test project
+make test
+make coverage
+```
```

### Comparing `ssh_certificate_parser-1.5.0/tests/test_basic.py` & `ssh_certificate_parser-1.6.0/tests/test_basic.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,14 +26,35 @@
     assert d['cert_type'] == 'SSH2_CERT_TYPE_HOST'
     assert d['crits'] == []
     assert d['exts'] == []
 
     assert isinstance(cert.ca, RSAPublicKey)
 
 
+def test_forever_cert(mocker):
+    with open('tests/data/web4_rsa_key-cert.pub', 'rb') as f:
+        cert = SSHCertificate.from_bytes(f.read())
+    assert cert.valid_after == datetime.datetime(1970, 1, 1, 0, 0, 0)
+    assert cert.valid_before == datetime.datetime(9999, 12, 31, 0, 0, 0)
+    assert cert.key_id == 'web4'
+    assert cert.principals == ['web4.example.com']
+    assert cert.serial == 0
+    mocker.patch('ssh_certificate_parser.utcnow', return_value=datetime.datetime(1970, 1, 2, 0, 0, 0))
+    assert cert.remaining_validity > 0
+    mocker.patch('ssh_certificate_parser.utcnow', return_value=datetime.datetime(2018, 2, 5, 0, 0, 0))
+    assert cert.remaining_validity > 0
+    mocker.patch('ssh_certificate_parser.utcnow', return_value=datetime.datetime(2099, 3, 8, 0, 0, 0))
+    assert cert.remaining_validity > 0
+    d = cert.asdict()
+    assert d['ca_fingerprint'] == 'SHA256:sZ8QWMpND0GZa8pm3MFNV8nHB2+ssdukl/FyZ49JBgU'
+    assert d['cert_type'] == 'SSH2_CERT_TYPE_USER'
+    assert d['crits'] == []
+    assert d['exts'] == []
+
+
 def test_ed25519_cert():
     with open('tests/data/web1_ed25519_key-cert.pub', 'rb') as f:
         cert = SSHCertificate.from_bytes(f.read())
     assert cert.key_type == 'ssh-ed25519-cert-v01@openssh.com'
     assert cert.valid_after == datetime.datetime(2018, 10, 9, 0, 8, 1)
     assert cert.valid_before == datetime.datetime(2019, 10, 15, 0, 8, 1)
     assert cert.key_id == 'web1'
```

### Comparing `ssh_certificate_parser-1.5.0/tests/test_parser_functions.py` & `ssh_certificate_parser-1.6.0/tests/test_parser_functions.py`

 * *Files identical despite different names*

