# Comparing `tmp/cdict-0.0.5.tar.gz` & `tmp/cdict-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdict-0.0.5.tar", last modified: Sun Feb 12 05:47:14 2023, max compression
+gzip compressed data, was "cdict-1.0.0.tar", last modified: Thu Jun  8 23:50:25 2023, max compression
```

## Comparing `cdict-0.0.5.tar` & `cdict-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jeffwu     (501) staff       (20)        0 2023-02-12 05:47:14.064507 cdict-0.0.5/
--rw-r--r--   0 jeffwu     (501) staff       (20)       42 2022-05-24 14:35:55.000000 cdict-0.0.5/.gitignore
--rw-r--r--   0 jeffwu     (501) staff       (20)     1080 2022-05-24 14:35:55.000000 cdict-0.0.5/LICENSE
--rw-r--r--   0 jeffwu     (501) staff       (20)      244 2023-02-12 05:47:14.064010 cdict-0.0.5/PKG-INFO
--rw-r--r--   0 jeffwu     (501) staff       (20)     2207 2023-02-12 05:36:20.000000 cdict-0.0.5/README.md
-drwxr-xr-x   0 jeffwu     (501) staff       (20)        0 2023-02-12 05:47:14.052662 cdict-0.0.5/cdict/
--rw-r--r--   0 jeffwu     (501) staff       (20)       29 2023-02-07 17:31:36.000000 cdict-0.0.5/cdict/__init__.py
--rw-r--r--   0 jeffwu     (501) staff       (20)     3707 2023-02-12 05:46:17.000000 cdict-0.0.5/cdict/main.py
-drwxr-xr-x   0 jeffwu     (501) staff       (20)        0 2023-02-12 05:47:14.062589 cdict-0.0.5/cdict.egg-info/
--rw-r--r--   0 jeffwu     (501) staff       (20)      244 2023-02-12 05:47:12.000000 cdict-0.0.5/cdict.egg-info/PKG-INFO
--rw-r--r--   0 jeffwu     (501) staff       (20)      204 2023-02-12 05:47:13.000000 cdict-0.0.5/cdict.egg-info/SOURCES.txt
--rw-r--r--   0 jeffwu     (501) staff       (20)        1 2023-02-12 05:47:12.000000 cdict-0.0.5/cdict.egg-info/dependency_links.txt
--rw-r--r--   0 jeffwu     (501) staff       (20)        6 2023-02-12 05:47:12.000000 cdict-0.0.5/cdict.egg-info/top_level.txt
--rw-r--r--   0 jeffwu     (501) staff       (20)       38 2023-02-12 05:47:14.064612 cdict-0.0.5/setup.cfg
--rw-r--r--   0 jeffwu     (501) staff       (20)      282 2023-02-12 05:46:59.000000 cdict-0.0.5/setup.py
-drwxr-xr-x   0 jeffwu     (501) staff       (20)        0 2023-02-12 05:47:14.063401 cdict-0.0.5/tests/
--rw-r--r--   0 jeffwu     (501) staff       (20)     4010 2023-02-12 05:38:35.000000 cdict-0.0.5/tests/test_main.py
+drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-06-08 23:50:25.678567 cdict-1.0.0/
+-rw-r--r--   0 jeffwu     (503) staff       (20)       42 2022-05-24 14:35:55.000000 cdict-1.0.0/.gitignore
+-rw-r--r--   0 jeffwu     (503) staff       (20)     1080 2022-05-24 14:35:55.000000 cdict-1.0.0/LICENSE
+-rw-r--r--   0 jeffwu     (503) staff       (20)      199 2023-06-08 23:50:25.678171 cdict-1.0.0/PKG-INFO
+-rw-r--r--   0 jeffwu     (503) staff       (20)     2469 2023-06-08 23:45:51.000000 cdict-1.0.0/README.md
+drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-06-08 23:50:25.652008 cdict-1.0.0/cdict/
+-rw-r--r--   0 jeffwu     (503) staff       (20)       29 2023-02-07 17:31:36.000000 cdict-1.0.0/cdict/__init__.py
+-rw-r--r--   0 jeffwu     (503) staff       (20)     4078 2023-06-08 23:39:41.000000 cdict-1.0.0/cdict/main.py
+drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-06-08 23:50:25.676838 cdict-1.0.0/cdict.egg-info/
+-rw-r--r--   0 jeffwu     (503) staff       (20)      199 2023-06-08 23:50:25.000000 cdict-1.0.0/cdict.egg-info/PKG-INFO
+-rw-r--r--   0 jeffwu     (503) staff       (20)      204 2023-06-08 23:50:25.000000 cdict-1.0.0/cdict.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffwu     (503) staff       (20)        1 2023-06-08 23:50:25.000000 cdict-1.0.0/cdict.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffwu     (503) staff       (20)        6 2023-06-08 23:50:25.000000 cdict-1.0.0/cdict.egg-info/top_level.txt
+-rw-r--r--   0 jeffwu     (503) staff       (20)       38 2023-06-08 23:50:25.678630 cdict-1.0.0/setup.cfg
+-rw-r--r--   0 jeffwu     (503) staff       (20)      282 2023-06-08 23:47:51.000000 cdict-1.0.0/setup.py
+drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-06-08 23:50:25.677534 cdict-1.0.0/tests/
+-rw-r--r--   0 jeffwu     (503) staff       (20)     4674 2023-06-08 23:44:41.000000 cdict-1.0.0/tests/test_main.py
```

### Comparing `cdict-0.0.5/LICENSE` & `cdict-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdict-0.0.5/README.md` & `cdict-1.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -34,17 +34,26 @@
 assert list(sweep_a * sweep_b) == [
     dict(a=1, aa=1, b=1),
     dict(a=1, aa=1, b=2),
     dict(a=2, aa=4, b=1),
     dict(a=2, aa=4, b=2),
 ]
 
