# Comparing `tmp/aws-cdk.aws-iotevents-actions-alpha-2.83.0a0.tar.gz` & `tmp/aws-cdk.aws-iotevents-actions-alpha-2.83.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src065889124/src/packages/@aws-cdk/aws-iotevents-actions-alpha/dist/python/aws-cdk.aws-iotevents-actions-alph", last modified: Wed Jun  7 12:17:28 2023, max compression
+gzip compressed data, was "/codebuild/output/src629398401/src/packages/@aws-cdk/aws-iotevents-actions-alpha/dist/python/aws-cdk.aws-iotevents-actions-alph", last modified: Fri Jun  9 09:55:25 2023, max compression
```

## Comparing `aws-cdk.aws-iotevents-actions-alpha-2.83.0a0.tar` & `aws-cdk.aws-iotevents-actions-alpha-2.83.1a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 12:17:28.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-07 12:17:23.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-07 12:17:23.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-07 12:17:23.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5723 2023-06-07 12:17:28.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4705 2023-06-07 12:17:23.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-07 12:17:23.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 12:17:28.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1987 2023-06-07 12:17:23.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 12:17:28.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 12:17:28.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 12:17:28.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk/aws_iotevents_actions_alpha/
--rw-r--r--   0 root         (0) root         (0)    19108 2023-06-07 12:17:23.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk/aws_iotevents_actions_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 12:17:28.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk/aws_iotevents_actions_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      502 2023-06-07 12:17:23.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk/aws_iotevents_actions_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30997 2023-06-07 12:17:23.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk/aws_iotevents_actions_alpha/_jsii/aws-iotevents-actions-alpha@2.83.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 12:17:23.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk/aws_iotevents_actions_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 12:17:28.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5723 2023-06-07 12:17:28.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      631 2023-06-07 12:17:28.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 12:17:28.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      143 2023-06-07 12:17:28.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-07 12:17:28.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:25.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-06-09 09:55:15.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-09 09:55:15.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-09 09:55:15.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5723 2023-06-09 09:55:25.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4705 2023-06-09 09:55:15.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-09 09:55:15.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 09:55:25.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-06-09 09:55:15.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:25.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:25.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:25.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk/aws_iotevents_actions_alpha/
+-rw-r--r--   0 root         (0) root         (0)    19108 2023-06-09 09:55:15.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk/aws_iotevents_actions_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:25.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk/aws_iotevents_actions_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      502 2023-06-09 09:55:15.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk/aws_iotevents_actions_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30996 2023-06-09 09:55:15.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk/aws_iotevents_actions_alpha/_jsii/aws-iotevents-actions-alpha@2.83.1-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:55:15.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk/aws_iotevents_actions_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:55:25.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5723 2023-06-09 09:55:25.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      631 2023-06-09 09:55:25.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:55:25.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      143 2023-06-09 09:55:25.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-09 09:55:25.000000 aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/LICENSE` & `aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/PKG-INFO` & `aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-iotevents-actions-alpha
-Version: 2.83.0a0
+Version: 2.83.1a0
 Summary: Receipt Detector Model actions for AWS IoT Events
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/README.md` & `aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/setup.py` & `aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-iotevents-actions-alpha",
-    "version": "2.83.0.a0",
+    "version": "2.83.1.a0",
     "description": "Receipt Detector Model actions for AWS IoT Events",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "aws_cdk.aws_iotevents_actions_alpha",
         "aws_cdk.aws_iotevents_actions_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_iotevents_actions_alpha._jsii": [
-            "aws-iotevents-actions-alpha@2.83.0-alpha.0.jsii.tgz"
+            "aws-iotevents-actions-alpha@2.83.1-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_iotevents_actions_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.83.0",
-        "aws-cdk.aws-iotevents-alpha==2.83.0.a0",
+        "aws-cdk-lib==2.83.1",
+        "aws-cdk.aws-iotevents-alpha==2.83.1.a0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk/aws_iotevents_actions_alpha/__init__.py` & `aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk/aws_iotevents_actions_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk/aws_iotevents_actions_alpha/_jsii/aws-iotevents-actions-alpha@2.83.0-alpha.0.jsii.tgz` & `aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk/aws_iotevents_actions_alpha/_jsii/aws-iotevents-actions-alpha@2.83.1-alpha.0.jsii.tgz`

 * *Files 3% similar despite different names*

#### Comparing `aws-iotevents-actions-alpha@2.83.0-alpha.0.jsii.tgz-content` & `aws-iotevents-actions-alpha@2.83.1-alpha.0.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9629629629629629%*

 * *Differences: {"'dependencies'": "{'@aws-cdk/aws-iotevents-alpha': '2.83.1-alpha.0', 'aws-cdk-lib': '2.83.1'}",*

 * * "'version'": "'2.83.1-alpha.0'"}*

```diff
@@ -4,16 +4,16 @@
         "organization": true,
         "roles": [
             "author"
         ],
         "url": "https://aws.amazon.com"
     },
     "dependencies": {
-        "@aws-cdk/aws-iotevents-alpha": "2.83.0-alpha.0",
-        "aws-cdk-lib": "2.83.0",
+        "@aws-cdk/aws-iotevents-alpha": "2.83.1-alpha.0",
+        "aws-cdk-lib": "2.83.1",
         "constructs": "^10.0.0"
     },
     "dependencyClosure": {
         "@aws-cdk/asset-awscli-v1": {
             "targets": {
                 "dotnet": {
                     "namespace": "Amazon.CDK.Asset.AwsCliV1",
@@ -3860,9 +3860,9 @@
                     "static": true
                 }
             ],
             "name": "TimerDuration",
             "symbolId": "lib/timer-duration:TimerDuration"
         }
     },
-    "version": "2.83.0-alpha.0"
+    "version": "2.83.1-alpha.0"
 }
```

##### package/lib/clear-timer-action.js

###### js-beautify {}

```diff
@@ -27,11 +27,11 @@
             },
         };
     }
 }
 _a = JSII_RTTI_SYMBOL_1;
 ClearTimerAction[_a] = {
     fqn: "@aws-cdk/aws-iotevents-actions-alpha.ClearTimerAction",
-    version: "2.83.0-alpha.0"
+    version: "2.83.1-alpha.0"
 };
 exports.ClearTimerAction = ClearTimerAction;
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiY2xlYXItdGltZXItYWN0aW9uLmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiY2xlYXItdGltZXItYWN0aW9uLnRzIl0sIm5hbWVzIjpbXSwibWFwcGluZ3MiOiI7Ozs7O0FBR0E7O0dBRUc7QUFDSCxNQUFhLGdCQUFnQjtJQUMzQjs7T0FFRztJQUNILFlBQTZCLFNBQWlCO1FBQWpCLGNBQVMsR0FBVCxTQUFTLENBQVE7S0FBSTtJQUVsRDs7T0FFRztJQUNJLEtBQUssQ0FBQyxNQUFpQixFQUFFLFFBQXFDO1FBQ25FLE9BQU87WUFDTCxhQUFhLEVBQUU7Z0JBQ2IsVUFBVSxFQUFFO29CQUNWLFNBQVMsRUFBRSxJQUFJLENBQUMsU0FBUztpQkFDMUI7YUFDRjtTQUNGLENBQUM7S0FDSDs7OztBQWpCVSw0Q0FBZ0IiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgKiBhcyBpb3RldmVudHMgZnJvbSAnQGF3cy1jZGsvYXdzLWlvdGV2ZW50cy1hbHBoYSc7XG5pbXBvcnQgeyBDb25zdHJ1Y3QgfSBmcm9tICdjb25zdHJ1Y3RzJztcblxuLyoqXG4gKiBUaGUgYWN0aW9uIHRvIGRlbGV0ZSBhbiBleGlzdGluZyB0aW1lci5cbiAqL1xuZXhwb3J0IGNsYXNzIENsZWFyVGltZXJBY3Rpb24gaW1wbGVtZW50cyBpb3RldmVudHMuSUFjdGlvbiB7XG4gIC8qKlxuICAgKiBAcGFyYW0gdGltZXJOYW1lIHRoZSBuYW1lIG9mIHRoZSB0aW1lclxuICAgKi9cbiAgY29uc3RydWN0b3IocHJpdmF0ZSByZWFkb25seSB0aW1lck5hbWU6IHN0cmluZykge31cblxuICAvKipcbiAgICogQGludGVybmFsXG4gICAqL1xuICBwdWJsaWMgX2JpbmQoX3Njb3BlOiBDb25zdHJ1Y3QsIF9vcHRpb25zOiBpb3RldmVudHMuQWN0aW9uQmluZE9wdGlvbnMpOiBpb3RldmVudHMuQWN0aW9uQ29uZmlnIHtcbiAgICByZXR1cm4ge1xuICAgICAgY29uZmlndXJhdGlvbjoge1xuICAgICAgICBjbGVhclRpbWVyOiB7XG4gICAgICAgICAgdGltZXJOYW1lOiB0aGlzLnRpbWVyTmFtZSxcbiAgICAgICAgfSxcbiAgICAgIH0sXG4gICAgfTtcbiAgfVxufVxuIl19
```

##### package/lib/lambda-invoke-action.js

###### js-beautify {}

```diff
@@ -28,11 +28,11 @@
             },
         };
     }
 }
 _a = JSII_RTTI_SYMBOL_1;
 LambdaInvokeAction[_a] = {
     fqn: "@aws-cdk/aws-iotevents-actions-alpha.LambdaInvokeAction",
-    version: "2.83.0-alpha.0"
+    version: "2.83.1-alpha.0"
 };
 exports.LambdaInvokeAction = LambdaInvokeAction;
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoibGFtYmRhLWludm9rZS1hY3Rpb24uanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyJsYW1iZGEtaW52b2tlLWFjdGlvbi50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiOzs7OztBQUlBOztHQUVHO0FBQ0gsTUFBYSxrQkFBa0I7SUFDN0I7O09BRUc7SUFDSCxZQUE2QixJQUFzQjtRQUF0QixTQUFJLEdBQUosSUFBSSxDQUFrQjtLQUNsRDtJQUVEOztPQUVHO0lBQ0ksS0FBSyxDQUFDLE1BQWlCLEVBQUUsT0FBb0M7UUFDbEUsSUFBSSxDQUFDLElBQUksQ0FBQyxXQUFXLENBQUMsT0FBTyxDQUFDLElBQUksQ0FBQyxDQUFDO1FBQ3BDLE9BQU87WUFDTCxhQUFhLEVBQUU7Z0JBQ2IsTUFBTSxFQUFFO29CQUNOLFdBQVcsRUFBRSxJQUFJLENBQUMsSUFBSSxDQUFDLFdBQVc7aUJBQ25DO2FBQ0Y7U0FDRixDQUFDO0tBQ0g7Ozs7QUFuQlUsZ0RBQWtCIiwic291cmNlc0NvbnRlbnQiOlsiaW1wb3J0ICogYXMgaW90ZXZlbnRzIGZyb20gJ0Bhd3MtY2RrL2F3cy1pb3RldmVudHMtYWxwaGEnO1xuaW1wb3J0ICogYXMgbGFtYmRhIGZyb20gJ2F3cy1jZGstbGliL2F3cy1sYW1iZGEnO1xuaW1wb3J0IHsgQ29uc3RydWN0IH0gZnJvbSAnY29uc3RydWN0cyc7XG5cbi8qKlxuICogVGhlIGFjdGlvbiB0byB3cml0ZSB0aGUgZGF0YSB0byBhbiBBV1MgTGFtYmRhIGZ1bmN0aW9uLlxuICovXG5leHBvcnQgY2xhc3MgTGFtYmRhSW52b2tlQWN0aW9uIGltcGxlbWVudHMgaW90ZXZlbnRzLklBY3Rpb24ge1xuICAvKipcbiAgICogQHBhcmFtIGZ1bmMgdGhlIEFXUyBMYW1iZGEgZnVuY3Rpb24gdG8gYmUgaW52b2tlZCBieSB0aGlzIGFjdGlvblxuICAgKi9cbiAgY29uc3RydWN0b3IocHJpdmF0ZSByZWFkb25seSBmdW5jOiBsYW1iZGEuSUZ1bmN0aW9uKSB7XG4gIH1cblxuICAvKipcbiAgICogQGludGVybmFsXG4gICAqL1xuICBwdWJsaWMgX2JpbmQoX3Njb3BlOiBDb25zdHJ1Y3QsIG9wdGlvbnM6IGlvdGV2ZW50cy5BY3Rpb25CaW5kT3B0aW9ucyk6IGlvdGV2ZW50cy5BY3Rpb25Db25maWcge1xuICAgIHRoaXMuZnVuYy5ncmFudEludm9rZShvcHRpb25zLnJvbGUpO1xuICAgIHJldHVybiB7XG4gICAgICBjb25maWd1cmF0aW9uOiB7XG4gICAgICAgIGxhbWJkYToge1xuICAgICAgICAgIGZ1bmN0aW9uQXJuOiB0aGlzLmZ1bmMuZnVuY3Rpb25Bcm4sXG4gICAgICAgIH0sXG4gICAgICB9LFxuICAgIH07XG4gIH1cbn1cbiJdfQ==
```

##### package/lib/reset-timer-action.js

###### js-beautify {}

```diff
@@ -27,11 +27,11 @@
             },
         };
     }
 }
 _a = JSII_RTTI_SYMBOL_1;
 ResetTimerAction[_a] = {
     fqn: "@aws-cdk/aws-iotevents-actions-alpha.ResetTimerAction",
-    version: "2.83.0-alpha.0"
+    version: "2.83.1-alpha.0"
 };
 exports.ResetTimerAction = ResetTimerAction;
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoicmVzZXQtdGltZXItYWN0aW9uLmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsicmVzZXQtdGltZXItYWN0aW9uLnRzIl0sIm5hbWVzIjpbXSwibWFwcGluZ3MiOiI7Ozs7O0FBR0E7O0dBRUc7QUFDSCxNQUFhLGdCQUFnQjtJQUMzQjs7T0FFRztJQUNILFlBQTZCLFNBQWlCO1FBQWpCLGNBQVMsR0FBVCxTQUFTLENBQVE7S0FBSTtJQUVsRDs7T0FFRztJQUNJLEtBQUssQ0FBQyxNQUFpQixFQUFFLFFBQXFDO1FBQ25FLE9BQU87WUFDTCxhQUFhLEVBQUU7Z0JBQ2IsVUFBVSxFQUFFO29CQUNWLFNBQVMsRUFBRSxJQUFJLENBQUMsU0FBUztpQkFDMUI7YUFDRjtTQUNGLENBQUM7S0FDSDs7OztBQWpCVSw0Q0FBZ0IiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgKiBhcyBpb3RldmVudHMgZnJvbSAnQGF3cy1jZGsvYXdzLWlvdGV2ZW50cy1hbHBoYSc7XG5pbXBvcnQgeyBDb25zdHJ1Y3QgfSBmcm9tICdjb25zdHJ1Y3RzJztcblxuLyoqXG4gKiBUaGUgYWN0aW9uIHRvIHJlc2V0IGFuIGV4aXN0aW5nIHRpbWVyLlxuICovXG5leHBvcnQgY2xhc3MgUmVzZXRUaW1lckFjdGlvbiBpbXBsZW1lbnRzIGlvdGV2ZW50cy5JQWN0aW9uIHtcbiAgLyoqXG4gICAqIEBwYXJhbSB0aW1lck5hbWUgdGhlIG5hbWUgb2YgdGhlIHRpbWVyXG4gICAqL1xuICBjb25zdHJ1Y3Rvcihwcml2YXRlIHJlYWRvbmx5IHRpbWVyTmFtZTogc3RyaW5nKSB7fVxuXG4gIC8qKlxuICAgKiBAaW50ZXJuYWxcbiAgICovXG4gIHB1YmxpYyBfYmluZChfc2NvcGU6IENvbnN0cnVjdCwgX29wdGlvbnM6IGlvdGV2ZW50cy5BY3Rpb25CaW5kT3B0aW9ucyk6IGlvdGV2ZW50cy5BY3Rpb25Db25maWcge1xuICAgIHJldHVybiB7XG4gICAgICBjb25maWd1cmF0aW9uOiB7XG4gICAgICAgIHJlc2V0VGltZXI6IHtcbiAgICAgICAgICB0aW1lck5hbWU6IHRoaXMudGltZXJOYW1lLFxuICAgICAgICB9LFxuICAgICAgfSxcbiAgICB9O1xuICB9XG59XG4iXX0=
```

##### package/lib/set-timer-action.js

###### js-beautify {}

```diff
@@ -39,11 +39,11 @@
             },
         };
     }
 }
 _a = JSII_RTTI_SYMBOL_1;
 SetTimerAction[_a] = {
     fqn: "@aws-cdk/aws-iotevents-actions-alpha.SetTimerAction",
-    version: "2.83.0-alpha.0"
+    version: "2.83.1-alpha.0"
 };
 exports.SetTimerAction = SetTimerAction;
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoic2V0LXRpbWVyLWFjdGlvbi5qcyIsInNvdXJjZVJvb3QiOiIiLCJzb3VyY2VzIjpbInNldC10aW1lci1hY3Rpb24udHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7O0FBSUE7O0dBRUc7QUFDSCxNQUFhLGNBQWM7SUFDekI7OztPQUdHO0lBQ0gsWUFDbUIsU0FBaUIsRUFDakIsYUFBNEI7UUFENUIsY0FBUyxHQUFULFNBQVMsQ0FBUTtRQUNqQixrQkFBYSxHQUFiLGFBQWEsQ0FBZTs7Ozs7OytDQVBwQyxjQUFjOzs7O0tBU3hCO0lBRUQ7O09BRUc7SUFDSSxLQUFLLENBQUMsTUFBaUIsRUFBRSxRQUFxQztRQUNuRSxPQUFPO1lBQ0wsYUFBYSxFQUFFO2dCQUNiLFFBQVEsRUFBRTtvQkFDUixTQUFTLEVBQUUsSUFBSSxDQUFDLFNBQVM7b0JBQ3pCLGtCQUFrQixFQUFFLElBQUksQ0FBQyxhQUFhLENBQUMsS0FBSyxFQUFFO2lCQUMvQzthQUNGO1NBQ0YsQ0FBQztLQUNIOzs7O0FBdkJVLHdDQUFjIiwic291cmNlc0NvbnRlbnQiOlsiaW1wb3J0ICogYXMgaW90ZXZlbnRzIGZyb20gJ0Bhd3MtY2RrL2F3cy1pb3RldmVudHMtYWxwaGEnO1xuaW1wb3J0IHsgQ29uc3RydWN0IH0gZnJvbSAnY29uc3RydWN0cyc7XG5pbXBvcnQgeyBUaW1lckR1cmF0aW9uIH0gZnJvbSAnLi90aW1lci1kdXJhdGlvbic7XG5cbi8qKlxuICogVGhlIGFjdGlvbiB0byBjcmVhdGUgYSB0aW1lciB3aXRoIGR1cmF0aW9uIGluIHNlY29uZHMuXG4gKi9cbmV4cG9ydCBjbGFzcyBTZXRUaW1lckFjdGlvbiBpbXBsZW1lbnRzIGlvdGV2ZW50cy5JQWN0aW9uIHtcbiAgLyoqXG4gICAqIEBwYXJhbSB0aW1lck5hbWUgdGhlIG5hbWUgb2YgdGhlIHRpbWVyXG4gICAqIEBwYXJhbSB0aW1lckR1cmF0aW9uIHRoZSBkdXJhdGlvbiBvZiB0aGUgdGltZXJcbiAgICovXG4gIGNvbnN0cnVjdG9yKFxuICAgIHByaXZhdGUgcmVhZG9ubHkgdGltZXJOYW1lOiBzdHJpbmcsXG4gICAgcHJpdmF0ZSByZWFkb25seSB0aW1lckR1cmF0aW9uOiBUaW1lckR1cmF0aW9uLFxuICApIHtcbiAgfVxuXG4gIC8qKlxuICAgKiBAaW50ZXJuYWxcbiAgICovXG4gIHB1YmxpYyBfYmluZChfc2NvcGU6IENvbnN0cnVjdCwgX29wdGlvbnM6IGlvdGV2ZW50cy5BY3Rpb25CaW5kT3B0aW9ucyk6IGlvdGV2ZW50cy5BY3Rpb25Db25maWcge1xuICAgIHJldHVybiB7XG4gICAgICBjb25maWd1cmF0aW9uOiB7XG4gICAgICAgIHNldFRpbWVyOiB7XG4gICAgICAgICAgdGltZXJOYW1lOiB0aGlzLnRpbWVyTmFtZSxcbiAgICAgICAgICBkdXJhdGlvbkV4cHJlc3Npb246IHRoaXMudGltZXJEdXJhdGlvbi5fYmluZCgpLFxuICAgICAgICB9LFxuICAgICAgfSxcbiAgICB9O1xuICB9XG59XG4iXX0=
```

##### package/lib/set-variable-action.js

###### js-beautify {}

```diff
@@ -30,11 +30,11 @@
             },
         };
     }
 }
 _a = JSII_RTTI_SYMBOL_1;
 SetVariableAction[_a] = {
     fqn: "@aws-cdk/aws-iotevents-actions-alpha.SetVariableAction",
-    version: "2.83.0-alpha.0"
+    version: "2.83.1-alpha.0"
 };
 exports.SetVariableAction = SetVariableAction;
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoic2V0LXZhcmlhYmxlLWFjdGlvbi5qcyIsInNvdXJjZVJvb3QiOiIiLCJzb3VyY2VzIjpbInNldC12YXJpYWJsZS1hY3Rpb24udHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFHQTs7R0FFRztBQUNILE1BQWEsaUJBQWlCO0lBQzVCOzs7T0FHRztJQUNILFlBQTZCLFlBQW9CLEVBQW1CLEtBQTJCO1FBQWxFLGlCQUFZLEdBQVosWUFBWSxDQUFRO1FBQW1CLFVBQUssR0FBTCxLQUFLLENBQXNCO0tBQzlGO0lBRUQ7O09BRUc7SUFDSSxLQUFLLENBQUMsTUFBaUIsRUFBRSxRQUFxQztRQUNuRSxPQUFPO1lBQ0wsYUFBYSxFQUFFO2dCQUNiLFdBQVcsRUFBRTtvQkFDWCxZQUFZLEVBQUUsSUFBSSxDQUFDLFlBQVk7b0JBQy9CLEtBQUssRUFBRSxJQUFJLENBQUMsS0FBSyxDQUFDLFFBQVEsRUFBRTtpQkFDN0I7YUFDRjtTQUNGLENBQUM7S0FDSDs7OztBQXBCVSw4Q0FBaUIiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgKiBhcyBpb3RldmVudHMgZnJvbSAnQGF3cy1jZGsvYXdzLWlvdGV2ZW50cy1hbHBoYSc7XG5pbXBvcnQgeyBDb25zdHJ1Y3QgfSBmcm9tICdjb25zdHJ1Y3RzJztcblxuLyoqXG4gKiBUaGUgYWN0aW9uIHRvIGNyZWF0ZSBhIHZhcmlhYmxlIHdpdGggYSBzcGVjaWZpZWQgdmFsdWUuXG4gKi9cbmV4cG9ydCBjbGFzcyBTZXRWYXJpYWJsZUFjdGlvbiBpbXBsZW1lbnRzIGlvdGV2ZW50cy5JQWN0aW9uIHtcbiAgLyoqXG4gICAqIEBwYXJhbSB2YXJpYWJsZU5hbWUgdGhlIG5hbWUgb2YgdGhlIHZhcmlhYmxlXG4gICAqIEBwYXJhbSB2YWx1ZSB0aGUgbmV3IHZhbHVlIG9mIHRoZSB2YXJpYWJsZVxuICAgKi9cbiAgY29uc3RydWN0b3IocHJpdmF0ZSByZWFkb25seSB2YXJpYWJsZU5hbWU6IHN0cmluZywgcHJpdmF0ZSByZWFkb25seSB2YWx1ZTogaW90ZXZlbnRzLkV4cHJlc3Npb24pIHtcbiAgfVxuXG4gIC8qKlxuICAgKiBAaW50ZXJuYWxcbiAgICovXG4gIHB1YmxpYyBfYmluZChfc2NvcGU6IENvbnN0cnVjdCwgX29wdGlvbnM6IGlvdGV2ZW50cy5BY3Rpb25CaW5kT3B0aW9ucyk6IGlvdGV2ZW50cy5BY3Rpb25Db25maWcge1xuICAgIHJldHVybiB7XG4gICAgICBjb25maWd1cmF0aW9uOiB7XG4gICAgICAgIHNldFZhcmlhYmxlOiB7XG4gICAgICAgICAgdmFyaWFibGVOYW1lOiB0aGlzLnZhcmlhYmxlTmFtZSxcbiAgICAgICAgICB2YWx1ZTogdGhpcy52YWx1ZS5ldmFsdWF0ZSgpLFxuICAgICAgICB9LFxuICAgICAgfSxcbiAgICB9O1xuICB9XG59XG4iXX0=
```

##### package/lib/timer-duration.js

###### js-beautify {}

```diff
@@ -39,15 +39,15 @@
     static fromExpression(expression) {
         return new TimerDurationImpl(expression.evaluate());
     }
 }
 _a = JSII_RTTI_SYMBOL_1;
 TimerDuration[_a] = {
     fqn: "@aws-cdk/aws-iotevents-actions-alpha.TimerDuration",
-    version: "2.83.0-alpha.0"
+    version: "2.83.1-alpha.0"
 };
 exports.TimerDuration = TimerDuration;
 class TimerDurationImpl extends TimerDuration {
     constructor(durationExpression) {
         super();
         this.durationExpression = durationExpression;
     }
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9652777777777778%*

 * *Differences: {"'devDependencies'": "{'@aws-cdk/cdk-build-tools': '2.83.1-alpha.0', '@aws-cdk/integ-runner': "*

 * *                      "'2.83.1-alpha.0', '@aws-cdk/pkglint': '2.83.1-alpha.0', 'aws-cdk-lib': "*

 * *                      "'2.83.1', '@aws-cdk/integ-tests-alpha': '2.83.1-alpha.0', "*

 * *                      "'@aws-cdk/aws-iotevents-alpha': '2.83.1-alpha.0'}",*

 * * "'peerDependencies'": "{'@aws-cdk/aws-iotevents-alpha': '2.83.1-alpha.0', 'aws-cdk-lib': "*

 * *                       "'2.83.1'}",*

 * * "'version'": "'2.83.1-alpha.0'"}*

```diff
@@ -16,21 +16,21 @@
         "env": {
             "AWSLINT_BASE_CONSTRUCT": true
         }
     },
     "dependencies": {},
     "description": "Receipt Detector Model actions for AWS IoT Events",
     "devDependencies": {
-        "@aws-cdk/aws-iotevents-alpha": "2.83.0-alpha.0",
-        "@aws-cdk/cdk-build-tools": "2.83.0-alpha.0",
-        "@aws-cdk/integ-runner": "2.83.0-alpha.0",
-        "@aws-cdk/integ-tests-alpha": "2.83.0-alpha.0",
-        "@aws-cdk/pkglint": "2.83.0-alpha.0",
+        "@aws-cdk/aws-iotevents-alpha": "2.83.1-alpha.0",
+        "@aws-cdk/cdk-build-tools": "2.83.1-alpha.0",
+        "@aws-cdk/integ-runner": "2.83.1-alpha.0",
+        "@aws-cdk/integ-tests-alpha": "2.83.1-alpha.0",
+        "@aws-cdk/pkglint": "2.83.1-alpha.0",
         "@types/jest": "^29.5.1",
-        "aws-cdk-lib": "2.83.0",
+        "aws-cdk-lib": "2.83.1",
         "constructs": "^10.0.0",
         "jest": "^29.5.0"
     },
     "engines": {
         "node": ">= 14.15.0"
     },
     "homepage": "https://github.com/aws/aws-cdk",
