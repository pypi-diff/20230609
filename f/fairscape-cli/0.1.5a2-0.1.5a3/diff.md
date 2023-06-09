# Comparing `tmp/fairscape_cli-0.1.5a2.tar.gz` & `tmp/fairscape_cli-0.1.5a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairscape_cli-0.1.5a2.tar", max compression
+gzip compressed data, was "fairscape_cli-0.1.5a3.tar", max compression
```

## Comparing `fairscape_cli-0.1.5a2.tar` & `fairscape_cli-0.1.5a3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     1066 2023-01-06 17:27:00.899279 fairscape_cli-0.1.5a2/LICENSE
--rw-r--r--   0        0        0     4058 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a2/README.md
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a2/fairscape_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a2/fairscape_cli/apps/__init__.py
--rw-r--r--   0        0        0      274 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a2/fairscape_cli/apps/cache.py
--rw-r--r--   0        0        0      510 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a2/fairscape_cli/apps/describe.py
--rw-r--r--   0        0        0      764 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/fairscape.py
--rw-r--r--   0        0        0       89 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/list.py
--rw-r--r--   0        0        0      173 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/models/__init__.py
--rw-r--r--   0        0        0      340 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/models/computation.py
--rw-r--r--   0        0        0     2559 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/models/dataset.py
--rw-r--r--   0        0        0     1890 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/models/software.py
--rw-r--r--   0        0        0     8135 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/objects.py
--rw-r--r--   0        0        0     3369 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/rocrate.py
--rw-r--r--   0        0        0     2276 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/utils.py
--rw-r--r--   0        0        0     2677 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/validator.py
--rw-r--r--   0        0        0      397 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5a2/fairscape_cli/main.py
--rw-r--r--   0        0        0      285 2023-05-11 18:22:39.597260 fairscape_cli-0.1.5a2/fairscape_cli/models/__init__.py
--rw-r--r--   0        0        0      291 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5a2/fairscape_cli/models/computation.py
--rw-r--r--   0        0        0      205 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/models/dataset.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/models/models.py
--rw-r--r--   0        0        0     4861 2023-05-17 17:28:34.300407 fairscape_cli-0.1.5a2/fairscape_cli/models/rocrate.py
--rw-r--r--   0        0        0    13053 2023-05-15 16:54:08.216085 fairscape_cli-0.1.5a2/fairscape_cli/models/schema.py
--rw-r--r--   0        0        0      128 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5a2/fairscape_cli/models/software.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/rocrate/__init__.py
--rw-r--r--   0        0        0    16263 2023-05-17 17:15:12.990546 fairscape_cli-0.1.5a2/fairscape_cli/rocrate/rocrate.py
--rw-r--r--   0        0        0     1326 2023-04-17 19:02:18.839104 fairscape_cli-0.1.5a2/fairscape_cli/rocrate/utils.py
--rw-r--r--   0        0        0        0 2023-05-15 16:53:18.146083 fairscape_cli-0.1.5a2/fairscape_cli/schema/__init__.py
--rw-r--r--   0        0        0      338 2023-05-15 16:57:34.786089 fairscape_cli-0.1.5a2/fairscape_cli/schema/schema.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/validate/__init__.py
--rw-r--r--   0        0        0     1365 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/validate/validate_json.py
--rw-r--r--   0        0        0     1499 2023-05-17 21:20:04.727973 fairscape_cli-0.1.5a2/pyproject.toml
--rw-r--r--   0        0        0     4949 1970-01-01 00:00:00.000000 fairscape_cli-0.1.5a2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-01-06 17:27:00.899279 fairscape_cli-0.1.5a3/LICENSE
+-rw-r--r--   0        0        0     4058 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a3/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a3/fairscape_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a3/fairscape_cli/apps/__init__.py
+-rw-r--r--   0        0        0      274 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a3/fairscape_cli/apps/cache.py
+-rw-r--r--   0        0        0      510 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a3/fairscape_cli/apps/describe.py
+-rw-r--r--   0        0        0      764 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a3/fairscape_cli/apps/fairscape.py
+-rw-r--r--   0        0        0       89 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a3/fairscape_cli/apps/list.py
+-rw-r--r--   0        0        0      173 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a3/fairscape_cli/apps/models/__init__.py
+-rw-r--r--   0        0        0      340 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a3/fairscape_cli/apps/models/computation.py
+-rw-r--r--   0        0        0     2559 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a3/fairscape_cli/apps/models/dataset.py
+-rw-r--r--   0        0        0     1890 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a3/fairscape_cli/apps/models/software.py
+-rw-r--r--   0        0        0     8135 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a3/fairscape_cli/apps/objects.py
+-rw-r--r--   0        0        0     3369 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a3/fairscape_cli/apps/rocrate.py
+-rw-r--r--   0        0        0     2276 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a3/fairscape_cli/apps/utils.py
+-rw-r--r--   0        0        0     2677 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a3/fairscape_cli/apps/validator.py
+-rw-r--r--   0        0        0      397 2023-05-30 16:31:53.800262 fairscape_cli-0.1.5a3/fairscape_cli/main.py
+-rw-r--r--   0        0        0      339 2023-06-07 17:58:52.914503 fairscape_cli-0.1.5a3/fairscape_cli/models/__init__.py
+-rw-r--r--   0        0        0     1395 2023-06-06 16:46:02.778647 fairscape_cli-0.1.5a3/fairscape_cli/models/base.py
+-rw-r--r--   0        0        0      707 2023-05-30 16:31:53.800262 fairscape_cli-0.1.5a3/fairscape_cli/models/computation.py
+-rw-r--r--   0        0        0     1340 2023-06-09 17:47:03.750076 fairscape_cli-0.1.5a3/fairscape_cli/models/dataset.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a3/fairscape_cli/models/models.py
+-rw-r--r--   0        0        0     7869 2023-06-06 21:23:26.408899 fairscape_cli-0.1.5a3/fairscape_cli/models/rocrate.py
+-rw-r--r--   0        0        0    13054 2023-05-30 16:31:53.800262 fairscape_cli-0.1.5a3/fairscape_cli/models/schema.py
+-rw-r--r--   0        0        0      758 2023-05-30 16:31:53.800262 fairscape_cli-0.1.5a3/fairscape_cli/models/software.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a3/fairscape_cli/rocrate/__init__.py
+-rw-r--r--   0        0        0    20849 2023-06-09 18:27:06.989184 fairscape_cli-0.1.5a3/fairscape_cli/rocrate/rocrate.py
+-rw-r--r--   0        0        0     1326 2023-05-30 16:31:53.800262 fairscape_cli-0.1.5a3/fairscape_cli/rocrate/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 16:31:53.800262 fairscape_cli-0.1.5a3/fairscape_cli/schema/__init__.py
+-rw-r--r--   0        0        0      338 2023-05-30 16:31:53.800262 fairscape_cli-0.1.5a3/fairscape_cli/schema/schema.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a3/fairscape_cli/validate/__init__.py
+-rw-r--r--   0        0        0     1365 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a3/fairscape_cli/validate/validate_json.py
+-rw-r--r--   0        0        0     1534 2023-06-09 20:05:51.859697 fairscape_cli-0.1.5a3/pyproject.toml
+-rw-r--r--   0        0        0     4913 1970-01-01 00:00:00.000000 fairscape_cli-0.1.5a3/PKG-INFO
```

### Comparing `fairscape_cli-0.1.5a2/LICENSE` & `fairscape_cli-0.1.5a3/LICENSE`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a2/README.md` & `fairscape_cli-0.1.5a3/README.md`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a2/fairscape_cli/apps/fairscape.py` & `fairscape_cli-0.1.5a3/fairscape_cli/apps/fairscape.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a2/fairscape_cli/apps/models/dataset.py` & `fairscape_cli-0.1.5a3/fairscape_cli/apps/models/dataset.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a2/fairscape_cli/apps/models/software.py` & `fairscape_cli-0.1.5a3/fairscape_cli/apps/models/software.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a2/fairscape_cli/apps/objects.py` & `fairscape_cli-0.1.5a3/fairscape_cli/apps/objects.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a2/fairscape_cli/apps/rocrate.py` & `fairscape_cli-0.1.5a3/fairscape_cli/apps/rocrate.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a2/fairscape_cli/apps/utils.py` & `fairscape_cli-0.1.5a3/fairscape_cli/apps/utils.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a2/fairscape_cli/apps/validator.py` & `fairscape_cli-0.1.5a3/fairscape_cli/apps/validator.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a2/fairscape_cli/models/schema.py` & `fairscape_cli-0.1.5a3/fairscape_cli/models/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,15 @@
     def __init__(self, error, message="DataValidationException: NA Values in required column"):
         self.error = error
         self.message = message
         super().__init__(self.message)
 
 class DatatypeValidationException(DataValidationException):
 
