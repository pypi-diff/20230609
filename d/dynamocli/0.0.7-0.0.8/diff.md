# Comparing `tmp/dynamocli-0.0.7.tar.gz` & `tmp/dynamocli-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamocli-0.0.7.tar", last modified: Fri Mar  3 12:48:02 2023, max compression
+gzip compressed data, was "dynamocli-0.0.8.tar", last modified: Fri Jun  9 12:46:35 2023, max compression
```

## Comparing `dynamocli-0.0.7.tar` & `dynamocli-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vblidh     (501) staff       (20)        0 2023-03-03 12:48:02.532825 dynamocli-0.0.7/
--rw-r--r--   0 vblidh     (501) staff       (20)     1873 2023-03-03 12:48:02.532704 dynamocli-0.0.7/PKG-INFO
--rw-r--r--   0 vblidh     (501) staff       (20)     1624 2023-02-10 09:13:03.000000 dynamocli-0.0.7/README
-drwxr-xr-x   0 vblidh     (501) staff       (20)        0 2023-03-03 12:48:02.531581 dynamocli-0.0.7/dynamocli.egg-info/
--rw-r--r--   0 vblidh     (501) staff       (20)     1873 2023-03-03 12:48:02.000000 dynamocli-0.0.7/dynamocli.egg-info/PKG-INFO
--rw-r--r--   0 vblidh     (501) staff       (20)      323 2023-03-03 12:48:02.000000 dynamocli-0.0.7/dynamocli.egg-info/SOURCES.txt
--rw-r--r--   0 vblidh     (501) staff       (20)        1 2023-03-03 12:48:02.000000 dynamocli-0.0.7/dynamocli.egg-info/dependency_links.txt
--rw-r--r--   0 vblidh     (501) staff       (20)       48 2023-03-03 12:48:02.000000 dynamocli-0.0.7/dynamocli.egg-info/entry_points.txt
--rw-r--r--   0 vblidh     (501) staff       (20)       19 2023-03-03 12:48:02.000000 dynamocli-0.0.7/dynamocli.egg-info/requires.txt
--rw-r--r--   0 vblidh     (501) staff       (20)        8 2023-03-03 12:48:02.000000 dynamocli-0.0.7/dynamocli.egg-info/top_level.txt
-drwxr-xr-x   0 vblidh     (501) staff       (20)        0 2023-03-03 12:48:02.532541 dynamocli-0.0.7/dynocli/
--rw-r--r--   0 vblidh     (501) staff       (20)       42 2023-01-13 17:25:15.000000 dynamocli-0.0.7/dynocli/__init__.py
--rw-r--r--   0 vblidh     (501) staff       (20)      817 2023-01-20 09:25:05.000000 dynamocli-0.0.7/dynocli/document_visualizer.py
--rw-r--r--   0 vblidh     (501) staff       (20)     6415 2023-01-20 15:40:12.000000 dynamocli-0.0.7/dynocli/dynamo_gateway.py
--rw-r--r--   0 vblidh     (501) staff       (20)     6449 2023-03-03 12:45:03.000000 dynamocli-0.0.7/dynocli/dyno.py
--rw-r--r--   0 vblidh     (501) staff       (20)       80 2022-12-30 15:39:08.000000 dynamocli-0.0.7/pyproject.toml
--rw-r--r--   0 vblidh     (501) staff       (20)       38 2023-03-03 12:48:02.532861 dynamocli-0.0.7/setup.cfg
--rw-r--r--   0 vblidh     (501) staff       (20)      633 2023-03-03 12:46:35.000000 dynamocli-0.0.7/setup.py
+drwxr-xr-x   0 vblidh     (501) staff       (20)        0 2023-06-09 12:46:35.489827 dynamocli-0.0.8/
+-rw-r--r--   0 vblidh     (501) staff       (20)     1873 2023-06-09 12:46:35.489718 dynamocli-0.0.8/PKG-INFO
+-rw-r--r--   0 vblidh     (501) staff       (20)     1624 2023-06-09 12:43:10.000000 dynamocli-0.0.8/README
+drwxr-xr-x   0 vblidh     (501) staff       (20)        0 2023-06-09 12:46:35.489179 dynamocli-0.0.8/dynamocli.egg-info/
+-rw-r--r--   0 vblidh     (501) staff       (20)     1873 2023-06-09 12:46:35.000000 dynamocli-0.0.8/dynamocli.egg-info/PKG-INFO
+-rw-r--r--   0 vblidh     (501) staff       (20)      323 2023-06-09 12:46:35.000000 dynamocli-0.0.8/dynamocli.egg-info/SOURCES.txt
+-rw-r--r--   0 vblidh     (501) staff       (20)        1 2023-06-09 12:46:35.000000 dynamocli-0.0.8/dynamocli.egg-info/dependency_links.txt
+-rw-r--r--   0 vblidh     (501) staff       (20)       48 2023-06-09 12:46:35.000000 dynamocli-0.0.8/dynamocli.egg-info/entry_points.txt
+-rw-r--r--   0 vblidh     (501) staff       (20)       19 2023-06-09 12:46:35.000000 dynamocli-0.0.8/dynamocli.egg-info/requires.txt
+-rw-r--r--   0 vblidh     (501) staff       (20)        8 2023-06-09 12:46:35.000000 dynamocli-0.0.8/dynamocli.egg-info/top_level.txt
+drwxr-xr-x   0 vblidh     (501) staff       (20)        0 2023-06-09 12:46:35.489577 dynamocli-0.0.8/dynocli/
+-rw-r--r--   0 vblidh     (501) staff       (20)       42 2023-01-13 17:25:15.000000 dynamocli-0.0.8/dynocli/__init__.py
+-rw-r--r--   0 vblidh     (501) staff       (20)      817 2023-01-20 09:25:05.000000 dynamocli-0.0.8/dynocli/document_visualizer.py
+-rw-r--r--   0 vblidh     (501) staff       (20)     6522 2023-06-09 12:45:14.000000 dynamocli-0.0.8/dynocli/dynamo_gateway.py
+-rw-r--r--   0 vblidh     (501) staff       (20)     6622 2023-06-09 12:45:47.000000 dynamocli-0.0.8/dynocli/dyno.py
+-rw-r--r--   0 vblidh     (501) staff       (20)       80 2022-12-30 15:39:08.000000 dynamocli-0.0.8/pyproject.toml
+-rw-r--r--   0 vblidh     (501) staff       (20)       38 2023-06-09 12:46:35.489857 dynamocli-0.0.8/setup.cfg
+-rw-r--r--   0 vblidh     (501) staff       (20)      633 2023-06-09 12:45:18.000000 dynamocli-0.0.8/setup.py
```

### Comparing `dynamocli-0.0.7/PKG-INFO` & `dynamocli-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamocli
-Version: 0.0.7
+Version: 0.0.8
 Summary: Command line interface for interacting with a DynamoDB instance
 Author: Viktor Blidh
 Author-email: viktor.blidh@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # DynamoDB CLI
