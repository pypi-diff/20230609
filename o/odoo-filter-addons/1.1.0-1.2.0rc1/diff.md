# Comparing `tmp/odoo_filter_addons-1.1.0.tar.gz` & `tmp/odoo_filter_addons-1.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_filter_addons-1.1.0.tar", last modified: Mon Mar 20 14:00:32 2023, max compression
+gzip compressed data, was "odoo_filter_addons-1.2.0rc1.tar", last modified: Fri Jun  9 08:43:08 2023, max compression
```

## Comparing `odoo_filter_addons-1.1.0.tar` & `odoo_filter_addons-1.2.0rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:00:32.083802 odoo_filter_addons-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-20 14:00:32.083802 odoo_filter_addons-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-03-20 14:00:15.000000 odoo_filter_addons-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:00:32.079802 odoo_filter_addons-1.1.0/odoo_filter_addons/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-20 14:00:15.000000 odoo_filter_addons-1.1.0/odoo_filter_addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-03-20 14:00:15.000000 odoo_filter_addons-1.1.0/odoo_filter_addons/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-20 14:00:15.000000 odoo_filter_addons-1.1.0/odoo_filter_addons/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:00:32.083802 odoo_filter_addons-1.1.0/odoo_filter_addons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-20 14:00:32.000000 odoo_filter_addons-1.1.0/odoo_filter_addons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-20 14:00:32.000000 odoo_filter_addons-1.1.0/odoo_filter_addons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 14:00:32.000000 odoo_filter_addons-1.1.0/odoo_filter_addons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-20 14:00:32.000000 odoo_filter_addons-1.1.0/odoo_filter_addons.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-20 14:00:32.000000 odoo_filter_addons-1.1.0/odoo_filter_addons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-20 14:00:32.000000 odoo_filter_addons-1.1.0/odoo_filter_addons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-20 14:00:15.000000 odoo_filter_addons-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 14:00:32.083802 odoo_filter_addons-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-20 14:00:15.000000 odoo_filter_addons-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:43:08.847087 odoo_filter_addons-1.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-09 08:43:08.847087 odoo_filter_addons-1.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:43:08.847087 odoo_filter_addons-1.2.0rc1/odoo_filter_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:43:08.847087 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:43:08.847087 odoo_filter_addons-1.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/setup.py
```

### Comparing `odoo_filter_addons-1.1.0/PKG-INFO` & `odoo_filter_addons-1.2.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo_filter_addons
-Version: 1.1.0
+Version: 1.2.0rc1
 Summary: Simple utlity to filter odoo addons into a single directory
 Author-email: Pablo Esteban <pablo.esteban@forgeflow.com>
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX
 Classifier: Framework :: Odoo
 Classifier: Programming Language :: Python :: 3
@@ -34,12 +34,13 @@
 results of running `gitaggregate` into the specified output directory.
 
 By default, both the input and output path default to the current working directory,
 but can be overridden through the `-i/--input-path` and `-o/--output-path` flags
 respectively. Additionally, some other flags can be provided to alter the behavior of
 the program:
 
-| Flag                      | Default | Description                                               |
-|---------------------------|---------|-----------------------------------------------------------|
-| -c, --clean / --no-clean  | True    | Clean intermediate output                                 |
-| -p, --push / --no-push    | False   | Push to remote repo if any changes are commited           |
-| -g, --gitlab-ci           | False   | Update client addon repository in GitLab CI               |
+| Flag                          | Default | Description                                               |
+|-------------------------------|---------|-----------------------------------------------------------|
+| -c, --clean / --no-clean      | True    | Clean intermediate output                                 |
+| -r, --release / --no-release  | False   | Create a release commit if any changes are made           |
+| -p, --push / --no-push        | False   | Push to remote repo if any changes are commited           |
+| -g, --gitlab-ci               | False   | Update client addon repository in GitLab CI               |
```

### Comparing `odoo_filter_addons-1.1.0/odoo_filter_addons/main.py` & `odoo_filter_addons-1.2.0rc1/odoo_filter_addons/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         else:
             last_hash = git("-C", rpath, "rev-parse", merge.replace(" ", "/"))
         lines.append("{} {}".format(merge, last_hash).strip())
     message = "\n".join(lines)
     print("Partial message:\n{}".format(message))
     return message
 
-def filter_repos(output_path, tmp_path, repos, addons, push, gitlab_ci):
+def filter_repos(output_path, tmp_path, repos, addons, release, push, gitlab_ci):
     os.chdir(output_path)
     # Remove old modules
     for fname in next(os.walk("."))[1]:
         if is_module(fname):
             git("rm", "-rf", fname)
     # Add new modules
     messages = []
@@ -96,15 +96,17 @@
         repo = repos.get(rname) or repos.get("./{}".format(rname))
         if not repo:
             raise UserException("addons.yml entry {} not found in repos.yml".format(rname))
         repo_message = filter_repo(tmp_path, rname, repo, modules)
         messages.append(repo_message)
     print_header("Finished filtering", '*')
     # Commit changes, if any, and push them to remote if specified
