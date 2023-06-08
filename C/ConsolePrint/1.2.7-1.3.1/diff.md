# Comparing `tmp/consoleprint-1.2.7.tar.gz` & `tmp/consoleprint-1.3.1.tar.gz`

## Comparing `consoleprint-1.2.7.tar` & `consoleprint-1.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.2.7/src/ConsolePrint/__init__.py
--rw-r--r--   0        0        0     9769 2020-02-02 00:00:00.000000 consoleprint-1.2.7/src/ConsolePrint/animate.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 consoleprint-1.2.7/src/ConsolePrint/console2file.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.2.7/src/ConsolePrint/loading.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 consoleprint-1.2.7/tests/tests.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.2.7/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.2.7/LICENSE
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 consoleprint-1.2.7/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 consoleprint-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 consoleprint-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.3.1/src/ConsolePrint/__init__.py
+-rw-r--r--   0        0        0     9769 2020-02-02 00:00:00.000000 consoleprint-1.3.1/src/ConsolePrint/animate.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 consoleprint-1.3.1/src/ConsolePrint/console2file.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.3.1/src/ConsolePrint/loading.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 consoleprint-1.3.1/tests/tests.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.3.1/LICENSE
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 consoleprint-1.3.1/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 consoleprint-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 consoleprint-1.3.1/PKG-INFO
```

### Comparing `consoleprint-1.2.7/src/ConsolePrint/animate.py` & `consoleprint-1.3.1/src/ConsolePrint/animate.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.2.7/src/ConsolePrint/console2file.py` & `consoleprint-1.3.1/src/ConsolePrint/console2file.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.2.7/src/ConsolePrint/loading.py` & `consoleprint-1.3.1/src/ConsolePrint/loading.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.2.7/tests/tests.py` & `consoleprint-1.3.1/tests/tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 # animate.py
 import ConsolePrint.animate as prt
 
 prt.printing("hello this should print letter by letter", delay=0.05, style="letter", stay=True, rev=False, format='strike')
 prt.printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format='red_bg')
 prt.flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format='green')
 prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
-prt.animate1("This text is animated with #", symbol="#", format='strike')
+prt.animate1("This text is animated with #", symbol="#", format='blue')
 prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
 prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='center', format='\033[48;5;4m')
 prt.star_square(10, symbol="@", align=15, flush="True", format="\033[104m")
 prt.asteriskify('This has been asteriskified', align='center', underscore=True, format='cyan')
 
-# console2file.pt
-import ConsolePrint.console2file as file
-import calendar
-
-file.startConsoleSave()
-
-print("Printing Calendar")
-print(calendar.calendar(2023))
-
-file.endConsoleSave()  
-
-# loading.py
-import ConsolePrint.loading as load
-
-load.countdown(5)
-print()
-load.loading1(20)  
-print()
-load.loading2(5, 'thinking...')
-print()
-load.loading3(5)
+# console2file.py
+# import ConsolePrint.console2file as file
+# import calendar
+
+# file.startConsoleSave()
+
+# print("Printing Calendar")
+# print(calendar.calendar(2023))
+
+# file.endConsoleSave()  
+
+# # loading.py
+# import ConsolePrint.loading as load
+
+# load.countdown(5)
+# print()
+# load.loading1(20)  
+# print()
+# load.loading2(5, 'thinking...')
+# print()
+# load.loading3(5)
```

### Comparing `consoleprint-1.2.7/LICENSE` & `consoleprint-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleprint-1.2.7/README.md` & `consoleprint-1.3.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,100 @@
-# ConsolePrint
-This module making printing to the terminal more exciting by animating the text output.
-It also makes output richer my modifying the color
+# ConsolePrint Module
+This module makes printing to the terminal more exciting by animating the text output.
+It also makes the output richer my providing access to color modification.
 You can also save routine console output to a file using the console2file module.
-Created using python 3.11
+Requires python 3.10 or later versions.
 
 # Installation
-You may install it form PyPI.org using the pip command.
+You may install it form PyPI.org using the pip command typed in your terminal.<br>
+`pip install ConsolePrint`
 
-pip install ConsolePrint
-
-# Usage
-Copy the code below and run it from your IDE, preferable Visual Studio Code.  May not produce the desired output on some terminals.
+# Test Cases
+1.  Run your function between the start and end console save functions to save it to file.
 ```python
-import ConsolePrint.animate as prt    
-
 import ConsolePrint.console2file as file  
 
-import ConsolePrint.loading as load        
-```
-# Test Cases
-1.  Here uou may change the arguments as desired
-```python
 file.startConsoleSave()
-
-'Saves all output between the start and end functions to file.'
-
+# Saves all output between the start and end functions to file
 from calendar import calendar
-
 print(calendar(2023))
-
 file.endConsoleSave()
 ```
