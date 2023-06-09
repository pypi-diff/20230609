# Comparing `tmp/cachew-0.8.1.tar.gz` & `tmp/cachew-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cachew-0.8.1.tar", last modified: Tue Nov 10 05:50:44 2020, max compression
+gzip compressed data, was "dist/cachew-0.9.0.tar", last modified: Sat Mar 20 17:23:18 2021, max compression
```

## Comparing `cachew-0.8.1.tar` & `cachew-0.9.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 05:50:44.000000 cachew-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (116)       35 2020-11-10 05:50:30.000000 cachew-0.8.1/.bandit.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 05:50:44.000000 cachew-0.8.1/.ci/
--rwxr-xr-x   0 runner    (1001) docker     (116)     2080 2020-11-10 05:50:30.000000 cachew-0.8.1/.ci/release
--rwxr-xr-x   0 runner    (1001) docker     (116)       73 2020-11-10 05:50:30.000000 cachew-0.8.1/.ci/run
--rw-r--r--   0 runner    (1001) docker     (116)       46 2020-11-10 05:50:30.000000 cachew-0.8.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 05:50:44.000000 cachew-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 05:50:44.000000 cachew-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2190 2020-11-10 05:50:30.000000 cachew-0.8.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2410 2020-11-10 05:50:30.000000 cachew-0.8.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 05:50:44.000000 cachew-0.8.1/.idea/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 05:50:44.000000 cachew-0.8.1/.idea/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (116)      215 2020-11-10 05:50:30.000000 cachew-0.8.1/.idea/dictionaries/karlicos.xml
--rw-r--r--   0 runner    (1001) docker     (116)      552 2020-11-10 05:50:30.000000 cachew-0.8.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)     1081 2020-11-10 05:50:30.000000 cachew-0.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)      318 2020-11-10 05:50:44.000000 cachew-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    18724 2020-11-10 05:50:30.000000 cachew-0.8.1/README.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)    13567 2020-11-10 05:50:30.000000 cachew-0.8.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (116)      231 2020-11-10 05:50:30.000000 cachew-0.8.1/generate-readme
--rw-r--r--   0 runner    (1001) docker     (116)     3799 2020-11-10 05:50:30.000000 cachew-0.8.1/github-issues.org
--rw-r--r--   0 runner    (1001) docker     (116)      220 2020-11-10 05:50:30.000000 cachew-0.8.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (116)      210 2020-11-10 05:50:30.000000 cachew-0.8.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (116)      302 2020-11-10 05:50:30.000000 cachew-0.8.1/readme.tpl
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-11-10 05:50:44.000000 cachew-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1398 2020-11-10 05:50:30.000000 cachew-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 05:50:44.000000 cachew-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 05:50:44.000000 cachew-0.8.1/src/cachew/
--rw-r--r--   0 runner    (1001) docker     (116)    33634 2020-11-10 05:50:30.000000 cachew-0.8.1/src/cachew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5285 2020-11-10 05:50:30.000000 cachew-0.8.1/src/cachew/compat.py
--rw-r--r--   0 runner    (1001) docker     (116)      262 2020-11-10 05:50:30.000000 cachew-0.8.1/src/cachew/experimental.py
--rw-r--r--   0 runner    (1001) docker     (116)      770 2020-11-10 05:50:30.000000 cachew-0.8.1/src/cachew/extra.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-10 05:50:30.000000 cachew-0.8.1/src/cachew/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 05:50:44.000000 cachew-0.8.1/src/cachew/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-10 05:50:30.000000 cachew-0.8.1/src/cachew/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    28556 2020-11-10 05:50:30.000000 cachew-0.8.1/src/cachew/tests/test_cachew.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-10 05:50:44.000000 cachew-0.8.1/src/cachew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      318 2020-11-10 05:50:43.000000 cachew-0.8.1/src/cachew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      617 2020-11-10 05:50:44.000000 cachew-0.8.1/src/cachew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-10 05:50:43.000000 cachew-0.8.1/src/cachew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-10 05:50:43.000000 cachew-0.8.1/src/cachew.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      117 2020-11-10 05:50:43.000000 cachew-0.8.1/src/cachew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-11-10 05:50:43.000000 cachew-0.8.1/src/cachew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      808 2020-11-10 05:50:30.000000 cachew-0.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 17:23:18.000000 cachew-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2021-03-20 17:23:05.000000 cachew-0.9.0/.bandit.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 17:23:18.000000 cachew-0.9.0/.ci/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2080 2021-03-20 17:23:05.000000 cachew-0.9.0/.ci/release
+-rwxr-xr-x   0 runner    (1001) docker     (121)       73 2021-03-20 17:23:05.000000 cachew-0.9.0/.ci/run
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-03-20 17:23:05.000000 cachew-0.9.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 17:23:18.000000 cachew-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 17:23:18.000000 cachew-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2391 2021-03-20 17:23:05.000000 cachew-0.9.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2410 2021-03-20 17:23:05.000000 cachew-0.9.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 17:23:18.000000 cachew-0.9.0/.idea/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 17:23:18.000000 cachew-0.9.0/.idea/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-20 17:23:05.000000 cachew-0.9.0/.idea/dictionaries/karlicos.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2021-03-20 17:23:05.000000 cachew-0.9.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)     1081 2021-03-20 17:23:05.000000 cachew-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2021-03-20 17:23:18.000000 cachew-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    19081 2021-03-20 17:23:05.000000 cachew-0.9.0/README.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    13862 2021-03-20 17:23:05.000000 cachew-0.9.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (121)      231 2021-03-20 17:23:05.000000 cachew-0.9.0/generate-readme
+-rw-r--r--   0 runner    (1001) docker     (121)     3799 2021-03-20 17:23:05.000000 cachew-0.9.0/github-issues.org
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2021-03-20 17:23:05.000000 cachew-0.9.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2021-03-20 17:23:05.000000 cachew-0.9.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2021-03-20 17:23:05.000000 cachew-0.9.0/readme.tpl
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-20 17:23:18.000000 cachew-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-03-20 17:23:05.000000 cachew-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 17:23:18.000000 cachew-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 17:23:18.000000 cachew-0.9.0/src/cachew/
+-rw-r--r--   0 runner    (1001) docker     (121)    34227 2021-03-20 17:23:05.000000 cachew-0.9.0/src/cachew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5285 2021-03-20 17:23:05.000000 cachew-0.9.0/src/cachew/compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2021-03-20 17:23:05.000000 cachew-0.9.0/src/cachew/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (121)      770 2021-03-20 17:23:05.000000 cachew-0.9.0/src/cachew/extra.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-20 17:23:05.000000 cachew-0.9.0/src/cachew/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 17:23:18.000000 cachew-0.9.0/src/cachew/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-20 17:23:05.000000 cachew-0.9.0/src/cachew/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30816 2021-03-20 17:23:05.000000 cachew-0.9.0/src/cachew/tests/test_cachew.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 17:23:18.000000 cachew-0.9.0/src/cachew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2021-03-20 17:23:18.000000 cachew-0.9.0/src/cachew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2021-03-20 17:23:18.000000 cachew-0.9.0/src/cachew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-20 17:23:18.000000 cachew-0.9.0/src/cachew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-20 17:23:18.000000 cachew-0.9.0/src/cachew.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2021-03-20 17:23:18.000000 cachew-0.9.0/src/cachew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-20 17:23:18.000000 cachew-0.9.0/src/cachew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2021-03-20 17:23:05.000000 cachew-0.9.0/tox.ini
```

### Comparing `cachew-0.8.1/.ci/release` & `cachew-0.9.0/.ci/release`

 * *Files identical despite different names*

### Comparing `cachew-0.8.1/.github/workflows/main.yml` & `cachew-0.9.0/.github/workflows/main.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # see https://github.com/karlicoss/pymplate for up-to-date reference
 
 name: CI
 on:
   push:
     branches: '*'
     tags: 'v[0-9]+.*' # only trigger on 'release' tags for PyPi