```

### Comparing `dynamocli-0.0.7/README` & `dynamocli-0.0.8/README`

 * *Files identical despite different names*

### Comparing `dynamocli-0.0.7/dynamocli.egg-info/PKG-INFO` & `dynamocli-0.0.8/dynamocli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamocli
-Version: 0.0.7
+Version: 0.0.8
 Summary: Command line interface for interacting with a DynamoDB instance
 Author: Viktor Blidh
 Author-email: viktor.blidh@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # DynamoDB CLI
```

### Comparing `dynamocli-0.0.7/dynocli/document_visualizer.py` & `dynamocli-0.0.8/dynocli/document_visualizer.py`

 * *Files identical despite different names*

### Comparing `dynamocli-0.0.7/dynocli/dynamo_gateway.py` & `dynamocli-0.0.8/dynocli/dynamo_gateway.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,31 +137,31 @@
         return items
 
     def scan(self, **kwargs):
         key = kwargs.get('key')
         opr = kwargs.get('opr')
         val = kwargs.get('value')
         items = []
-        obj = Key(key)
-        m = getattr(obj, opr)
-        fe = m(val)
-        res = self.table.scan(FilterExpression=fe, Limit=100)
+        keyObject = Key(key)
+        conditionMethod = getattr(keyObject, opr)
+        filter_expression = conditionMethod(val)
+        res = self.table.scan(FilterExpression=filter_expression, Limit=100)
         items.extend(res.get('Items'))
 
         last_evaluated = res.get('LastEvaluatedKey')
         done = last_evaluated is None
         i = 1
         while not done and i < 100:
             print('scan iteration', i)
             iteration_res = self.table.scan(
-                FilterExpression=fe, Limit=100, ExclusiveStartKey=last_evaluated)
+                FilterExpression=filter_expression, Limit=100, ExclusiveStartKey=last_evaluated)
             items.extend(iteration_res.get('Items'))
             last_evaluated = iteration_res.get('LastEvaluatedKey')
             done = last_evaluated is None
             i += 1
 
