# Comparing `tmp/frontmatter_cli-2023.3.1.tar.gz` & `tmp/frontmatter_cli-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jefftriplett/.virtualenvs/frontmatter-cli/src/frontmatter-cli-git/dist/tmpacuheaaq/frontmatter_cli-2023.3.1.tar", last modified: Tue Mar 14 01:52:18 2023, max compression
+gzip compressed data, was "frontmatter_cli-2023.6.1.tar", last modified: Fri Jun  9 02:31:19 2023, max compression
```

## Comparing `frontmatter_cli-2023.3.1.tar` & `frontmatter_cli-2023.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-03-14 01:52:18.000000 frontmatter_cli-2023.3.1/
--rw-r--r--   0 jefftriplett   (501) staff       (20)     2222 2023-03-14 01:52:18.000000 frontmatter_cli-2023.3.1/PKG-INFO
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1513 2018-01-23 03:27:47.000000 frontmatter_cli-2023.3.1/LICENSE
--rw-r--r--   0 jefftriplett   (501) staff       (20)       11 2018-01-23 03:28:08.000000 frontmatter_cli-2023.3.1/HISTORY.md
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1289 2023-03-14 01:51:25.000000 frontmatter_cli-2023.3.1/pyproject.toml
--rw-r--r--   0 jefftriplett   (501) staff       (20)      134 2018-01-23 01:48:22.000000 frontmatter_cli-2023.3.1/MANIFEST.in
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1233 2023-03-14 01:25:41.000000 frontmatter_cli-2023.3.1/README.md
--rw-r--r--   0 jefftriplett   (501) staff       (20)       38 2021-04-10 18:01:51.000000 frontmatter_cli-2023.3.1/setup.py
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1221 2023-03-14 01:52:18.000000 frontmatter_cli-2023.3.1/setup.cfg
-drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-03-14 01:52:18.000000 frontmatter_cli-2023.3.1/frontmatter_cli/
--rw-r--r--   0 jefftriplett   (501) staff       (20)      160 2023-03-14 01:50:54.000000 frontmatter_cli-2023.3.1/frontmatter_cli/__init__.py
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1313 2023-03-14 01:50:54.000000 frontmatter_cli-2023.3.1/frontmatter_cli/cli.py
--rw-r--r--   0 jefftriplett   (501) staff       (20)       74 2020-07-11 04:28:39.000000 frontmatter_cli-2023.3.1/frontmatter_cli/__main__.py
-drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-03-14 01:52:18.000000 frontmatter_cli-2023.3.1/frontmatter_cli.egg-info/
--rw-r--r--   0 jefftriplett   (501) staff       (20)     2222 2023-03-14 01:52:18.000000 frontmatter_cli-2023.3.1/frontmatter_cli.egg-info/PKG-INFO
--rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2018-01-23 03:32:37.000000 frontmatter_cli-2023.3.1/frontmatter_cli.egg-info/not-zip-safe
--rw-r--r--   0 jefftriplett   (501) staff       (20)      427 2023-03-14 01:52:18.000000 frontmatter_cli-2023.3.1/frontmatter_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)       91 2023-03-14 01:52:18.000000 frontmatter_cli-2023.3.1/frontmatter_cli.egg-info/entry_points.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)       45 2023-03-14 01:52:18.000000 frontmatter_cli-2023.3.1/frontmatter_cli.egg-info/requires.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)       16 2023-03-14 01:52:18.000000 frontmatter_cli-2023.3.1/frontmatter_cli.egg-info/top_level.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-03-14 01:52:18.000000 frontmatter_cli-2023.3.1/frontmatter_cli.egg-info/dependency_links.txt
+drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-06-09 02:31:19.274107 frontmatter_cli-2023.6.1/
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       11 2023-06-09 02:13:44.000000 frontmatter_cli-2023.6.1/HISTORY.md
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1513 2023-06-09 02:13:44.000000 frontmatter_cli-2023.6.1/LICENSE
+-rw-r--r--   0 jefftriplett   (501) staff       (20)      134 2023-06-09 02:13:44.000000 frontmatter_cli-2023.6.1/MANIFEST.in
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     2652 2023-06-09 02:31:19.274159 frontmatter_cli-2023.6.1/PKG-INFO
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1683 2023-06-09 02:23:17.000000 frontmatter_cli-2023.6.1/README.md
+drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-06-09 02:31:19.272969 frontmatter_cli-2023.6.1/frontmatter_cli/
+-rw-r--r--   0 jefftriplett   (501) staff       (20)      160 2023-06-09 02:26:44.000000 frontmatter_cli-2023.6.1/frontmatter_cli/__init__.py
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       74 2023-06-09 02:13:44.000000 frontmatter_cli-2023.6.1/frontmatter_cli/__main__.py
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1364 2023-06-09 02:26:44.000000 frontmatter_cli-2023.6.1/frontmatter_cli/cli.py
+drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-06-09 02:31:19.274006 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     2652 2023-06-09 02:31:19.000000 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jefftriplett   (501) staff       (20)      427 2023-06-09 02:31:19.000000 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-06-09 02:31:19.000000 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       90 2023-06-09 02:31:19.000000 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-06-09 02:14:15.000000 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/not-zip-safe
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       52 2023-06-09 02:31:19.000000 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/requires.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       16 2023-06-09 02:31:19.000000 frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/top_level.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1291 2023-06-09 02:26:44.000000 frontmatter_cli-2023.6.1/pyproject.toml
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1229 2023-06-09 02:31:19.274470 frontmatter_cli-2023.6.1/setup.cfg
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       38 2023-06-09 02:13:44.000000 frontmatter_cli-2023.6.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `frontmatter_cli-2023.3.1/PKG-INFO` & `frontmatter_cli-2023.6.1/frontmatter_cli.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: frontmatter_cli
-Version: 2023.3.1
+Name: frontmatter-cli
+Version: 2023.6.1
 Summary: Frontmatter CLI tool to make working with frontmatter easier.
 Home-page: https://github.com/jefftriplett/frontmatter-cli
 Author: Jeff Triplett
 Author-email: jeff.triplett@gmail.com
 License: BSD-3-Clause
 Keywords: frontmatter,frontmatter-cli
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -52,17 +51,26 @@
 ---
 title: My New Blog Post
 ---
 
 Hello World!
 ```
 