-    # Ideally I would put this in the pypi job... but github syntax doesn't allow for regexes there :shrug:
-    # P.S. fuck made up yaml DSLs.
-    # TODO cron?
+  # Note that people who fork it need to go to "Actions" tab on their fork and click "I understand my workflows, go ahead and enable them".
+  pull_request: # needed to trigger on others' PRs
   workflow_dispatch: # needed to trigger workflows manually
+  # todo cron?
 
 env:
   # useful for scripts & sometimes tests to know
   CI: true
 
 jobs:
   build:
     strategy:
       matrix:
-        platform: [ubuntu-latest] # , macos-latest] # TODO windows-latest??
+        platform: [ubuntu-latest, macos-latest] # TODO windows-latest??
         python-version: [3.6, 3.7, 3.8]
 
     runs-on: ${{ matrix.platform }}
 
     steps:
     # ugh https://github.com/actions/toolkit/blob/main/docs/commands.md#path-manipulation
     - run: echo "$HOME/.local/bin" >> $GITHUB_PATH
@@ -30,24 +30,25 @@
     - uses: actions/setup-python@v1
       with:
         python-version: ${{ matrix.python-version }}
 
     - uses: actions/checkout@v2
       with:
         submodules: recursive
+        fetch-depth: 0  # nicer to have all git history when debugging/for tests
 
     # uncomment for SSH debugging
     # - uses: mxschmitt/action-tmate@v3
 
     - run: .ci/run
 
     - uses: actions/upload-artifact@v2
       with:
