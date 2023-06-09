# Comparing `tmp/swoop.db-0.1.2.tar.gz` & `tmp/swoop.db-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swoop.db-0.1.2.tar", last modified: Thu Jun  8 21:08:26 2023, max compression
+gzip compressed data, was "swoop.db-0.1.3.tar", last modified: Fri Jun  9 13:21:24 2023, max compression
```

## Comparing `swoop.db-0.1.2.tar` & `swoop.db-0.1.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.644108 swoop.db-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.636107 swoop.db-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.640107 swoop.db-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.github/workflows/publish-image.yml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.github/workflows/snyk-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.snyk
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.sqlfluff
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-08 21:08:04.000000 swoop.db-0.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-08 21:08:04.000000 swoop.db-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-08 21:08:04.000000 swoop.db-0.1.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-08 21:08:04.000000 swoop.db-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-08 21:08:26.640107 swoop.db-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-08 21:08:04.000000 swoop.db-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-08 21:08:04.000000 swoop.db-0.1.2/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-08 21:08:04.000000 swoop.db-0.1.2/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-08 21:08:04.000000 swoop.db-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-08 21:08:04.000000 swoop.db-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 21:08:26.644108 swoop.db-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.636107 swoop.db-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.636107 swoop.db-0.1.2/src/swoop/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.640107 swoop.db-0.1.2/src/swoop/db/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-08 21:08:04.000000 swoop.db-0.1.2/src/swoop/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-08 21:08:04.000000 swoop.db-0.1.2/src/swoop/db/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-08 21:08:04.000000 swoop.db-0.1.2/src/swoop/db/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.640107 swoop.db-0.1.2/src/swoop/db/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-08 21:08:04.000000 swoop.db-0.1.2/src/swoop/db/fixtures/base_01.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.640107 swoop.db-0.1.2/src/swoop/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    15652 2023-06-08 21:08:04.000000 swoop.db-0.1.2/src/swoop/db/migrations/00000_base_schema.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:04.000000 swoop.db-0.1.2/src/swoop/db/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15807 2023-06-08 21:08:04.000000 swoop.db-0.1.2/src/swoop/db/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.640107 swoop.db-0.1.2/src/swoop.db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-08 21:08:26.000000 swoop.db-0.1.2/src/swoop.db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-08 21:08:26.000000 swoop.db-0.1.2/src/swoop.db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 21:08:26.000000 swoop.db-0.1.2/src/swoop.db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 21:08:26.000000 swoop.db-0.1.2/src/swoop.db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-08 21:08:26.000000 swoop.db-0.1.2/src/swoop.db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 21:08:26.000000 swoop.db-0.1.2/src/swoop.db.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.640107 swoop.db-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-08 21:08:04.000000 swoop.db-0.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.640107 swoop.db-0.1.2/tests/pgtap/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-08 21:08:04.000000 swoop.db-0.1.2/tests/pgtap/test_action.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-08 21:08:04.000000 swoop.db-0.1.2/tests/pgtap/test_item_inserts.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-08 21:08:04.000000 swoop.db-0.1.2/tests/pgtap/test_limit-locking.sql
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-08 21:08:04.000000 swoop.db-0.1.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-08 21:08:04.000000 swoop.db-0.1.2/tests/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.407055 swoop.db-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.github/workflows/publish-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.github/workflows/snyk-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.snyk
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-09 13:21:11.000000 swoop.db-0.1.3/.sqlfluff
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-09 13:21:11.000000 swoop.db-0.1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-09 13:21:11.000000 swoop.db-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-09 13:21:11.000000 swoop.db-0.1.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-09 13:21:11.000000 swoop.db-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-09 13:21:24.411055 swoop.db-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-09 13:21:11.000000 swoop.db-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-09 13:21:11.000000 swoop.db-0.1.3/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-09 13:21:11.000000 swoop.db-0.1.3/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-09 13:21:11.000000 swoop.db-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-09 13:21:11.000000 swoop.db-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 13:21:24.411055 swoop.db-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.407055 swoop.db-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.407055 swoop.db-0.1.3/src/swoop/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/src/swoop/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-09 13:21:11.000000 swoop.db-0.1.3/src/swoop/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-09 13:21:11.000000 swoop.db-0.1.3/src/swoop/db/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-09 13:21:11.000000 swoop.db-0.1.3/src/swoop/db/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/src/swoop/db/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-09 13:21:11.000000 swoop.db-0.1.3/src/swoop/db/fixtures/base_01.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/src/swoop/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-06-09 13:21:11.000000 swoop.db-0.1.3/src/swoop/db/migrations/00000_base_schema.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:11.000000 swoop.db-0.1.3/src/swoop/db/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-06-09 13:21:11.000000 swoop.db-0.1.3/src/swoop/db/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/src/swoop.db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-09 13:21:24.000000 swoop.db-0.1.3/src/swoop.db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-09 13:21:24.000000 swoop.db-0.1.3/src/swoop.db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:21:24.000000 swoop.db-0.1.3/src/swoop.db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 13:21:24.000000 swoop.db-0.1.3/src/swoop.db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-09 13:21:24.000000 swoop.db-0.1.3/src/swoop.db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 13:21:24.000000 swoop.db-0.1.3/src/swoop.db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-09 13:21:11.000000 swoop.db-0.1.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:24.411055 swoop.db-0.1.3/tests/pgtap/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-09 13:21:11.000000 swoop.db-0.1.3/tests/pgtap/test_action.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-09 13:21:11.000000 swoop.db-0.1.3/tests/pgtap/test_item_inserts.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-09 13:21:11.000000 swoop.db-0.1.3/tests/pgtap/test_limit-locking.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-09 13:21:11.000000 swoop.db-0.1.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-09 13:21:11.000000 swoop.db-0.1.3/tests/test_database.py
```

### Comparing `swoop.db-0.1.2/.github/workflows/publish-image.yml` & `swoop.db-0.1.3/.github/workflows/publish-image.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/.github/workflows/python-publish.yml` & `swoop.db-0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/.github/workflows/python-test.yml` & `swoop.db-0.1.3/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/.github/workflows/snyk-scan.yml` & `swoop.db-0.1.3/.github/workflows/snyk-scan.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/.gitignore` & `swoop.db-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/.pre-commit-config.yaml` & `swoop.db-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/.snyk` & `swoop.db-0.1.3/.snyk`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/CONTRIBUTING.md` & `swoop.db-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/Dockerfile` & `swoop.db-0.1.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/LICENSE` & `swoop.db-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/PKG-INFO` & `swoop.db-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 0.1.2
+Version: 0.1.3
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-0.1.2/README.md` & `swoop.db-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/RELEASE.md` & `swoop.db-0.1.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/docker-compose.yml` & `swoop.db-0.1.3/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/pyproject.toml` & `swoop.db-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/src/swoop/db/cli.py` & `swoop.db-0.1.3/src/swoop/db/cli.py`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/src/swoop/db/fixtures/base_01.sql` & `swoop.db-0.1.3/src/swoop/db/fixtures/base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/src/swoop/db/migrations/00000_base_schema.up.sql` & `swoop.db-0.1.3/src/swoop/db/migrations/00000_base_schema.up.sql`

 * *Files 3% similar despite different names*

```diff
@@ -434,71 +434,68 @@
     SELECT pg_advisory_unlock(to_regclass('swoop.thread')::oid::integer, _lock_id)
   );
 END;
 $$;
 
 CREATE FUNCTION swoop.check_cache(plhash bytea, wf_version smallint, wf_name text, invalid timestamptz)
 RETURNS RECORD
