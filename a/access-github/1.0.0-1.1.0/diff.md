# Comparing `tmp/access-github-1.0.0.tar.gz` & `tmp/access-github-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "access-github-1.0.0.tar", last modified: Sun May 28 12:20:58 2023, max compression
+gzip compressed data, was "access-github-1.1.0.tar", last modified: Fri Jun  9 13:19:55 2023, max compression
```

## Comparing `access-github-1.0.0.tar` & `access-github-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-28 12:20:58.555766 access-github-1.0.0/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4785 2023-05-28 12:20:58.555624 access-github-1.0.0/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     4686 2023-05-28 12:20:58.000000 access-github-1.0.0/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-28 12:20:58.555419 access-github-1.0.0/access_github.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4785 2023-05-28 12:20:58.000000 access-github-1.0.0/access_github.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      259 2023-05-28 12:20:58.000000 access-github-1.0.0/access_github.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-28 12:20:58.000000 access-github-1.0.0/access_github.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       53 2023-05-28 12:20:58.000000 access-github-1.0.0/access_github.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        9 2023-05-28 12:20:58.000000 access-github-1.0.0/access_github.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       14 2023-05-28 12:20:58.000000 access-github-1.0.0/access_github.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     7843 2023-05-28 12:20:58.000000 access-github-1.0.0/access_github.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-28 12:20:58.555808 access-github-1.0.0/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      516 2023-05-28 12:20:58.000000 access-github-1.0.0/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-09 13:19:55.642040 access-github-1.1.0/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4785 2023-06-09 13:19:55.641924 access-github-1.1.0/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4686 2023-06-09 13:19:55.000000 access-github-1.1.0/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-09 13:19:55.641762 access-github-1.1.0/access_github.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4785 2023-06-09 13:19:55.000000 access-github-1.1.0/access_github.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      259 2023-06-09 13:19:55.000000 access-github-1.1.0/access_github.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-06-09 13:19:55.000000 access-github-1.1.0/access_github.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       53 2023-06-09 13:19:55.000000 access-github-1.1.0/access_github.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        9 2023-06-09 13:19:55.000000 access-github-1.1.0/access_github.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       14 2023-06-09 13:19:55.000000 access-github-1.1.0/access_github.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)    10421 2023-06-09 13:19:55.000000 access-github-1.1.0/access_github.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-06-09 13:19:55.642073 access-github-1.1.0/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      516 2023-06-09 13:19:55.000000 access-github-1.1.0/setup.py
```

### Comparing `access-github-1.0.0/PKG-INFO` & `access-github-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access-github
-Version: 1.0.0
+Version: 1.1.0
 Description-Content-Type: text/markdown
 
 # Access GitHub
 
 ## 緣由與動機
 🔑關鍵：最關鍵的動機是讓全球百萬開發者，都能免費享受分散運算 20 VMs 加速能力!驅動 Github Actions。
 💣地雷：直接去用 gpt-4 開發 github api 會撞牆，寫出一堆與最新文件不相容的程式碼，因此要避開此地雷。
```

### Comparing `access-github-1.0.0/README.md` & `access-github-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `access-github-1.0.0/access_github.egg-info/PKG-INFO` & `access-github-1.1.0/access_github.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access-github
-Version: 1.0.0
+Version: 1.1.0
 Description-Content-Type: text/markdown
 
 # Access GitHub
 
 ## 緣由與動機
 🔑關鍵：最關鍵的動機是讓全球百萬開發者，都能免費享受分散運算 20 VMs 加速能力!驅動 Github Actions。
 💣地雷：直接去用 gpt-4 開發 github api 會撞牆，寫出一堆與最新文件不相容的程式碼，因此要避開此地雷。
```

### Comparing `access-github-1.0.0/access_github.py` & `access-github-1.1.0/access_github.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,69 @@
 #!/usr/bin/env python
 # access_github.py
 import argparse
 import base64
+import os
 
 import requests
 
 
-def get_tree(token, url):
-    repo_api_url = get_repo_api_url(url)
-    headers = get_headers_with_authorization_and_version(token)
+def get_tree(token, repo_url):
+    headers, repo_api_url = get_api_url_headers(token, repo_url)
     response = requests.get(f"{repo_api_url}/branches/main", headers=headers)
     response_json = response.json()
     latest_commit_sha = response_json['commit']['sha']
 
     tree_url = f"{repo_api_url}/git/trees/{latest_commit_sha}?recursive=1"
     response = requests.get(tree_url, headers=headers)
     tree = response.json()
     return tree
 
 