-        name: .mypy-coverage_${{ matrix.platform }}_${{ matrix.python-version }}
-        path: .mypy-coverage/
+        name: .coverage.mypy_${{ matrix.platform }}_${{ matrix.python-version }}
+        path: .coverage.mypy/
 
 
   pypi:
     runs-on: ubuntu-latest
     needs: build
 
     steps:
@@ -60,19 +61,19 @@
 
     - uses: actions/checkout@v2
       with:
         submodules: recursive
 
     - name: 'release to test pypi'
       # always deploy merged master to test pypi
-      if: github.event.ref == 'refs/heads/master'
+      if: github.event_name != 'pull_request' && github.event.ref == 'refs/heads/master'
       env:
         TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD_TEST }}
       run: pip3 install --user wheel twine && .ci/release --test
 
     - name: 'release to pypi'
       # always deploy tags to release pypi
       # NOTE: release tags are guarded by on: push: tags on the top
-      if: startsWith(github.event.ref, 'refs/tags')
+      if: github.event_name != 'pull_request' && startsWith(github.event.ref, 'refs/tags')
       env:
         TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD }}
       run: pip3 install --user wheel twine && .ci/release
```

### Comparing `cachew-0.8.1/.gitignore` & `cachew-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cachew-0.8.1/.pylintrc` & `cachew-0.9.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `cachew-0.8.1/LICENSE.txt` & `cachew-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cachew-0.8.1/README.ipynb` & `cachew-0.9.0/README.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8730505952380953%*

 * *Differences: {"'cells'": '{1: {\'source\': ["dmd(f\'\'\'\\n", \'<!--\\n\', \'THIS FILE IS AUTOGENERATED BY '*

 * *            'README.ipynb.\\n\', "Ideally you should edit README.ipynb and use \'generate-readme\' '*

 * *            'to produce README.md. \\n", "But it\'s okay to edit README.md too directly if you '*

 * *            'want to fix something -- I can run generate-readme myself later.\\n", \'-->\\n\', '*

 * *            '"\'\'\')"]}, 16: {\'source\': {insert: [(4, \'- `DEFAULT_CACHEW_DIR`: override to set '*

 * *            'a diffe […]*

```diff
@@ -67,15 +67,21 @@
                 "ein.tags": "worksheet-0",
                 "slideshow": {
                     "slide_type": "-"
                 }
             },
             "outputs": [],
             "source": [
-                "dmd(f'<!--THIS FILE IS AUTOGENERATED BY README.ipynb. Use generate-readme to update it.-->')"
+                "dmd(f'''\n",
+                "<!--\n",
+                "THIS FILE IS AUTOGENERATED BY README.ipynb.\n",
+                "Ideally you should edit README.ipynb and use 'generate-readme' to produce README.md. \n",
+                "But it's okay to edit README.md too directly if you want to fix something -- I can run generate-readme myself later.\n",
+                "-->\n",
+                "''')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "ein.tags": "worksheet-0",
                 "slideshow": {
@@ -426,15 +432,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "dmd(f'''\n",
                 "{flink('cachew.settings')} exposes some parameters that allow you to control `cachew` behaviour:\n",
                 "- `ENABLE`: set to `False` if you want to disable caching for without removing the decorators (useful for testing and debugging).\n",
                 "   You can also use {flink('cachew.extra.disabled_cachew')} context manager to do it temporarily.\n",
-                "- `DEFAULT_CACHEW_DIR`: override to set a different base directory.\n",
+                "- `DEFAULT_CACHEW_DIR`: override to set a different base directory. The default is the \"user cache directory\" (see [appdirs docs](https://github.com/ActiveState/appdirs#some-example-output)).\n",
                 "- `THROW_ON_ERROR`: by default, cachew is defensive and simply attemps to cause the original function on caching issues.\n",
                 "   Set to `True` to catch errors earlier.\n",
                 "\n",
                 "''')"
             ]
         },
         {
@@ -459,14 +465,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.2"
+            "version": "3.8.5"
         },
         "name": "README.ipynb"
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `cachew-0.8.1/README.md` & `cachew-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-<!--THIS FILE IS AUTOGENERATED BY README.ipynb. Use generate-readme to update it.-->
+<!--
+THIS FILE IS AUTOGENERATED BY README.ipynb.
+Ideally you should edit README.ipynb and use 'generate-readme' to produce README.md. 
+But it's okay to edit README.md too directly if you want to fix something -- I can run generate-readme myself later.
+-->
 
 
 # What is Cachew?
 TLDR: cachew lets you **cache function calls** into an sqlite database on your disk in a matter of **single decorator** (similar to [functools.lru_cache](https://docs.python.org/3/library/functools.html#functools.lru_cache)). The difference from `functools.lru_cache` is that cached data is persisted between program runs, so next time you call your function, it will only be a matter of reading from the cache.
 Cache is **invalidated automatically** if your function's arguments change, so you don't have to think about maintaining it.
 
 In order to be cacheable, your function needs to return (an [Iterator](https://docs.python.org/3/library/typing.html#typing.Iterator), that is a generator, tuple or list) of simple data types:
@@ -112,70 +116,70 @@
 - as long as `chunks` stay same, data stays same so you always read from sqlite cache which is very fast
 - you don't need to maintain the database, cache is automatically refreshed when `chunks` change (i.e. you got new data)
 
   All the complexity of handling database is hidden in `cachew` implementation.
 
 
 # How it works
-Basically, your data objects get [flattened out](src/cachew/__init__.py#L447)
-and python types are mapped [onto sqlite types and back](src/cachew/__init__.py#L517).
+Basically, your data objects get [flattened out](src/cachew/__init__.py#L452)
+and python types are mapped [onto sqlite types and back](src/cachew/__init__.py#L522).
 
-When the function is called, cachew [computes the hash of your function's arguments ](src/cachew/__init__.py:#L839)
+When the function is called, cachew [computes the hash of your function's arguments ](src/cachew/__init__.py:#L841)
 and compares it against the previously stored hash value.
     
 - If they match, it would deserialize and yield whatever is stored in the cache database
 - If the hash mismatches, the original function is called and new data is stored along with the new hash
 
 
 
 # Features
 
 
 
-* automatic schema inference: [1](src/cachew/tests/test_cachew.py#L281), [2](src/cachew/tests/test_cachew.py#L295)
+* automatic schema inference: [1](src/cachew/tests/test_cachew.py#L341), [2](src/cachew/tests/test_cachew.py#L355)
 * supported types:    
 
     * primitive: `str`, `int`, `float`, `bool`, `datetime`, `date`, `dict`, `list`, `Exception`
     
-      See [tests.test_types](src/cachew/tests/test_cachew.py#L561), [tests.test_primitive](src/cachew/tests/test_cachew.py#L608), [tests.test_dates](src/cachew/tests/test_cachew.py#L521)
-    * [Optional](src/cachew/tests/test_cachew.py#L420) types
-    * [Union](src/cachew/tests/test_cachew.py#L678) types
-    * [nested datatypes](src/cachew/tests/test_cachew.py#L337)
-    * [Exceptions](src/cachew/tests/test_cachew.py#L920)
+      See [tests.test_types](src/cachew/tests/test_cachew.py#L621), [tests.test_primitive](src/cachew/tests/test_cachew.py#L668), [tests.test_dates](src/cachew/tests/test_cachew.py#L581)
+    * [Optional](src/cachew/tests/test_cachew.py#L480) types
+    * [Union](src/cachew/tests/test_cachew.py#L738) types
+    * [nested datatypes](src/cachew/tests/test_cachew.py#L397)
+    * [Exceptions](src/cachew/tests/test_cachew.py#L995)
     
-* detects [datatype schema changes](src/cachew/tests/test_cachew.py#L367) and discards old data automatically
+* detects [datatype schema changes](src/cachew/tests/test_cachew.py#L427) and discards old data automatically
 
 
 # Performance
 Updating cache takes certain overhead, but that would depend on how complicated your datatype in the first place, so I'd suggest measuring if you're not sure.
 
 During reading cache all that happens is reading rows from sqlite and mapping them onto your target datatype, so the only overhead would be from reading sqlite, which is quite fast.
 
 I haven't set up proper benchmarks/performance regressions yet, so don't want to make specific claims, however that would almost certainly make your programm faster if computations take more than several seconds.
 
 
-If you want to experiment for youself, check out [tests.test_many](src/cachew/tests/test_cachew.py#L226)
+If you want to experiment for youself, check out [tests.test_many](src/cachew/tests/test_cachew.py#L286)
 
 
 
 # Using
-See [docstring](src/cachew/__init__.py#L711) for up-to-date documentation on parameters and return types. 
+See [docstring](src/cachew/__init__.py#L713) for up-to-date documentation on parameters and return types. 
 You can also use [extensive unit tests](src/cachew/tests/test_cachew.py) as a reference.
     
 Some useful (but optional) arguments of `@cachew` decorator:
     
-* `cache_path` can be a directory, or a callable that [returns a path](src/cachew/tests/test_cachew.py#L317) and depends on function's arguments.
+* `cache_path` can be a directory, or a callable that [returns a path](src/cachew/tests/test_cachew.py#L377) and depends on function's arguments.
     
    By default, `settings.DEFAULT_CACHEW_DIR` is used.
     
 * `depends_on` is a function which determines whether your inputs have changed, and the cache needs to be invalidated.
     
    By default it just uses string representation of the arguments, you can also specify a custom callable.
     
-   For instance, it can be used to [discard cache](src/cachew/tests/test_cachew.py#L91) if the input file was modified.
+   For instance, it can be used to [discard cache](src/cachew/tests/test_cachew.py#L92) if the input file was modified.
     
 * `cls` is the type that would be serialized.
 
    By default, it is inferred from return type annotations, but can be specified if you don't control the code you want to cache.
 
 
 # Installing
@@ -252,17 +256,17 @@
 
 
 Now you can use `@mcachew` in place of `@cachew`, and be certain things don't break if `cachew` is missing.
 
 ## Settings
 
 
-[cachew.settings](src/cachew/__init__.py#L61) exposes some parameters that allow you to control `cachew` behaviour:
+[cachew.settings](src/cachew/__init__.py#L64) exposes some parameters that allow you to control `cachew` behaviour:
 - `ENABLE`: set to `False` if you want to disable caching for without removing the decorators (useful for testing and debugging).
    You can also use [cachew.extra.disabled_cachew](src/cachew/__init__.py#L18) context manager to do it temporarily.
-- `DEFAULT_CACHEW_DIR`: override to set a different base directory.
+- `DEFAULT_CACHEW_DIR`: override to set a different base directory. The default is the "user cache directory" (see [appdirs docs](https://github.com/ActiveState/appdirs#some-example-output)).
 - `THROW_ON_ERROR`: by default, cachew is defensive and simply attemps to cause the original function on caching issues.
    Set to `True` to catch errors earlier.
 
 
 ## Updating this readme
 This is a literate readme, implemented as a Jupiter notebook: [README.ipynb](README.ipynb). To update the (autogenerated) [README.md](README.md), use [generate-readme](generate-readme) script.
```