-    if filter(None, messages) and git["diff", "--staged", "--quiet"] & TF(1):
+    if not release:
+        print("No changes, nothing commited")
+    elif filter(None, messages) and git["diff", "--staged", "--quiet"] & TF(1):
         messages = [f"[AUTO] {__package__} {__version__}"] + messages
         message = "\n".join(messages)
         git("commit", "-m", message)
         print("Changes commited")
         if push:
             if git["rev-parse", "@{u}"] & TF:
                 git("push")
@@ -158,51 +160,52 @@
     with set_argv(new_argv):
         gitaggregate()
     print("Writing gitaggregate output to '{}'".format(tmp_path))
 
 #####################################################################
 
 # API entry point
-def main(input_path=None, output_path=None, clean=True, push=False, gitlab_ci=False):
+def main(input_path=None, output_path=None, clean=True, release=False, push=False, gitlab_ci=False):
     input_path = Path(input_path).resolve() if input_path else Path.cwd()
     output_path = Path(output_path).resolve() if output_path else Path.cwd()
     tmp_path = Path(mkdtemp())
 
     print("Loading configuration files from '{}'".format(input_path))
     repos, repos_suffix = load_yml(input_path/"repos", True)
     addons, addons_suffix = load_yml(input_path/"addons")
     if gitlab_ci:
         repos = update_ci_urls(repos)
         dump_yml("repos.yml", update_ci_urls(repos))
 
     try:
         print("Filtering addons to '{}'".format(output_path))
         initialize_repos(output_path, input_path, tmp_path, repos_suffix)
-        filter_repos(output_path, tmp_path, repos, addons, push, gitlab_ci)
+        filter_repos(output_path, tmp_path, repos, addons, release, push, gitlab_ci)
     except Exception as e:
         if clean:
             rmtree(tmp_path)
         raise e
     if clean:
         print("Cleaning up intermediate output")
         rmtree(tmp_path)
 
 # CLI entry point
 @click.command(context_settings=dict(help_option_names=['-h', '--help']))
 @click.version_option()
 @click.option("-i", "--input-path", help="Path to directory containing configuration files.")
 @click.option("-o", "--output-path", help="Path to the directory that will contain the output.")
 @click.option("-c", "--clean/--no-clean", is_flag=True, default=True, help="Clean intermediate output.")
+@click.option("-r", "--release/--no-release", is_flag=True, default=False, help="Create a relase commit if any changes are made.")
 @click.option("-p", "--push/--no-push", is_flag=True, default=False, help="Push to remote repo if any changes are commited.")
 @click.option("-g", "--gitlab-ci", is_flag=True, default=False, help="Update client addon repository in GitLab CI.")
-def cli_main(input_path, output_path, clean, push, gitlab_ci):
+def cli_main(input_path, output_path, clean, release, push, gitlab_ci):
     import sys
     import traceback
     try:
-        main(input_path, output_path, clean, push, gitlab_ci)
+        main(input_path, output_path, clean, release, push, gitlab_ci)
         sys.exit(0)
     except UserException as e:
         print("User error:", e)
     except yaml.YAMLError as e:
         print("Invalid YAML content:", e)
     except ProcessExecutionError as e:
         print("Process execution error:", e)
```

### Comparing `odoo_filter_addons-1.1.0/odoo_filter_addons.egg-info/PKG-INFO` & `odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-filter-addons
-Version: 1.1.0
+Version: 1.2.0rc1
 Summary: Simple utlity to filter odoo addons into a single directory
 Author-email: Pablo Esteban <pablo.esteban@forgeflow.com>
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX
 Classifier: Framework :: Odoo
 Classifier: Programming Language :: Python :: 3
@@ -34,12 +34,13 @@
 results of running `gitaggregate` into the specified output directory.
 
 By default, both the input and output path default to the current working directory,
 but can be overridden through the `-i/--input-path` and `-o/--output-path` flags
 respectively. Additionally, some other flags can be provided to alter the behavior of
 the program:
 
-| Flag                      | Default | Description                                               |
-|---------------------------|---------|-----------------------------------------------------------|
-| -c, --clean / --no-clean  | True    | Clean intermediate output                                 |
-| -p, --push / --no-push    | False   | Push to remote repo if any changes are commited           |
-| -g, --gitlab-ci           | False   | Update client addon repository in GitLab CI               |
+| Flag                          | Default | Description                                               |
+|-------------------------------|---------|-----------------------------------------------------------|
+| -c, --clean / --no-clean      | True    | Clean intermediate output                                 |
+| -r, --release / --no-release  | False   | Create a release commit if any changes are made           |
+| -p, --push / --no-push        | False   | Push to remote repo if any changes are commited           |
+| -g, --gitlab-ci               | False   | Update client addon repository in GitLab CI               |
```

### Comparing `odoo_filter_addons-1.1.0/pyproject.toml` & `odoo_filter_addons-1.2.0rc1/pyproject.toml`

 * *Files identical despite different names*