-def read_file(token, url, path):
-    repo_api_url = get_repo_api_url(url)
-    file_url = f"{repo_api_url}/contents/{path}"
-    headers = get_headers_with_authorization(token)
-    response = requests.get(file_url, headers=headers)
-    content = response.json()
-    return content
+def read_file(token, repo_url, path):
+    headers, repo_api_url = get_api_url_headers(token, repo_url)
+    return requests.get(f"{repo_api_url}/contents/{path}", headers=headers).json()
 
 
-def update_file(token, name, email, url, path, content):
-    repo_api_url = get_repo_api_url(url)
+def update_file(token, name, email, repo_url, path, content):
+    headers, repo_api_url = get_api_url_headers(token, repo_url)
     file_url = f"{repo_api_url}/contents/{path}"
-    headers = get_headers_with_authorization_and_version(token)
     response = requests.get(file_url, headers=headers)
 
     if response.status_code == 200:
         response = update_existing_file(file_url, content, email, headers, name, response)
 
     return response.json()
 
 
-def create(token, name, email, url, path, content=None, is_folder=False):  # 添加 content 參數
-    repo_api_url = get_repo_api_url(url)
-    headers = get_headers_with_authorization_and_version(token)
+def create(token, name, email, repo_url, path, content=None, is_folder=False):  # 添加 content 參數
+    headers, repo_api_url = get_api_url_headers(token, repo_url)
     file_url = f"{repo_api_url}/contents/{path}"
 
     if content is None:  # 新增這個條件判斷
         content = ""
 
     create_data = get_create_data(name, email, content)  # 將 content 傳遞給 get_create_data 函數
 
     if is_folder:
         path += "/.gitkeep"
 
     response = requests.put(file_url, json=create_data, headers=headers)
     return response.json()
 
 
-def delete(token, url, path, is_folder=False):
-    repo_api_url = get_repo_api_url(url)
-    headers = get_headers_with_authorization_and_version(token)
+def delete(token, repo_url, path, is_folder=False):
+    headers, repo_api_url = get_api_url_headers(token, repo_url)
 
     if is_folder:
         return delete_folder(repo_api_url, headers, path)
     else:
         return delete_file(repo_api_url, headers, path)
 
 
-def main():
-    parser = get_arg_parser()
-    args = parser.parse_args()
-
-    operations = {
-        "get_tree": get_tree,
-        "read_file": read_file,
-        "update_file": update_file,
-        "create": create,
-        "delete": delete,
-        "create_or_update_github_action": create_or_update_github_action,
-        "dispatch_github_action": dispatch_github_action,
-    }
-
-    operation = operations[args.operation]
-    required_args = operation.__code__.co_varnames[:operation.__code__.co_argcount]
-
-    operation_args = {k: v for k, v in vars(args).items() if k in required_args and v is not None}
-
-    if args.operation == "create" and args.content:
-        operation_args["content"] = args.content
-
-    if args.operation == "get_tree":  # Add these lines
-        operation_args["repo_api_url"] = get_repo_api_url(args.url)
-        operation_args["headers"] = get_headers_with_authorization_and_version(args.token)
-
-    result = operation(**operation_args)
-    print(result)
-
-
 def update_existing_file(file_url, content, email, headers, name, response):
     file_data = response.json()
     sha = file_data["sha"]
     update_data = get_update_data(name, email, content, sha)
     response = requests.put(file_url, json=update_data, headers=headers)
     return response
 
@@ -170,25 +133,24 @@
 
 def get_tree(repo_api_url, headers):
     tree_url = f"{repo_api_url}/git/trees/main?recursive=1"
     response = requests.get(tree_url, headers=headers)
     return response.json()
 
 
-def create_or_update_github_action(token, url, path, content):
-    existing_file = read_file(token, url, path)
+def create_or_update_github_action(token, repo_url, path, content):
+    existing_file = read_file(token, repo_url, path)
     if 'message' in existing_file and existing_file['message'] == 'Not Found':
-        create(token, 'GitHub Actions Bot', 'actions@github.com', url, path, content)
+        create(token, 'GitHub Actions Bot', 'actions@github.com', repo_url, path, content)
     else:
-        return update_file(token, 'GitHub Actions Bot', 'actions@github.com', url, path, content)
+        return update_file(token, 'GitHub Actions Bot', 'actions@github.com', repo_url, path, content)
 
 
-def dispatch_github_action(token, url, workflow_yml_filename, event_type=None, client_payload=None):
-    repo_api_url = get_repo_api_url(url)
-    headers = get_headers_with_authorization_and_version(token)
+def dispatch_github_action(token, repo_url, workflow_yml_filename, event_type=None, client_payload=None):
+    headers, repo_api_url = get_api_url_headers(token, repo_url)
     dispatch_url = f"{repo_api_url}/actions/workflows/{workflow_yml_filename}/dispatches"
 
     data = {
         'ref': 'main',
         'inputs': {}
     }
 
@@ -197,32 +159,126 @@
     if client_payload:
         data['inputs']['client_payload'] = client_payload
 
     response = requests.post(dispatch_url, json=data, headers=headers)
     return response.text
 
 