-2. Here you may use ANSI escape sequences for the format argument and change others as desired.
-Preset arguments for format:
-//colours
-'default':          '\033[0m'
-'grey':             '\033[30m'
-'red':              '\033[31m'
-'green':            '\033[32m'
-'yellow':           '\033[33m'
-'blue':             '\033[34m'
-'magenta':          '\033[35m'
-'cyan':             '\033[36m'
-'white':            '\033[37m'
-//Text Formats
-'bold':             '\033[1m'
-'italics':          '\033[3m'
-'underscore':       '\033[4m'
-'strike':           '\033[9m'
-'double_under':     '\033[21m'
-'red_bg':           '\033[41m'
-'green_bg':         '\033[42m'
-'yellow_bg':        '\033[43m'
-'blue_bg':          '\033[44m'
-'magenta_bg':       '\033[45m'
-'cyan_bg':          '\033[46m'
-'white_bg':         '\033[47m'
+2.  Here you may use ANSI escape sequences for the format argument and change others as desired.<br>
+<b>Preset string values for the format argument</b>
+<table>
+    <tr>
+        <td>'default' =        '\033[0m'</td>
+        <td>'grey' =           '\033[30m'</td>
+        <td>'red' =            '\033[31m'</td>
+    </tr>
+    <tr>
+        <td>'green' =          '\033[32m'</td>
+        <td>'yellow' =         '\033[33m'</td>
+        <td>'blue' =           '\033[34m'</td>
+    </tr>
+    <tr>
+        <td>'magenta' =        '\033[35m'</td>
+        <td>'cyan' =           '\033[36m'</td>
+        <td>'white' =          '\033[37m'</td>
+    </tr>
+    <tr>
+        <td>'bold' =           '\033[1m'</td>
+        <td>'italics' =        '\033[3m'</td>
+        <td>'underscore' =     '\033[4m'</td>
+    </tr>
+    <tr>
+        <td>'strike' =         '\033[9m'</td>
+        <td>'double_under' =   '\033[21m'</td>
+        <td>'red_bg' =         '\033[41m'</td>
+    </tr>
+    <tr>
+        <td>'green_bg' =       '\033[42m'</td>
+        <td>'yellow_bg' =      '\033[43m'</td>
+        <td>'blue_bg' =        '\033[44m'</td>
+    </tr>
+    <tr>
+        <td>'magenta_bg' =     '\033[45m'</td>
+        <td>'cyan_bg' =        '\033[46m'</td>
+        <td>'white_bg' =       '\033[47m'</td>
+    </tr>
+</table>
 
 ```python
-prt.printing("hello this should print letter by letter", delay=0.05, style="letter", stay=True, rev=False, format='strike')
+import ConsolePrint.animate as prt 
 
+prt.printing("hello this should print letter by letter", delay=0.05, style="letter", stay=True, rev=False, format='strike')
 prt.printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format='red_bg')
-
 prt.flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format='green')
-
 prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
-
-prt.animate1("This text is animated with #", symbol="#", format='white')
-
+prt.animate1("This text is animated with #", symbol="#", format='magenta')
 prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
-
-prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='center', format='\033[48;5;4m')
-
+prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='right', format='\033[48;5;4m')
 prt.asteriskify('This has been asteriskified', align='center', underscore=True, format='cyan')
 ```
 
-3.  Here, the load time is specified in seconds
+3.  Here, the load time is specified as an integer in seconds.
 ```python
-load.countdown(5)
+import ConsolePrint.loading as load  
 
+load.countdown(5)
 load.loading1(10)
-
 print()
-
 load.loading2(5)
-
 print()
-
 load.loading3(5)
 ```
-# License
+## License
 This project is given free for use and download under the MIT license.
 
-# Project Status
+## Project Status
 Still undergoing enhancements.
 
-# How to Contribute
+## How to Contribute
 Fork the repository and create your branch from main.
 Clone the repository and make your changes.
 Run tests and make sure they pass: python -m unittest
 Commit your changes and push to your branch.
 Create a pull request.
 
-# Support
+## Support
 If you encounter any issues or have questions about the project, please contact me at udemezue@gmail.com.
```

### Comparing `consoleprint-1.2.7/pyproject.toml` & `consoleprint-1.3.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ConsolePrint"
-version = "1.2.7"
+version = "1.3.1"
 authors = [
   { name="Udemezue Iloabachie", email="udemezue@gmail.com" },
 ]
 description = "A package to animate and beautify print output to console"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `consoleprint-1.2.7/PKG-INFO` & `consoleprint-1.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,120 +1,114 @@
 Metadata-Version: 2.1
 Name: ConsolePrint
-Version: 1.2.7
+Version: 1.3.1
 Summary: A package to animate and beautify print output to console
 Project-URL: Homepage, https://github.com/iloabachie/ConsolePrint
 Project-URL: Bug Tracker, https://github.com/iloabachie/ConsolePrint/issues
 Author-email: Udemezue Iloabachie <udemezue@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
-# ConsolePrint
-This module making printing to the terminal more exciting by animating the text output.
-It also makes output richer my modifying the color
+# ConsolePrint Module
+This module makes printing to the terminal more exciting by animating the text output.
+It also makes the output richer my providing access to color modification.
 You can also save routine console output to a file using the console2file module.
-Created using python 3.11
+Requires python 3.10 or later versions.
 
 # Installation
-You may install it form PyPI.org using the pip command.
+You may install it form PyPI.org using the pip command typed in your terminal.<br>
+`pip install ConsolePrint`
 
-pip install ConsolePrint
-
-# Usage
-Copy the code below and run it from your IDE, preferable Visual Studio Code.  May not produce the desired output on some terminals.
+# Test Cases
+1.  Run your function between the start and end console save functions to save it to file.
 ```python
