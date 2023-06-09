# Comparing `tmp/logicgate-0.2.6.tar.gz` & `tmp/logicgate-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logicgate-0.2.6.tar", max compression
+gzip compressed data, was "logicgate-0.2.7.tar", max compression
```

## Comparing `logicgate-0.2.6.tar` & `logicgate-0.2.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-04-15 10:25:03.782472 logicgate-0.2.6/LICENSE
--rw-r--r--   0        0        0    12812 2023-05-17 08:15:09.686291 logicgate-0.2.6/LogicGate/LogicGate.py
--rw-r--r--   0        0        0     4593 2023-05-17 08:15:15.734285 logicgate-0.2.6/LogicGate/lgEncrypt.py
--rw-r--r--   0        0        0     5175 2023-04-28 07:51:30.723628 logicgate-0.2.6/README.rst
--rw-r--r--   0        0        0      827 2023-05-20 00:28:34.207396 logicgate-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     6070 1970-01-01 00:00:00.000000 logicgate-0.2.6/setup.py
--rw-r--r--   0        0        0     5993 1970-01-01 00:00:00.000000 logicgate-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 10:25:03.782472 logicgate-0.2.7/LICENSE
+-rw-r--r--   0        0        0    14763 2023-06-09 14:58:22.476940 logicgate-0.2.7/LogicGate/LogicGate.py
+-rw-r--r--   0        0        0     4613 2023-06-09 14:16:33.643817 logicgate-0.2.7/LogicGate/lgEncrypt.py
+-rw-r--r--   0        0        0     5557 2023-06-09 15:19:28.426915 logicgate-0.2.7/README.rst
+-rw-r--r--   0        0        0      827 2023-06-09 14:17:58.136248 logicgate-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     6450 1970-01-01 00:00:00.000000 logicgate-0.2.7/setup.py
+-rw-r--r--   0        0        0     6375 1970-01-01 00:00:00.000000 logicgate-0.2.7/PKG-INFO
```

### Comparing `logicgate-0.2.6/LICENSE` & `logicgate-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `logicgate-0.2.6/LogicGate/LogicGate.py` & `logicgate-0.2.7/LogicGate/LogicGate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from os.path import exists
 from sys import argv
 import sys, os
 from random import randint
 from math import sqrt
 
 
-def run(
+def decompile(
     filename: str,
-    gate: bool = False,  #show gate in result
-    ascii: bool = True,  #show ascii in result
-    debug: bool = False,  #log during process
-    check: str = '',  #check for error in code, mostly for debug
+    gate: bool = False,
+    ascii: bool = True,
+    debug: bool = False,
+    check: str = '',
     out: bool = True):
-  """To run this filename is the only thing needed, Error will be raised and nothing will return if something went wrong. If ascii is on, it will return the ascii result, otherwise 0.
+  """To run this, filename is the only thing needed, Error will be raised and nothing will return if something went wrong. It will return the wrong bits if check, gate and ascii is on, decrypted result if ascii is on, or 0 otherwise.
   
   Arguments, type of input, usecases:
       filename: string, specify which file needed to run
       gate: boolean(True or False), if the result shows gate result or not
       ascii: boolean, if the result converts to ascii and show or not
       debug: boolean, show the unhuman log during the interpute
       check: string, if it is specified then the result will be colored. It compares the difference between the gate result and the binary of check input, only works if both gate and ascii is True 
              (color: green=correct bit
                      red=incorrect bit
                      blue box=missing bit 1
                      purple box=missing bit 0)
-      out: boolean, enable for outputs
+      out: boolean, it is seldom called as the silent argument, enable it for outputs, will not change return value
                      """
 
   def process(
     obj,  #first command
     line: tuple = (
       0, 0
     ),  #for error reporting, first is line and second is index, sometimes third for the latest gate called
@@ -37,15 +37,15 @@
   ) -> tuple:  #(0 or 1, unprocessed commands that may be used by and/or gates in previous commands in list)
     'One line code processor, return one output from a line of input, internal use only'
     if debug: print('called, args:', obj, line, aft, an)
     if len(str(obj)) == 1:  #if the first process string is a single command
       obj = str(obj).upper()
       if obj == "#":
         if aft[:2] == '##':
-          return
+          return ('', '')
       AnList = None
       if an != None:
         #if AnList exists, it is an and/or gate, depends on the first index is True(and) or False(or)
         AnList = [an]
         if debug: print('AnList init:', AnList)
       if obj == '1':
         if debug: print('1:', aft)
@@ -84,14 +84,18 @@
                          aft=aft[1:],
                          an=False)
           if debug: print('or:', proc)
           if AnList:
             AnList.append(proc)
           else:
             return tuple(proc)
+        elif obj != "0" and obj != "1":
+          sys.tracebacklimit = 0
+          sys.stdout = sys.__stdout__
+          raise SyntaxError(f'Invalid gate {obj} in line {line[0]} index {line[1]}')
       if AnList != None:
         if debug: print('And/Or gate:', AnList)
         try:
           if AnList[1][1] == None:
             raise IndexError()
           AnList.append(
             process(
@@ -222,15 +226,15 @@
   filename: str = 'main.lgeso',
   output: str = 'Hello World!',
   randomize: bool = True,
   random_range: list = [1, 5],
   write: bool = True,
   override: bool = False,
   BitLock: int = -1
-) -> None:  #I swear if this thing returns anything somehow somewhere and somewhat, python is dying or my brain is dying
+) -> str | None:
   """compile string to lgeso file, random_range is needed only when randomize is true.
   filename: string, specify which file to write the data into, new file named as filename will be created if it doesn't exist
   output: string, specify what result will be produced
   randomize: boolean, if the data written is pure binary or further encrypted with gates
   random_range: list, the maximum set of gates in the written data will be the square of the second item while the minimum will be the square of the first item.
   write: boolean, if the result is returned or is written to file
   override: boolean, safety checks are off, proceed with caution
@@ -310,9 +314,42 @@
         out += "-"
     print(
       f'compilation completed and result {"written in" if write else "returned"} {filename if write else ""} with output as {output}\nrandomizaion is {"on" if randomize else "off"}\n\n\n'
     )
     return None if write else out
 
 
+def run(
+    filename: str,
+    gate: bool = False,
+    ascii: bool = True,
+    debug: bool = False,
+    check: str = '',
+    out: bool = True):
+  """NOTE: this function is just a replacement of decompile function, the function will no longer accessible with run() anymore after update 0.3.0, please change all use of this function to "decompile()" before that for any unexpected error of function not exist
+  
+  To run this filename is the only thing needed, Error will be raised and nothing will return if something went wrong. It will return the wrong bits if check, gate and ascii is on, decrypted result if ascii is on, or 0 otherwise.
+
+  
+  Arguments, type of input, usecases:
+      filename: string, specify which file needed to run
+      gate: boolean(True or False), if the result shows gate result or not
+      ascii: boolean, if the result converts to ascii and show or not
+      debug: boolean, show the unhuman log during the interpute
+      check: string, if it is specified then the result will be colored. It compares the difference between the gate result and the binary of check input, only works if both gate and ascii is True 
+             (color: green=correct bit
+                     red=incorrect bit
+                     blue box=missing bit 1
+                     purple box=missing bit 0)
+      out: boolean, it is seldom called as the silent argument, enable it for outputs, will not change return value
+                     """
+
+  print("WARNING: this function is called with the old function name 'run', please change it to 'decrypt' before update 0.3.0 when function 'run' will no longer work\n\n\n\n")
+  return decompile(filename=filename,
+                   gate=gate,
+                   ascii=ascii,
+                   debug=debug,
+                   check=check,
+                   out=out)
+
 if __name__ == '__main__':
   exit(run((str(argv[1]) if len(argv) != 1 else 'main.lgeso')))
```

