# Comparing `tmp/consoleprint-1.3.3.tar.gz` & `tmp/consoleprint-1.3.4.tar.gz`

## Comparing `consoleprint-1.3.3.tar` & `consoleprint-1.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.3.3/src/ConsolePrint/__init__.py
--rw-r--r--   0        0        0     9691 2020-02-02 00:00:00.000000 consoleprint-1.3.3/src/ConsolePrint/animate.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 consoleprint-1.3.3/src/ConsolePrint/console2file.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.3.3/src/ConsolePrint/loading.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 consoleprint-1.3.3/tests/tests.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.3.3/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.3.3/LICENSE
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 consoleprint-1.3.3/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 consoleprint-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 consoleprint-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.3.4/src/ConsolePrint/__init__.py
+-rw-r--r--   0        0        0     9691 2020-02-02 00:00:00.000000 consoleprint-1.3.4/src/ConsolePrint/animate.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 consoleprint-1.3.4/src/ConsolePrint/console2file.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.3.4/src/ConsolePrint/loading.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 consoleprint-1.3.4/tests/tests.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.3.4/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.3.4/LICENSE
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 consoleprint-1.3.4/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 consoleprint-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 consoleprint-1.3.4/PKG-INFO
```

### Comparing `consoleprint-1.3.3/src/ConsolePrint/animate.py` & `consoleprint-1.3.4/src/ConsolePrint/animate.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.3/src/ConsolePrint/loading.py` & `consoleprint-1.3.4/src/ConsolePrint/loading.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.3/tests/tests.py` & `consoleprint-1.3.4/tests/tests.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.3/LICENSE` & `consoleprint-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.3/README.md` & `consoleprint-1.3.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 Requires python 3.10 or later versions.
 
 # Installation
 You may install it form PyPI.org using the pip command typed in your terminal.<br>
 `pip install ConsolePrint`
 
 # Test Cases
-1.  Run your function between the start and end console save functions to save it to file.
+1.  This permits output of programs to be saved in a file.  Run your code between the start and end console save functions to save the output to file.
 ```python
 import ConsolePrint.console2file as file  
 
 file.startConsoleSave()
 # Saves all output between the start and end functions to file
 from calendar import calendar
 print(calendar(2023))
 file.endConsoleSave()
 ```
-2.  Here you may use ANSI escape sequences for the format argument and change others as desired.<br>
+2.  This module permits differnt colourful print animations to be output to file.  The format argument takes an ANSI escape sequences as a string.  You may also modify other arguments as desired.<br>
 <b>Preset string values for the format argument</b>
 <table>
     <tr>
         <td>'default' =        '\033[0m'</td>
         <td>'grey' =           '\033[30m'</td>
         <td>'red' =            '\033[31m'</td>
     </tr>
@@ -68,15 +68,15 @@
 prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
 prt.animate1("This text is animated with #", symbol="#", format='magenta')
 prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
 prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='right', format='\033[48;5;4m')
 prt.asteriskify('This has been asteriskified', align='center', underscore=True, format='cyan')
 ```
 
-3.  Here, the load time is specified as an integer in seconds.
+3.  This adds loading animations to terminal program.  The load time argument is specified as an integer in seconds.
 ```python
 import ConsolePrint.loading as load  
 
 load.countdown(5)
 load.loading1(10)
 print()
 load.loading2(5)
```

### Comparing `consoleprint-1.3.3/pyproject.toml` & `consoleprint-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ConsolePrint"
-version = "1.3.3"
+version = "1.3.4"
 authors = [
   { name="Udemezue Iloabachie", email="udemezue@gmail.com" },
 ]
 description = "A package to animate and beautify print output to console"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `consoleprint-1.3.3/PKG-INFO` & `consoleprint-1.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConsolePrint
-Version: 1.3.3
+Version: 1.3.4
 Summary: A package to animate and beautify print output to console
 Project-URL: Homepage, https://github.com/iloabachie/ConsolePrint
 Project-URL: Bug Tracker, https://github.com/iloabachie/ConsolePrint/issues
 Author-email: Udemezue Iloabachie <udemezue@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,25 +19,25 @@
 Requires python 3.10 or later versions.
 
 # Installation
 You may install it form PyPI.org using the pip command typed in your terminal.<br>
 `pip install ConsolePrint`
 
 # Test Cases
-1.  Run your function between the start and end console save functions to save it to file.
+1.  This permits output of programs to be saved in a file.  Run your code between the start and end console save functions to save the output to file.
 ```python
 import ConsolePrint.console2file as file  
 
 file.startConsoleSave()
 # Saves all output between the start and end functions to file
 from calendar import calendar
 print(calendar(2023))
 file.endConsoleSave()
 ```
-2.  Here you may use ANSI escape sequences for the format argument and change others as desired.<br>
+2.  This module permits differnt colourful print animations to be output to file.  The format argument takes an ANSI escape sequences as a string.  You may also modify other arguments as desired.<br>
 <b>Preset string values for the format argument</b>
 <table>
     <tr>
         <td>'default' =        '\033[0m'</td>
         <td>'grey' =           '\033[30m'</td>
         <td>'red' =            '\033[31m'</td>
     </tr>
@@ -82,15 +82,15 @@
 prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
 prt.animate1("This text is animated with #", symbol="#", format='magenta')
 prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
 prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='right', format='\033[48;5;4m')
 prt.asteriskify('This has been asteriskified', align='center', underscore=True, format='cyan')
 ```
 
-3.  Here, the load time is specified as an integer in seconds.
+3.  This adds loading animations to terminal program.  The load time argument is specified as an integer in seconds.
 ```python
 import ConsolePrint.loading as load  
 
 load.countdown(5)
 load.loading1(10)
 print()
 load.loading2(5)
```