-    def __init__(self, error, message)
+    def __init__(self, error, message):
         self.error = error
         self.message = message
         super().__init__(self.message)
 
 
 class PathNotFoundException(DataValidationException):
```

### Comparing `fairscape_cli-0.1.5a2/fairscape_cli/rocrate/rocrate.py` & `fairscape_cli-0.1.5a3/fairscape_cli/rocrate/rocrate.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json
 from pydantic import ValidationError
 
 from fairscape_cli.models import (
     Dataset,
     Software,
     Computation,
+    DatasetContainer,
     ROCrate
 )
 
 from fairscape_cli.rocrate.utils import (
     generate_id,
     inside_crate 
 )
@@ -150,15 +151,14 @@
     url: str,
     date_modified: str,
     filepath: str,
     used_by_computation: Optional[List[str]],
     associated_publication: Optional[str],
     additional_documentation: Optional[str]
     ):
-
     
     metadata_path = rocrate_path / "ro-crate-metadata.json"
 
     # check if you are in the rocrate path
     # ro-crate-metadata.json should be a local file
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
@@ -175,16 +175,19 @@
             "author": author,
             "dateModified": date_modified,
             "description": description,
             "version": version,
             "associatedPublication": associated_publication,
             "additionalDocumentation": additional_documentation,
             "format": file_format,
