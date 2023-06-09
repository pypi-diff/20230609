# Comparing `tmp/mr4mp-2.6.3.tar.gz` & `tmp/mr4mp-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mr4mp-2.6.3.tar", last modified: Wed Apr  5 03:55:26 2023, max compression
+gzip compressed data, was "mr4mp-2.7.0.tar", last modified: Fri Jun  9 03:57:24 2023, max compression
```

## Comparing `mr4mp-2.6.3.tar` & `mr4mp-2.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 03:55:26.323598 mr4mp-2.6.3/
--rw-rw-rw-   0        0        0     1091 2022-04-16 19:30:13.000000 mr4mp-2.6.3/LICENSE
--rw-rw-rw-   0        0        0     6963 2023-04-05 03:55:26.323598 mr4mp-2.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     6443 2023-04-05 03:50:04.000000 mr4mp-2.6.3/README.rst
--rw-rw-rw-   0        0        0     1027 2023-04-05 03:51:48.000000 mr4mp-2.6.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-05 03:55:26.323598 mr4mp-2.6.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-05 03:55:26.306601 mr4mp-2.6.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-05 03:55:26.311456 mr4mp-2.6.3/src/mr4mp/
--rw-rw-rw-   0        0        0      109 2022-04-16 19:30:13.000000 mr4mp-2.6.3/src/mr4mp/__init__.py
--rw-rw-rw-   0        0        0    13241 2022-08-01 07:37:44.000000 mr4mp-2.6.3/src/mr4mp/mr4mp.py
-drwxrwxrwx   0        0        0        0 2023-04-05 03:55:26.318916 mr4mp-2.6.3/src/mr4mp.egg-info/
--rw-rw-rw-   0        0        0     6963 2023-04-05 03:55:26.000000 mr4mp-2.6.3/src/mr4mp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-04-05 03:55:26.000000 mr4mp-2.6.3/src/mr4mp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 03:55:26.000000 mr4mp-2.6.3/src/mr4mp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      225 2023-04-05 03:55:26.000000 mr4mp-2.6.3/src/mr4mp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-05 03:55:26.000000 mr4mp-2.6.3/src/mr4mp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 03:55:26.323598 mr4mp-2.6.3/test/
--rw-rw-rw-   0        0        0    10068 2022-08-01 07:28:46.000000 mr4mp-2.6.3/test/test_mr4mp.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:57:24.629584 mr4mp-2.7.0/
+-rw-rw-rw-   0        0        0     1091 2022-04-16 19:30:13.000000 mr4mp-2.7.0/LICENSE
+-rw-rw-rw-   0        0        0     8943 2023-06-09 03:57:24.629584 mr4mp-2.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8423 2023-06-09 03:46:31.000000 mr4mp-2.7.0/README.rst
+-rw-rw-rw-   0        0        0     1028 2023-06-04 20:54:16.000000 mr4mp-2.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 03:57:24.629584 mr4mp-2.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 03:57:24.615220 mr4mp-2.7.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 03:57:24.619368 mr4mp-2.7.0/src/mr4mp/
+-rw-rw-rw-   0        0        0      109 2022-04-16 19:30:13.000000 mr4mp-2.7.0/src/mr4mp/__init__.py
+-rw-rw-rw-   0        0        0    13241 2022-08-01 07:37:44.000000 mr4mp-2.7.0/src/mr4mp/mr4mp.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:57:24.627874 mr4mp-2.7.0/src/mr4mp.egg-info/
+-rw-rw-rw-   0        0        0     8943 2023-06-09 03:57:24.000000 mr4mp-2.7.0/src/mr4mp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-09 03:57:24.000000 mr4mp-2.7.0/src/mr4mp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 03:57:24.000000 mr4mp-2.7.0/src/mr4mp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      226 2023-06-09 03:57:24.000000 mr4mp-2.7.0/src/mr4mp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 03:57:24.000000 mr4mp-2.7.0/src/mr4mp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 03:57:24.627874 mr4mp-2.7.0/test/
+-rw-rw-rw-   0        0        0    10614 2023-06-09 03:56:20.000000 mr4mp-2.7.0/test/test_mr4mp.py
```

### Comparing `mr4mp-2.6.3/LICENSE` & `mr4mp-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mr4mp-2.6.3/PKG-INFO` & `mr4mp-2.7.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: mr4mp
-Version: 2.6.3
-Summary: Thin MapReduce-like layer that wraps the Python multiprocessing library.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/lapets/mr4mp
-Project-URL: Documentation, https://mr4mp.readthedocs.io
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
 =====
 mr4mp
 =====
 
 Thin MapReduce-like layer that wraps the Python multiprocessing library.
 
 |pypi| |readthedocs| |actions| |coveralls|