+LANGUAGE plpgsql VOLATILE
 AS $$
 DECLARE
   rec RECORD;
 BEGIN
     IF EXISTS (SELECT * FROM swoop.payload_cache WHERE payload_hash = plhash) THEN
-    -- cache already exists
+    -- An entry exists in the cache
         DECLARE
-            _status text;
-            _jobid uuid;
-            _payloadid uuid;
+            v_status text;
+            v_job_id uuid;
+            v_payload_id uuid;
         BEGIN
             SELECT t.status, t.action_uuid, p.payload_uuid
-            INTO _status,_jobid, _payloadid
+            INTO v_status, v_job_id, v_payload_id
             FROM swoop.payload_cache p
             INNER JOIN swoop.action a
             ON p.payload_uuid = a.payload_uuid
             INNER JOIN swoop.thread t
             ON a.action_uuid = t.action_uuid
             WHERE p.payload_hash = plhash
             ORDER BY t.created_at DESC
 			LIMIT 1;
 
-            IF _status IN ('RUNNING', 'PENDING', 'QUEUED', 'BACKOFF', 'SUCCESSFUL', 'INVALID') THEN
-            -- redirect to job details for that workflow, do not process
-                SELECT FALSE, _jobid INTO rec;
+            IF v_status IN ('RUNNING', 'PENDING', 'QUEUED', 'BACKOFF', 'SUCCESSFUL', 'INVALID') THEN
+            -- Redirect to job details for that workflow, and do not process
+                SELECT FALSE, v_job_id INTO rec;
             ELSE