-            "usedByComputation": used_by_computation,
-            }
+            # sanitize new line characters for multiple inputs
+            "usedByComputation": [
+                computation.strip("\n") for computation in used_by_computation
+            ],
+        }
 
     if filepath != "" and filepath is not None:
             software_metadata["contentUrl"] = f"file://{str(filepath)}" 
     else:
         # if filepath is null and url is null
         # raise an error
         if url == "" or url is None:
@@ -200,14 +203,15 @@
         click.Abort()
         
     crate.registerSoftware(software_model)
  
     click.echo(guid)
 
 
+
 @register.command('dataset')
 @click.argument('rocrate-path', type=click.Path(exists=True, path_type=pathlib.Path))
 @click.option('--guid', required=False, default="", type=str)
 @click.option('--name', required=True, prompt="Dataset Name")
 @click.option('--url', required=False)
 @click.option('--author', required=True, prompt="Dataset Author")
 @click.option('--version', required=True, prompt="Dataset Version")
@@ -254,16 +258,22 @@
             "name": name,
             "description": description,
             "datePublished": date_published,
             "version": version,
             "associatedPublication": associated_publication,
             "additionalDocumentation": additional_documentation,
             "format": data_format,
-            "derivedFrom": derived_from,
-            "usedBy": used_by
+
+            # sanitize input lists of newline breaks
+            "derivedFrom": [
+                derived.strip("\n") for derived in derived_from
+            ],
+            "usedBy": [
+                used.strip("\n") for used in used_by 
+            ],
             }
 
     if filepath != "" and filepath is not None:
         dataset_metadata["contentUrl"] = f"file://{str(filepath)}" 
 
 
     try:
@@ -323,17 +333,24 @@
             **{
             "@id": guid,
             "@type": "https://w3id.org/EVI#Computation",
             "name": name,
             "runBy": run_by,
             "dateCreated": date_created,
             "description": description,
-            "usedSoftware": used_software,
-            "usedDataset": used_dataset,
-            "generated": generated,
+            # sanitize input lists of newline breaks
+            "usedSoftware": [
+                software.strip("\n") for software in used_software
+            ],
+            "usedDataset": [
+                dataset.strip("\n") for dataset in used_dataset 
+            ],
+            "generated": [
+                output.strip("\n") for output in generated
+            ],
             }
         )
     except ValidationError as e:
         click.echo("Computation Validation Error")
         click.echo(e)
         click.Abort()
 
@@ -342,14 +359,132 @@
     click.echo(guid)
         #click.echo("Added Computation")
         #click.echo(
         #    json.dumps(computation_model.dict(by_alias=True), indent=2)
         #)
 
 