+def get_workflow_runs(token, repo_url, workflow_yml_filename, per_page=1):
+    headers, repo_api_url = get_api_url_headers(token, repo_url)
+    return requests.get(f"{repo_api_url}/actions/workflows/{workflow_yml_filename}/runs?per_page={per_page}",
+                        headers=headers).json()
+
+
+def get_run_status(token, repo_url, run_id):
+    headers, repo_api_url = get_api_url_headers(token, repo_url)
+    return requests.get(f"{repo_api_url}/actions/runs/{run_id}", headers=headers).json()
+
+
+def get_api_url_headers(token, repo_url):
+    repo_api_url = get_repo_api_url(repo_url)
+    headers = get_headers_with_authorization_and_version(token)
+    return headers, repo_api_url
+
+
+def get_latest_artifacts_url(token, repo_url, workflow_yml_filename):
+    workflow_runs = get_workflow_runs(token, repo_url, workflow_yml_filename, 1)
+    latest_run_id = workflow_runs['workflow_runs'][0]['id']
+    latest_run_status = get_run_status(token, repo_url, latest_run_id)
+    latest_artifacts_url = latest_run_status['artifacts_url']
+    return latest_artifacts_url
+
+
+def download_latest_artifacts(token, repo_url, workflow_yml_filename, output_path):
+    latest_artifacts_url = get_latest_artifacts_url(token, repo_url, workflow_yml_filename)
+    artifacts = requests.get(latest_artifacts_url, headers=get_headers_with_authorization(token)).json()
+
+    if not artifacts['artifacts']:
+        raise ValueError("No artifacts found for the specified workflow.")
+
+    artifact_download_url = artifacts['artifacts'][0]['archive_download_url']
+    file_name = artifacts['artifacts'][0]['name']
+    download_response = requests.get(artifact_download_url, headers=get_headers_with_authorization(token), stream=True)
+    download_response.raise_for_status()
+
+    dir1 = os.path.dirname(output_path)
+    if not os.path.exists(dir1):
+        os.makedirs(dir1)
+
+    with open(os.path.join(output_path), 'wb') as f:
+        for chunk in download_response.iter_content(chunk_size=8192):
+            f.write(chunk)
+
+    print(f"Artifacts downloaded to: {output_path}")
+    return output_path
+
+
 def get_arg_parser():
     parser = argparse.ArgumentParser(description="Access GitHub")
     parser.add_argument("operation",
                         choices=["get_tree",
                                  "read_file",
                                  "update_file",
                                  "create",
                                  "delete",
                                  "create_or_update_github_action",
-                                 "dispatch_github_action"])
+                                 "dispatch_github_action",
+                                 "get_workflow_runs",
+                                 "get_run_status",
+                                 "get_latest_artifacts_url",
+                                 "download_latest_artifacts",
+                                 ])
     parser.add_argument("--token", type=str, required=True)
-    parser.add_argument("--url", type=str, required=True)
+    parser.add_argument("--repo_url", type=str, required=True)
     parser.add_argument("--path", type=str)
     parser.add_argument("--content", type=str)
     parser.add_argument("--is_folder", action="store_true")
     parser.add_argument("--name", type=str)
     parser.add_argument("--email", type=str)
     parser.add_argument("--workflow_yml_filename", type=str)
     parser.add_argument("--event_type", type=str)
     parser.add_argument("--client_payload", type=str)
+    parser.add_argument("--per_page", type=int, default=1)
+    parser.add_argument("--run_id", type=str)
+    parser.add_argument("--output_path", type=str)
     return parser
 
 
+def main():
+    parser = get_arg_parser()
+    args = parser.parse_args()
+
+    operations = {
+        "get_tree": get_tree,
+        "read_file": read_file,
+        "update_file": update_file,
+        "create": create,
+        "delete": delete,
+        "create_or_update_github_action": create_or_update_github_action,
+        "dispatch_github_action": dispatch_github_action,
+        "get_workflow_runs": get_workflow_runs,
+        "get_run_status": get_run_status,
+        "get_latest_artifacts_url": get_latest_artifacts_url,
+        "download_latest_artifacts": download_latest_artifacts,
+    }
+
+    operation = operations[args.operation]
+    required_args = operation.__code__.co_varnames[:operation.__code__.co_argcount]
+
+    operation_args = {k: v for k, v in vars(args).items() if k in required_args and v is not None}
+
+    if args.operation == "create" and args.content:
+        operation_args["content"] = args.content
+
+    if args.operation == "get_tree":
+        operation_args["repo_api_url"] = get_repo_api_url(args.repo_url)
+        operation_args["headers"] = get_headers_with_authorization_and_version(args.token)
+
+    if args.operation == "download_latest_artifacts":
+        operation_args["output_path"] = args.output_path
+
+    result = operation(**operation_args)
+    print(result)
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `access-github-1.0.0/setup.py` & `access-github-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="access-github",
-    version="1.0.0",
+    version="1.1.0",
     packages=find_packages(),
     py_modules=['access_github'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'access_github = access_github:main',
         ],
```