@@ -38,15 +20,15 @@
 
 .. |coveralls| image:: https://coveralls.io/repos/github/lapets/mr4mp/badge.svg?branch=main
    :target: https://coveralls.io/github/lapets/mr4mp?branch=main
    :alt: Coveralls test coverage summary.
 
 Purpose
 -------
-This package provides a streamlined interface for the built-in Python `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`__ library. The interface makes it possible to parallelize in a succinct way (sometimes using only one line of code) a data workflow that can be expressed in a `MapReduce <https://en.wikipedia.org/wiki/MapReduce>`__-like form. More background information about this package's design and implementation, as well a detailed use case, can be found in a `related article <https://github.com/python-supply/map-reduce-and-multiprocessing>`__.
+This package provides a streamlined interface for the built-in Python `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`__ library. The interface makes it possible to parallelize in a succinct way (sometimes using only one line of code) a data workflow that can be expressed in a  `MapReduce <https://en.wikipedia.org/wiki/MapReduce>`__-like form. More background information about this package's design and implementation, as well a detailed use case, can be found in a `related article <https://github.com/python-supply/map-reduce-and-multiprocessing>`__.
 
 Installation and Usage
 ----------------------
 This library is available as a `package on PyPI <https://pypi.org/project/mr4mp>`__:
 
 .. code-block:: bash
 
@@ -54,61 +36,81 @@
 
 The library can be imported in the usual way:
 
 .. code-block:: python
 
     import mr4mp
 
-Word-Document Index Example
-^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Examples
+^^^^^^^^
+
+In addition to the `use case in a related article <https://github.com/python-supply/map-reduce-and-multiprocessing>`__ and the example below, smaller examples for each of the methods can be found in the `documentation <https://mr4mp.readthedocs.io>`__.
 
-Suppose we have some functions that we can use to build an index of randomly generated words:
+Word-Document Index
+~~~~~~~~~~~~~~~~~~~
+
+Assume there exists a collection of documents and that each document contains a collection of 7-letter "words". This example demonstrates how a dictionary that associates each word to the collection of documents in which that word appears can be built by leveraging `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`__ and the `MapReduce <https://en.wikipedia.org/wiki/MapReduce>`__ paradigm. Suppose the function definitions below are found within a module ``example.py``:
 
 .. code-block:: python
 
     from random import choice
     from string import ascii_lowercase
+    from uuid import uuid4
 
     def word(): # Generate a random 7-letter "word".
         return ''.join(choice(ascii_lowercase) for _ in range(7))
-    
-    def index(identifier): # Build an index mapping some random words to an identifier.
-        return {w:{identifier} for w in {word() for _ in range(100)}}
-    
-    def merge(i, j): # Merge two index dictionaries i and j.
-        return {k:(i.get(k,set()) | j.get(k,set())) for k in i.keys() | j.keys()}
 
-We can then construct an index in the following way:
+    def doc(): # Generate a random 100-word "document" and its identifier.
+        return ([word() for _ in range(100)], uuid4())
 
-.. code-block:: python
+    def word_to_doc_id_dict(doc): # Build dictionary mapping a document's words to its identifier.
+        (ws, identifier) = doc
+        return {w: {identifier} for w in ws}
 