-        print(items)
+        self.visualizer.print_items(items)
 
     def describe_table(self):
         description = self.client.describe_table(TableName=self.table_name)
         self.logger.debug(description)
         print(description)
```

### Comparing `dynamocli-0.0.7/dynocli/dyno.py` & `dynamocli-0.0.8/dynocli/dyno.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,18 @@
             attr = input('Select attribute to remove ')
             update['attribute'] = attr
         updates.append(update)
         resp = input('Add more operations? (y/N) ')
         done = not resp or not resp.lower().startswith('y')
     return updates
 
+def print_config(config: configparser.ConfigParser):
+    conn = config['Connection']
+    for key in conn:
+        print(f'{key}: {conn[key]}')
 
 def main():
     parser = argparse.ArgumentParser(
         description="A simple command line tool to interact with a DynamoDB instance."
     )
     parser.add_argument(
         'op', choices=['describe', 'query', 'scan', 'get-config', 'set-config'])
@@ -80,29 +84,30 @@
     config = configparser.ConfigParser()
     config_dir_path = user_config_dir('dynocli')
     config_file_path = os.path.join(config_dir_path, '.config.ini')
     if args.op == 'set-config':
         if not os.path.isdir(config_dir_path):
             mkdir(path=config_dir_path)
         is_new = not os.path.isfile(config_file_path)
+        print(config_dir_path)
         if not is_new:
             config.read(config_file_path)
         config = update_configuration(config=config, is_new=is_new)
         with open(config_file_path, 'w') as config_file:
             config.write(config_file)
         return
     if not os.path.isfile(config_file_path):
         raise Exception(
             'No configuration file found. Use --set-config to create one')
     config.read(config_file_path)
-    dynamo_gateway = DynamoGateway(config, args.verbose)
     if (args.op == 'get-config'):
         config.read(config_file_path)
-        print(dict(config))
-    elif args.op == 'describe':
+        print_config(config)
+    dynamo_gateway = DynamoGateway(config, args.verbose)
+    if args.op == 'describe':
         dynamo_gateway.describe_table()
     elif (args.op == 'query'):
         index = args.index
         pk = args.pk
         sk = args.pk if args.sk == 'pk' else args.sk if args.sk else ''
         items = dynamo_gateway.query(index, pk, sk)
         if (items):
```

### Comparing `dynamocli-0.0.7/setup.py` & `dynamocli-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README", "r", encoding="utf-8") as fhand:
     long_description = fhand.read()
 
 setup(
     name='dynamocli',
     author='Viktor Blidh',
     author_email='viktor.blidh@gmail.com',
-    version='0.0.7',
+    version='0.0.8',
     description='Command line interface for interacting with a DynamoDB instance',
     long_description_content_type="text/markdown",
     long_description=long_description,
     install_requires=[
         'boto3',
         'rich',
         'appdirs'
```