@@ -72,16 +72,16 @@
         "aws-iotevents-actions"
     ],
     "license": "Apache-2.0",
     "main": "lib/index.js",
     "maturity": "experimental",
     "name": "@aws-cdk/aws-iotevents-actions-alpha",
     "peerDependencies": {
-        "@aws-cdk/aws-iotevents-alpha": "2.83.0-alpha.0",
-        "aws-cdk-lib": "2.83.0",
+        "@aws-cdk/aws-iotevents-alpha": "2.83.1-alpha.0",
+        "aws-cdk-lib": "2.83.1",
         "constructs": "^10.0.0"
     },
     "pkglint": {
         "exclude": [
             "naming/package-matches-directory",
             "assert/assert-dependency"
         ]
@@ -109,9 +109,9 @@
         "pkglint": "pkglint -f",
         "rosetta:extract": "yarn --silent jsii-rosetta extract",
         "test": "cdk-test",
         "watch": "cdk-watch"
     },
     "stability": "experimental",
     "types": "lib/index.d.ts",
-    "version": "2.83.0-alpha.0"
+    "version": "2.83.1-alpha.0"
 }
```

### Comparing `aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-iotevents-actions-alpha
-Version: 2.83.0a0
+Version: 2.83.1a0
 Summary: Receipt Detector Model actions for AWS IoT Events
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-iotevents-actions-alpha-2.83.0a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-iotevents-actions-alpha-2.83.1a0/src/aws_cdk.aws_iotevents_actions_alpha.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_iotevents_actions_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_iotevents_actions_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_iotevents_actions_alpha.egg-info/requires.txt
 src/aws_cdk.aws_iotevents_actions_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_iotevents_actions_alpha/__init__.py
 src/aws_cdk/aws_iotevents_actions_alpha/py.typed
 src/aws_cdk/aws_iotevents_actions_alpha/_jsii/__init__.py
-src/aws_cdk/aws_iotevents_actions_alpha/_jsii/aws-iotevents-actions-alpha@2.83.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_iotevents_actions_alpha/_jsii/aws-iotevents-actions-alpha@2.83.1-alpha.0.jsii.tgz
```