-    from timeit import default_timer
+    def merge_dicts(u, v): # Merge two dictionaries ``u`` and ``v``.
+        return {w: (u.get(w, set()) | v.get(w, set())) for w in u.keys() | v.keys()}
+
+.. |pool| replace:: ``pool``
+.. _pool: https://mr4mp.readthedocs.io/en/2.7.0/_source/mr4mp.html#mr4mp.mr4mp.pool
+
+The code below (also included in ``example.py``) constructs a dictionary that maps each individual word to the set of document identifiers in which that word appears. The code does so by incrementally building up larger and larger dictionaries (starting from one dictionary per document via the ``word_to_doc_id_dict`` function and merging them via the ``merge_dicts`` function), all while using the maximum number of processes supported by the system: 
+
+.. code-block:: python
 
-    start = default_timer()
-    pool = mr4mp.pool()
-    pool.mapreduce(index, merge, range(100))
-    pool.close()
-    print("Finished in " + str(default_timer()-start) + "s using " + str(len(pool)) + " process(es).")
+    if __name__ == '__main__':
+        import mr4mp
+        from timeit import default_timer
+
+        start = default_timer()
+        p = mr4mp.pool()
+        p.mapreduce(word_to_doc_id_dict, merge_dicts, [doc() for _ in range(100)])
+        p.close()
+        print(
+            "Finished in " + str(default_timer()-start) + "s " +
+            "using " + str(len(p)) + " process(es)."
+        )
 
-The above might yield the following output:
+Note that any code invoking library methods must be protected inside an ``if __name__ == '__main__':`` block to ensure that the `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`__ library methods can `safely load the module <https://docs.python.org/3/library/multiprocessing.html#the-process-class>`__ without causing side effects. Executing the module might yield the output below:
 
 .. code-block:: bash
 
+    python example.py
     Finished in 0.664681524217187s using 2 process(es).
 
-Suppose that we instead explicitly specify that only one process can be used:
+Suppose that it is explicitly indicated (by adding ``processes=1`` to the invocation of |pool|_) that only one process can be used:
 
 .. code-block:: python
 
-    pool = mr4mp.pool(1)
+    p = mr4mp.pool(processes=1)
 
-After the above modification, we might see the following output from the code block:
+After the above modification, executing the module might yield the output below:
 
 .. code-block:: bash
 
+    python example.py
     Finished in 2.23329004518571s using 1 process(es).
 
 Development
 -----------
 All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
 
 .. code-block:: bash
```

### Comparing `mr4mp-2.6.3/README.rst` & `mr4mp-2.7.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: mr4mp
+Version: 2.7.0
+Summary: Thin MapReduce-like layer that wraps the Python multiprocessing library.
+Author: Andrei Lapets
+Author-email: a@lapets.io
+License: MIT
+Project-URL: Repository, https://github.com/lapets/mr4mp
+Project-URL: Documentation, https://mr4mp.readthedocs.io
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: coveralls
+Provides-Extra: publish
+License-File: LICENSE
+
 =====
 mr4mp
 =====
 
 Thin MapReduce-like layer that wraps the Python multiprocessing library.
 
 |pypi| |readthedocs| |actions| |coveralls|
@@ -20,15 +38,15 @@
 
 .. |coveralls| image:: https://coveralls.io/repos/github/lapets/mr4mp/badge.svg?branch=main
    :target: https://coveralls.io/github/lapets/mr4mp?branch=main
    :alt: Coveralls test coverage summary.
 
 Purpose
 -------