### Comparing `logicgate-0.2.6/LogicGate/lgEncrypt.py` & `logicgate-0.2.7/LogicGate/lgEncrypt.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,33 +102,33 @@
       dk = open('__decrypt2__.lgeso', 'w')
       Fdt = f.read()
       Kdt = k.read()
       df.write(Fdt)
       dk.write(Kdt)
       df.close()
       dk.close()
-      out = lg.run('__decrypt__.lgeso',
+      out = lg.decompile('__decrypt__.lgeso',
                    ascii=True,
                    gate=True,
-                   check=lg.run('__decrypt2__.lgeso', ascii=True, out=False),
+                   check=lg.decompile('__decrypt2__.lgeso', ascii=True, out=False),
                    out=False).split('-')
       do = open('__decrypt__.lgeso', 'w')
       out = ''.join(out)
       outP = []
       for O in range(0, len(out), 7):
         outP.append(out[O:O + 7])
       for n in outP:
         do.write("\n".join(n))
         do.write("\n---\n")
       print('\n\n\n')
       do.close()
-      uh = lg.run('__decrypt__.lgeso', gate=True, out=not sause)
+      out = lg.decompile('__decrypt__.lgeso', gate=True, out=not sause)
       remove('__decrypt__.lgeso')
       remove('__decrypt2__.lgeso')
-      return uh
+      return out
   else:
     print("filename or key_file doesn't exist, exiting")
 
 
 if __name__ == '__main__':
   f = 'encFile'
   k = 'encKey'
```

### Comparing `logicgate-0.2.6/README.rst` & `logicgate-0.2.7/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 LogicGate
 =========
 
-This language is inspired by logic gates, by using simple alphabet you
-could make a program.
+This language is inspired by logic gates, by using simple alphabet you could make a program.
 
 It is designed as a way for manual encryption, which kinda failed
 
 All you can do in this language is to make a program with logic gates,
 sounds difficult and indeed it is.
 
 Startup
 -------
 
-First, make a logic gate file. The file extension should be lgeso
+First, make a logic gate file. The file extension should be .lgeso
 
 Runner
 ------
 
-To use it, import the python file **LogicGate.py** in your python
-script, or just run the LogicGate.py.
-Remember for the run function, only
-the filename argument is needed. The run function will return an exit
-code if you use the run function, and outputs of the file will be
-printed(binary to ascii, and logical binary if enabled). The compile
-function does the otherwise, it doesn’t return anything but it can write
-code into lgeso file.
+To use it, import **LogicGate** in your python script.
+
+Remember for the decompile function, only the filename argument is needed.
+
+The decompile function will return the incorrect bits if check, gate and ascii is True, decompiled result if ascii is True, and 0 if otherwise.
+
+Outputs of the file will be printed(binary to ascii, and logical binary if enabled) if out is True (true by defalt).
+
+
+The compile function does the otherwise, it normally doesn't return anything but it can write code into lgeso file, or if write is False(defalt on) then the compiled result will be returned instead of writing into file.
 
 Special encrypt module
 ----------------------
-a special encrypt module is included in this package, which is lgEncrypt.py. 
+a special encrypt module is included in this package, which is **lgEncrypt**.
+
 it contain two functions, encrypt() and decrypt().
-encrypt() generates a key file and a data file, they are pure random string when transfered to ascii, but shows message when both being processed by decrypt()
-encrypth) have 3 arguments, data file name, key file name, message
-They are very self explainatory
 
