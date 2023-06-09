# Comparing `tmp/irene_pro-0.0.62.tar.gz` & `tmp/irene_pro-0.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.62.tar", last modified: Thu Jun  8 14:26:00 2023, max compression
+gzip compressed data, was "irene_pro-0.0.63.tar", last modified: Fri Jun  9 07:09:00 2023, max compression
```

## Comparing `irene_pro-0.0.62.tar` & `irene_pro-0.0.63.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 14:26:00.371809 irene_pro-0.0.62/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.62/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.62/MANIFEST.in
--rw-rw-rw-   0        0        0     1940 2023-06-08 14:26:00.368816 irene_pro-0.0.62/PKG-INFO
--rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.62/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 14:26:00.346876 irene_pro-0.0.62/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.62/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.62/irene_pro/logic.py
--rw-rw-rw-   0        0        0    33012 2023-06-08 14:25:12.000000 irene_pro-0.0.62/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-08 14:26:00.365826 irene_pro-0.0.62/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1940 2023-06-08 14:26:00.000000 irene_pro-0.0.62/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-06-08 14:26:00.000000 irene_pro-0.0.62/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 14:26:00.000000 irene_pro-0.0.62/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-08 14:26:00.000000 irene_pro-0.0.62/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-08 14:26:00.000000 irene_pro-0.0.62/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 14:26:00.372805 irene_pro-0.0.62/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-06-08 14:25:28.000000 irene_pro-0.0.62/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 07:09:00.216568 irene_pro-0.0.63/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.63/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.63/MANIFEST.in
+-rw-rw-rw-   0        0        0     1940 2023-06-09 07:09:00.214572 irene_pro-0.0.63/PKG-INFO
+-rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.63/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 07:09:00.191633 irene_pro-0.0.63/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.63/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.63/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    33024 2023-06-09 07:07:26.000000 irene_pro-0.0.63/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-09 07:09:00.211581 irene_pro-0.0.63/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1940 2023-06-09 07:09:00.000000 irene_pro-0.0.63/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-09 07:09:00.000000 irene_pro-0.0.63/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 07:09:00.000000 irene_pro-0.0.63/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-09 07:09:00.000000 irene_pro-0.0.63/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-09 07:09:00.000000 irene_pro-0.0.63/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 07:09:00.217565 irene_pro-0.0.63/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-06-09 07:07:52.000000 irene_pro-0.0.63/setup.py
```

### Comparing `irene_pro-0.0.62/PKG-INFO` & `irene_pro-0.0.63/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.62
+Version: 0.0.63
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.62/README.md` & `irene_pro-0.0.63/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.62/irene_pro/logic.py` & `irene_pro-0.0.63/irene_pro/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.62/irene_pro/widgets.py` & `irene_pro-0.0.63/irene_pro/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,16 +84,16 @@
         style.theme_use("clam")
         style.map("Treeview", background=[('selected', 'gray40')], foreground = [('selected', 'gold')])
         self.tag_configure('odd', background='gray70')
         self.tag_configure('even', background='khaki')
 
     def insert_data(self,data, wrap_length = 70):
         def wrapping(data_list):
+            """I assume that datalist is a list as the name implies"""
             all_row = []
-            print(f"data list: {data_list}")
             for item in data_list:
                 # print(f"CURRENT ITEM: {item}")
                 if type(item) == str:
                     wrapped = wrap(item, wrap_length)
                     all_row.append("\n".join(wrapped))
                 else:
                     all_row.append(item)
@@ -118,19 +118,19 @@
                 
             else:
                 for index, row in enumerate(data):
                     tag = ('odd')
                     if self.index_for_single_list_data % 2 ==0:
                         tag = ('even',)
                     if self.include_index:
-                        data_wrapped = wrapping(row[index])
+                        data_wrapped = wrapping(row)
                         print(" [H: ] {data_wrapped}")
                         self.insert("", index=index,text=self.index_for_single_list_data+1, values = data_wrapped, tags=tag)
                     else:
-                        data_wrapped = wrapping(row[index])
+                        data_wrapped = wrapping(row)
                         print(" [G: ] {data_wrapped}")
                         self.insert("", index=index, values = data_wrapped)
                     self.index_for_single_list_data += 1
         except IndexError:
             pass
 
 class btn(Button):
```

### Comparing `irene_pro-0.0.62/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.63/irene_pro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.62
+Version: 0.0.63
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.62/setup.py` & `irene_pro-0.0.63/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3632 270d 0a44 4553 4352   '0.0.62'..DESCR
+00000100: 2027 302e 302e 3633 270d 0a44 4553 4352   '0.0.63'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