-This package provides a streamlined interface for the built-in Python `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`__ library. The interface makes it possible to parallelize in a succinct way (sometimes using only one line of code) a data workflow that can be expressed in a `MapReduce <https://en.wikipedia.org/wiki/MapReduce>`__-like form. More background information about this package's design and implementation, as well a detailed use case, can be found in a `related article <https://github.com/python-supply/map-reduce-and-multiprocessing>`__.
+This package provides a streamlined interface for the built-in Python `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`__ library. The interface makes it possible to parallelize in a succinct way (sometimes using only one line of code) a data workflow that can be expressed in a  `MapReduce <https://en.wikipedia.org/wiki/MapReduce>`__-like form. More background information about this package's design and implementation, as well a detailed use case, can be found in a `related article <https://github.com/python-supply/map-reduce-and-multiprocessing>`__.
 
 Installation and Usage
 ----------------------
 This library is available as a `package on PyPI <https://pypi.org/project/mr4mp>`__:
 
 .. code-block:: bash
 
@@ -36,61 +54,81 @@
 
 The library can be imported in the usual way:
 
 .. code-block:: python
 
     import mr4mp
 
-Word-Document Index Example
-^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Examples
+^^^^^^^^
+
+In addition to the `use case in a related article <https://github.com/python-supply/map-reduce-and-multiprocessing>`__ and the example below, smaller examples for each of the methods can be found in the `documentation <https://mr4mp.readthedocs.io>`__.
 
-Suppose we have some functions that we can use to build an index of randomly generated words:
+Word-Document Index
+~~~~~~~~~~~~~~~~~~~
+
+Assume there exists a collection of documents and that each document contains a collection of 7-letter "words". This example demonstrates how a dictionary that associates each word to the collection of documents in which that word appears can be built by leveraging `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`__ and the `MapReduce <https://en.wikipedia.org/wiki/MapReduce>`__ paradigm. Suppose the function definitions below are found within a module ``example.py``:
 
 .. code-block:: python
 
     from random import choice
     from string import ascii_lowercase
+    from uuid import uuid4
 
     def word(): # Generate a random 7-letter "word".
         return ''.join(choice(ascii_lowercase) for _ in range(7))
-    
-    def index(identifier): # Build an index mapping some random words to an identifier.
-        return {w:{identifier} for w in {word() for _ in range(100)}}
-    
-    def merge(i, j): # Merge two index dictionaries i and j.
-        return {k:(i.get(k,set()) | j.get(k,set())) for k in i.keys() | j.keys()}
 
-We can then construct an index in the following way:
+    def doc(): # Generate a random 100-word "document" and its identifier.
+        return ([word() for _ in range(100)], uuid4())
 
-.. code-block:: python
+    def word_to_doc_id_dict(doc): # Build dictionary mapping a document's words to its identifier.
+        (ws, identifier) = doc
+        return {w: {identifier} for w in ws}
 
-    from timeit import default_timer
+    def merge_dicts(u, v): # Merge two dictionaries ``u`` and ``v``.
+        return {w: (u.get(w, set()) | v.get(w, set())) for w in u.keys() | v.keys()}
+
+.. |pool| replace:: ``pool``
+.. _pool: https://mr4mp.readthedocs.io/en/2.7.0/_source/mr4mp.html#mr4mp.mr4mp.pool
+
+The code below (also included in ``example.py``) constructs a dictionary that maps each individual word to the set of document identifiers in which that word appears. The code does so by incrementally building up larger and larger dictionaries (starting from one dictionary per document via the ``word_to_doc_id_dict`` function and merging them via the ``merge_dicts`` function), all while using the maximum number of processes supported by the system: 
+
+.. code-block:: python
 
-    start = default_timer()
-    pool = mr4mp.pool()
-    pool.mapreduce(index, merge, range(100))
-    pool.close()
-    print("Finished in " + str(default_timer()-start) + "s using " + str(len(pool)) + " process(es).")
+    if __name__ == '__main__':
+        import mr4mp
+        from timeit import default_timer
+
+        start = default_timer()
+        p = mr4mp.pool()
+        p.mapreduce(word_to_doc_id_dict, merge_dicts, [doc() for _ in range(100)])
+        p.close()
+        print(
+            "Finished in " + str(default_timer()-start) + "s " +
+            "using " + str(len(p)) + " process(es)."
+        )
 
