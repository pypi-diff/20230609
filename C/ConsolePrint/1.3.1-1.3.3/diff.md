# Comparing `tmp/consoleprint-1.3.1.tar.gz` & `tmp/consoleprint-1.3.3.tar.gz`

## Comparing `consoleprint-1.3.1.tar` & `consoleprint-1.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.3.1/src/ConsolePrint/__init__.py
--rw-r--r--   0        0        0     9769 2020-02-02 00:00:00.000000 consoleprint-1.3.1/src/ConsolePrint/animate.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 consoleprint-1.3.1/src/ConsolePrint/console2file.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.3.1/src/ConsolePrint/loading.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 consoleprint-1.3.1/tests/tests.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.3.1/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.3.1/LICENSE
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 consoleprint-1.3.1/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 consoleprint-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 consoleprint-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.3.3/src/ConsolePrint/__init__.py
+-rw-r--r--   0        0        0     9691 2020-02-02 00:00:00.000000 consoleprint-1.3.3/src/ConsolePrint/animate.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 consoleprint-1.3.3/src/ConsolePrint/console2file.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.3.3/src/ConsolePrint/loading.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 consoleprint-1.3.3/tests/tests.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.3.3/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.3.3/LICENSE
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 consoleprint-1.3.3/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 consoleprint-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 consoleprint-1.3.3/PKG-INFO
```

### Comparing `consoleprint-1.3.1/src/ConsolePrint/animate.py` & `consoleprint-1.3.3/src/ConsolePrint/animate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import time
 import os
 
-def ansify_color(color:str):  
+if __name__ == "__main__":
+    os.system('cls')
+    print('\033[0m', end="\r")
+
+_terminal_width = os.get_terminal_size().columns
+
+def _ansify_color(color:str):  
     match color:
-        #colours
         case 'default': color = '\033[0m'
         case 'grey': color = '\033[30m'
         case 'red': color = '\033[31m'
         case 'green': color = '\033[32m'
         case 'yellow': color = '\033[33m'
         case 'blue': color = '\033[34m'
         case 'magenta': color = '\033[35m'
         case 'cyan': color = '\033[36m'
         case 'white': color = '\033[37m'
-        # Text Formats
         case 'bold': color = '\033[1m'
         case 'italics': color = '\033[3m'
         case 'underscore': color = '\033[4m'
         case 'strike': color = '\033[9m'
         case 'double_under': color = '\033[21m'
         case 'red_bg': color = '\033[41m'
         case 'green_bg': color = '\033[42m'
@@ -27,24 +31,17 @@
         case 'cyan_bg': color = '\033[46m'
         case 'white_bg': color = '\033[47m'
         case _:
             if '[' not in color or color[-1] != 'm' or not color[2:3].isdigit():
                 raise Exception("Invalid ANSI escape sequence for argument format")
     return color
 
-
-if __name__ == "__main__":
-    os.system('cls')
-    print('\033[0m', end="\r")
-
-terminal_width = os.get_terminal_size().columns
-
 def printing(text:str, delay:float=0.05, style:str='letter', stay:bool=True, rev:bool=False, format:str='default'):
     """Prints text to console letter by letter or word by word"""
-    format = ansify_color(format)
+    format = _ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     match rev:
         case False:
             if style.lower() == 'letter':
                 for _ in range(len(text)):
                     print(text[:_ + 1], end='\r')
@@ -67,31 +64,29 @@
     if stay:
         print()
     print('\033[0m', end='\r')
 
 
 def flashprint(text:str, blinks:int=5, delay:float=0.2, stay:bool=True, format:str='default'):
     """Gets printed output to blink"""
-    format = ansify_color(format)
+    format = _ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     for _ in range(blinks):
         print(text, end='\r'), time.sleep(delay)
         print(' ' * len(text), end='\r'), time.sleep(delay)
     if stay:
         print(text)
     print('\033[0m', end='\r')
 
 
 def flashtext(phrase:str, text:str, index='end', blinks:int=5, delay:float=0.2, format:str='default'):
     """Hilights key word by flashing it"""
-    format = ansify_color(format)
+    format = _ansify_color(format)
     print(format, end='\r')
-    text = text.strip()
-    phrase = phrase.strip()
     textb = ' ' * len(text)
     if index == 'end':
         phrase1 = phrase
         phrase2 = ''
     else:
         phrase1 = phrase[:index]
         phrase2 = phrase[index:]
@@ -105,26 +100,26 @@
     print('\033[0m', end='\r')
 
 
 def animate1(text:str, symbol:str="#", format:str='default'):
     """Flashing masked text to transition to flasing text"""
     if len(symbol) != 1:
         raise Exception("Symbol input should be a single character")
-    format = ansify_color(format)
+    format = _ansify_color(format)
     text = text.strip()
     symbol = len(text) * symbol
     flashprint(symbol, blinks=3, stay=False, format=format)
     flashprint(text, blinks=2, stay=True, format=format)
 
 
 def animate2(text:str, symbol:str="#", delay:float=0.05, format:str='default'):
     """Reveals all characters text by text but first masked then flashes"""
     if len(symbol) != 1:
         raise Exception("Symbol input should be a single character")
-    format = ansify_color(format)
+    format = _ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     symbol = len(text) * symbol
     for _ in symbol + "\r" + text + "\r":
         print(_, end="", flush=True)
         time.sleep(delay)
     flashprint(text, blinks=2, stay=True, format=format)
@@ -133,27 +128,27 @@
 def text_box(text:str, symbol:str="#", spread:bool=False, padding:bool=False, wall:bool=True, align:str="center", format:str='default'):
     """Prints text in a box of symbols.
 If the align parameter is a number then the box is indented by the number count"""
     if spread:
         text = " ".join(list(text)).upper()
     if len(symbol) != 1:
         raise Exception("Symbol input should be a single character")