+## Contributing
+
+PRs are welcome at <https://github.com/jefftriplett/frontmatter-cli>.
+
+Linting should be verified by running `just lint`. There are currently no tests, so `just test` is expected to fail.
+
+In addition to the development supporting packages that will be installed by `just`, you may need to install the following:
+
+- [just](https://github.com/casey/just#installation)
+- [pre-commit](https://pre-commit.com/) `pip install pre-commit`
+
 ## Contact / Social Media
 
 Here are a few ways to keep up with me online. If you have a question about this project, please consider opening a GitHub Issue.
 
 [![](https://jefftriplett.com/assets/images/social/github.png)](https://github.com/jefftriplett)
 [![](https://jefftriplett.com/assets/images/social/globe.png)](https://jefftriplett.com/)
 [![](https://jefftriplett.com/assets/images/social/twitter.png)](https://twitter.com/webology)
 [![](https://jefftriplett.com/assets/images/social/docker.png)](https://hub.docker.com/u/jefftriplett/)
-
-
```

### Comparing `frontmatter_cli-2023.3.1/LICENSE` & `frontmatter_cli-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frontmatter_cli-2023.3.1/pyproject.toml` & `frontmatter_cli-2023.6.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.bumpver]
-current_version = "2023.3.1"
+current_version = "2023.6.1"
 version_pattern = "YYYY.MM.INC1"
 commit_message = ":bookmark: Bump version {old_version} -> {new_version}"
 commit = true
 push = true  # disable for GitHub Actions
 tag = true
 
 [tool.bumpver.file_patterns]
@@ -53,13 +53,13 @@
 
 # Same as Black.
 line-length = 120
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-# Assume Python 3.7
-target-version = "py37"
+# Assume Python 3.11
+target-version = "py311"
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
```

### Comparing `frontmatter_cli-2023.3.1/README.md` & `frontmatter_cli-2023.6.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -26,14 +26,25 @@
 ---
 title: My New Blog Post
 ---
 
 Hello World!
 ```
 
+## Contributing
+
+PRs are welcome at <https://github.com/jefftriplett/frontmatter-cli>.
+
+Linting should be verified by running `just lint`. There are currently no tests, so `just test` is expected to fail.
+
+In addition to the development supporting packages that will be installed by `just`, you may need to install the following:
+
+- [just](https://github.com/casey/just#installation)
+- [pre-commit](https://pre-commit.com/) `pip install pre-commit`
+
 ## Contact / Social Media
 
 Here are a few ways to keep up with me online. If you have a question about this project, please consider opening a GitHub Issue.
 
 [![](https://jefftriplett.com/assets/images/social/github.png)](https://github.com/jefftriplett)
 [![](https://jefftriplett.com/assets/images/social/globe.png)](https://jefftriplett.com/)
 [![](https://jefftriplett.com/assets/images/social/twitter.png)](https://twitter.com/webology)
```

### Comparing `frontmatter_cli-2023.3.1/setup.cfg` & `frontmatter_cli-2023.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = frontmatter_cli
-version = 2023.3.1
+version = 2023.6.1
 description = Frontmatter CLI tool to make working with frontmatter easier.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jefftriplett/frontmatter-cli
 author = Jeff Triplett
 author_email = jeff.triplett@gmail.com
 license = BSD-3-Clause
@@ -25,14 +25,15 @@
 keywords = frontmatter, frontmatter-cli
 
 [options]
 packages = frontmatter_cli
 install_requires = 
 	click
 	click-default-group
+	pydash
 	python-frontmatter
 python_requires = >=3.7
 zip_safe = False
 
 [options.entry_points]
 console_scripts = 
 	frontmatter = frontmatter_cli:cli
```

### Comparing `frontmatter_cli-2023.3.1/frontmatter_cli/cli.py` & `frontmatter_cli-2023.6.1/frontmatter_cli/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 
 import click
 import frontmatter
 
 from click_default_group import DefaultGroup
+from pydash import set_
 
 __author__ = "Jeff Triplett"
 __email__ = "jeff.triplett@gmail.com"
-__version__ = "2023.3.1"
+__version__ = "2023.6.1"
 
 
 def validate_extra_context(ctx, param, value):
     """Validate extra context."""
-
     for key in value:
         if "=" not in key:
             raise click.BadParameter(
                 "EXTRA_CONTEXT should contain items of the form key=value; "
                 "'{}' doesn't match that form".format(key)
             )
 
@@ -25,28 +25,25 @@
 
 @click.group(cls=DefaultGroup, default="main", default_if_no_args=True)
 @click.pass_context
 def cli(context):
     pass
 
 
-@cli.command(
-    context_settings=dict(
-        ignore_unknown_options=True,
-    )
-)
+@cli.command(context_settings=dict(ignore_unknown_options=True))
 @click.version_option(prog_name="frontmatter-cli", version=__version__)
 @click.argument("extra_context", nargs=-1, callback=validate_extra_context)
 @click.argument("input", type=click.File("rb"), default="-")
 @click.argument("output", type=click.File("wb"), default="-")
 def main(input, output, extra_context):
     chunk = input.read()
     post = frontmatter.loads(chunk)
 
     if extra_context:
-        post.metadata.update(extra_context)
+        for key, value in extra_context.items():
+            set_(post.metadata, key, value)
 
     frontmatter.dump(post, output)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `frontmatter_cli-2023.3.1/frontmatter_cli.egg-info/PKG-INFO` & `frontmatter_cli-2023.6.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: frontmatter-cli
-Version: 2023.3.1
+Name: frontmatter_cli
+Version: 2023.6.1
 Summary: Frontmatter CLI tool to make working with frontmatter easier.
 Home-page: https://github.com/jefftriplett/frontmatter-cli
 Author: Jeff Triplett
 Author-email: jeff.triplett@gmail.com
 License: BSD-3-Clause
 Keywords: frontmatter,frontmatter-cli
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -52,17 +51,26 @@
 ---
 title: My New Blog Post
 ---
 
 Hello World!
 ```
 
+## Contributing
+
+PRs are welcome at <https://github.com/jefftriplett/frontmatter-cli>.
+
+Linting should be verified by running `just lint`. There are currently no tests, so `just test` is expected to fail.
+
+In addition to the development supporting packages that will be installed by `just`, you may need to install the following:
+
+- [just](https://github.com/casey/just#installation)
+- [pre-commit](https://pre-commit.com/) `pip install pre-commit`
+
 ## Contact / Social Media
 
 Here are a few ways to keep up with me online. If you have a question about this project, please consider opening a GitHub Issue.
 
 [![](https://jefftriplett.com/assets/images/social/github.png)](https://github.com/jefftriplett)
 [![](https://jefftriplett.com/assets/images/social/globe.png)](https://jefftriplett.com/)
 [![](https://jefftriplett.com/assets/images/social/twitter.png)](https://twitter.com/webology)
 [![](https://jefftriplett.com/assets/images/social/docker.png)](https://hub.docker.com/u/jefftriplett/)
-
-
```