-decrypt() have 3 arguments, data file, key file, sause
+encrypt() generates a key file and a data file, they are pure random string when transfered to ascii, but shows message when both being processed by decrypt(). 
+encrypt() have 3 arguments, data file name, key file name, message. They are very self explainatory
+
+decrypt() have 3 arguments, data file, key file, sause. 
 the first 2 is very self explainatory, for sause parameter it determinates if the output text is shown or returned for further decryption, assuming the message through encrypt() is encrypted beforehand
 
 syntax
 ------
 
 For syntax it is very straight forward. It process each character in
-each line as each command For gates with multiple inputs (such as or,
-and) type like other syntax, the quota for the gate will automatically
-be processed. No linking between words, unless the syntax at the middle
-is invalid
+every line as individual command.
+
+For gates with multiple inputs (such as or,
+and) type like other syntax, the quota for the gate will automatically be processed. Any invalid command will raise SyntaxError, in almost all scenarios, the case of the gate does not matter.
 
-Basic gates(gates that doesn’t require includes):
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Basic gates(gates that doesn’t require includes, include feature is in progress):
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 A (and gate): the next **2** results will be accepted as inputs. If both
 inputs are 1, output is 1, else 0
 
 O (or gate): the next **2** results will be accepted as inputs. If one
 of the inputs are 1, output is 1, else 0
 
