# Comparing `tmp/qdrant_tools-0.0.1.tar.gz` & `tmp/qdrant_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_tools-0.0.1.tar", max compression
+gzip compressed data, was "qdrant_tools-0.0.2.tar", max compression
```

## Comparing `qdrant_tools-0.0.1.tar` & `qdrant_tools-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-06-08 09:46:17.915415 qdrant_tools-0.0.1/LICENSE
--rw-r--r--   0        0        0    16740 2023-06-07 08:39:41.202548 qdrant_tools-0.0.1/README.md
--rw-r--r--   0        0        0      391 2023-06-08 15:57:47.987147 qdrant_tools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      110 2023-06-08 09:43:33.573836 qdrant_tools-0.0.1/qdrant_tools/README.md
--rw-r--r--   0        0        0        0 2023-06-08 09:43:33.573544 qdrant_tools-0.0.1/qdrant_tools/__init__.py
--rw-r--r--   0        0        0       43 2023-06-08 09:43:33.573347 qdrant_tools-0.0.1/qdrant_tools/requirements.txt
--rw-r--r--   0        0        0     4041 2023-06-08 13:27:04.352078 qdrant_tools-0.0.1/qdrant_tools/vectordb.py
--rw-r--r--   0        0        0    17337 1970-01-01 00:00:00.000000 qdrant_tools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-08 09:46:17.915415 qdrant_tools-0.0.2/LICENSE
+-rw-r--r--   0        0        0    17801 2023-06-09 06:38:08.001002 qdrant_tools-0.0.2/README.md
+-rw-r--r--   0        0        0      391 2023-06-09 06:38:55.494069 qdrant_tools-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-06-08 09:43:33.573836 qdrant_tools-0.0.2/qdrant_tools/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 09:43:33.573544 qdrant_tools-0.0.2/qdrant_tools/__init__.py
+-rw-r--r--   0        0        0       43 2023-06-08 09:43:33.573347 qdrant_tools-0.0.2/qdrant_tools/requirements.txt
+-rw-r--r--   0        0        0     4041 2023-06-08 13:27:04.352078 qdrant_tools-0.0.2/qdrant_tools/vectordb.py
+-rw-r--r--   0        0        0    18398 1970-01-01 00:00:00.000000 qdrant_tools-0.0.2/PKG-INFO
```

### Comparing `qdrant_tools-0.0.1/LICENSE` & `qdrant_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_tools-0.0.1/README.md` & `qdrant_tools-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,67 @@
+Metadata-Version: 2.1
+Name: qdrant-tools
+Version: 0.0.2
+Summary: 
+License: MIT
+Author: NirantK
+Author-email: nirant.bits@gmail.com
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pinecone-client (>=2.2.2,<3.0.0)
+Requires-Dist: qdrant-client (>=1.2.0,<2.0.0)
+Description-Content-Type: text/markdown
+
 # Migrating from Pinecone to Qdrant Vector Database: A Comprehensive Guide
 
+## Installation
+
+```python
+pip install qdrant-tools
+```
+
+## Usage
+
+```
+from qdrant_tools.vectordb import PineconeExport, QdrantImport, QdrantMode
+index_name = "hindi-search" # Existing Pinecone index name
+
+# Init Pinecone
+
+pinecone_export = PineconeExport(index_name=index_name)
+print(pinecone_export.index.describe_index_stats())
+source_index = pinecone_export.index
+
+# Fetch all vector ids from Pinecone
+
+vector_ids = ["1", "2", "3", "4", "5"] # Example vector ids, list of strings -- this is the main input for the replication
+points = pinecone_export.fetch_vectors(vector_ids) # Fetch vectors from Pinecone
+
+# Init Qdrant
+
+vector_dimension = source_index.describe_index_stats()[
+"dimension"
+] # Get dimension from existing index
+qdrant = QdrantImport(mode=QdrantMode.local)
+qdrant.create_collection(index_name, vector_dimension)
+qdrant.upsert_vectors(index_name, vector_ids, source_index) # source_index is a pinecone index object
+
+
+# Testing if it works!
+qdrant.qdrant_client.search(
+    collection_name=index_name,
+    query_vector= # query_vector
+)
+```
+
 ## Introduction
 
 Are you considering a transition from Pinecone to Qdrant? If so, this article will guide you through the process, outlining the similarities and differences between the two systems, and providing a step-by-step migration plan.
 
 ### Understanding the Terminology
 
 Before diving into the migration process, it's important to familiarize yourself with some key terms.