+
+@register.command('dataset-container')
+@click.argument('rocrate-path', type=click.Path(exists=True, path_type=pathlib.Path))
+@click.option('--guid', required=False, default="", type=str, show_default=False)
+@click.option('--name', required=True, prompt="DatasetContainer Name")
+@click.option('--description', required=True)
+@click.option('--has-part', required=False, multiple=True)
+@click.option('--is-part-of', required=False, multiple=True)
+def registerDatasetContainer(
+    rocrate_path, 
+    guid, 
+    name, 
+    description, 
+    has_part, 
+    is_part_of
+):
+    '''Add a DatasetContainer to the ROCrate.
+
+    A Dataset Container is used for grouping sets of datasets. Only Datasets may be added to the dataset container hasPart property.
+    '''
+   
+    # check that crate exists 
+    metadata_path = rocrate_path / "ro-crate-metadata.json"
+    if metadata_path.exists() != True:
+        click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
+        click.Abort()
+
+    crate = ROCrate(path=metadata_path)
+
+    if guid == "":
+        guid = generate_id(metadata_path, name, "Dataset")
+
+    # validate the provided metadata
+    try: 
+        dscontainer = DatasetContainer(**{
+            "guid": guid,
+            "name": name,
+            "description": description,
+            "hasPart": has_part,
+            "isPartOf": is_part_of
+        })
+
+        crate.registerObject(dscontainer) 
+        click.echo(guid)
+
+    except ValidationError as e:
+        click.echo("DatasetContainer Validation Error")
+        click.echo(e)
+        click.Abort()
+
+    
+
+
+###############################################################################
+#                             Dataset Container Commands                      #
+###############################################################################
+
+@rocrate.group('dataset-container')
+def datasetContainer():
+    pass
+
+@datasetContainer.command('pop')
+@click.argument('rocrate-path', type=click.Path(exists=True, path_type=pathlib.Path))
+@click.option('--dataset-container', required=True)
+@click.option('--dataset-guid', required=True, multiple=True)
+def popDatasetContainer(rocrate_path, dataset_container, dataset_guid):
+    """ Add dataset elements to the specified dataset container
+    """
+    # check that crate exists 
+    metadata_path = rocrate_path / "ro-crate-metadata.json"
+    if metadata_path.exists() != True:
+        click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
+        click.Abort()
+
+    crate = ROCrate(path=metadata_path)
+
+    # TODO check that dataset container is guid
+
+    # TODO check that dataset guid is guid
+
+    try:
+        crate.popDatasetContainer(dataset_container, dataset_guid)
+
+    except Exception as e:
+        click.echo("Error poping element from DatasetContainer")
+        click.Abort()
+
+
+@datasetContainer.command('push')
+@click.argument('rocrate-path', type=click.Path(exists=True, path_type=pathlib.Path))
+@click.option('--dataset-container', required=True)
+@click.option('--dataset-guid', required=True, multiple=True)
+def pushDatasetContainer(rocrate_path, dataset_container, dataset_guid):
+    """ Add dataset elements to the specified dataset container
+    """
+
+    # check that crate exists 
+    metadata_path = rocrate_path / "ro-crate-metadata.json"
+    if metadata_path.exists() != True:
+        click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
+        click.Abort()
+
+    crate = ROCrate(path=metadata_path)
+
+    # TODO check that dataset container is guid
+
+    # TODO check that dataset guid is guid
+
+    try:
+        crate.pushDatasetContainer(dataset_container, dataset_guid)
+
+    except Exception as e:
+        click.echo("Error pushing element to DatasetContainer")
+        click.Abort()
+
+    
+
+
 # RO Crate add subcommands
 @rocrate.group('add')
 def add():
     pass
 
 
 @add.command('software')
@@ -412,15 +547,18 @@
             "author": author,
             "dateModified": date_modified,
             "description": description,
             "version": version,
             "associatedPublication": associated_publication,
             "additionalDocumentation": additional_documentation,
             "format": file_format,
-            "usedByComputation": used_by_computation,
+            # sanitize multiple inputs
+            "usedByComputation": [
+                computation.strip("\n") for computation in used_by_computation
+            ],
             "contentUrl": "file://" + str(destination_path)
             }
         )
 
     except ValidationError as e:
         click.echo("Software Validation Error")
         click.echo(e)
@@ -502,16 +640,20 @@
             "name": name,
             "description": description,
             "datePublished": date_published,
             "version": version,
             "associatedPublication": associated_publication,
             "additionalDocumentation": additional_documentation,
             "format": data_format,
-            "derivedFrom": derived_from,
-            "usedBy": used_by,
+            "derivedFrom": [
+                derived.strip("\n") for derived in derived_from
+            ],
+            "usedBy": [
+                used.strip("\n") for used in used_by 
+            ],
             "contentUrl": "file://" + str(destination_path)
             }
         )
 
     except ValidationError as e:
         click.echo("Software Validation Error")
         click.echo(e)
```

### Comparing `fairscape_cli-0.1.5a2/fairscape_cli/rocrate/utils.py` & `fairscape_cli-0.1.5a3/fairscape_cli/rocrate/utils.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a2/fairscape_cli/validate/validate_json.py` & `fairscape_cli-0.1.5a3/fairscape_cli/validate/validate_json.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a2/pyproject.toml` & `fairscape_cli-0.1.5a3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -22,17 +22,21 @@
 
 [project.urls]
 Homepage = "https://github.com/fairscape/fairscape-cli"
 
 
 [tool.poetry]
 name = "fairscape-cli"
-version = "0.1.5a2"
+version = "0.1.5a3"
 description = "A cli for validating metadata, packaging ROCrates, and interacting with the FAIRSCAPE API"
-authors = ["mlev71 <max.adam.levinson@gmail.com>"]
+authors = [
+        "Max Levinson",
+        "Sadnan Al Manir", 
+        "Tim Clark"
+]
 license = "LICENSE"
 readme = "README.md"
 packages = [{include = "fairscape_cli"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `fairscape_cli-0.1.5a2/PKG-INFO` & `fairscape_cli-0.1.5a3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: fairscape-cli
-Version: 0.1.5a2
+Version: 0.1.5a3
 Summary: A cli for validating metadata, packaging ROCrates, and interacting with the FAIRSCAPE API
 License: LICENSE
-Author: mlev71
-Author-email: max.adam.levinson@gmail.com
+Author: Max Levinson
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