@@ -62,23 +64,19 @@
 are the results, self explanatory
 
 special syntax
 ~~~~~~~~~~~~~~
 
 There are 2 special syntax
 
-—-- (three hyphens): new word, used for the ascii output separating the
-binary for ascii translation
+—-- (three hyphens): new word, used for the ascii output separating the binary for ascii translation. Everything else on the line with this syntax will be ignored.
 
 ### (three hashes): comment everything after the syntax
 
-For any of the special syntax, they are not being interpreted as special
-syntax unless the entire syntax appears. They can be anywhere in a line,
-and that line will act like what the syntax shows (if the special syntax
-appears in the same line, they will be scanned and processed according
+For any of the special syntax, they are not being interpreted as special syntax unless the entire syntax appears. They can be anywhere in a line, and that line will act like what the syntax shows (if more tham one special syntax appears in the same line, they will be scanned and processed according
 to here)
 
 examples
 ========
 
 This is a hello world in LogicGate
 
@@ -89,12 +87,12 @@
 
 Sources
 -------
 
 `gitbub
 <https://github.com/TaokyleYT/LogicGate/>`__\
 
-Esolang wiki:
+Esolang seldom outdated wiki:
 `LogicGate <https://esolangs.org/wiki/LogicGate>`__\
 
 Replit up-to-date version:
 `replit <https://replit.com/@s3D27ZHOU/LogicGate>`__
```

### Comparing `logicgate-0.2.6/pyproject.toml` & `logicgate-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LogicGate"
-version = "0.2.6"
+version = "0.2.7"
 description = "an esolang designed for manual encryption with logic gates"
 license = "MIT"
 authors = ["Taokyle <taokyle415@gmail.com>"]
 readme = "README.rst"
 repository = "https://replit.com/@s3D27ZHOU/LogicGate"
 keywords = ["logic", "gate", "encrypt", "encryption"]
 packages = [
```

### Comparing `logicgate-0.2.6/setup.py` & `logicgate-0.2.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 package_dir = \
 {'': 'LogicGate'}
 
 modules = \
 ['LogicGate', 'lgEncrypt']
 setup_kwargs = {
     'name': 'logicgate',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': 'an esolang designed for manual encryption with logic gates',
-    'long_description': 'LogicGate\n=========\n\nThis language is inspired by logic gates, by using simple alphabet you\ncould make a program.\n\nIt is designed as a way for manual encryption, which kinda failed\n\nAll you can do in this language is to make a program with logic gates,\nsounds difficult and indeed it is.\n\nStartup\n-------\n\nFirst, make a logic gate file. The file extension should be lgeso\n\nRunner\n------\n\nTo use it, import the python file **LogicGate.py** in your python\nscript, or just run the LogicGate.py.\nRemember for the run function, only\nthe filename argument is needed. The run function will return an exit\ncode if you use the run function, and outputs of the file will be\nprinted(binary to ascii, and logical binary if enabled). The compile\nfunction does the otherwise, it doesn’t return anything but it can write\ncode into lgeso file.\n\nSpecial encrypt module\n----------------------\na special encrypt module is included in this package, which is lgEncrypt.py. \nit contain two functions, encrypt() and decrypt().\nencrypt() generates a key file and a data file, they are pure random string when transfered to ascii, but shows message when both being processed by decrypt()\nencrypth) have 3 arguments, data file name, key file name, message\nThey are very self explainatory\n\ndecrypt() have 3 arguments, data file, key file, sause\nthe first 2 is very self explainatory, for sause parameter it determinates if the output text is shown or returned for further decryption, assuming the message through encrypt() is encrypted beforehand\n\nsyntax\n------\n\nFor syntax it is very straight forward. It process each character in\neach line as each command For gates with multiple inputs (such as or,\nand) type like other syntax, the quota for the gate will automatically\nbe processed. No linking between words, unless the syntax at the middle\nis invalid\n\nBasic gates(gates that doesn’t require includes):\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nA (and gate): the next **2** results will be accepted as inputs. If both\ninputs are 1, output is 1, else 0\n\nO (or gate): the next **2** results will be accepted as inputs. If one\nof the inputs are 1, output is 1, else 0\n\nN (not gate): the next **1** result will be accepted as inputs. If the\ninput is 1, output is 0, else 0\n\n1 and 0 (True and False): **NO** result will be accepted as inputs. They\nare the results, self explanatory\n\nspecial syntax\n~~~~~~~~~~~~~~\n\nThere are 2 special syntax\n\n—-- (three hyphens): new word, used for the ascii output separating the\nbinary for ascii translation\n\n### (three hashes): comment everything after the syntax\n\nFor any of the special syntax, they are not being interpreted as special\nsyntax unless the entire syntax appears. They can be anywhere in a line,\nand that line will act like what the syntax shows (if the special syntax\nappears in the same line, they will be scanned and processed according\nto here)\n\nexamples\n========\n\nThis is a hello world in LogicGate\n\n``1\\n 0\\n 0\\n 1\\n 0\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 0\\n ---\\n 1\\n 0\\n 1\\n 0\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 0\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 1\\n``\n\nanother version generated by LogicGate.compile():\n``O1NNAANNNNA1AA1AO0AA1AO1NNANNAA1A1111111111\\n NNANNAAAO0O000001\\n OO0NNN10\\n O1O1NNA1O01\\n NNOONNA0O0000\\n 0\\n AA0NNANNOONNNNAO0A1O0000001\\n ---\\n OO1O1OAO1NNAO111111\\n NNNNO0NNAA1O0N01\\n OANNOA0O00000\\n ANNNNA001\\n NNA11\\n NNANNA1ANNO0001\\n NNAANNAOOA1NNAO10110111\\n ---\\n OA111\\n A1OA1OO0A1O1NNA1O0ONNNNNNN0000\\n A1O0A00\\n A1O0NNAO0O0A111\\n NNAO1NNONNNNA1O1111\\n O0A1OANNA0NNOO0ON10000\\n 0\\n ---\\n O0NNN0\\n A1ANNNNNNNNNNO101\\n O00\\n NNA1OO1ONNAO10110\\n OAA1110\\n OO0AAO0AAONNO0O0NNO00001100\\n NNO0A0ONNN10\\n ---\\n O0O1O0A1NNO1ANNO0AA1O1AA1A1A11111\\n NNANNO1ONNNNNNNNNNO0AO11101\\n O0OONNNNAAO0N11000\\n A1O0N0\\n OONNNNOA1ONNOO0AA11100100\\n NNO0ON00\\n O0OA1NNA1O100\\n ---\\n O0OO1OO1A1O1000\\n NNOO0AONNONNO0A0NNA0NNA010010\\n NNAA0OOOA0O000001\\n A0NNNNN1\\n AO0NNNNA1OO0001\\n O0OA1O0O0OO0OA1O00000\\n ---\\n 1\\n A0NNAO0A0OA0NNA1A0000\\n NNO0NNA1NNOO011\\n NNO0NNA0A0A0NNOO000\\n ANNA1AA1NNNNNNNNAA1NNAA1A111111\\n NNA1ANNA1OAO1O11111\\n A1A1NNA1O1NNANNA1AA1111\\n ---\\n ONNNNAOO11110\\n OANNOONNA1AA1110111\\n AA0NNNNNNO0O0A0O0N10\\n NNNNNNOA110\\n O1OONNA1101\\n A1NNNNA11\\n ANNOONNAAO1A1ANNA11111011\\n ---\\n O0NNO0AO0A111\\n NNNNNNA1O0ONNA1NNNNO0NNANNOOA1ANNNNAA11110111\\n NNO11\\n AO0AN101\\n OAA1000\\n 1\\n O0A0NNO0O0NNA0A0NNA1ON10\\n ---\\n O0N0\\n NNNNNNO0ONNA1N00\\n O00\\n O0AN01\\n NNONNNNNNNNA111\\n NNNNONNOO0000\\n AONNO0ANNO00101\\n ---\\n O1ONNANNNNA1111\\n NNNNOOOO0NNAA1NNONNO1011111\\n NNA0A0A01\\n AA1N10\\n O1OANNNNNNA1ONNNNOO1AOOO1AAN0110111110\\n 0\\n OOAO0NNO0A0OAANNA0AONNO0001100000\\n ---\\n A1A1NNO0NNA11\\n OA100\\n NNANNOA1001\\n 0\\n NNO0OA0O000\\n ANNO0OONNA1O11001\\n ---``\n\nSources\n-------\n\n`gitbub\n<https://github.com/TaokyleYT/LogicGate/>`__\\\n\nEsolang wiki:\n`LogicGate <https://esolangs.org/wiki/LogicGate>`__\\\n\nReplit up-to-date version:\n`replit <https://replit.com/@s3D27ZHOU/LogicGate>`__\n',
+    'long_description': "LogicGate\n=========\n\nThis language is inspired by logic gates, by using simple alphabet you could make a program.\n\nIt is designed as a way for manual encryption, which kinda failed\n\nAll you can do in this language is to make a program with logic gates,\nsounds difficult and indeed it is.\n\nStartup\n-------\n\nFirst, make a logic gate file. The file extension should be .lgeso\n\nRunner\n------\n\nTo use it, import **LogicGate** in your python script.\n\nRemember for the decompile function, only the filename argument is needed.\n\nThe decompile function will return the incorrect bits if check, gate and ascii is True, decompiled result if ascii is True, and 0 if otherwise.\n\nOutputs of the file will be printed(binary to ascii, and logical binary if enabled) if out is True (true by defalt).\n\n\nThe compile function does the otherwise, it normally doesn't return anything but it can write code into lgeso file, or if write is False(defalt on) then the compiled result will be returned instead of writing into file.\n\nSpecial encrypt module\n----------------------\na special encrypt module is included in this package, which is **lgEncrypt**.\n\nit contain two functions, encrypt() and decrypt().\n\nencrypt() generates a key file and a data file, they are pure random string when transfered to ascii, but shows message when both being processed by decrypt(). \nencrypt() have 3 arguments, data file name, key file name, message. They are very self explainatory\n\ndecrypt() have 3 arguments, data file, key file, sause. \nthe first 2 is very self explainatory, for sause parameter it determinates if the output text is shown or returned for further decryption, assuming the message through encrypt() is encrypted beforehand\n\nsyntax\n------\n\nFor syntax it is very straight forward. It process each character in\nevery line as individual command.\n\nFor gates with multiple inputs (such as or,\nand) type like other syntax, the quota for the gate will automatically be processed. Any invalid command will raise SyntaxError, in almost all scenarios, the case of the gate does not matter.\n\nBasic gates(gates that doesn’t require includes, include feature is in progress):\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nA (and gate): the next **2** results will be accepted as inputs. If both\ninputs are 1, output is 1, else 0\n\nO (or gate): the next **2** results will be accepted as inputs. If one\nof the inputs are 1, output is 1, else 0\n\nN (not gate): the next **1** result will be accepted as inputs. If the\ninput is 1, output is 0, else 0\n\n1 and 0 (True and False): **NO** result will be accepted as inputs. They\nare the results, self explanatory\n\nspecial syntax\n~~~~~~~~~~~~~~\n\nThere are 2 special syntax\n\n—-- (three hyphens): new word, used for the ascii output separating the binary for ascii translation. Everything else on the line with this syntax will be ignored.\n\n### (three hashes): comment everything after the syntax\n\nFor any of the special syntax, they are not being interpreted as special syntax unless the entire syntax appears. They can be anywhere in a line, and that line will act like what the syntax shows (if more tham one special syntax appears in the same line, they will be scanned and processed according\nto here)\n\nexamples\n========\n\nThis is a hello world in LogicGate\n\n``1\\n 0\\n 0\\n 1\\n 0\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 0\\n ---\\n 1\\n 0\\n 1\\n 0\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 0\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 1\\n``\n\nanother version generated by LogicGate.compile():\n``O1NNAANNNNA1AA1AO0AA1AO1NNANNAA1A1111111111\\n NNANNAAAO0O000001\\n OO0NNN10\\n O1O1NNA1O01\\n NNOONNA0O0000\\n 0\\n AA0NNANNOONNNNAO0A1O0000001\\n ---\\n OO1O1OAO1NNAO111111\\n NNNNO0NNAA1O0N01\\n OANNOA0O00000\\n ANNNNA001\\n NNA11\\n NNANNA1ANNO0001\\n NNAANNAOOA1NNAO10110111\\n ---\\n OA111\\n A1OA1OO0A1O1NNA1O0ONNNNNNN0000\\n A1O0A00\\n A1O0NNAO0O0A111\\n NNAO1NNONNNNA1O1111\\n O0A1OANNA0NNOO0ON10000\\n 0\\n ---\\n O0NNN0\\n A1ANNNNNNNNNNO101\\n O00\\n NNA1OO1ONNAO10110\\n OAA1110\\n OO0AAO0AAONNO0O0NNO00001100\\n NNO0A0ONNN10\\n ---\\n O0O1O0A1NNO1ANNO0AA1O1AA1A1A11111\\n NNANNO1ONNNNNNNNNNO0AO11101\\n O0OONNNNAAO0N11000\\n A1O0N0\\n OONNNNOA1ONNOO0AA11100100\\n NNO0ON00\\n O0OA1NNA1O100\\n ---\\n O0OO1OO1A1O1000\\n NNOO0AONNONNO0A0NNA0NNA010010\\n NNAA0OOOA0O000001\\n A0NNNNN1\\n AO0NNNNA1OO0001\\n O0OA1O0O0OO0OA1O00000\\n ---\\n 1\\n A0NNAO0A0OA0NNA1A0000\\n NNO0NNA1NNOO011\\n NNO0NNA0A0A0NNOO000\\n ANNA1AA1NNNNNNNNAA1NNAA1A111111\\n NNA1ANNA1OAO1O11111\\n A1A1NNA1O1NNANNA1AA1111\\n ---\\n ONNNNAOO11110\\n OANNOONNA1AA1110111\\n AA0NNNNNNO0O0A0O0N10\\n NNNNNNOA110\\n O1OONNA1101\\n A1NNNNA11\\n ANNOONNAAO1A1ANNA11111011\\n ---\\n O0NNO0AO0A111\\n NNNNNNA1O0ONNA1NNNNO0NNANNOOA1ANNNNAA11110111\\n NNO11\\n AO0AN101\\n OAA1000\\n 1\\n O0A0NNO0O0NNA0A0NNA1ON10\\n ---\\n O0N0\\n NNNNNNO0ONNA1N00\\n O00\\n O0AN01\\n NNONNNNNNNNA111\\n NNNNONNOO0000\\n AONNO0ANNO00101\\n ---\\n O1ONNANNNNA1111\\n NNNNOOOO0NNAA1NNONNO1011111\\n NNA0A0A01\\n AA1N10\\n O1OANNNNNNA1ONNNNOO1AOOO1AAN0110111110\\n 0\\n OOAO0NNO0A0OAANNA0AONNO0001100000\\n ---\\n A1A1NNO0NNA11\\n OA100\\n NNANNOA1001\\n 0\\n NNO0OA0O000\\n ANNO0OONNA1O11001\\n ---``\n\nSources\n-------\n\n`gitbub\n<https://github.com/TaokyleYT/LogicGate/>`__\\\n\nEsolang seldom outdated wiki:\n`LogicGate <https://esolangs.org/wiki/LogicGate>`__\\\n\nReplit up-to-date version:\n`replit <https://replit.com/@s3D27ZHOU/LogicGate>`__\n",
     'author': 'Taokyle',
     'author_email': 'taokyle415@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://replit.com/@s3D27ZHOU/LogicGate',
     'package_dir': package_dir,
     'py_modules': modules,
```

### Comparing `logicgate-0.2.6/PKG-INFO` & `logicgate-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logicgate
-Version: 0.2.6
+Version: 0.2.7
 Summary: an esolang designed for manual encryption with logic gates
 Home-page: https://replit.com/@s3D27ZHOU/LogicGate
 License: MIT
 Keywords: logic,gate,encrypt,encryption
 Author: Taokyle
 Author-email: taokyle415@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -17,61 +17,63 @@
 Project-URL: github, https://github.com/TaokyleYT/LogicGate
 Project-URL: up-to-date source code(replit), https://replit.com/@s3D27ZHOU/LogicGate
 Description-Content-Type: text/x-rst
 
 LogicGate
 =========
 
-This language is inspired by logic gates, by using simple alphabet you
-could make a program.
+This language is inspired by logic gates, by using simple alphabet you could make a program.
 
 It is designed as a way for manual encryption, which kinda failed
 
 All you can do in this language is to make a program with logic gates,
 sounds difficult and indeed it is.
 
 Startup
 -------
 
-First, make a logic gate file. The file extension should be lgeso
+First, make a logic gate file. The file extension should be .lgeso
 
 Runner
 ------
 
-To use it, import the python file **LogicGate.py** in your python
-script, or just run the LogicGate.py.
-Remember for the run function, only
-the filename argument is needed. The run function will return an exit
-code if you use the run function, and outputs of the file will be
-printed(binary to ascii, and logical binary if enabled). The compile
-function does the otherwise, it doesn’t return anything but it can write
-code into lgeso file.
+To use it, import **LogicGate** in your python script.
+
+Remember for the decompile function, only the filename argument is needed.
+
+The decompile function will return the incorrect bits if check, gate and ascii is True, decompiled result if ascii is True, and 0 if otherwise.
+
+Outputs of the file will be printed(binary to ascii, and logical binary if enabled) if out is True (true by defalt).
+
+
+The compile function does the otherwise, it normally doesn't return anything but it can write code into lgeso file, or if write is False(defalt on) then the compiled result will be returned instead of writing into file.
 
 Special encrypt module
 ----------------------
-a special encrypt module is included in this package, which is lgEncrypt.py. 
+a special encrypt module is included in this package, which is **lgEncrypt**.
+
 it contain two functions, encrypt() and decrypt().
-encrypt() generates a key file and a data file, they are pure random string when transfered to ascii, but shows message when both being processed by decrypt()
-encrypth) have 3 arguments, data file name, key file name, message
-They are very self explainatory
 
-decrypt() have 3 arguments, data file, key file, sause
+encrypt() generates a key file and a data file, they are pure random string when transfered to ascii, but shows message when both being processed by decrypt(). 
+encrypt() have 3 arguments, data file name, key file name, message. They are very self explainatory
+
+decrypt() have 3 arguments, data file, key file, sause. 
 the first 2 is very self explainatory, for sause parameter it determinates if the output text is shown or returned for further decryption, assuming the message through encrypt() is encrypted beforehand
 
 syntax
 ------
 
 For syntax it is very straight forward. It process each character in
-each line as each command For gates with multiple inputs (such as or,
-and) type like other syntax, the quota for the gate will automatically
-be processed. No linking between words, unless the syntax at the middle
-is invalid
+every line as individual command.
+
+For gates with multiple inputs (such as or,
+and) type like other syntax, the quota for the gate will automatically be processed. Any invalid command will raise SyntaxError, in almost all scenarios, the case of the gate does not matter.
 
-Basic gates(gates that doesn’t require includes):
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Basic gates(gates that doesn’t require includes, include feature is in progress):
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 A (and gate): the next **2** results will be accepted as inputs. If both
 inputs are 1, output is 1, else 0
 
 O (or gate): the next **2** results will be accepted as inputs. If one
 of the inputs are 1, output is 1, else 0
 
@@ -82,23 +84,19 @@
 are the results, self explanatory
 
 special syntax
 ~~~~~~~~~~~~~~
 
 There are 2 special syntax
 
-—-- (three hyphens): new word, used for the ascii output separating the
-binary for ascii translation
+—-- (three hyphens): new word, used for the ascii output separating the binary for ascii translation. Everything else on the line with this syntax will be ignored.
 
 ### (three hashes): comment everything after the syntax
 
-For any of the special syntax, they are not being interpreted as special
-syntax unless the entire syntax appears. They can be anywhere in a line,
-and that line will act like what the syntax shows (if the special syntax
-appears in the same line, they will be scanned and processed according
+For any of the special syntax, they are not being interpreted as special syntax unless the entire syntax appears. They can be anywhere in a line, and that line will act like what the syntax shows (if more tham one special syntax appears in the same line, they will be scanned and processed according
 to here)
 
 examples
 ========
 
 This is a hello world in LogicGate
 
@@ -109,13 +107,13 @@
 
 Sources
 -------
 
 `gitbub
 <https://github.com/TaokyleYT/LogicGate/>`__\
 
-Esolang wiki:
+Esolang seldom outdated wiki:
 `LogicGate <https://esolangs.org/wiki/LogicGate>`__\
 
 Replit up-to-date version:
 `replit <https://replit.com/@s3D27ZHOU/LogicGate>`__
```