@@ -231,7 +289,8 @@
 3. **Compliance and Certifications**: While Pinecone's SOC2 Type II certification and GDPR-readiness are reassuring, they may not be sufficient for some organizations who want to work strictly within their VPC. This means deploying an on-premise of Pinecone under enterprise offering, which can be prohibitively expensive for some organizations.ß
 
 4. **Security Policies and Practices**: Pinecone's rigorous security policies may not align with the security practices of all organizations. This also moves the burden of finding the difference between the security policies and ironing them out to the end user.
 
 5. **Incident Management and Monitoring**: Pinecone's incident management and monitoring practices are not integrated with the organisation's existing incident management and monitoring systems, potentially complicating incident response.
 
 In conclusion, Qdrant's minimalist approach to security allows for greater flexibility and customization according to the specific needs of the deployment environment. It puts the control of security measures in the hands of the deployer, allowing for robust, tailored security configurations. On the other hand, Pinecone's built-in security measures and compliance certifications provide a comprehensive, ready-to-use security solution that may not provide the same level of customization as Qdrant. The choice between the two depends largely on the specific security needs of your application and the flexibility of your deployment environment.
+
```

### Comparing `qdrant_tools-0.0.1/qdrant_tools/vectordb.py` & `qdrant_tools-0.0.2/qdrant_tools/vectordb.py`

 * *Files identical despite different names*

### Comparing `qdrant_tools-0.0.1/PKG-INFO` & `qdrant_tools-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,49 @@
-Metadata-Version: 2.1
-Name: qdrant-tools
-Version: 0.0.1
-Summary: 
-License: MIT
-Author: NirantK
-Author-email: nirant.bits@gmail.com
-Requires-Python: >=3.8,<3.12
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pinecone-client (>=2.2.2,<3.0.0)
-Requires-Dist: qdrant-client (>=1.2.0,<2.0.0)
-Description-Content-Type: text/markdown
-
 # Migrating from Pinecone to Qdrant Vector Database: A Comprehensive Guide
 
+## Installation
+
+```python
+pip install qdrant-tools
+```
+
+## Usage
+
+```
+from qdrant_tools.vectordb import PineconeExport, QdrantImport, QdrantMode
+index_name = "hindi-search" # Existing Pinecone index name
+
+# Init Pinecone
+
+pinecone_export = PineconeExport(index_name=index_name)
+print(pinecone_export.index.describe_index_stats())
+source_index = pinecone_export.index
+
+# Fetch all vector ids from Pinecone
+
+vector_ids = ["1", "2", "3", "4", "5"] # Example vector ids, list of strings -- this is the main input for the replication
+points = pinecone_export.fetch_vectors(vector_ids) # Fetch vectors from Pinecone
+
+# Init Qdrant
+
+vector_dimension = source_index.describe_index_stats()[
+"dimension"
+] # Get dimension from existing index
+qdrant = QdrantImport(mode=QdrantMode.local)
+qdrant.create_collection(index_name, vector_dimension)
+qdrant.upsert_vectors(index_name, vector_ids, source_index) # source_index is a pinecone index object
+
+
+# Testing if it works!
+qdrant.qdrant_client.search(
+    collection_name=index_name,
+    query_vector= # query_vector
+)
+```
+
 ## Introduction
 
 Are you considering a transition from Pinecone to Qdrant? If so, this article will guide you through the process, outlining the similarities and differences between the two systems, and providing a step-by-step migration plan.
 
 ### Understanding the Terminology
 
 Before diving into the migration process, it's important to familiarize yourself with some key terms.
@@ -249,8 +271,7 @@
 3. **Compliance and Certifications**: While Pinecone's SOC2 Type II certification and GDPR-readiness are reassuring, they may not be sufficient for some organizations who want to work strictly within their VPC. This means deploying an on-premise of Pinecone under enterprise offering, which can be prohibitively expensive for some organizations.ß
 
 4. **Security Policies and Practices**: Pinecone's rigorous security policies may not align with the security practices of all organizations. This also moves the burden of finding the difference between the security policies and ironing them out to the end user.
 
 5. **Incident Management and Monitoring**: Pinecone's incident management and monitoring practices are not integrated with the organisation's existing incident management and monitoring systems, potentially complicating incident response.
 
 In conclusion, Qdrant's minimalist approach to security allows for greater flexibility and customization according to the specific needs of the deployment environment. It puts the control of security measures in the hands of the deployer, allowing for robust, tailored security configurations. On the other hand, Pinecone's built-in security measures and compliance certifications provide a comprehensive, ready-to-use security solution that may not provide the same level of customization as Qdrant. The choice between the two depends largely on the specific security needs of your application and the flexibility of your deployment environment.
-
```