-# overriding behavior
-assert list(b1 * b2) == [
-    dict(b=2)
+# conflicting keys errors by default
+with pytest.raises(ValueError):
+    list(b1 * b2)
+
+# implementing a cdict_combine lets you override that behavior
+class summing_number(int):
+    def cdict_combine(self, other):
+        return summing_number(self + other)
+b1 = C.dict(b=1)
+b2 = C.dict(b=2)
+asserrt list(b1 * b2) == [
+    dict(b=3)
 ]
 
 # also some convenience ways to union
 sweep_concise = C.dict(a=C.list(1, 2), b=C.list(1, 2))
 assert list(sweep_concise) == [
     dict(a=1, b=1),
     dict(a=1, b=2),
@@ -73,17 +82,16 @@
 
 def square_a(x):
     x['aa'] = x['a']**2
     return x
 
 a3 = a3.map(square_a)
 assert list(a3) == [dict(a=3, aa=9)]
-
 ```
 
 ## Properties
 
 - `*` `+` and `|` are associative
-- `*` distributes over `+`, that is `a * c + b * c = (a + b) * c`.  On the other hand `c * a + c * b = c * (a + b)` is only true ignoring order of the resulting items.
+- `*` is left-distributive over `+`, that is `a * c + b * c = (a + b) * c`.  It is right-distributive if ignoring order of the resulting items.
 - `+`  is commutative if you don’t care about order of the resulting items
-- `|` is commutative if you never overwrite keys
-- `*` is commutative if you don’t care about order of the resulting items and never overwrite keys
+- `|` is commutative if key-combination is commutative
+- `*` is commutative if you don’t care about order of the resulting items and key-combination is commutative
```

### Comparing `cdict-0.0.5/cdict/main.py` & `cdict-1.0.0/cdict/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,25 @@
     def __init__(self, _items: List[cdict]) -> None:
         for c in _items:
             assert isinstance(c, cdict), "Cannot multiply"
         self._items = _items
 
     def __iter__(self):
         for ds in itertools.product(*self._items):
-            yield dict(sum((list(d.items()) for d in ds), []))
+            res = {}
+            for d in ds:
+                for k, v in d.items():
+                    if k in res:
+                        if hasattr(res[k], "cdict_combine"):
+                            res[k] = res[k].cdict_combine(v)
+                        else:
+                            raise ValueError(f"Cannot combine {res[k]} and {v}")
+                    else:
+                        res[k] = v
+            yield res
 
     def __repr_helper__(self) -> str:
         return " * ".join([d.__repr_helper__() for d in self._items])
 
 
 def safe_zip(*iterables: Iterable) -> Generator[Tuple[Any], None, None]:
     sentinel = object()
```