-            --     -- this means there is already a record in both payload_cache and action tables for this
-            --     -- need to reprocess
+            -- Reprocess payload
                 DECLARE
-                    _ver smallint;
-                    _invalid timestamptz;
+                    n_version smallint;
+                    d_invalid timestamptz;
                 BEGIN
                     SELECT workflow_version, invalid_after
-                    INTO _ver, _invalid
+                    INTO n_version, d_invalid
                     FROM   swoop.payload_cache
                     WHERE  payload_hash = plhash;
 
-                    IF wf_version > _ver OR _invalid < NOW() THEN
-                        IF wf_version > _ver AND _invalid < NOW() THEN
+                    -- Check workflow version and invalidation
+                    IF wf_version > n_version OR d_invalid < NOW() THEN
+                        IF wf_version > n_version AND d_invalid < NOW() THEN
                             UPDATE swoop.payload_cache SET workflow_version = wf_version, invalid_after = NULL WHERE payload_hash = plhash;
-                        ELSIF wf_version > _ver THEN
+                        ELSIF wf_version > n_version THEN
                             UPDATE swoop.payload_cache SET workflow_version = wf_version WHERE payload_hash = plhash;
                         ELSE
                             UPDATE swoop.payload_cache SET invalid_after = NULL WHERE payload_hash = plhash;
                         END IF;
-
-                        -- reprocess the payload
-                        SELECT TRUE, _payloadid, gen_random_uuid() INTO rec;
-                    ELSE
-                        SELECT FALSE, _jobid INTO rec;
                     END IF;
+                    -- Reprocess payload with a new action_uuid
+                    SELECT TRUE, v_payload_id, gen_random_uuid() INTO rec;
                 END;
             END IF;
         END;
 	ELSE
+        -- Insert a new entry into cache table and process payload with a new action_uuid
         INSERT INTO swoop.payload_cache(payload_hash, workflow_version, workflow_name, invalid_after)
         VALUES (plhash, wf_version, wf_name, invalid)
         RETURNING TRUE, payload_uuid, gen_random_uuid() INTO rec;
-    -- process the payload
 	END IF;
     RETURN rec;
 END;
-$$
-LANGUAGE plpgsql;
+$$;
```

### Comparing `swoop.db-0.1.2/src/swoop/db/schema.sql` & `swoop.db-0.1.3/src/swoop/db/schema.sql`

 * *Files 3% similar despite different names*

```diff
@@ -442,71 +442,68 @@
     SELECT pg_advisory_unlock(to_regclass('swoop.thread')::oid::integer, _lock_id)
   );
 END;
 $$;
 
 CREATE FUNCTION swoop.check_cache(plhash bytea, wf_version smallint, wf_name text, invalid timestamptz)
 RETURNS RECORD
+LANGUAGE plpgsql VOLATILE
 AS $$
 DECLARE
   rec RECORD;
 BEGIN
     IF EXISTS (SELECT * FROM swoop.payload_cache WHERE payload_hash = plhash) THEN
-    -- cache already exists
+    -- An entry exists in the cache
         DECLARE