### Comparing `cachew-0.8.1/github-issues.org` & `cachew-0.9.0/github-issues.org`

 * *Files identical despite different names*

### Comparing `cachew-0.8.1/setup.py` & `cachew-0.9.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 url = 'https://github.com/karlicoss/cachew'
 author = 'Dima Gerasimov'
 author_email = 'karlicoss@gmail.com'
 description = 'Easy sqlite-backed persistent cache for dataclasses'
 
 install_requires = [
-    'sqlalchemy',
+    'appdirs'   ,  # default cache dir
+    'sqlalchemy',  # cache DB interaction
 ]
 
 
 from setuptools import setup, find_namespace_packages # type: ignore
 
 
 def main():
```

### Comparing `cachew-0.8.1/src/cachew/__init__.py` & `cachew-0.9.0/src/cachew/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import typing
 from pkg_resources import get_distribution, DistributionNotFound
 
 try:
     # Change here if project is renamed and does not equal the package name
     dist_name = __name__
     __version__ = get_distribution(dist_name).version
 except DistributionNotFound:
@@ -19,23 +18,27 @@
 import logging
 from itertools import chain, islice
 import inspect
 from datetime import datetime, date
 import stat
 import tempfile
 from pathlib import Path
+import time
+import sqlite3
 import sys
 import typing
 from typing import (Any, Callable, Iterator, List, NamedTuple, Optional, Tuple,
                     Type, Union, TypeVar, Generic, Sequence, Iterable, Set, cast)
 import dataclasses
 import warnings
 
 