-import ConsolePrint.animate as prt    
-
 import ConsolePrint.console2file as file  
 
-import ConsolePrint.loading as load        
-```
-# Test Cases
-1.  Here uou may change the arguments as desired
-```python
 file.startConsoleSave()
-
-'Saves all output between the start and end functions to file.'
-
+# Saves all output between the start and end functions to file
 from calendar import calendar
-
 print(calendar(2023))
-
 file.endConsoleSave()
 ```
-2. Here you may use ANSI escape sequences for the format argument and change others as desired.
-Preset arguments for format:
-//colours
-'default':          '\033[0m'
-'grey':             '\033[30m'
-'red':              '\033[31m'
-'green':            '\033[32m'
-'yellow':           '\033[33m'
-'blue':             '\033[34m'
-'magenta':          '\033[35m'
-'cyan':             '\033[36m'
-'white':            '\033[37m'
-//Text Formats
-'bold':             '\033[1m'
-'italics':          '\033[3m'
-'underscore':       '\033[4m'
-'strike':           '\033[9m'
-'double_under':     '\033[21m'
-'red_bg':           '\033[41m'
-'green_bg':         '\033[42m'
-'yellow_bg':        '\033[43m'
-'blue_bg':          '\033[44m'
-'magenta_bg':       '\033[45m'
-'cyan_bg':          '\033[46m'
-'white_bg':         '\033[47m'
+2.  Here you may use ANSI escape sequences for the format argument and change others as desired.<br>
+<b>Preset string values for the format argument</b>
+<table>
+    <tr>
+        <td>'default' =        '\033[0m'</td>
+        <td>'grey' =           '\033[30m'</td>
+        <td>'red' =            '\033[31m'</td>
+    </tr>
+    <tr>
+        <td>'green' =          '\033[32m'</td>
+        <td>'yellow' =         '\033[33m'</td>
+        <td>'blue' =           '\033[34m'</td>
+    </tr>
+    <tr>
+        <td>'magenta' =        '\033[35m'</td>
+        <td>'cyan' =           '\033[36m'</td>
+        <td>'white' =          '\033[37m'</td>
+    </tr>
+    <tr>
+        <td>'bold' =           '\033[1m'</td>
+        <td>'italics' =        '\033[3m'</td>
+        <td>'underscore' =     '\033[4m'</td>
+    </tr>
+    <tr>
+        <td>'strike' =         '\033[9m'</td>
+        <td>'double_under' =   '\033[21m'</td>
+        <td>'red_bg' =         '\033[41m'</td>
+    </tr>
+    <tr>
+        <td>'green_bg' =       '\033[42m'</td>
+        <td>'yellow_bg' =      '\033[43m'</td>
+        <td>'blue_bg' =        '\033[44m'</td>
+    </tr>
+    <tr>
+        <td>'magenta_bg' =     '\033[45m'</td>
+        <td>'cyan_bg' =        '\033[46m'</td>
+        <td>'white_bg' =       '\033[47m'</td>
+    </tr>
+</table>
 
 ```python
-prt.printing("hello this should print letter by letter", delay=0.05, style="letter", stay=True, rev=False, format='strike')
+import ConsolePrint.animate as prt 
 
+prt.printing("hello this should print letter by letter", delay=0.05, style="letter", stay=True, rev=False, format='strike')
 prt.printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format='red_bg')
-
 prt.flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format='green')
-
 prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
-
-prt.animate1("This text is animated with #", symbol="#", format='white')
-
+prt.animate1("This text is animated with #", symbol="#", format='magenta')
 prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
-
-prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='center', format='\033[48;5;4m')
-
+prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='right', format='\033[48;5;4m')
 prt.asteriskify('This has been asteriskified', align='center', underscore=True, format='cyan')
 ```
 
-3.  Here, the load time is specified in seconds
+3.  Here, the load time is specified as an integer in seconds.
 ```python
-load.countdown(5)
+import ConsolePrint.loading as load  
 
+load.countdown(5)
 load.loading1(10)
-
 print()
-
 load.loading2(5)
-
 print()
-
 load.loading3(5)
 ```
-# License
+## License
 This project is given free for use and download under the MIT license.
 
-# Project Status
+## Project Status
 Still undergoing enhancements.
 
-# How to Contribute
+## How to Contribute
 Fork the repository and create your branch from main.
 Clone the repository and make your changes.
 Run tests and make sure they pass: python -m unittest
 Commit your changes and push to your branch.
 Create a pull request.
 
-# Support
+## Support
 If you encounter any issues or have questions about the project, please contact me at udemezue@gmail.com.
```