-The above might yield the following output:
+Note that any code invoking library methods must be protected inside an ``if __name__ == '__main__':`` block to ensure that the `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`__ library methods can `safely load the module <https://docs.python.org/3/library/multiprocessing.html#the-process-class>`__ without causing side effects. Executing the module might yield the output below:
 
 .. code-block:: bash
 
+    python example.py
     Finished in 0.664681524217187s using 2 process(es).
 
-Suppose that we instead explicitly specify that only one process can be used:
+Suppose that it is explicitly indicated (by adding ``processes=1`` to the invocation of |pool|_) that only one process can be used:
 
 .. code-block:: python
 
-    pool = mr4mp.pool(1)
+    p = mr4mp.pool(processes=1)
 
-After the above modification, we might see the following output from the code block:
+After the above modification, executing the module might yield the output below:
 
 .. code-block:: bash
 
+    python example.py
     Finished in 2.23329004518571s using 1 process(es).
 
 Development
 -----------
 All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
 
 .. code-block:: bash
```

### Comparing `mr4mp-2.6.3/pyproject.toml` & `mr4mp-2.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 [project]
 name = "mr4mp"
-version = "2.6.3"
+version = "2.7.0"
 description = """\
     Thin MapReduce-like layer that wraps the \
     Python multiprocessing library.\
     """
 license = {text = "MIT"}
 authors = [
     {name = "Andrei Lapets"},
     {email = "a@lapets.io"}
 ]
 readme = "README.rst"
 requires-python = ">=3.7"
 dependencies = [
-    "parts~=1.5"
+    "parts~=1.6"
 ]
 
 [project.urls]
 Repository = "https://github.com/lapets/mr4mp"
 Documentation = "https://mr4mp.readthedocs.io"
 
 [project.optional-dependencies]
 docs = [
     "toml~=0.10.2",
     "sphinx~=4.2.0",
     "sphinx-rtd-theme~=1.0.0",
     "sphinx-autodoc-typehints~=1.12.0"
 ]
 test = [
-    "pytest~=7.0",
-    "pytest-cov~=3.0"
+    "pytest~=7.2",
+    "pytest-cov~=4.0"
 ]
 lint = [
-    "pylint~=2.14.0"
+    "pylint~=2.17.0"
 ]
 coveralls = [
     "coveralls~=3.3.1"
 ]
 publish = [
-    "build~=0.8",
+    "build~=0.10",
     "twine~=4.0"
 ]
 
 [build-system]
 requires = [
-    "setuptools~=62.0"
+    "setuptools~=67.6"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --ignore=docs --cov=mr4mp --cov-report term-missing"
```

### Comparing `mr4mp-2.6.3/src/mr4mp/mr4mp.py` & `mr4mp-2.7.0/src/mr4mp/mr4mp.py`

 * *Files identical despite different names*

### Comparing `mr4mp-2.6.3/src/mr4mp.egg-info/PKG-INFO` & `mr4mp-2.7.0/src/mr4mp.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mr4mp
-Version: 2.6.3
+Version: 2.7.0
 Summary: Thin MapReduce-like layer that wraps the Python multiprocessing library.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/lapets/mr4mp
 Project-URL: Documentation, https://mr4mp.readthedocs.io
 Requires-Python: >=3.7
@@ -38,15 +38,15 @@
 
 .. |coveralls| image:: https://coveralls.io/repos/github/lapets/mr4mp/badge.svg?branch=main
    :target: https://coveralls.io/github/lapets/mr4mp?branch=main
    :alt: Coveralls test coverage summary.
 
 Purpose
 -------
-This package provides a streamlined interface for the built-in Python `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`__ library. The interface makes it possible to parallelize in a succinct way (sometimes using only one line of code) a data workflow that can be expressed in a `MapReduce <https://en.wikipedia.org/wiki/MapReduce>`__-like form. More background information about this package's design and implementation, as well a detailed use case, can be found in a `related article <https://github.com/python-supply/map-reduce-and-multiprocessing>`__.
+This package provides a streamlined interface for the built-in Python `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`__ library. The interface makes it possible to parallelize in a succinct way (sometimes using only one line of code) a data workflow that can be expressed in a  `MapReduce <https://en.wikipedia.org/wiki/MapReduce>`__-like form. More background information about this package's design and implementation, as well a detailed use case, can be found in a `related article <https://github.com/python-supply/map-reduce-and-multiprocessing>`__.
 
 Installation and Usage
 ----------------------
 This library is available as a `package on PyPI <https://pypi.org/project/mr4mp>`__:
 
 .. code-block:: bash
 
@@ -54,61 +54,81 @@
 
 The library can be imported in the usual way:
 
 .. code-block:: python
 
     import mr4mp
 
-Word-Document Index Example
-^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Examples
+^^^^^^^^
 
-Suppose we have some functions that we can use to build an index of randomly generated words:
+In addition to the `use case in a related article <https://github.com/python-supply/map-reduce-and-multiprocessing>`__ and the example below, smaller examples for each of the methods can be found in the `documentation <https://mr4mp.readthedocs.io>`__.
+
+Word-Document Index
+~~~~~~~~~~~~~~~~~~~
+
+Assume there exists a collection of documents and that each document contains a collection of 7-letter "words". This example demonstrates how a dictionary that associates each word to the collection of documents in which that word appears can be built by leveraging `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`__ and the `MapReduce <https://en.wikipedia.org/wiki/MapReduce>`__ paradigm. Suppose the function definitions below are found within a module ``example.py``:
 
 .. code-block:: python
 
     from random import choice
     from string import ascii_lowercase
+    from uuid import uuid4
 
     def word(): # Generate a random 7-letter "word".
         return ''.join(choice(ascii_lowercase) for _ in range(7))
-    
-    def index(identifier): # Build an index mapping some random words to an identifier.
-        return {w:{identifier} for w in {word() for _ in range(100)}}
-    
-    def merge(i, j): # Merge two index dictionaries i and j.
-        return {k:(i.get(k,set()) | j.get(k,set())) for k in i.keys() | j.keys()}
 
-We can then construct an index in the following way:
+    def doc(): # Generate a random 100-word "document" and its identifier.
+        return ([word() for _ in range(100)], uuid4())
 
-.. code-block:: python
+    def word_to_doc_id_dict(doc): # Build dictionary mapping a document's words to its identifier.
+        (ws, identifier) = doc
+        return {w: {identifier} for w in ws}
+
+    def merge_dicts(u, v): # Merge two dictionaries ``u`` and ``v``.
+        return {w: (u.get(w, set()) | v.get(w, set())) for w in u.keys() | v.keys()}
 
-    from timeit import default_timer
+.. |pool| replace:: ``pool``
+.. _pool: https://mr4mp.readthedocs.io/en/2.7.0/_source/mr4mp.html#mr4mp.mr4mp.pool
+
+The code below (also included in ``example.py``) constructs a dictionary that maps each individual word to the set of document identifiers in which that word appears. The code does so by incrementally building up larger and larger dictionaries (starting from one dictionary per document via the ``word_to_doc_id_dict`` function and merging them via the ``merge_dicts`` function), all while using the maximum number of processes supported by the system: 
+
+.. code-block:: python
 
-    start = default_timer()
-    pool = mr4mp.pool()
-    pool.mapreduce(index, merge, range(100))
-    pool.close()
-    print("Finished in " + str(default_timer()-start) + "s using " + str(len(pool)) + " process(es).")
+    if __name__ == '__main__':
+        import mr4mp
+        from timeit import default_timer
+
+        start = default_timer()
+        p = mr4mp.pool()
+        p.mapreduce(word_to_doc_id_dict, merge_dicts, [doc() for _ in range(100)])
+        p.close()
+        print(
+            "Finished in " + str(default_timer()-start) + "s " +
+            "using " + str(len(p)) + " process(es)."
+        )
 
-The above might yield the following output:
+Note that any code invoking library methods must be protected inside an ``if __name__ == '__main__':`` block to ensure that the `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`__ library methods can `safely load the module <https://docs.python.org/3/library/multiprocessing.html#the-process-class>`__ without causing side effects. Executing the module might yield the output below:
 
 .. code-block:: bash
 
+    python example.py
     Finished in 0.664681524217187s using 2 process(es).
 
-Suppose that we instead explicitly specify that only one process can be used:
+Suppose that it is explicitly indicated (by adding ``processes=1`` to the invocation of |pool|_) that only one process can be used:
 
 .. code-block:: python
 
-    pool = mr4mp.pool(1)
+    p = mr4mp.pool(processes=1)
 
-After the above modification, we might see the following output from the code block:
+After the above modification, executing the module might yield the output below:
 
 .. code-block:: bash
 
+    python example.py
     Finished in 2.23329004518571s using 1 process(es).
 
 Development
 -----------
 All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
 
 .. code-block:: bash
```

### Comparing `mr4mp-2.6.3/test/test_mr4mp.py` & `mr4mp-2.7.0/test/test_mr4mp.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,25 +26,28 @@
     # pylint: disable=missing-function-docstring
     def test_module(self):
         module = import_module('mr4mp.mr4mp')
         self.assertTrue(api_methods().issubset(module.__dict__.keys()))
 
 def word(identifier, k):
     """Create a random three-character word."""
-    return ''.join(ascii_lowercase[i % 7] for i in sha256(bytes(identifier * k)).digest()[:3])
+    return ''.join(
+        ascii_lowercase[i % 7]
+        for i in sha256(bytes(identifier * k)).digest()[:3]
+    )
 
-def index(identifier):
-    """Given an index value, make 25 words that map to it."""
+def word_to_doc_id_dict(identifier):
+    """Given a document identifier, map 25 random words to that identifier."""
     return {w:{identifier} for w in {word(identifier, k) for k in range(25)}}
 
-def merge(i, j):
-    """Merge two word counts."""
-    return {k:(i.get(k,set()) | j.get(k,set())) for k in i.keys() | j.keys()}
+def merge_dicts(u, v):
+    """Merge two dictionaries."""
+    return {w: (u.get(w, set()) | v.get(w, set())) for w in u.keys() | v.keys()}
 
-result_reference = reduce(merge, map(index, range(50)))
+result_reference = reduce(merge_dicts, map(word_to_doc_id_dict, range(50)))
 
 def add_one(x):
     """
     Simple function defined within module (and not within a method body)
     so that tests that use multiple processes can invoke it.
     """
     return [x + 1]
@@ -76,62 +79,62 @@
         """
         # pylint: disable=missing-function-docstring
         def test_pool_mapreduce_pool_close(self):
             pool = mr4mp.pool(processes, close=True)
             self.assertFalse(pool.closed())
             print("Starting.")
             start = default_timer()
-            result = pool.mapreduce(index, merge, range(50), close=False)
+            result = pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50), close=False)
             self.assertFalse(pool.closed())
-            result = pool.mapreduce(index, merge, range(50))
+            result = pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50))
             self.assertTrue(pool.closed())
             print("Finished in " + str(default_timer()-start) +
                   "s using " + str(len(pool)) + " processes.")
             self.assertEqual(result, result_reference)
 
         def test_pool_mapreduce_function_close(self):
             pool = mr4mp.pool(processes, close=False)
             self.assertFalse(pool.closed())
             print("Starting.")
             start = default_timer()
-            result = pool.mapreduce(index, merge, range(50), close=False)
+            result = pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50), close=False)
             self.assertFalse(pool.closed())
-            result = pool.mapreduce(index, merge, range(50), close=True)
+            result = pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50), close=True)
             self.assertTrue(pool.closed())
             print("Finished in " + str(default_timer()-start) +
                   "s using " + str(len(pool)) + " processes.")
             self.assertEqual(result, result_reference)
 
         def test_pool_mapreduce_pool_open_reuse(self):
             pool = mr4mp.pool(processes, close=False)
-            result = pool.mapreduce(index, merge, range(50))
-            result = pool.mapreduce(index, merge, range(50))
-            result = pool.mapreduce(index, merge, range(50))
+            result = pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50))
+            result = pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50))
+            result = pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50))
             self.assertFalse(pool.closed())
             pool.close()
             self.assertTrue(pool.closed())
             self.assertEqual(result, result_reference)
 
         def test_pool_mapreduce_pool_close_reuse_exception(self):
             pool = mr4mp.pool(processes, close=True)
-            pool.mapreduce(index, merge, range(50))
+            pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50))
             with self.assertRaises(ValueError):
-                pool.mapreduce(index, merge, range(50))
+                pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50))
 
         def test_pool_mapreduce_function_close_reuse_exception(self):
             pool = mr4mp.pool(processes, close=False)
-            pool.mapreduce(index, merge, range(50), close=True)
+            pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50), close=True)
             with self.assertRaises(ValueError):
-                pool.mapreduce(index, merge, range(50))
+                pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50))
 
         def test_pool_mapreduce_many_with_as(self):
             with mr4mp.pool(processes) as pool:
-                result = pool.mapreduce(index, merge, range(50))
-                result = pool.mapreduce(index, merge, range(50))
-                result = pool.mapreduce(index, merge, range(50))
+                result = pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50))
+                result = pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50))
+                result = pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50))
                 self.assertFalse(pool.closed())
             self.assertEqual(result, result_reference)
 
     return Test_pool_close
 
 def define_class_pool_stages_progress(processes, stages, progress):
     """
@@ -143,15 +146,21 @@
         Tests of feature that allows a workflow to be broken down into stages,
         with progress being reported at the end of each stage.
         """
         # pylint: disable=missing-function-docstring
         def test_pool_mapreduce(self):
             logger = log() if progress else None
             pool = mr4mp.pool(processes, close=True)
-            result = pool.mapreduce(index, merge, range(50), stages=stages, progress=logger)
+            result = pool.mapreduce(
+                word_to_doc_id_dict,
+                merge_dicts,
+                range(50),
+                stages=stages,
+                progress=logger
+            )
             self.assertEqual(result, result_reference)
             if progress:
                 self.assertEqual(
                     logger.to_list(),
                     list(range(50)) if stages is not None else []
                 )
 
@@ -177,15 +186,15 @@
         """
         Tests of one-shot functions for executing workflows.
         """
         # pylint: disable=missing-function-docstring
         def test_mapreduce(self):
             logger = log() if progress else None
             result = mr4mp.mapreduce(
-                index, merge, range(50),
+                word_to_doc_id_dict, merge_dicts, range(50),
                 processes=processes, stages=stages, progress=logger
             )
             self.assertEqual(result, result_reference)
             if progress:
                 self.assertEqual(
                     logger.to_list(),
                     list(range(50)) if stages is not None else []
@@ -222,24 +231,24 @@
         self.assertEqual(len(pool), mp.cpu_count() - 1)
         pool.close()
 
     def test_pool_mapreduce(self):
         pool = mr4mp.pool(close=True)
         print("Starting.")
         start = default_timer()
-        result = pool.mapreduce(index, merge, range(50))
+        result = pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50))
         print("Finished in " + str(default_timer()-start) +
               "s using " + str(len(pool)) + " processes.")
         self.assertEqual(result, result_reference)
 
     def test_pool_mapreduce_terminate(self):
         pool = mr4mp.pool()
         print("Starting.")
         start = default_timer()
-        result = pool.mapreduce(index, merge, range(50))
+        result = pool.mapreduce(word_to_doc_id_dict, merge_dicts, range(50))
         print("Finished in " + str(default_timer()-start) +
               "s using " + str(len(pool)) + " processes.")
         self.assertEqual(result, result_reference)
         pool.terminate()
         self.assertTrue(pool.closed())
 
 # The instantiated test classes below are discovered in the local scope
```