-import sqlalchemy # type: ignore
+import appdirs  # type: ignore[import]
+
+import sqlalchemy  # type: ignore[import]
 from sqlalchemy import Column, Table, event
 
 
 if sys.version_info[1] < 7:
     from .compat import fromisoformat
 else:
     fromisoformat = datetime.fromisoformat
@@ -60,16 +63,15 @@
 '''
 class settings:
     '''
     Toggle to disable caching
     '''
     ENABLE: bool = True
 
-    # switch to appdirs and using user cache dir?
-    DEFAULT_CACHEW_DIR: PathIsh = Path(tempfile.gettempdir()) / 'cachew'
+    DEFAULT_CACHEW_DIR: PathIsh = Path(appdirs.user_cache_dir('cachew'))
 
     '''
     Set to true if you want to fail early. Otherwise falls back to non-cached version
     '''
     THROW_ON_ERROR: bool = False
 
 
@@ -423,15 +425,18 @@
             if primitive:
                 if name is None:
                     name = '_cachew_primitive' # meh. presumably, top level
             if primitive:
                 fields = ()
                 span = 1
             else:
-                fields = tuple(NTBinder.make(tp=ann, name=fname) for fname, ann in tp.__annotations__.items())
+                annotations = getattr(tp, '__annotations__', None)
+                if annotations is None:
+                    raise CachewException(f"{tp}: doesn't look like a supported type to cache. See https://github.com/karlicoss/cachew#features for the list of supported types.")
+                fields = tuple(NTBinder.make(tp=ann, name=fname) for fname, ann in annotations.items())
                 span = sum(f.span for f in fields) + (1 if optional else 0)
         return NTBinder(
             name=name,
             type_=tp,
             span=span,
             primitive=primitive,
             optional=optional,
@@ -553,30 +558,27 @@
 
 class DbHelper:
     def __init__(self, db_path: Path, cls: Type) -> None:
         self.engine = sqlalchemy.create_engine(f'sqlite:///{db_path}', connect_args={'timeout': 0})
         # NOTE: timeout is necessary so we don't lose time waiting during recursive calls
         # by default, it's several seconds? you'd see 'test_recursive' test performance degrade
 
-        import sqlite3
-        import time
-
-        from sqlalchemy.engine import Engine # type: ignore
-        @event.listens_for(Engine, 'connect')
+        @event.listens_for(self.engine, 'connect')
         def set_sqlite_pragma(dbapi_connection, connection_record):
             # without wal, concurrent reading/writing is not gonna work
 
             # ugh. that's odd, how are we supposed to set WAL if the very fact of setting wal might lock the db?
             while True:
                 try:
                     dbapi_connection.execute('PRAGMA journal_mode=WAL')
                     break
                 except sqlite3.OperationalError as oe:
                     if 'database is locked' not in str(oe):
-                        raise oe
+                        # ugh, pretty annoying that exception doesn't include database path for some reason
+                        raise CachewException(f'Error while setting WAL on {db_path}') from oe
                 time.sleep(0.1)
 
 
         self.connection = self.engine.connect()
 
         """
         Erm... this is pretty confusing.
@@ -672,15 +674,15 @@
         return bail(f"wrong number of __args__: {args}")
     arg = args[0]
     if is_primitive(arg):
         return arg
     if is_union(arg):
         return arg # meh?
     if not is_dataclassish(arg):
-        return bail(f"{arg} is not NamedTuple")
+        return bail(f"{arg} is not NamedTuple/dataclass")
     return arg
 
 
 # https://stackoverflow.com/questions/653368/how-to-create-a-python-decorator-that-can-be-used-either-with-or-without-paramet
 def doublewrap(f):
     @functools.wraps(f)
     def new_dec(*args, **kwargs):
@@ -698,15 +700,15 @@
 
 def cachew_error(e: Exception) -> None:
     if settings.THROW_ON_ERROR:
         raise e
     else:
         logger = get_logger()
         # todo add func name?
-        logger.error("Error while setting up cache, falling back to non-cached version")
+        logger.error("cachew: error while setting up cache, falling back to non-cached version")
         logger.exception(e)
 
 
 use_default_path = cast(Path, object())
 
 @doublewrap
 # pylint: disable=too-many-arguments
@@ -772,25 +774,25 @@
     if hashf is not None:
         warnings.warn("'hashf' is deprecated. Please use 'depends_on' instead")
         depends_on = hashf
 
     cn = cname(func)
     # todo not very nice that ENABLE check is scattered across two places
     if not settings.ENABLE or cache_path is None:
-        logger.info('[%s]: cache disabled', cn)
+        logger.info('[%s]: cache explicitly disabled (settings.ENABLE is False or cache_path is None)', cn)
         return func
 
     if cache_path is use_default_path:
         cache_path = settings.DEFAULT_CACHEW_DIR
         logger.info('[%s]: no cache_path specified, using the default %s', cn, cache_path)
 
     # TODO fuzz infer_type, should never crash?
     inferred = infer_type(func)
     if isinstance(inferred, Failure):
-        msg = f"failed to infer cache type: {inferred}"
+        msg = f"failed to infer cache type: {inferred}. See https://github.com/karlicoss/cachew#features for the list of supported types."
         if cls is None:
             ex = CachewException(msg)
             cachew_error(ex)
             return func
         else:
             # it's ok, assuming user knows better
             logger.debug(msg)
@@ -869,29 +871,29 @@
     cls        = C.cls
     depend_on  = C.depends_on
     logger     = C.logger
     chunk_by   = C.chunk_by
 
     cn = cname(func)
     if not settings.ENABLE:
-        logger.info('[%s]: cache disabled', cn)
+        logger.info('[%s]: cache explicitly disabled (settings.ENABLE is False)', cn)
         yield from func(*args, **kwargs)
         return
 
     early_exit = False
 
     # WARNING: annoyingly huge try/catch ahead...
     # but it lets us save a function call, hence a stack frame
     # see test_recursive and test_deep_recursive
     try:
         dbp: Path
         if callable(cache_path):
             pp = cache_path(*args, **kwargs) # type: ignore
             if pp is None:
-                logger.info('[%s]: cache disabled', cn)
+                logger.info('[%s]: cache explicitly disabled (cache_path is None)', cn)
                 yield from func(*args, **kwargs)
                 return
             else:
                 dbp = Path(pp)
         else:
             dbp = Path(cache_path)
```

### Comparing `cachew-0.8.1/src/cachew/compat.py` & `cachew-0.9.0/src/cachew/compat.py`

 * *Files identical despite different names*

### Comparing `cachew-0.8.1/src/cachew/extra.py` & `cachew-0.9.0/src/cachew/extra.py`

 * *Files identical despite different names*

### Comparing `cachew-0.8.1/src/cachew/tests/test_cachew.py` & `cachew-0.9.0/src/cachew/tests/test_cachew.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 from .. import cachew, get_logger, PRIMITIVES, NTBinder, CachewException, Types, Values, settings
 
 
 logger = get_logger()
 
 @pytest.fixture(autouse=True)
 def throw_on_errors():
-    # a more reasonable default for tests
+    # NOTE: in tests we always throw on errors, it's a more reasonable default for testing.
+    # we still check defensive behaviour in test_defensive
     settings.THROW_ON_ERROR = True
     yield
 
 
 @pytest.fixture
 def restore_settings():
     orig = {k: v for k, v in settings.__dict__.items() if not k.startswith('__')}
@@ -36,15 +37,15 @@
     finally:
         for k, v in orig.items():
             setattr(settings, k, v)
 
 
 @pytest.fixture
 def tdir(tmp_path):
-    # TODO just use tmp_path instead?
+    # todo just use tmp_path instead?
     yield Path(tmp_path)
 
 
 @pytest.mark.skipif(sys.version_info < (3, 7), reason="""
 wtf??? 
 >>> from typing import Union
 >>> from datetime import date, datetime
@@ -156,15 +157,51 @@
     assert t > 5.0, 'should take at least 5 seconds'
 
     t, cnt = cast(Tuple[float, int], timer.timeit(number=1))
     assert cnt == 5
     assert t < 2.0, 'should be pretty much instantaneous'
 
 
-def test_cache_path(tdir):
+def test_error(tmp_path: Path) -> None:
+    '''
+    Test behaviour when the first time cache is initialized it ends up with an error
+    '''
+    cache_file = tmp_path / 'cache'
+    assert not cache_file.exists(), cache_file  # just precondition
+
+    should_raise = True
+
+    @cachew(cache_file, force_file=True)
+    def fun() -> Iterator[str]:
+        yield 'string1'
+        if should_raise:
+            raise RuntimeError('oops')
+        yield 'string2'
+
+    with pytest.raises(RuntimeError, match='oops'):
+        list(fun())
+
+    # vvv this would be nice but might be tricky because of the way sqlite works (i.e. wal mode creates a file)
+    # assert not cache_file.exists(), cache_file
+
+    # perhaps doesn't hurt either way as long this vvv works properly
+    # shouldn't cache anything and crach again
+    with pytest.raises(RuntimeError, match='oops'):
+        list(fun())
+
+    should_raise = False
+    assert list(fun()) == ['string1', 'string2']
+
+
+def test_cache_path(tmp_path: Path) -> None:
+    '''
+    Tests various ways of specifying cache path
+    '''
+    tdir = tmp_path
+
     calls = 0
     def orig() -> Iterable[int]:
         nonlocal calls
         yield 1
         yield 2
         calls += 1
 
@@ -212,14 +249,37 @@
     assert calls == 7
     # TODO this won't work at the moment
     # f.write_text('garbage')
     # not sure... on the one hand could just delete the garbage file and overwrite with db
     # on the other hand, wouldn't want to delete some user file by accident
 
 
+class UGood(NamedTuple):
+    x: int
+class UBad:
+    pass
+
+def test_unsupported_class(tmp_path: Path) -> None:
+    with pytest.raises(CachewException, match='.*failed to infer cache type.*'):
+        @cachew(cache_path=tmp_path)
+        def fun() -> List[UBad]:
+            return [UBad()]
+
+    # now something a bit nastier
+    # TODO hmm, should really throw at the definition time... but can fix later I suppose
+    @cachew(cache_path=tmp_path)
+    def fun2() -> Iterable[Union[UGood, UBad]]:
+        yield UGood(x=1)
+        yield UBad()
+        yield UGood(x=2)
+
+    with pytest.raises(CachewException, match=".*doesn't look like a supported type.*"):
+        list(fun2())
+
+
 class TE2(NamedTuple):
     value: int
     uuu: UUU
     value2: int
 
 
 # TODO also profile datetimes?
@@ -500,21 +560,21 @@
     def get_people_data() -> Iterator[Person]:
         yield from make_people_data(count=N)
 
     list(get_people_data())
     print(f"Cache db size for {N} entries: estimated size {one * N // 1024} Kb, actual size {cache_file.stat().st_size // 1024} Kb;")
 
 
-def test_dataclass(tdir):
+def test_dataclass(tmp_path: Path) -> None:
     from dataclasses import dataclass
     @dataclass
     class Test:
         field: int
 
-    @cachew(tdir)
+    @cachew(tmp_path)
     def get_dataclasses() -> Iterator[Test]:
         yield from [Test(field=i) for i in range(5)]
 
     assert list(get_dataclasses()) == [Test(field=i) for i in range(5)]
     assert list(get_dataclasses()) == [Test(field=i) for i in range(5)]
 
 
@@ -671,24 +731,39 @@
     assert list(fun(456)) == [O(3)]
     assert calls == 5
 
 
 class U(NamedTuple):
     x: Union[str, O]
 
-def test_union(tmp_path: Path):
+def test_union(tmp_path: Path) -> None:
     @cachew(tmp_path)
     def fun() -> Iterator[U]:
         yield U('hi')
         yield U(O(123))
 
     list(fun())
     assert list(fun()) == [U('hi'), U(O(123))]
 
 
+def test_union_with_dataclass(tmp_path: Path) -> None:
+    from dataclasses import dataclass
+    # NOTE: empty dataclass doesn't have __annotations__ ??? not sure if need to handle it...
+    @dataclass
+    class DD:
+        x: int
+
+    @cachew(tmp_path)
+    def fun() -> Iterator[Union[int, DD]]:
+        yield 123
+        yield DD(456)
+
+    assert list(fun()) == [123, DD(456)]
+
+
 def _concurrent_helper(cache_path: Path, count: int, sleep_s=0.1):
     from time import sleep
     @cachew(cache_path)
     def test(count: int) -> Iterator[int]:
         for i in range(count):
             print(f"{count}: GENERATING {i}")
             sleep(sleep_s)
```

### Comparing `cachew-0.8.1/src/cachew.egg-info/SOURCES.txt` & `cachew-0.9.0/src/cachew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cachew-0.8.1/tox.ini` & `cachew-0.9.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 [tox]
 minversion = 3.5
 # relies on the correct version of Python installed
-envlist = py3,pylint,mypy
+envlist = tests,pylint,mypy
 
 [testenv]
 passenv = CI CI_* CIRCLE*
+
+[testenv:tests]
 commands =
     pip install -e .[testing]
     python -m pytest -rap src {posargs}
 
 
 [testenv:mypy]
 commands =
     pip install -e .[testing]
     python -m mypy src                               \
                    # txt report is a bit more convenient to view on CI
-                   --txt-report  .mypy-coverage      \
-                   --html-report .mypy-coverage      \
+                   --txt-report  .coverage.mypy      \
+                   --html-report .coverage.mypy      \
                    {posargs}
 
 
+# todo get rid of pylint?
 [testenv:pylint]
 commands =
     pip install -e .[testing]
     python -m pylint -E src/cachew {posargs}
 
 
 # todo not sure if really need bandit at all?
```