-            _status text;
-            _jobid uuid;
-            _payloadid uuid;
+            v_status text;
+            v_job_id uuid;
+            v_payload_id uuid;
         BEGIN
             SELECT t.status, t.action_uuid, p.payload_uuid
-            INTO _status,_jobid, _payloadid
+            INTO v_status, v_job_id, v_payload_id
             FROM swoop.payload_cache p
             INNER JOIN swoop.action a
             ON p.payload_uuid = a.payload_uuid
             INNER JOIN swoop.thread t
             ON a.action_uuid = t.action_uuid
             WHERE p.payload_hash = plhash
             ORDER BY t.created_at DESC
 			LIMIT 1;
 
-            IF _status IN ('RUNNING', 'PENDING', 'QUEUED', 'BACKOFF', 'SUCCESSFUL', 'INVALID') THEN
-            -- redirect to job details for that workflow, do not process
-                SELECT FALSE, _jobid INTO rec;
+            IF v_status IN ('RUNNING', 'PENDING', 'QUEUED', 'BACKOFF', 'SUCCESSFUL', 'INVALID') THEN
+            -- Redirect to job details for that workflow, and do not process
+                SELECT FALSE, v_job_id INTO rec;
             ELSE
-            --     -- this means there is already a record in both payload_cache and action tables for this
-            --     -- need to reprocess
+            -- Reprocess payload
                 DECLARE
-                    _ver smallint;
-                    _invalid timestamptz;
+                    n_version smallint;
+                    d_invalid timestamptz;
                 BEGIN
                     SELECT workflow_version, invalid_after
-                    INTO _ver, _invalid
+                    INTO n_version, d_invalid
                     FROM   swoop.payload_cache
                     WHERE  payload_hash = plhash;
 
-                    IF wf_version > _ver OR _invalid < NOW() THEN
-                        IF wf_version > _ver AND _invalid < NOW() THEN
+                    -- Check workflow version and invalidation
+                    IF wf_version > n_version OR d_invalid < NOW() THEN
+                        IF wf_version > n_version AND d_invalid < NOW() THEN
                             UPDATE swoop.payload_cache SET workflow_version = wf_version, invalid_after = NULL WHERE payload_hash = plhash;
-                        ELSIF wf_version > _ver THEN
+                        ELSIF wf_version > n_version THEN
                             UPDATE swoop.payload_cache SET workflow_version = wf_version WHERE payload_hash = plhash;
                         ELSE
                             UPDATE swoop.payload_cache SET invalid_after = NULL WHERE payload_hash = plhash;
                         END IF;
-
-                        -- reprocess the payload
-                        SELECT TRUE, _payloadid, gen_random_uuid() INTO rec;
-                    ELSE
-                        SELECT FALSE, _jobid INTO rec;
                     END IF;
+                    -- Reprocess payload with a new action_uuid
+                    SELECT TRUE, v_payload_id, gen_random_uuid() INTO rec;
                 END;
             END IF;
         END;
 	ELSE
+        -- Insert a new entry into cache table and process payload with a new action_uuid
         INSERT INTO swoop.payload_cache(payload_hash, workflow_version, workflow_name, invalid_after)
         VALUES (plhash, wf_version, wf_name, invalid)
         RETURNING TRUE, payload_uuid, gen_random_uuid() INTO rec;
-    -- process the payload
 	END IF;
     RETURN rec;
 END;
-$$
-LANGUAGE plpgsql;
+$$;
```

### Comparing `swoop.db-0.1.2/src/swoop.db.egg-info/PKG-INFO` & `swoop.db-0.1.3/src/swoop.db.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 0.1.2
+Version: 0.1.3
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-0.1.2/src/swoop.db.egg-info/SOURCES.txt` & `swoop.db-0.1.3/src/swoop.db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/tests/conftest.py` & `swoop.db-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/tests/pgtap/test_action.sql` & `swoop.db-0.1.3/tests/pgtap/test_action.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/tests/pgtap/test_item_inserts.sql` & `swoop.db-0.1.3/tests/pgtap/test_item_inserts.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.2/tests/pgtap/test_limit-locking.sql` & `swoop.db-0.1.3/tests/pgtap/test_limit-locking.sql`

 * *Files identical despite different names*