-    format = ansify_color(format)
+    format = _ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     end = 5 if padding else 3
     text_row = 3 if padding else 2
     length = len(text) + 8
     left_border = text_row - 1  if padding else text_row
     right_border = text_row + 1 if padding else text_row
     
     if align == "left": indent = 0
-    elif align == "right": indent = terminal_width - length
-    elif align == "center": indent = terminal_width//2 - length//2
-    elif isinstance(align, int) and align <= (terminal_width - length): indent = align
+    elif align == "right": indent = _terminal_width - length
+    elif align == "center": indent = _terminal_width//2 - length//2
+    elif isinstance(align, int) and align <= (_terminal_width - length): indent = align
     else: raise Exception(f"Error in the align argument: {align=}")  
     
     for row in range(1, end + 1):
         for col in range(1, length + 1):
             if col == 1:
                 print('\033[0m' + (" " * indent) + format, end="")
             if row == 1 or row == end or col == 1 or col == length:
@@ -172,25 +167,25 @@
             if col == length:
                 print('\033[0m')
                 
                 
 def star_square(num:int, symbol:str="#", align:str='center', flush:bool=True, format:str='default'):
     if len(symbol) != 1:
         raise Exception("Symbol input should be a single character")
-    format = ansify_color(format)
+    format = _ansify_color(format)
     print(format, end='\r')
-    if num < 5 or num > terminal_width or not isinstance(num, int):
-        raise Exception(f"Invalid square size. Number must be an integer greater than 4 and less than the terminal width: {terminal_width}")
+    if num < 5 or num > _terminal_width or not isinstance(num, int):
+        raise Exception(f"Invalid square size. Number must be an integer greater than 4 and less than the terminal width: {_terminal_width}")
     elif align == 'center':
-        indent = '\033[0m' + (' ' * (terminal_width//2 - num//2)) + format
+        indent = '\033[0m' + (' ' * (_terminal_width//2 - num//2)) + format
     elif align == 'right':
-        indent = '\033[0m' + (' ' * (terminal_width - num)) + format
+        indent = '\033[0m' + (' ' * (_terminal_width - num)) + format
     elif align == 'left':
         indent = ''  
-    elif isinstance(align, int) and terminal_width - align > num:
+    elif isinstance(align, int) and _terminal_width - align > num:
         indent = '\033[0m' + (" " * align) + format
     else:
         raise Exception("Align parameter is invalid")    
           
     for row in range(1, num + 1):
         time.sleep(0.04)
         print(indent, end="")
@@ -205,23 +200,23 @@
             else:
                 print(" ", end="", flush=flush)              
             if col == num:
                 print('\033[0m')
     
 
 def asteriskify(text:str, align:str="center", underscore:bool=True, format:str='default'):
-    format = ansify_color(format)
+    format = _ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     length = len(text)
     
     if align == 'center':
-        indent = '\033[0m' + ' ' * (terminal_width//2 - length//2) + format
+        indent = '\033[0m' + ' ' * (_terminal_width//2 - length//2) + format
     elif align == 'right':
-        indent = '\033[0m' + ' ' * (terminal_width - length) + format
+        indent = '\033[0m' + ' ' * (_terminal_width - length) + format
     elif align == 'left':
         indent = ''
     else:
         raise Exception("Align argument error") 
     print(indent + text)
     if underscore:
         print(indent + '*' * length)
```

### Comparing `consoleprint-1.3.1/src/ConsolePrint/console2file.py` & `consoleprint-1.3.3/src/ConsolePrint/console2file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """This module  saves terminal output to file."""
 import sys
 import subprocess
+from loading import loading2
 
 def startConsoleSave():
     """Starts the process to save the output to file"""
     global filename
-    filename = input("Choose filename and extension: ") # specified filename/path      
+    filename = input("Enter the output filename and extension: ") # specified filename/path      
     sys.stdout = open(filename, 'a')  # redirects output to specified file
 
 
 def endConsoleSave():  
     """Ends the save to file process and returns output to console"""  
     sys.stdout.close()
     sys.stdout = sys.__stdout__   # redirects output from file back to terminal
+    loading2(1, "")
+    print("    ")
     print(f"Output has been saved to {filename}")
-    open_file = input("Would you like to open the file? y/n: ")
+    open_file = input("\nWould you like to open the file? y/n: ")
     if open_file.strip().lower() == "y":
         try:
             subprocess.Popen(["start", "", filename], shell=True)
         except FileNotFoundError:
             print("File not found.")
         except OSError:
             print("Error opening file.")
```

### Comparing `consoleprint-1.3.1/src/ConsolePrint/loading.py` & `consoleprint-1.3.3/src/ConsolePrint/loading.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.1/tests/tests.py` & `consoleprint-1.3.3/tests/tests.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.1/LICENSE` & `consoleprint-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.1/README.md` & `consoleprint-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.1/pyproject.toml` & `consoleprint-1.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ConsolePrint"
-version = "1.3.1"
+version = "1.3.3"
 authors = [
   { name="Udemezue Iloabachie", email="udemezue@gmail.com" },
 ]
 description = "A package to animate and beautify print output to console"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `consoleprint-1.3.1/PKG-INFO` & `consoleprint-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConsolePrint
-Version: 1.3.1
+Version: 1.3.3
 Summary: A package to animate and beautify print output to console
 Project-URL: Homepage, https://github.com/iloabachie/ConsolePrint
 Project-URL: Bug Tracker, https://github.com/iloabachie/ConsolePrint/issues
 Author-email: Udemezue Iloabachie <udemezue@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

