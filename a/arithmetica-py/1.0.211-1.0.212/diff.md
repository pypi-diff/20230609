# Comparing `tmp/arithmetica-py-1.0.211.tar.gz` & `tmp/arithmetica-py-1.0.212.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetica-py-1.0.211.tar", last modified: Fri Jun  9 07:42:25 2023, max compression
+gzip compressed data, was "arithmetica-py-1.0.212.tar", last modified: Fri Jun  9 08:33:40 2023, max compression
```

## Comparing `arithmetica-py-1.0.211.tar` & `arithmetica-py-1.0.212.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:42:25.088927 arithmetica-py-1.0.211/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-09 07:41:59.000000 arithmetica-py-1.0.211/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-09 07:42:25.088927 arithmetica-py-1.0.211/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-09 07:41:59.000000 arithmetica-py-1.0.211/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:42:25.088927 arithmetica-py-1.0.211/arithmetica_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-09 07:42:24.000000 arithmetica-py-1.0.211/arithmetica_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-09 07:42:25.000000 arithmetica-py-1.0.211/arithmetica_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 07:42:24.000000 arithmetica-py-1.0.211/arithmetica_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 07:42:24.000000 arithmetica-py-1.0.211/arithmetica_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 07:42:25.088927 arithmetica-py-1.0.211/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-09 07:41:59.000000 arithmetica-py-1.0.211/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:42:25.084927 arithmetica-py-1.0.211/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:42:25.088927 arithmetica-py-1.0.211/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)   186606 2023-06-09 07:42:24.000000 arithmetica-py-1.0.211/src/python-module/libarithmetica.a
--rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-06-09 07:42:24.000000 arithmetica-py-1.0.211/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-09 07:41:59.000000 arithmetica-py-1.0.211/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 07:42:24.000000 arithmetica-py-1.0.211/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:33:40.709133 arithmetica-py-1.0.212/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-09 08:33:20.000000 arithmetica-py-1.0.212/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-09 08:33:40.709133 arithmetica-py-1.0.212/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-09 08:33:20.000000 arithmetica-py-1.0.212/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:33:40.705133 arithmetica-py-1.0.212/arithmetica_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-09 08:33:40.000000 arithmetica-py-1.0.212/arithmetica_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-09 08:33:40.000000 arithmetica-py-1.0.212/arithmetica_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:33:40.000000 arithmetica-py-1.0.212/arithmetica_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 08:33:40.000000 arithmetica-py-1.0.212/arithmetica_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:33:40.709133 arithmetica-py-1.0.212/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-09 08:33:20.000000 arithmetica-py-1.0.212/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:33:40.705133 arithmetica-py-1.0.212/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:33:40.709133 arithmetica-py-1.0.212/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)   187086 2023-06-09 08:33:40.000000 arithmetica-py-1.0.212/src/python-module/libarithmetica.a
+-rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-06-09 08:33:40.000000 arithmetica-py-1.0.212/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-09 08:33:20.000000 arithmetica-py-1.0.212/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 08:33:40.000000 arithmetica-py-1.0.212/src/python-module/version.txt
```

### Comparing `arithmetica-py-1.0.211/LICENSE` & `arithmetica-py-1.0.212/LICENSE`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.211/README.md` & `arithmetica-py-1.0.212/README.md`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.211/setup.py` & `arithmetica-py-1.0.212/setup.py`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.211/src/python-module/libarithmetica.a` & `arithmetica-py-1.0.212/src/python-module/libarithmetica.a`

 * *Files 1% similar despite different names*

#### file list

```diff
@@ -5,15 +5,15 @@
 ?rw-r--r--   0        0        0     4056 1970-01-01 00:00:00.000000 arcsin.c.o
 ?rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 arctan.c.o
 ?rw-r--r--   0        0        0     1768 1970-01-01 00:00:00.000000 check_accuracy.c.o
 ?rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 continued_fraction_to_fraction.c.o
 ?rw-r--r--   0        0        0     3968 1970-01-01 00:00:00.000000 cosine.c.o
 ?rw-r--r--   0        0        0     3896 1970-01-01 00:00:00.000000 exponential.c.o
 ?rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 factorial.c.o
-?rw-r--r--   0        0        0    12688 1970-01-01 00:00:00.000000 find_roots_of_polynomial.c.o
+?rw-r--r--   0        0        0    13168 1970-01-01 00:00:00.000000 find_roots_of_polynomial.c.o
 ?rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 fraction_to_continued_fraction.c.o
 ?rw-r--r--   0        0        0     2616 1970-01-01 00:00:00.000000 igcd.c.o
 ?rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 ilcm.c.o
 ?rw-r--r--   0        0        0     2632 1970-01-01 00:00:00.000000 natural_logarithm.c.o
 ?rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 power.c.o
 ?rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 power_integer.c.o
 ?rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 repeating_decimal_to_fraction.c.o
```

#### find_roots_of_polynomial.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          11792 (bytes into file)
+  Start of section headers:          12272 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         14
   Section header string table index: 13
```

##### readelf --wide --sections {}

```diff
@@ -1,23 +1,23 @@
-There are 14 section headers, starting at offset 0x2e10:
+There are 14 section headers, starting at offset 0x2ff0:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .text             PROGBITS        0000000000000000 000040 001318 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 001a88 0012a8 18   I 11   1  8
-  [ 3] .data             PROGBITS        0000000000000000 001358 000000 00  WA  0   0  1
-  [ 4] .bss              NOBITS          0000000000000000 001358 000000 00  WA  0   0  1
-  [ 5] .rodata.str1.1    PROGBITS        0000000000000000 001358 000008 01 AMS  0   0  1
-  [ 6] .comment          PROGBITS        0000000000000000 001360 00002c 01  MS  0   0  1
-  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 00138c 000000 00      0   0  1
-  [ 8] .note.gnu.property NOTE            0000000000000000 001390 000020 00   A  0   0  8
-  [ 9] .eh_frame         PROGBITS        0000000000000000 0013b0 000150 00   A  0   0  8
-  [10] .rela.eh_frame    RELA            0000000000000000 002d30 000060 18   I 11   9  8
-  [11] .symtab           SYMTAB          0000000000000000 001500 000378 18     12   5  8
-  [12] .strtab           STRTAB          0000000000000000 001878 00020e 00      0   0  1
-  [13] .shstrtab         STRTAB          0000000000000000 002d90 00007b 00      0   0  1
+  [ 1] .text             PROGBITS        0000000000000000 000040 0013db 00  AX  0   0 16
+  [ 2] .rela.text        RELA            0000000000000000 001b48 0013c8 18   I 11   1  8
+  [ 3] .data             PROGBITS        0000000000000000 00141b 000000 00  WA  0   0  1
+  [ 4] .bss              NOBITS          0000000000000000 00141b 000000 00  WA  0   0  1
+  [ 5] .rodata.str1.1    PROGBITS        0000000000000000 00141b 000008 01 AMS  0   0  1
+  [ 6] .comment          PROGBITS        0000000000000000 001423 00002c 01  MS  0   0  1
+  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 00144f 000000 00      0   0  1
+  [ 8] .note.gnu.property NOTE            0000000000000000 001450 000020 00   A  0   0  8
+  [ 9] .eh_frame         PROGBITS        0000000000000000 001470 000150 00   A  0   0  8
+  [10] .rela.eh_frame    RELA            0000000000000000 002f10 000060 18   I 11   9  8
+  [11] .symtab           SYMTAB          0000000000000000 0015c0 000378 18     12   5  8
+  [12] .strtab           STRTAB          0000000000000000 001938 00020e 00      0   0  1
+  [13] .shstrtab         STRTAB          0000000000000000 002f70 00007b 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -17,21 +17,21 @@
     13: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
     14: 0000000000000180   333 FUNC    GLOBAL DEFAULT    1 find_roots_of_polynomial_substitute_fraction
     15: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND parse_fraction
     16: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND multiply_fraction
     17: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND add_fraction
     18: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND delete_fraction
     19: 00000000000002d0   314 FUNC    GLOBAL DEFAULT    1 find_roots_of_polynomial_divide_polynomial
-    20: 0000000000000410  3848 FUNC    GLOBAL DEFAULT    1 find_roots_of_polynomial
+    20: 0000000000000410  4043 FUNC    GLOBAL DEFAULT    1 find_roots_of_polynomial
     21: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND stpcpy
     22: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strchr
     23: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND divide
     24: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND increment_whole
-    25: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strcmp
-    26: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND subtract
+    25: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND subtract
+    26: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strcmp
     27: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND terminating_decimal_to_fraction
     28: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND fraction_to_continued_fraction
     29: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND continued_fraction_to_fraction
     30: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND abs_mod
     31: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND equal_fraction
     32: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memset
     33: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND remove_zeroes
```

##### readelf --wide --relocs {}

```diff
@@ -1,9 +1,9 @@
 
-Relocation section '.rela.text' at offset 0x1a88 contains 199 entries:
+Relocation section '.rela.text' at offset 0x1b48 contains 211 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000036  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 0000000000000044  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 000000000000004f  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 000000000000005b  0000000800000004 R_X86_64_PLT32         0000000000000000 malloc - 4
 0000000000000071  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
 000000000000007d  0000000a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
@@ -96,114 +96,126 @@
 0000000000000862  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 00000000000008b5  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 00000000000008c0  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 00000000000008cf  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 00000000000008e0  0000000b00000004 R_X86_64_PLT32         0000000000000000 multiply - 4
 00000000000008ec  0000001800000004 R_X86_64_PLT32         0000000000000000 increment_whole - 4
 0000000000000907  0000000800000004 R_X86_64_PLT32         0000000000000000 malloc - 4
-0000000000000975  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000987  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000009ba  0000001900000004 R_X86_64_PLT32         0000000000000000 strcmp - 4
-00000000000009d4  0000000500000004 R_X86_64_PLT32         0000000000000000 find_roots_of_polynomial_substitute - 4
-00000000000009e9  0000000500000004 R_X86_64_PLT32         0000000000000000 find_roots_of_polynomial_substitute - 4
-00000000000009f4  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000009ff  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000a18  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000a2e  0000001700000004 R_X86_64_PLT32         0000000000000000 divide - 4
-0000000000000a36  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000a41  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000a50  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000a66  0000001a00000004 R_X86_64_PLT32         0000000000000000 subtract - 4
-0000000000000a71  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000a79  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000a81  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000a89  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000aa5  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000ace  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000ae0  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000af8  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000b11  0000001b00000004 R_X86_64_PLT32         0000000000000000 terminating_decimal_to_fraction - 4
-0000000000000b24  0000001c00000004 R_X86_64_PLT32         0000000000000000 fraction_to_continued_fraction - 4
-0000000000000b79  0000001200000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000b81  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000ba0  0000000800000004 R_X86_64_PLT32         0000000000000000 malloc - 4
-0000000000000bb7  0000001d00000004 R_X86_64_PLT32         0000000000000000 continued_fraction_to_fraction - 4
-0000000000000bd0  0000001e00000004 R_X86_64_PLT32         0000000000000000 abs_mod - 4
-0000000000000be2  0000001e00000004 R_X86_64_PLT32         0000000000000000 abs_mod - 4
-0000000000000c0e  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000c16  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000c23  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000c2f  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000c4a  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000c56  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000c9c  0000001f00000004 R_X86_64_PLT32         0000000000000000 equal_fraction - 4
-0000000000000cc6  0000000e00000004 R_X86_64_PLT32         0000000000000180 find_roots_of_polynomial_substitute_fraction - 4
-0000000000000ce5  0000001f00000004 R_X86_64_PLT32         0000000000000000 equal_fraction - 4
-0000000000000cf5  0000001200000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000cfd  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000d34  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000d43  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000d5c  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000d72  0000001700000004 R_X86_64_PLT32         0000000000000000 divide - 4
-0000000000000d8a  0000001300000004 R_X86_64_PLT32         00000000000002d0 find_roots_of_polynomial_divide_polynomial - 4
-0000000000000d95  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000dc1  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000dd0  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000df9  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000e0e  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000e1b  0000002000000004 R_X86_64_PLT32         0000000000000000 memset - 4
-0000000000000e5c  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000e6c  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000e7b  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000e8c  0000000b00000004 R_X86_64_PLT32         0000000000000000 multiply - 4
-0000000000000e9d  0000001800000004 R_X86_64_PLT32         0000000000000000 increment_whole - 4
-0000000000000ee9  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000efb  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000f0a  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000f17  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000f24  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000f50  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000f65  0000001200000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000f9d  0000001200000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-0000000000000fab  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000fd9  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-000000000000100a  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-000000000000101e  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000001028  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000001032  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000001059  0000002100000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
-000000000000106b  0000002100000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
-000000000000107b  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000001085  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-00000000000010c8  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000010d7  0000002200000004 R_X86_64_PLT32         0000000000000000 realloc - 4
-00000000000010eb  0000002300000004 R_X86_64_PLT32         0000000000000000 memmove - 4
-0000000000001130  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000001139  0000000800000004 R_X86_64_PLT32         0000000000000000 malloc - 4
-0000000000001149  0000000a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
-0000000000001161  0000000800000004 R_X86_64_PLT32         0000000000000000 malloc - 4
-0000000000001180  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000001195  0000001200000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-00000000000011bc  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000011c8  0000000800000004 R_X86_64_PLT32         0000000000000000 malloc - 4
-00000000000011db  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-00000000000011e7  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000011f3  0000000800000004 R_X86_64_PLT32         0000000000000000 malloc - 4
-0000000000001206  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000120d  0000000800000004 R_X86_64_PLT32         0000000000000000 malloc - 4
-0000000000001223  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000001237  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000001285  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000001292  0000002000000004 R_X86_64_PLT32         0000000000000000 memset - 4
-00000000000012b8  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-00000000000012cc  0000002200000004 R_X86_64_PLT32         0000000000000000 realloc - 4
-00000000000012d7  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000012e7  0000002300000004 R_X86_64_PLT32         0000000000000000 memmove - 4
-00000000000012fd  0000002300000004 R_X86_64_PLT32         0000000000000000 memmove - 4
-0000000000001314  0000002400000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+0000000000000973  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000985  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+000000000000099f  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000009eb  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+00000000000009f3  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000a05  0000000500000004 R_X86_64_PLT32         0000000000000000 find_roots_of_polynomial_substitute - 4
+0000000000000a1a  0000000500000004 R_X86_64_PLT32         0000000000000000 find_roots_of_polynomial_substitute - 4
+0000000000000a25  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000a30  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000a46  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000a5c  0000001700000004 R_X86_64_PLT32         0000000000000000 divide - 4
+0000000000000a64  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000a71  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000a85  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000a98  0000001900000004 R_X86_64_PLT32         0000000000000000 subtract - 4
+0000000000000aa3  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000aab  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000ab3  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000abb  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000ad6  0000001a00000004 R_X86_64_PLT32         0000000000000000 strcmp - 4
+0000000000000ae6  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000af1  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000b00  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000b11  0000001900000004 R_X86_64_PLT32         0000000000000000 subtract - 4
+0000000000000b2b  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000b36  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000b45  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000b56  0000001900000004 R_X86_64_PLT32         0000000000000000 subtract - 4
+0000000000000b84  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000b8c  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000bab  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000bbd  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000bd5  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000bee  0000001b00000004 R_X86_64_PLT32         0000000000000000 terminating_decimal_to_fraction - 4
+0000000000000c01  0000001c00000004 R_X86_64_PLT32         0000000000000000 fraction_to_continued_fraction - 4
+0000000000000c59  0000001200000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000c61  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000c80  0000000800000004 R_X86_64_PLT32         0000000000000000 malloc - 4
+0000000000000c97  0000001d00000004 R_X86_64_PLT32         0000000000000000 continued_fraction_to_fraction - 4
+0000000000000cb0  0000001e00000004 R_X86_64_PLT32         0000000000000000 abs_mod - 4
+0000000000000cc2  0000001e00000004 R_X86_64_PLT32         0000000000000000 abs_mod - 4
+0000000000000cef  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000cf7  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000d04  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000d10  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000d2b  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000d37  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000d7c  0000001f00000004 R_X86_64_PLT32         0000000000000000 equal_fraction - 4
+0000000000000da6  0000000e00000004 R_X86_64_PLT32         0000000000000180 find_roots_of_polynomial_substitute_fraction - 4
+0000000000000dc5  0000001f00000004 R_X86_64_PLT32         0000000000000000 equal_fraction - 4
+0000000000000dd5  0000001200000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000ddd  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000e17  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000e26  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000e3c  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000e52  0000001700000004 R_X86_64_PLT32         0000000000000000 divide - 4
+0000000000000e6a  0000001300000004 R_X86_64_PLT32         00000000000002d0 find_roots_of_polynomial_divide_polynomial - 4
+0000000000000e75  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000e99  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000ea8  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000ed2  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000ee7  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000ef4  0000002000000004 R_X86_64_PLT32         0000000000000000 memset - 4
+0000000000000f34  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000f43  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000f52  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000f63  0000000b00000004 R_X86_64_PLT32         0000000000000000 multiply - 4
+0000000000000f74  0000001800000004 R_X86_64_PLT32         0000000000000000 increment_whole - 4
+0000000000000fc9  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000fdd  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000fea  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000ff7  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000001004  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000001038  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+000000000000104d  0000001200000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+000000000000107d  0000001200000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+000000000000108b  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+00000000000010b9  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+00000000000010ea  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+00000000000010fe  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000001108  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000001112  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000001138  0000002100000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
+0000000000001149  0000002100000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
+0000000000001159  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000001163  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+00000000000011a0  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000011af  0000002200000004 R_X86_64_PLT32         0000000000000000 realloc - 4
+00000000000011c3  0000002300000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+00000000000011f8  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000001201  0000000800000004 R_X86_64_PLT32         0000000000000000 malloc - 4
+0000000000001211  0000000a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
+0000000000001229  0000000800000004 R_X86_64_PLT32         0000000000000000 malloc - 4
+0000000000001243  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000001258  0000001200000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+000000000000127f  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+000000000000128b  0000000800000004 R_X86_64_PLT32         0000000000000000 malloc - 4
+000000000000129e  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000012aa  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000012b6  0000000800000004 R_X86_64_PLT32         0000000000000000 malloc - 4
+00000000000012c9  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000012d0  0000000800000004 R_X86_64_PLT32         0000000000000000 malloc - 4
+00000000000012e6  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000012fa  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000001341  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000001355  0000002000000004 R_X86_64_PLT32         0000000000000000 memset - 4
+000000000000137b  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
+000000000000138f  0000002200000004 R_X86_64_PLT32         0000000000000000 realloc - 4
+000000000000139a  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000013aa  0000002300000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+00000000000013c0  0000002300000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+00000000000013d7  0000002400000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
 
-Relocation section '.rela.eh_frame' at offset 0x2d30 contains 4 entries:
+Relocation section '.rela.eh_frame' at offset 0x2f10 contains 4 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
 000000000000006c  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 180
 00000000000000b8  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 2d0
 0000000000000104  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 410
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -126,15 +126,15 @@
   DW_CFA_def_cfa_offset: 16
   DW_CFA_advance_loc: 2 to 0000000000000409
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000fc 0000000000000050 00000100 FDE cie=00000000 pc=0000000000000410..0000000000001318
+000000fc 0000000000000050 00000100 FDE cie=00000000 pc=0000000000000410..00000000000013db
   DW_CFA_advance_loc: 6 to 0000000000000416
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
   DW_CFA_advance_loc: 2 to 0000000000000418
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_advance_loc: 5 to 000000000000041d
@@ -147,30 +147,30 @@
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_advance_loc: 1 to 0000000000000428
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_advance_loc: 15 to 0000000000000437
   DW_CFA_def_cfa_offset: 336
-  DW_CFA_advance_loc2: 3192 to 00000000000010af
+  DW_CFA_advance_loc2: 3406 to 0000000000001185
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 00000000000010b0
+  DW_CFA_advance_loc: 4 to 0000000000001189
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000010b1
+  DW_CFA_advance_loc: 1 to 000000000000118a
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000010b3
+  DW_CFA_advance_loc: 2 to 000000000000118c
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000010b5
+  DW_CFA_advance_loc: 2 to 000000000000118e
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000010b7
+  DW_CFA_advance_loc: 2 to 0000000000001190
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000010b9
+  DW_CFA_advance_loc: 2 to 0000000000001192
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 00000000000010c0
+  DW_CFA_advance_loc: 6 to 0000000000001198
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -349,43 +349,43 @@
 	push   %r12
 	lea    -0x2(%r13),%r12
 	push   %rbp
 	push   %rbx
 	lea    0x0(,%r13,8),%rbx
 	sub    $0x118,%rsp
 	mov    (%rdi),%rdi
-	mov    %rsi,0xa0(%rsp)
-	mov    %rdx,0x88(%rsp)
+	mov    %rsi,0x98(%rsp)
+	mov    %rdx,0x80(%rsp)
 	mov    %fs:0x28,%rax
 	mov    %rax,0x108(%rsp)
 	xor    %eax,%eax
 	call   462 <find_roots_of_polynomial+0x52>
  R_X86_64_PLT32	strlen-0x4
 	mov    -0x8(%r14,%rbx,1),%rdi
 	mov    %rax,%rbp
 	call   46f <find_roots_of_polynomial+0x5f>
  R_X86_64_PLT32	strlen-0x4
 	lea    0x0(%rip),%rdi        
  R_X86_64_PC32	.LC1-0x4
 	cmp    %rbp,%rax
 	cmovb  %rbp,%rax
 	lea    0x2(%rax,%rax,1),%rax
-	mov    %rax,0x30(%rsp)
+	mov    %rax,0x58(%rsp)
 	call   48c <find_roots_of_polynomial+0x7c>
  R_X86_64_PLT32	parse_fraction-0x4
 	mov    %rbx,%rdi
-	mov    %rax,0xa8(%rsp)
-	mov    %rdx,0xb0(%rsp)
+	mov    %rax,0xa0(%rsp)
+	mov    %rdx,0xa8(%rsp)
 	call   4a4 <find_roots_of_polynomial+0x94>
  R_X86_64_PLT32	malloc-0x4
 	lea    -0x1(%r13),%rcx
-	mov    %rax,0x90(%rsp)
-	mov    %rcx,0xd0(%rsp)
+	mov    %rax,0x88(%rsp)
+	mov    %rcx,0xc8(%rsp)
 	test   %r13,%r13
-	je     11b0 <find_roots_of_polynomial+0xda0>
+	je     1273 <find_roots_of_polynomial+0xe63>
 	xor    %ebp,%ebp
 	mov    %rax,%r15
 	cs nopw 0x0(%rax,%rax,1)
 	mov    $0x10,%edi
 	call   4da <find_roots_of_polynomial+0xca>
  R_X86_64_PLT32	malloc-0x4
 	mov    (%r14,%rbp,8),%rdi
@@ -398,19 +398,19 @@
 	movdqa (%rsp),%xmm0
 	movups %xmm0,(%rax)
 	mov    %rbp,%rax
 	lea    0x1(%rbp),%rbp
 	cmp    %rbp,%r13
 	jne    4d0 <find_roots_of_polynomial+0xc0>
 	mov    %rax,%r13
-	mov    0x90(%rsp),%rax
+	mov    0x88(%rsp),%rax
 	mov    (%rax),%r15
 	mov    (%r15),%rsi
 	mov    %rsi,%rdi
-	mov    %rsi,0x38(%rsp)
+	mov    %rsi,0x30(%rsp)
 	call   526 <find_roots_of_polynomial+0x116>
  R_X86_64_PLT32	strlen-0x4
 	lea    0x1(%rax),%rdx
 	mov    %rax,0x10(%rsp)
 	mov    %rdx,%rdi
 	mov    %rdx,0x28(%rsp)
 	call   53c <find_roots_of_polynomial+0x12c>
@@ -419,28 +419,28 @@
 	mov    %rax,(%rsp)
 	call   549 <find_roots_of_polynomial+0x139>
  R_X86_64_PLT32	strlen-0x4
 	lea    0x1(%rax),%rdi
 	call   552 <find_roots_of_polynomial+0x142>
  R_X86_64_PLT32	malloc-0x4
 	mov    0x28(%rsp),%rdx
-	mov    0x38(%rsp),%rsi
+	mov    0x30(%rsp),%rsi
 	mov    (%rsp),%rdi
 	mov    %rax,%rbp
 	call   568 <find_roots_of_polynomial+0x158>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x8(%r15),%rsi
 	mov    %rbp,%rdi
 	call   574 <find_roots_of_polynomial+0x164>
  R_X86_64_PLT32	stpcpy-0x4
 	mov    (%rsp),%rcx
 	cmpb   $0x2d,(%rcx)
-	je     12c1 <find_roots_of_polynomial+0xeb1>
+	je     1384 <find_roots_of_polynomial+0xf74>
 	movq   %rbp,%xmm2
-	mov    0x90(%rsp),%rbp
+	mov    0x88(%rsp),%rbp
 	xor    %r15d,%r15d
 	movhps (%rsp),%xmm2
 	movaps %xmm2,0x10(%rsp)
 	nopw   0x0(%rax,%rax,1)
 	mov    0x0(%rbp,%r15,8),%rax
 	mov    0x18(%rsp),%rcx
 	mov    0x10(%rsp),%rdx
@@ -459,58 +459,58 @@
 	call   5df <find_roots_of_polynomial+0x1cf>
  R_X86_64_PLT32	free-0x4
 	mov    0x0(%rbp,%r15,8),%rax
 	movdqa (%rsp),%xmm1
 	movups %xmm1,(%rax)
 	mov    %r15,%rax
 	add    $0x1,%r15
-	cmp    %rax,%r13
+	cmp    %r13,%rax
 	jne    5a0 <find_roots_of_polynomial+0x190>
 	mov    0x10(%rsp),%rdi
 	mov    0x18(%rsp),%rsi
 	call   607 <find_roots_of_polynomial+0x1f7>
  R_X86_64_PLT32	delete_fraction-0x4
-	mov    0x90(%rsp),%rax
+	mov    0x88(%rsp),%rax
 	mov    -0x8(%rax,%rbx,1),%rbp
 	mov    0x0(%rbp),%rsi
 	mov    %rsi,%rdi
 	mov    %rsi,(%rsp)
 	call   624 <find_roots_of_polynomial+0x214>
  R_X86_64_PLT32	strlen-0x4
 	lea    0x1(%rax),%r15
 	mov    %r15,%rdi
 	call   630 <find_roots_of_polynomial+0x220>
  R_X86_64_PLT32	malloc-0x4
 	mov    (%rsp),%rsi
 	mov    %r15,%rdx
 	mov    %rax,%rdi
-	mov    %rax,0x50(%rsp)
+	mov    %rax,0x48(%rsp)
 	call   644 <find_roots_of_polynomial+0x234>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x8(%rbp),%rbp
 	mov    %rbp,%rdi
 	call   650 <find_roots_of_polynomial+0x240>
  R_X86_64_PLT32	strlen-0x4
 	lea    0x1(%rax),%r15
 	mov    %r15,%rdi
 	call   65c <find_roots_of_polynomial+0x24c>
  R_X86_64_PLT32	malloc-0x4
 	mov    %r15,%rdx
 	mov    %rbp,%rsi
 	xor    %ebp,%ebp
 	mov    %rax,%rdi
-	mov    %rax,0x58(%rsp)
+	mov    %rax,0x50(%rsp)
 	call   671 <find_roots_of_polynomial+0x261>
  R_X86_64_PLT32	memcpy-0x4
 	mov    %rbx,0x10(%rsp)
-	mov    0x50(%rsp),%r15
+	mov    0x48(%rsp),%r15
 	mov    %r12,0x28(%rsp)
-	mov    0x90(%rsp),%rbx
-	mov    %r14,0x38(%rsp)
-	mov    0x58(%rsp),%r12
+	mov    0x88(%rsp),%rbx
+	mov    %r14,0x30(%rsp)
+	mov    0x50(%rsp),%r12
 	jmp    73a <find_roots_of_polynomial+0x32a>
 	nopw   0x0(%rax,%rax,1)
 	mov    %r8,%rdi
 	mov    %r8,(%rsp)
 	call   6ac <find_roots_of_polynomial+0x29c>
  R_X86_64_PLT32	strlen-0x4
 	mov    %r15,%rdi
@@ -565,17 +565,17 @@
 	jne    6a0 <find_roots_of_polynomial+0x290>
 	cmpb   $0x0,0x1(%r8)
 	jne    6a0 <find_roots_of_polynomial+0x290>
 	lea    0x1(%rbp),%rax
 	cmp    %rbp,%r13
 	jne    737 <find_roots_of_polynomial+0x327>
 	mov    0x10(%rsp),%rbx
-	mov    0x38(%rsp),%r14
-	mov    %r15,0x50(%rsp)
-	mov    %r12,0x58(%rsp)
+	mov    0x30(%rsp),%r14
+	mov    %r15,0x48(%rsp)
+	mov    %r12,0x50(%rsp)
 	mov    0x28(%rsp),%r12
 	mov    %rbx,%rdi
 	lea    (%rbx,%r14,1),%rbp
 	mov    %r14,%r15
 	xor    %ebx,%ebx
 	call   78a <find_roots_of_polynomial+0x37a>
  R_X86_64_PLT32	malloc-0x4
@@ -587,27 +587,27 @@
  R_X86_64_PLT32	strchr-0x4
 	test   %rax,%rax
 	mov    $0x1,%eax
 	cmovne %eax,%ebx
 	add    $0x8,%r15
 	cmp    %r15,%rbp
 	jne    790 <find_roots_of_polynomial+0x380>
-	mov    0x30(%rsp),%rax
+	mov    0x58(%rsp),%rax
 	xor    %r15d,%r15d
 	lea    0x3(%rax),%rbp
 	test   %bl,%bl
-	je     111d <find_roots_of_polynomial+0xd0d>
+	je     11e5 <find_roots_of_polynomial+0xdd5>
 	mov    %r12,(%rsp)
 	mov    %rax,%r14
 	mov    %r13,%rax
 	mov    %rbp,%r13
 	mov    %r15,%rbp
 	mov    %rax,%r15
 	nopl   0x0(%rax,%rax,1)
-	mov    0x90(%rsp),%rax
+	mov    0x88(%rsp),%rax
 	mov    (%rax,%rbp,8),%r12
 	mov    (%r12),%rdi
 	call   7f5 <find_roots_of_polynomial+0x3e5>
  R_X86_64_PLT32	strlen-0x4
 	mov    0x8(%r12),%rdi
 	mov    %rax,%rbx
 	call   802 <find_roots_of_polynomial+0x3f2>
@@ -626,30 +626,30 @@
 	call   830 <find_roots_of_polynomial+0x420>
  R_X86_64_PLT32	divide-0x4
 	mov    %rbp,%rax
 	add    $0x1,%rbp
 	cmp    %rax,%r15
 	jne    7e0 <find_roots_of_polynomial+0x3d0>
 	mov    (%rsp),%r12
-	mov    0xd0(%rsp),%rdi
+	mov    0xc8(%rsp),%rdi
 	mov    $0x8,%esi
 	call   852 <find_roots_of_polynomial+0x442>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    $0x2,%edi
-	mov    %rax,0x78(%rsp)
+	mov    %rax,0x70(%rsp)
 	call   866 <find_roots_of_polynomial+0x456>
  R_X86_64_PLT32	calloc-0x4
 	mov    %rax,0xf8(%rsp)
 	mov    %rax,%rbp
 	movb   $0x31,(%rax)
 	cmp    $0xffffffffffffffff,%r12
-	je     115e <find_roots_of_polynomial+0xd4e>
+	je     1226 <find_roots_of_polynomial+0xe16>
 	lea    0xf8(%rsp),%r15
-	mov    0x78(%rsp),%r14
+	mov    0x70(%rsp),%r14
 	mov    %rbp,%r13
 	mov    %r15,0xe8(%rsp)
 	jmp    8a8 <find_roots_of_polynomial+0x498>
 	nopl   0x0(%rax,%rax,1)
 	mov    0xf8(%rsp),%r13
 	mov    0x28(%rsp),%rax
 	mov    (%rax,%r12,8),%rbp
@@ -672,681 +672,741 @@
  R_X86_64_PLT32	multiply-0x4
 	mov    %rbx,(%r14,%r12,8)
 	mov    %r15,%rdi
 	call   8f0 <find_roots_of_polynomial+0x4e0>
  R_X86_64_PLT32	increment_whole-0x4
 	sub    $0x1,%r12
 	jae    8a0 <find_roots_of_polynomial+0x490>
-	mov    0xd0(%rsp),%rbx
+	mov    0xc8(%rsp),%rbx
 	lea    0x0(,%rbx,8),%rdi
 	call   90b <find_roots_of_polynomial+0x4fb>
  R_X86_64_PLT32	malloc-0x4
-	mov    %rax,0xc8(%rsp)
-	mov    0x88(%rsp),%rax
+	mov    %rax,%r14
+	mov    0x80(%rsp),%rax
 	movq   $0x0,(%rax)
 	test   %rbx,%rbx
-	je     1306 <find_roots_of_polynomial+0xef6>
-	mov    0xa0(%rsp),%rax
-	movq   $0x0,0x98(%rsp)
-	mov    %rax,0x68(%rsp)
+	je     13c9 <find_roots_of_polynomial+0xfb9>
+	mov    0x98(%rsp),%rax
+	mov    %r14,0xd0(%rsp)
+	movq   $0x0,0x90(%rsp)
+	mov    %rax,0x60(%rsp)
 	lea    0x100(%rsp),%rax
 	mov    %rax,0xd8(%rsp)
-	mov    0x30(%rsp),%rax
+	mov    0x58(%rsp),%rax
 	add    $0x3,%rax
-	mov    %rax,0x80(%rsp)
+	mov    %rax,0x78(%rsp)
 	nopl   (%rax)
 	mov    $0x1,%esi
 	mov    $0x2,%edi
-	xor    %ebp,%ebp
-	call   979 <find_roots_of_polynomial+0x569>
+	call   977 <find_roots_of_polynomial+0x567>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    $0x2,%edi
-	mov    %rax,%r15
-	call   98b <find_roots_of_polynomial+0x57b>
+	mov    %rax,%r12
+	call   989 <find_roots_of_polynomial+0x579>
  R_X86_64_PLT32	calloc-0x4
-	mov    %r15,%r14
-	movb   $0x30,(%r15)
+	movb   $0x30,(%r12)
+	mov    $0x1,%esi
+	mov    $0x2,%edi
 	movb   $0x31,(%rax)
-	mov    %rax,%r12
-	mov    0x68(%rsp),%rax
-	mov    %rbp,(%rsp)
+	mov    %rax,%rbx
+	call   9a3 <find_roots_of_polynomial+0x593>
+ R_X86_64_PLT32	calloc-0x4
+	movq   $0x0,(%rsp)
+	movb   $0x31,(%rax)
+	mov    %rax,%r15
+	mov    0x60(%rsp),%rax
+	movb   $0x0,0x3f(%rsp)
 	sub    $0x1,%rax
-	mov    %rax,0x70(%rsp)
-	jmp    9b3 <find_roots_of_polynomial+0x5a3>
+	mov    %rax,0x68(%rsp)
+	jmp    acf <find_roots_of_polynomial+0x6bf>
 	nopl   0x0(%rax)
-	mov    %rbx,%r12
-	mov    %r14,%rsi
-	mov    %r12,%rdi
-	call   9be <find_roots_of_polynomial+0x5ae>
- R_X86_64_PLT32	strcmp-0x4
-	test   %eax,%eax
-	je     1110 <find_roots_of_polynomial+0xd00>
-	mov    0x68(%rsp),%rsi
+	cmp    %rax,0x58(%rsp)
+	seta   %al
+	or     0x3f(%rsp),%al
+	mov    %al,0x10(%rsp)
+	movzbl %bpl,%ebp
+	mov    %r13,%rdi
+	sub    %rbp,%rdi
+	call   9ef <find_roots_of_polynomial+0x5df>
+ R_X86_64_PLT32	free-0x4
+	mov    %r14,%rdi
+	call   9f7 <find_roots_of_polynomial+0x5e7>
+ R_X86_64_PLT32	free-0x4
+	mov    0x60(%rsp),%rsi
 	mov    0x28(%rsp),%rdi
-	mov    %r12,%rdx
-	call   9d8 <find_roots_of_polynomial+0x5c8>
+	mov    %rbx,%rdx
+	call   a09 <find_roots_of_polynomial+0x5f9>
  R_X86_64_PLT32	find_roots_of_polynomial_substitute-0x4
-	mov    0x70(%rsp),%rsi
-	mov    0x78(%rsp),%rdi
-	mov    %r12,%rdx
-	mov    %rax,%rbp
-	call   9ed <find_roots_of_polynomial+0x5dd>
- R_X86_64_PLT32	find_roots_of_polynomial_substitute-0x4
-	mov    %rbp,%rdi
+	mov    0x68(%rsp),%rsi
+	mov    0x70(%rsp),%rdi
+	mov    %rbx,%rdx
 	mov    %rax,%r13
-	call   9f8 <find_roots_of_polynomial+0x5e8>
- R_X86_64_PLT32	strlen-0x4
+	call   a1e <find_roots_of_polynomial+0x60e>
+ R_X86_64_PLT32	find_roots_of_polynomial_substitute-0x4
 	mov    %r13,%rdi
-	mov    %rax,%rbx
-	call   a03 <find_roots_of_polynomial+0x5f3>
+	mov    %rax,%r14
+	call   a29 <find_roots_of_polynomial+0x619>
  R_X86_64_PLT32	strlen-0x4
-	mov    0x80(%rsp),%rcx
+	mov    %r14,%rdi
+	mov    %rax,%rbp
+	call   a34 <find_roots_of_polynomial+0x624>
+ R_X86_64_PLT32	strlen-0x4
+	mov    0x78(%rsp),%rcx
 	mov    $0x1,%esi
-	lea    (%rcx,%rbx,1),%rdi
+	lea    (%rcx,%rbp,1),%rdi
 	add    %rax,%rdi
-	call   a1c <find_roots_of_polynomial+0x60c>
+	call   a4a <find_roots_of_polynomial+0x63a>
  R_X86_64_PLT32	calloc-0x4
-	mov    0x30(%rsp),%rcx
-	mov    %r13,%rsi
-	mov    %rbp,%rdi
+	mov    0x58(%rsp),%rcx
+	mov    %r14,%rsi
+	mov    %r13,%rdi
 	mov    %rax,%rdx
-	mov    %rax,%r15
-	call   a32 <find_roots_of_polynomial+0x622>
+	mov    %rax,%rbp
+	call   a60 <find_roots_of_polynomial+0x650>
  R_X86_64_PLT32	divide-0x4
-	mov    %r12,%rdi
-	call   a3a <find_roots_of_polynomial+0x62a>
+	mov    %rbx,%rdi
+	call   a68 <find_roots_of_polynomial+0x658>
  R_X86_64_PLT32	strlen-0x4
-	mov    %r15,%rdi
-	mov    %rax,%rbx
-	call   a45 <find_roots_of_polynomial+0x635>
+	mov    %rbp,%rdi
+	mov    %rax,0x30(%rsp)
+	call   a75 <find_roots_of_polynomial+0x665>
  R_X86_64_PLT32	strlen-0x4
+	mov    0x30(%rsp),%rdx
 	mov    $0x1,%esi
-	lea    0x3(%rbx,%rax,1),%rdi
-	call   a54 <find_roots_of_polynomial+0x644>
+	lea    0x3(%rdx,%rax,1),%rdi
+	call   a89 <find_roots_of_polynomial+0x679>
  R_X86_64_PLT32	calloc-0x4
-	mov    %r15,%rsi
-	mov    %r12,%rdi
+	mov    %rbp,%rsi
+	mov    %rbx,%rdi
 	mov    %rax,%rdx
-	mov    %rax,0x60(%rsp)
-	mov    %rax,%rbx
-	call   a6a <find_roots_of_polynomial+0x65a>
+	mov    %rax,0x30(%rsp)
+	call   a9c <find_roots_of_polynomial+0x68c>
  R_X86_64_PLT32	subtract-0x4
+	mov    %r12,%rdi
+	mov    %rbx,%r12
+	call   aa7 <find_roots_of_polynomial+0x697>
+ R_X86_64_PLT32	free-0x4
+	mov    %r13,%rdi
+	call   aaf <find_roots_of_polynomial+0x69f>
+ R_X86_64_PLT32	free-0x4
 	mov    %r14,%rdi
-	mov    %r12,%r14
-	call   a75 <find_roots_of_polynomial+0x665>
+	call   ab7 <find_roots_of_polynomial+0x6a7>
  R_X86_64_PLT32	free-0x4
 	mov    %rbp,%rdi
-	call   a7d <find_roots_of_polynomial+0x66d>
+	call   abf <find_roots_of_polynomial+0x6af>
  R_X86_64_PLT32	free-0x4
+	cmpb   $0x0,0x10(%rsp)
+	mov    0x30(%rsp),%rbx
+	je     b80 <find_roots_of_polynomial+0x770>
+	mov    %r12,%rsi
+	mov    %rbx,%rdi
+	call   ada <find_roots_of_polynomial+0x6ca>
+ R_X86_64_PLT32	strcmp-0x4
+	test   %eax,%eax
+	je     b80 <find_roots_of_polynomial+0x770>
+	mov    %rbx,%rdi
+	call   aea <find_roots_of_polynomial+0x6da>
+ R_X86_64_PLT32	strlen-0x4
+	mov    %r12,%rdi
+	mov    %rax,%rbp
+	call   af5 <find_roots_of_polynomial+0x6e5>
+ R_X86_64_PLT32	strlen-0x4
+	mov    $0x1,%esi
+	lea    0x3(%rbp,%rax,1),%rdi
+	call   b04 <find_roots_of_polynomial+0x6f4>
+ R_X86_64_PLT32	calloc-0x4
+	mov    %r12,%rsi
+	mov    %rbx,%rdi
+	mov    %rax,%rdx
+	mov    %rax,%r13
+	call   b15 <find_roots_of_polynomial+0x705>
+ R_X86_64_PLT32	subtract-0x4
+	cmpb   $0x2d,0x0(%r13)
+	sete   %al
+	sete   %bpl
+	movzbl %al,%eax
+	add    %rax,%r13
 	mov    %r13,%rdi
-	call   a85 <find_roots_of_polynomial+0x675>
- R_X86_64_PLT32	free-0x4
+	call   b2f <find_roots_of_polynomial+0x71f>
+ R_X86_64_PLT32	strlen-0x4
 	mov    %r15,%rdi
-	call   a8d <find_roots_of_polynomial+0x67d>
- R_X86_64_PLT32	free-0x4
+	mov    %rax,%r14
+	call   b3a <find_roots_of_polynomial+0x72a>
+ R_X86_64_PLT32	strlen-0x4
+	mov    $0x1,%esi
+	lea    0x3(%r14,%rax,1),%rdi
+	call   b49 <find_roots_of_polynomial+0x739>
+ R_X86_64_PLT32	calloc-0x4
+	mov    %r15,%rsi
+	mov    %r13,%rdi
+	mov    %rax,%r14
+	mov    %rax,%rdx
+	call   b5a <find_roots_of_polynomial+0x74a>
+ R_X86_64_PLT32	subtract-0x4
 	addq   $0x1,(%rsp)
+	cmpb   $0x2d,(%r14)
 	mov    (%rsp),%rax
-	cmp    %rax,0x30(%rsp)
-	jne    9b0 <find_roots_of_polynomial+0x5a0>
+	jne    9d0 <find_roots_of_polynomial+0x5c0>
+	movb   $0x1,0x10(%rsp)
+	movb   $0x1,0x3f(%rsp)
+	jmp    9e0 <find_roots_of_polynomial+0x5d0>
+	nopl   0x0(%rax)
 	mov    %r12,%rdi
-	call   aa9 <find_roots_of_polynomial+0x699>
+	call   b88 <find_roots_of_polynomial+0x778>
+ R_X86_64_PLT32	free-0x4
+	mov    %r15,%rdi
+	call   b90 <find_roots_of_polynomial+0x780>
  R_X86_64_PLT32	free-0x4
-	mov    0x60(%rsp),%rbx
 	movzbl (%rbx),%eax
 	cmp    $0x2d,%al
-	mov    %al,0x47(%rsp)
+	mov    %al,0x3f(%rsp)
 	sete   %al
 	movzbl %al,%eax
 	add    %rax,%rbx
 	mov    %rax,0x10(%rsp)
 	mov    %rbx,%rdi
-	mov    %rbx,0x60(%rsp)
-	call   ad2 <find_roots_of_polynomial+0x6c2>
+	call   baf <find_roots_of_polynomial+0x79f>
  R_X86_64_PLT32	strlen-0x4
 	mov    $0x1,%esi
 	lea    0x1(%rax,%rax,1),%rbp
 	mov    %rbp,%rdi
-	call   ae4 <find_roots_of_polynomial+0x6d4>
+	call   bc1 <find_roots_of_polynomial+0x7b1>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    %rbp,%rdi
 	mov    %rax,%r15
-	mov    %rax,0xb8(%rsp)
-	call   afc <find_roots_of_polynomial+0x6ec>
+	mov    %rax,0xb0(%rsp)
+	call   bd9 <find_roots_of_polynomial+0x7c9>
  R_X86_64_PLT32	calloc-0x4
 	mov    %r15,%rsi
 	mov    %rbx,%rdi
 	mov    %rax,%rdx
 	mov    %rax,%r14
-	mov    %rax,0xc0(%rsp)
-	call   b15 <find_roots_of_polynomial+0x705>
+	mov    %rax,0xb8(%rsp)
+	call   bf2 <find_roots_of_polynomial+0x7e2>
  R_X86_64_PLT32	terminating_decimal_to_fraction-0x4
 	mov    0xd8(%rsp),%rdx
-	mov    %r15,%rdi
 	mov    %r14,%rsi
-	call   b28 <find_roots_of_polynomial+0x718>
+	mov    %r15,%rdi
+	call   c05 <find_roots_of_polynomial+0x7f5>
  R_X86_64_PLT32	fraction_to_continued_fraction-0x4
 	cmpq   $0x0,0x100(%rsp)
-	mov    %rax,%r15
-	je     ef7 <find_roots_of_polynomial+0xae7>
-	mov    0x68(%rsp),%rax
+	mov    %rax,0x30(%rsp)
+	je     fd7 <find_roots_of_polynomial+0xbc7>
+	mov    0x60(%rsp),%rax
 	mov    0x28(%rsp),%rcx
-	mov    %r15,0x38(%rsp)
-	xor    %r13d,%r13d
-	mov    0xc8(%rsp),%r15
+	xor    %r14d,%r14d
+	mov    %rbx,0xc0(%rsp)
+	mov    0xd0(%rsp),%r15
 	shl    $0x3,%rax
 	mov    %rax,0xe0(%rsp)
 	lea    -0x8(%rcx,%rax,1),%rax
-	mov    %rax,0x48(%rsp)
-	jmp    b96 <find_roots_of_polynomial+0x786>
-	nopl   0x0(%rax)
+	mov    %rax,0x40(%rsp)
+	jmp    c76 <find_roots_of_polynomial+0x866>
+	xchg   %ax,%ax
 	mov    0x0(%rbp),%rdi
 	mov    0x8(%rbp),%rsi
-	call   b7d <find_roots_of_polynomial+0x76d>
+	call   c5d <find_roots_of_polynomial+0x84d>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbp,%rdi
-	call   b85 <find_roots_of_polynomial+0x775>
+	call   c65 <find_roots_of_polynomial+0x855>
  R_X86_64_PLT32	free-0x4
 	mov    0x100(%rsp),%rax
-	cmp    %rax,%r13
-	jae    1100 <find_roots_of_polynomial+0xcf0>
+	cmp    %rax,%r14
+	jae    11d8 <find_roots_of_polynomial+0xdc8>
 	mov    $0x10,%edi
-	add    $0x1,%r13
-	call   ba4 <find_roots_of_polynomial+0x794>
+	add    $0x1,%r14
+	call   c84 <find_roots_of_polynomial+0x874>
  R_X86_64_PLT32	malloc-0x4
-	mov    0x38(%rsp),%rdi
-	mov    %r13,%rsi
+	mov    0x30(%rsp),%rdi
+	mov    %r14,%rsi
 	lea    0x8(%rax),%rcx
 	mov    %rax,%rdx
 	mov    %rax,%rbp
-	call   bbb <find_roots_of_polynomial+0x7ab>
+	call   c9b <find_roots_of_polynomial+0x88b>
  R_X86_64_PLT32	continued_fraction_to_fraction-0x4
-	cmpb   $0x2d,0x47(%rsp)
-	je     10c0 <find_roots_of_polynomial+0xcb0>
+	cmpb   $0x2d,0x3f(%rsp)
+	je     1198 <find_roots_of_polynomial+0xd88>
 	mov    0x0(%rbp),%rsi
-	mov    0x50(%rsp),%rdi
-	call   bd4 <find_roots_of_polynomial+0x7c4>
+	mov    0x48(%rsp),%rdi
+	call   cb4 <find_roots_of_polynomial+0x8a4>
  R_X86_64_PLT32	abs_mod-0x4
 	mov    0x8(%rbp),%rsi
-	mov    0x58(%rsp),%rdi
+	mov    0x50(%rsp),%rdi
 	mov    %rax,(%rsp)
-	call   be6 <find_roots_of_polynomial+0x7d6>
+	call   cc6 <find_roots_of_polynomial+0x8b6>
  R_X86_64_PLT32	abs_mod-0x4
 	mov    (%rsp),%r8
-	mov    %rax,%r14
+	mov    %rax,%r13
 	movzbl (%r8),%r12d
 	sub    $0x30,%r12d
-	jne    bfc <find_roots_of_polynomial+0x7ec>
+	jne    cdc <find_roots_of_polynomial+0x8cc>
 	movzbl 0x1(%r8),%r12d
-	movzbl (%r14),%ebx
+	movzbl 0x0(%r13),%ebx
 	sub    $0x30,%ebx
-	jne    c0a <find_roots_of_polynomial+0x7fa>
-	movzbl 0x1(%r14),%ebx
+	jne    ceb <find_roots_of_polynomial+0x8db>
+	movzbl 0x1(%r13),%ebx
 	mov    %r8,%rdi
-	call   c12 <find_roots_of_polynomial+0x802>
+	call   cf3 <find_roots_of_polynomial+0x8e3>
  R_X86_64_PLT32	free-0x4
-	mov    %r14,%rdi
-	call   c1a <find_roots_of_polynomial+0x80a>
+	mov    %r13,%rdi
+	call   cfb <find_roots_of_polynomial+0x8eb>
  R_X86_64_PLT32	free-0x4
-	mov    0x48(%rsp),%rax
+	mov    0x40(%rsp),%rax
 	mov    (%rax),%rdi
-	call   c27 <find_roots_of_polynomial+0x817>
+	call   d08 <find_roots_of_polynomial+0x8f8>
  R_X86_64_PLT32	strlen-0x4
 	mov    0x0(%rbp),%rdi
-	mov    %rax,%r14
-	call   c33 <find_roots_of_polynomial+0x823>
+	mov    %rax,%r13
+	call   d14 <find_roots_of_polynomial+0x904>
  R_X86_64_PLT32	strlen-0x4
 	sub    0x10(%rsp),%rax
-	cmp    %rax,%r14
-	jb     b70 <find_roots_of_polynomial+0x760>
+	cmp    %rax,%r13
+	jb     c50 <find_roots_of_polynomial+0x840>
 	mov    0x28(%rsp),%rax
 	mov    (%rax),%rdi
-	call   c4e <find_roots_of_polynomial+0x83e>
+	call   d2f <find_roots_of_polynomial+0x91f>
  R_X86_64_PLT32	strlen-0x4
 	mov    0x8(%rbp),%rdi
-	mov    %rax,%r14
-	call   c5a <find_roots_of_polynomial+0x84a>
+	mov    %rax,%r13
+	call   d3b <find_roots_of_polynomial+0x92b>
  R_X86_64_PLT32	strlen-0x4
 	sub    0x10(%rsp),%rax
-	cmp    %rax,%r14
-	jb     b70 <find_roots_of_polynomial+0x760>
+	cmp    %rax,%r13
+	jb     c50 <find_roots_of_polynomial+0x840>
 	or     %r12d,%ebx
-	jne    b70 <find_roots_of_polynomial+0x760>
-	mov    0x88(%rsp),%rax
+	jne    c50 <find_roots_of_polynomial+0x840>
+	mov    0x80(%rsp),%rax
 	xor    %ebx,%ebx
 	cmpq   $0x0,(%rax)
 	mov    %rax,%r12
-	je     cb2 <find_roots_of_polynomial+0x8a2>
-	nopl   0x0(%rax)
+	je     d92 <find_roots_of_polynomial+0x982>
+	nopl   (%rax)
 	mov    (%r15,%rbx,8),%rax
 	mov    0x0(%rbp),%rdx
 	mov    0x8(%rbp),%rcx
 	mov    (%rax),%rdi
 	mov    0x8(%rax),%rsi
-	call   ca0 <find_roots_of_polynomial+0x890>
+	call   d80 <find_roots_of_polynomial+0x970>
  R_X86_64_PLT32	equal_fraction-0x4
 	test   %al,%al
-	jne    b70 <find_roots_of_polynomial+0x760>
+	jne    c50 <find_roots_of_polynomial+0x840>
 	add    $0x1,%rbx
 	cmp    %rbx,(%r12)
-	ja     c88 <find_roots_of_polynomial+0x878>
-	mov    0xa0(%rsp),%rsi
-	mov    0x90(%rsp),%rdi
+	ja     d68 <find_roots_of_polynomial+0x958>
+	mov    0x98(%rsp),%rsi
+	mov    0x88(%rsp),%rdi
 	mov    %rbp,%rdx
-	call   cca <find_roots_of_polynomial+0x8ba>
+	call   daa <find_roots_of_polynomial+0x99a>
  R_X86_64_PLT32	find_roots_of_polynomial_substitute_fraction-0x4
-	mov    0xa8(%rsp),%rdx
-	mov    0xb0(%rsp),%rcx
+	mov    0xa0(%rsp),%rdx
+	mov    0xa8(%rsp),%rcx
 	mov    (%rax),%rdi
 	mov    0x8(%rax),%rsi
 	mov    %rax,%r12
-	call   ce9 <find_roots_of_polynomial+0x8d9>
+	call   dc9 <find_roots_of_polynomial+0x9b9>
  R_X86_64_PLT32	equal_fraction-0x4
 	mov    (%r12),%rdi
 	mov    0x8(%r12),%rsi
 	mov    %eax,%ebx
-	call   cf9 <find_roots_of_polynomial+0x8e9>
+	call   dd9 <find_roots_of_polynomial+0x9c9>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %r12,%rdi
-	call   d01 <find_roots_of_polynomial+0x8f1>
+	call   de1 <find_roots_of_polynomial+0x9d1>
  R_X86_64_PLT32	free-0x4
 	test   %bl,%bl
-	je     b70 <find_roots_of_polynomial+0x760>
-	mov    0x88(%rsp),%rcx
-	mov    0xc8(%rsp),%rdx
+	je     c50 <find_roots_of_polynomial+0x840>
+	mov    0x80(%rsp),%rcx
+	mov    0xd0(%rsp),%rdx
 	mov    0x0(%rbp),%r13
-	mov    0x38(%rsp),%r15
+	mov    0xc0(%rsp),%rbx
 	mov    (%rcx),%rax
 	mov    %r13,%rdi
 	mov    %rbp,(%rdx,%rax,8)
 	add    $0x1,%rax
 	mov    %rax,(%rcx)
-	call   d38 <find_roots_of_polynomial+0x928>
+	call   e1b <find_roots_of_polynomial+0xa0b>
  R_X86_64_PLT32	strlen-0x4
-	mov    0x8(%rbp),%rbp
-	mov    %rax,%rbx
-	mov    %rbp,%rdi
-	call   d47 <find_roots_of_polynomial+0x937>
+	mov    0x8(%rbp),%r14
+	mov    %rax,%r12
+	mov    %r14,%rdi
+	call   e2a <find_roots_of_polynomial+0xa1a>
  R_X86_64_PLT32	strlen-0x4
-	mov    0x80(%rsp),%rcx
+	mov    0x78(%rsp),%rcx
 	mov    $0x1,%esi
-	lea    (%rcx,%rbx,1),%rdi
+	lea    (%rcx,%r12,1),%rdi
 	add    %rax,%rdi
-	call   d60 <find_roots_of_polynomial+0x950>
+	call   e40 <find_roots_of_polynomial+0xa30>
  R_X86_64_PLT32	calloc-0x4
-	mov    0x30(%rsp),%rcx
-	mov    %rbp,%rsi
+	mov    0x58(%rsp),%rcx
+	mov    %r14,%rsi
 	mov    %r13,%rdi
 	mov    %rax,%rdx
-	mov    %rax,%r12
-	call   d76 <find_roots_of_polynomial+0x966>
+	mov    %rax,%rbp
+	call   e56 <find_roots_of_polynomial+0xa46>
  R_X86_64_PLT32	divide-0x4
-	mov    0x68(%rsp),%r14
-	mov    0x28(%rsp),%rbx
-	mov    %r12,%rdx
-	mov    %rbx,%rdi
+	mov    0x60(%rsp),%r14
+	mov    0x28(%rsp),%r15
+	mov    %rbp,%rdx
+	mov    %r15,%rdi
 	mov    %r14,%rsi
-	call   d8e <find_roots_of_polynomial+0x97e>
+	call   e6e <find_roots_of_polynomial+0xa5e>
  R_X86_64_PLT32	find_roots_of_polynomial_divide_polynomial-0x4
-	mov    %r12,%rdi
-	mov    %rax,%rbp
-	call   d99 <find_roots_of_polynomial+0x989>
+	mov    %rbp,%rdi
+	mov    %rax,%r12
+	call   e79 <find_roots_of_polynomial+0xa69>
  R_X86_64_PLT32	free-0x4
 	test   %r14,%r14
-	je     12b2 <find_roots_of_polynomial+0xea2>
-	mov    %rbx,%rax
-	mov    %rbx,%r12
-	mov    0xe0(%rsp),%rbx
-	add    %rax,%rbx
-	nopl   0x0(%rax,%rax,1)
-	mov    (%r12),%rdi
-	add    $0x8,%r12
-	call   dc5 <find_roots_of_polynomial+0x9b5>
+	je     1375 <find_roots_of_polynomial+0xf65>
+	mov    0xe0(%rsp),%rbp
+	mov    %r15,%r13
+	add    %r15,%rbp
+	mov    0x0(%r13),%rdi
+	add    $0x8,%r13
+	call   e9d <find_roots_of_polynomial+0xa8d>
  R_X86_64_PLT32	free-0x4
-	cmp    %r12,%rbx
-	jne    db8 <find_roots_of_polynomial+0x9a8>
+	cmp    %rbp,%r13
+	jne    e90 <find_roots_of_polynomial+0xa80>
 	mov    0x28(%rsp),%rdi
-	call   dd4 <find_roots_of_polynomial+0x9c4>
+	call   eac <find_roots_of_polynomial+0xa9c>
  R_X86_64_PLT32	free-0x4
-	cmpq   $0x0,0x70(%rsp)
-	je     1272 <find_roots_of_polynomial+0xe62>
-	mov    0x78(%rsp),%r12
+	cmpq   $0x0,0x68(%rsp)
+	je     1335 <find_roots_of_polynomial+0xf25>
 	mov    0x70(%rsp),%r13
-	xor    %ebx,%ebx
+	mov    0x68(%rsp),%r14
+	xor    %ebp,%ebp
 	nopl   0x0(%rax)
-	mov    (%r12,%rbx,8),%rdi
-	add    $0x1,%rbx
-	call   dfd <find_roots_of_polynomial+0x9ed>
+	mov    0x0(%r13,%rbp,8),%rdi
+	add    $0x1,%rbp
+	call   ed6 <find_roots_of_polynomial+0xac6>
  R_X86_64_PLT32	free-0x4
-	cmp    %r13,%rbx
-	jb     df0 <find_roots_of_polynomial+0x9e0>
-	mov    0xf8(%rsp),%r12
-	mov    %r12,%rdi
-	call   e12 <find_roots_of_polynomial+0xa02>
+	cmp    %r14,%rbp
+	jb     ec8 <find_roots_of_polynomial+0xab8>
+	mov    0xf8(%rsp),%rbp
+	mov    %rbp,%rdi
+	call   eeb <find_roots_of_polynomial+0xadb>
  R_X86_64_PLT32	strlen-0x4
+	mov    %rbp,%rdi
 	xor    %esi,%esi
-	mov    %r12,%rdi
 	mov    %rax,%rdx
-	call   e1f <find_roots_of_polynomial+0xa0f>
+	call   ef8 <find_roots_of_polynomial+0xae8>
  R_X86_64_PLT32	memset-0x4
 	mov    0xf8(%rsp),%rax
 	movb   $0x31,(%rax)
-	mov    0x68(%rsp),%rax
-	lea    -0x3(%rax),%rbx
+	mov    0x60(%rsp),%rax
+	lea    -0x3(%rax),%rbp
 	cmp    $0x2,%rax
-	je     124e <find_roots_of_polynomial+0xe3e>
-	mov    %r15,(%rsp)
-	mov    0xe8(%rsp),%r14
-	nopl   0x0(%rax)
-	mov    0xf8(%rsp),%r15
-	mov    %r15,%rdi
-	call   e60 <find_roots_of_polynomial+0xa50>
+	je     1311 <find_roots_of_polynomial+0xf01>
+	mov    %rbx,(%rsp)
+	mov    0xe8(%rsp),%r15
+	nopw   0x0(%rax,%rax,1)
+	mov    0xf8(%rsp),%r14
+	mov    %r14,%rdi
+	call   f38 <find_roots_of_polynomial+0xb28>
  R_X86_64_PLT32	strlen-0x4
-	mov    0x0(%rbp,%rbx,8),%r13
-	mov    %rax,%r12
-	mov    %r13,%rdi
-	call   e70 <find_roots_of_polynomial+0xa60>
+	mov    (%r12,%rbp,8),%rbx
+	mov    %rax,%r13
+	mov    %rbx,%rdi
+	call   f47 <find_roots_of_polynomial+0xb37>
  R_X86_64_PLT32	strlen-0x4
 	mov    $0x1,%esi
-	lea    0x3(%r12,%rax,1),%rdi
-	call   e7f <find_roots_of_polynomial+0xa6f>
+	lea    0x3(%r13,%rax,1),%rdi
+	call   f56 <find_roots_of_polynomial+0xb46>
  R_X86_64_PLT32	calloc-0x4
-	mov    %r15,%rdi
-	mov    %r13,%rsi
+	mov    %r14,%rdi
+	mov    %rbx,%rsi
 	mov    %rax,%rdx
-	mov    %rax,%r12
-	call   e90 <find_roots_of_polynomial+0xa80>
+	mov    %rax,%r13
+	call   f67 <find_roots_of_polynomial+0xb57>
  R_X86_64_PLT32	multiply-0x4
-	mov    0x78(%rsp),%rax
-	mov    %r14,%rdi
-	mov    %r12,(%rax,%rbx,8)
-	call   ea1 <find_roots_of_polynomial+0xa91>
+	mov    0x70(%rsp),%rax
+	mov    %r15,%rdi
+	mov    %r13,(%rax,%rbp,8)
+	call   f78 <find_roots_of_polynomial+0xb68>
  R_X86_64_PLT32	increment_whole-0x4
-	sub    $0x1,%rbx
-	jae    e50 <find_roots_of_polynomial+0xa40>
-	mov    0x68(%rsp),%rdx
-	mov    0x70(%rsp),%rcx
-	mov    %rbp,0x28(%rsp)
-	mov    (%rsp),%r15
+	sub    $0x1,%rbp
+	jae    f28 <find_roots_of_polynomial+0xb18>
+	mov    0x60(%rsp),%rdx
+	mov    0x68(%rsp),%rcx
+	mov    %r12,0x28(%rsp)
+	mov    (%rsp),%rbx
 	mov    0x100(%rsp),%rax
 	sub    $0x2,%rdx
-	mov    %rcx,0x68(%rsp)
-	mov    %rdx,0x70(%rsp)
-	test   %rax,%rax
-	je     ef7 <find_roots_of_polynomial+0xae7>
-	xor    %ebx,%ebx
+	mov    %rcx,0x60(%rsp)
+	mov    %rdx,0x68(%rsp)
 	nopw   0x0(%rax,%rax,1)
-	mov    (%r15,%rbx,8),%rdi
-	add    $0x1,%rbx
-	call   eed <find_roots_of_polynomial+0xadd>
+	test   %rax,%rax
+	je     fd7 <find_roots_of_polynomial+0xbc7>
+	mov    0x30(%rsp),%r12
+	xor    %ebp,%ebp
+	nopl   0x0(%rax)
+	mov    (%r12,%rbp,8),%rdi
+	add    $0x1,%rbp
+	call   fcd <find_roots_of_polynomial+0xbbd>
  R_X86_64_PLT32	free-0x4
-	cmp    %rbx,0x100(%rsp)
-	ja     ee0 <find_roots_of_polynomial+0xad0>
-	mov    %r15,%rdi
-	call   eff <find_roots_of_polynomial+0xaef>
+	cmp    %rbp,0x100(%rsp)
+	ja     fc0 <find_roots_of_polynomial+0xbb0>
+	mov    0x30(%rsp),%rdi
+	call   fe1 <find_roots_of_polynomial+0xbd1>
  R_X86_64_PLT32	free-0x4
-	mov    0x60(%rsp),%rdi
-	sub    0x10(%rsp),%rdi
-	call   f0e <find_roots_of_polynomial+0xafe>
+	sub    0x10(%rsp),%rbx
+	mov    %rbx,%rdi
+	call   fee <find_roots_of_polynomial+0xbde>
  R_X86_64_PLT32	free-0x4
-	mov    0xb8(%rsp),%rdi
-	call   f1b <find_roots_of_polynomial+0xb0b>
+	mov    0xb0(%rsp),%rdi
+	call   ffb <find_roots_of_polynomial+0xbeb>
  R_X86_64_PLT32	free-0x4
-	mov    0xc0(%rsp),%rdi
-	call   f28 <find_roots_of_polynomial+0xb18>
+	mov    0xb8(%rsp),%rdi
+	call   1008 <find_roots_of_polynomial+0xbf8>
  R_X86_64_PLT32	free-0x4
-	addq   $0x1,0x98(%rsp)
-	mov    0x98(%rsp),%rax
-	cmp    0xd0(%rsp),%rax
+	addq   $0x1,0x90(%rsp)
+	mov    0x90(%rsp),%rax
+	cmp    0xc8(%rsp),%rax
 	jne    968 <find_roots_of_polynomial+0x558>
 	mov    0xf8(%rsp),%rdi
-	call   f54 <find_roots_of_polynomial+0xb44>
+	mov    0xd0(%rsp),%r14
+	call   103c <find_roots_of_polynomial+0xc2c>
  R_X86_64_PLT32	free-0x4
-	mov    0xa8(%rsp),%rdi
-	mov    0xb0(%rsp),%rsi
-	call   f69 <find_roots_of_polynomial+0xb59>
+	mov    0xa0(%rsp),%rdi
+	mov    0xa8(%rsp),%rsi
+	call   1051 <find_roots_of_polynomial+0xc41>
  R_X86_64_PLT32	delete_fraction-0x4
-	cmpq   $0x0,0xa0(%rsp)
-	je     fb4 <find_roots_of_polynomial+0xba4>
-	mov    0x90(%rsp),%rbp
-	mov    0xa0(%rsp),%r12
+	cmpq   $0x0,0x98(%rsp)
+	je     1094 <find_roots_of_polynomial+0xc84>
+	mov    0x88(%rsp),%rbp
+	mov    0x98(%rsp),%r12
 	xor    %ebx,%ebx
-	cs nopw 0x0(%rax,%rax,1)
+	xchg   %ax,%ax
 	mov    0x0(%rbp,%rbx,8),%rax
 	mov    (%rax),%rdi
 	mov    0x8(%rax),%rsi
-	call   fa1 <find_roots_of_polynomial+0xb91>
+	call   1081 <find_roots_of_polynomial+0xc71>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    0x0(%rbp,%rbx,8),%rdi
 	add    $0x1,%rbx
-	call   faf <find_roots_of_polynomial+0xb9f>
+	call   108f <find_roots_of_polynomial+0xc7f>
  R_X86_64_PLT32	free-0x4
 	cmp    %rbx,%r12
-	ja     f90 <find_roots_of_polynomial+0xb80>
+	ja     1070 <find_roots_of_polynomial+0xc60>
 	mov    0x28(%rsp),%rax
-	mov    0x68(%rsp),%rcx
+	mov    0x60(%rsp),%rcx
 	mov    %rax,%rbp
 	lea    (%rax,%rcx,8),%rbx
 	test   %rcx,%rcx
-	je     fea <find_roots_of_polynomial+0xbda>
+	je     10ca <find_roots_of_polynomial+0xcba>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x0(%rbp),%rdi
 	add    $0x8,%rbp
-	call   fdd <find_roots_of_polynomial+0xbcd>
+	call   10bd <find_roots_of_polynomial+0xcad>
  R_X86_64_PLT32	free-0x4
 	cmp    %rbp,%rbx
-	jne    fd0 <find_roots_of_polynomial+0xbc0>
-	cmpq   $0x0,0x70(%rsp)
-	je     1013 <find_roots_of_polynomial+0xc03>
-	mov    0x78(%rsp),%rbp
-	mov    0x70(%rsp),%r12
+	jne    10b0 <find_roots_of_polynomial+0xca0>
+	cmpq   $0x0,0x68(%rsp)
+	je     10f3 <find_roots_of_polynomial+0xce3>
+	mov    0x70(%rsp),%rbp
+	mov    0x68(%rsp),%r12
 	xor    %ebx,%ebx
 	cs nopw 0x0(%rax,%rax,1)
 	mov    0x0(%rbp,%rbx,8),%rdi
 	add    $0x1,%rbx
-	call   100e <find_roots_of_polynomial+0xbfe>
+	call   10ee <find_roots_of_polynomial+0xcde>
  R_X86_64_PLT32	free-0x4
 	cmp    %r12,%rbx
-	jb     1000 <find_roots_of_polynomial+0xbf0>
-	mov    0x90(%rsp),%rdi
+	jb     10e0 <find_roots_of_polynomial+0xcd0>
+	mov    0x88(%rsp),%rdi
 	xor    %ebx,%ebx
-	call   1022 <find_roots_of_polynomial+0xc12>
+	call   1102 <find_roots_of_polynomial+0xcf2>
  R_X86_64_PLT32	free-0x4
 	mov    0x28(%rsp),%rdi
-	call   102c <find_roots_of_polynomial+0xc1c>
+	call   110c <find_roots_of_polynomial+0xcfc>
  R_X86_64_PLT32	free-0x4
-	mov    0x78(%rsp),%rdi
-	call   1036 <find_roots_of_polynomial+0xc26>
+	mov    0x70(%rsp),%rdi
+	call   1116 <find_roots_of_polynomial+0xd06>
  R_X86_64_PLT32	free-0x4
-	mov    0x88(%rsp),%rax
-	mov    0xc8(%rsp),%rbp
+	mov    0x80(%rsp),%rax
 	cmpq   $0x0,(%rax)
-	mov    %rax,%r12
-	je     1075 <find_roots_of_polynomial+0xc65>
-	nop
-	mov    0x0(%rbp,%rbx,8),%rax
+	mov    %rax,%rbp
+	je     1153 <find_roots_of_polynomial+0xd43>
+	nopw   0x0(%rax,%rax,1)
+	mov    (%r14,%rbx,8),%rax
 	mov    (%rax),%rdi
-	call   105d <find_roots_of_polynomial+0xc4d>
+	call   113c <find_roots_of_polynomial+0xd2c>
  R_X86_64_PLT32	remove_zeroes-0x4
-	mov    0x0(%rbp,%rbx,8),%rax
+	mov    (%r14,%rbx,8),%rax
 	add    $0x1,%rbx
 	mov    0x8(%rax),%rdi
-	call   106f <find_roots_of_polynomial+0xc5f>
+	call   114d <find_roots_of_polynomial+0xd3d>
  R_X86_64_PLT32	remove_zeroes-0x4
-	cmp    %rbx,(%r12)
-	ja     1050 <find_roots_of_polynomial+0xc40>
-	mov    0x50(%rsp),%rdi
-	call   107f <find_roots_of_polynomial+0xc6f>
+	cmp    %rbx,0x0(%rbp)
+	ja     1130 <find_roots_of_polynomial+0xd20>
+	mov    0x48(%rsp),%rdi
+	call   115d <find_roots_of_polynomial+0xd4d>
  R_X86_64_PLT32	free-0x4
-	mov    0x58(%rsp),%rdi
-	call   1089 <find_roots_of_polynomial+0xc79>
+	mov    0x50(%rsp),%rdi
+	call   1167 <find_roots_of_polynomial+0xd57>
  R_X86_64_PLT32	free-0x4
 	mov    0x108(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    1313 <find_roots_of_polynomial+0xf03>
-	mov    0xc8(%rsp),%rax
+	jne    13d6 <find_roots_of_polynomial+0xfc6>
 	add    $0x118,%rsp
+	mov    %r14,%rax
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
-	nopw   0x0(%rax,%rax,1)
+	nopl   0x0(%rax,%rax,1)
 	mov    0x0(%rbp),%r12
 	mov    %r12,%rdi
-	call   10cc <find_roots_of_polynomial+0xcbc>
+	call   11a4 <find_roots_of_polynomial+0xd94>
  R_X86_64_PLT32	strlen-0x4
 	mov    %r12,%rdi
 	lea    0x2(%rax),%rsi
 	mov    %rax,%rbx
-	call   10db <find_roots_of_polynomial+0xccb>
+	call   11b3 <find_roots_of_polynomial+0xda3>
  R_X86_64_PLT32	realloc-0x4
 	lea    0x1(%rbx),%rdx
 	mov    %rax,0x0(%rbp)
 	mov    %rax,%rsi
 	lea    0x1(%rax),%rdi
-	call   10ef <find_roots_of_polynomial+0xcdf>
+	call   11c7 <find_roots_of_polynomial+0xdb7>
  R_X86_64_PLT32	memmove-0x4
 	mov    0x0(%rbp),%rax
 	movb   $0x2d,(%rax)
-	jmp    bc6 <find_roots_of_polynomial+0x7b6>
+	jmp    ca6 <find_roots_of_polynomial+0x896>
 	nopl   0x0(%rax,%rax,1)
-	mov    0x38(%rsp),%r15
-	jmp    ed0 <find_roots_of_polynomial+0xac0>
-	nopw   0x0(%rax,%rax,1)
-	mov    %r12,0x60(%rsp)
-	mov    %r14,%r12
-	jmp    aa1 <find_roots_of_polynomial+0x691>
+	mov    0xc0(%rsp),%rbx
+	jmp    fb0 <find_roots_of_polynomial+0xba0>
 	mov    0x28(%rsp),%rbp
 	xor    %ebx,%ebx
 	nopl   0x0(%rax)
 	mov    (%r14,%rbx,8),%r15
 	mov    %r15,%rdi
-	call   1134 <find_roots_of_polynomial+0xd24>
+	call   11fc <find_roots_of_polynomial+0xdec>
  R_X86_64_PLT32	strlen-0x4
 	lea    0x1(%rax),%rdi
-	call   113d <find_roots_of_polynomial+0xd2d>
+	call   1205 <find_roots_of_polynomial+0xdf5>
  R_X86_64_PLT32	malloc-0x4
 	mov    %r15,%rsi
 	mov    %rax,0x0(%rbp,%rbx,8)
 	mov    %rax,%rdi
-	call   114d <find_roots_of_polynomial+0xd3d>
+	call   1215 <find_roots_of_polynomial+0xe05>
  R_X86_64_PLT32	strcpy-0x4
 	mov    %rbx,%rax
 	add    $0x1,%rbx
-	cmp    %rax,%r13
-	jne    1128 <find_roots_of_polynomial+0xd18>
+	cmp    %r13,%rax
+	jne    11f0 <find_roots_of_polynomial+0xde0>
 	jmp    840 <find_roots_of_polynomial+0x430>
 	xor    %edi,%edi
-	call   1165 <find_roots_of_polynomial+0xd55>
+	call   122d <find_roots_of_polynomial+0xe1d>
  R_X86_64_PLT32	malloc-0x4
-	mov    %rax,0xc8(%rsp)
-	mov    0x88(%rsp),%rax
+	mov    %rax,%r14
+	mov    0x80(%rsp),%rax
 	movq   $0x0,(%rax)
 	mov    %rbp,%rdi
-	call   1184 <find_roots_of_polynomial+0xd74>
+	call   1247 <find_roots_of_polynomial+0xe37>
  R_X86_64_PLT32	free-0x4
-	mov    0xa8(%rsp),%rdi
-	mov    0xb0(%rsp),%rsi
-	call   1199 <find_roots_of_polynomial+0xd89>
+	mov    0xa0(%rsp),%rdi
+	mov    0xa8(%rsp),%rsi
+	call   125c <find_roots_of_polynomial+0xe4c>
  R_X86_64_PLT32	delete_fraction-0x4
-	movq   $0x0,0x70(%rsp)
-	movq   $0x1,0x68(%rsp)
-	jmp    f74 <find_roots_of_polynomial+0xb64>
+	movq   $0x0,0x68(%rsp)
+	movq   $0x1,0x60(%rsp)
+	jmp    105c <find_roots_of_polynomial+0xc4c>
 	mov    -0x8(%rax,%rbx,1),%rbx
 	mov    (%rbx),%rbp
 	mov    %rbp,%rdi
-	call   11c0 <find_roots_of_polynomial+0xdb0>
+	call   1283 <find_roots_of_polynomial+0xe73>
  R_X86_64_PLT32	strlen-0x4
 	lea    0x1(%rax),%r13
 	mov    %r13,%rdi
-	call   11cc <find_roots_of_polynomial+0xdbc>
+	call   128f <find_roots_of_polynomial+0xe7f>
  R_X86_64_PLT32	malloc-0x4
 	mov    %r13,%rdx
 	mov    %rbp,%rsi
 	mov    %rax,%rdi
-	mov    %rax,0x50(%rsp)
-	call   11df <find_roots_of_polynomial+0xdcf>
+	mov    %rax,0x48(%rsp)
+	call   12a2 <find_roots_of_polynomial+0xe92>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x8(%rbx),%rbp
 	mov    %rbp,%rdi
-	call   11eb <find_roots_of_polynomial+0xddb>
+	call   12ae <find_roots_of_polynomial+0xe9e>
  R_X86_64_PLT32	strlen-0x4
 	lea    0x1(%rax),%r13
 	mov    %r13,%rdi
-	call   11f7 <find_roots_of_polynomial+0xde7>
+	call   12ba <find_roots_of_polynomial+0xeaa>
  R_X86_64_PLT32	malloc-0x4
 	mov    %r13,%rdx
 	mov    %rbp,%rsi
 	mov    %rax,%rdi
-	mov    %rax,0x58(%rsp)
-	call   120a <find_roots_of_polynomial+0xdfa>
+	mov    %rax,0x50(%rsp)
+	call   12cd <find_roots_of_polynomial+0xebd>
  R_X86_64_PLT32	memcpy-0x4
 	xor    %edi,%edi
-	call   1211 <find_roots_of_polynomial+0xe01>
+	call   12d4 <find_roots_of_polynomial+0xec4>
  R_X86_64_PLT32	malloc-0x4
 	mov    $0x8,%esi
 	mov    $0xffffffffffffffff,%rdi
 	mov    %rax,0x28(%rsp)
-	call   1227 <find_roots_of_polynomial+0xe17>
+	call   12ea <find_roots_of_polynomial+0xeda>
  R_X86_64_PLT32	calloc-0x4
 	mov    $0x1,%esi
 	mov    $0x2,%edi
-	mov    %rax,0x78(%rsp)
-	call   123b <find_roots_of_polynomial+0xe2b>
+	mov    %rax,0x70(%rsp)
+	call   12fe <find_roots_of_polynomial+0xeee>
  R_X86_64_PLT32	calloc-0x4
 	mov    %rax,0xf8(%rsp)
 	mov    %rax,%rbp
 	movb   $0x31,(%rax)
 	jmp    87e <find_roots_of_polynomial+0x46e>
-	mov    %rbp,0x28(%rsp)
+	mov    %r12,0x28(%rsp)
 	mov    0x100(%rsp),%rax
-	movq   $0x0,0x70(%rsp)
-	movq   $0x1,0x68(%rsp)
-	jmp    ed0 <find_roots_of_polynomial+0xac0>
-	mov    0xf8(%rsp),%r12
-	mov    $0xfffffffffffffffe,%rbx
-	mov    %r12,%rdi
-	call   1289 <find_roots_of_polynomial+0xe79>
+	movq   $0x0,0x68(%rsp)
+	movq   $0x1,0x60(%rsp)
+	jmp    fb0 <find_roots_of_polynomial+0xba0>
+	mov    0xf8(%rsp),%rbp
+	mov    %rbp,%rdi
+	call   1345 <find_roots_of_polynomial+0xf35>
  R_X86_64_PLT32	strlen-0x4
+	mov    %rbp,%rdi
 	xor    %esi,%esi
-	mov    %r12,%rdi
+	mov    $0xfffffffffffffffe,%rbp
 	mov    %rax,%rdx
-	call   1296 <find_roots_of_polynomial+0xe86>
+	call   1359 <find_roots_of_polynomial+0xf49>
  R_X86_64_PLT32	memset-0x4
 	mov    0xf8(%rsp),%rax
-	mov    %r15,(%rsp)
-	mov    0xe8(%rsp),%r14
+	mov    %rbx,(%rsp)
+	mov    0xe8(%rsp),%r15
 	movb   $0x31,(%rax)
-	jmp    e50 <find_roots_of_polynomial+0xa40>
+	jmp    f28 <find_roots_of_polynomial+0xb18>
 	mov    0x28(%rsp),%rdi
-	call   12bc <find_roots_of_polynomial+0xeac>
+	call   137f <find_roots_of_polynomial+0xf6f>
  R_X86_64_PLT32	free-0x4
-	jmp    de0 <find_roots_of_polynomial+0x9d0>
+	jmp    eb8 <find_roots_of_polynomial+0xaa8>
 	sub    %rbp,%rax
 	mov    %rbp,%rdi
 	lea    0x2(%rax),%rsi
-	call   12d0 <find_roots_of_polynomial+0xec0>
+	call   1393 <find_roots_of_polynomial+0xf83>
  R_X86_64_PLT32	realloc-0x4
 	mov    %rax,%rdi
 	mov    %rax,%rbp
-	call   12db <find_roots_of_polynomial+0xecb>
+	call   139e <find_roots_of_polynomial+0xf8e>
  R_X86_64_PLT32	strlen-0x4
 	lea    0x1(%rbp),%rdi
 	mov    %rbp,%rsi
 	lea    0x1(%rax),%rdx
-	call   12eb <find_roots_of_polynomial+0xedb>
+	call   13ae <find_roots_of_polynomial+0xf9e>
  R_X86_64_PLT32	memmove-0x4
 	mov    (%rsp),%rdi
 	movb   $0x2d,0x0(%rbp)
 	mov    0x10(%rsp),%rdx
 	lea    0x1(%rdi),%rsi
-	call   1301 <find_roots_of_polynomial+0xef1>
+	call   13c4 <find_roots_of_polynomial+0xfb4>
  R_X86_64_PLT32	memmove-0x4
 	jmp    581 <find_roots_of_polynomial+0x171>
 	mov    0xf8(%rsp),%rbp
-	jmp    117c <find_roots_of_polynomial+0xd6c>
-	call   1318 <find_roots_of_polynomial+0xf08>
+	jmp    123f <find_roots_of_polynomial+0xe2f>
+	call   13db <find_roots_of_polynomial+0xfcb>
  R_X86_64_PLT32	__stack_chk_fail-0x4
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -13,13 +13,13 @@
   0x00000090 38830747 0e60031f 010e3844 0e30410e 8..G.`....8D.0A.
   0x000000a0 28420e20 420e1842 0e10420e 08000000 (B. B..B..B.....
   0x000000b0 48000000 b4000000 00000000 3a010000 H...........:...
   0x000000c0 00460e10 8f02420e 188e0342 0e208d04 .F....B....B. ..
   0x000000d0 420e288c 05440e30 8606410e 38830748 B.(..D.0..A.8..H
   0x000000e0 0e600316 010e3841 0e30410e 28420e20 .`....8A.0A.(B. 
   0x000000f0 420e1842 0e10420e 08000000 50000000 B..B..B.....P...
-  0x00000100 00010000 00000000 080f0000 00460e10 .............F..
+  0x00000100 00010000 00000000 cb0f0000 00460e10 .............F..
   0x00000110 8f02420e 188e0345 0e208d04 450e288c ..B....E. ..E.(.
   0x00000120 05450e30 8606410e 3883074f 0ed00203 .E.0..A.8..O....
-  0x00000130 780c0a0e 38410e30 410e2842 0e20420e x...8A.0A.(B. B.
-  0x00000140 18420e10 420e0847 0b000000 00000000 .B..B..G........
+  0x00000130 4e0d0a0e 38440e30 410e2842 0e20420e N...8D.0A.(B. B.
+  0x00000140 18420e10 420e0846 0b000000 00000000 .B..B..F........
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -17,16 +17,16 @@
   0x000000e0 5f667261 6374696f 6e006669 6e645f72 _fraction.find_r
   0x000000f0 6f6f7473 5f6f665f 706f6c79 6e6f6d69 oots_of_polynomi
   0x00000100 616c5f64 69766964 655f706f 6c796e6f al_divide_polyno
   0x00000110 6d69616c 0066696e 645f726f 6f74735f mial.find_roots_
   0x00000120 6f665f70 6f6c796e 6f6d6961 6c007374 of_polynomial.st
   0x00000130 70637079 00737472 63687200 64697669 pcpy.strchr.divi
   0x00000140 64650069 6e637265 6d656e74 5f77686f de.increment_who
-  0x00000150 6c650073 7472636d 70007375 62747261 le.strcmp.subtra
-  0x00000160 63740074 65726d69 6e617469 6e675f64 ct.terminating_d
+  0x00000150 6c650073 75627472 61637400 73747263 le.subtract.strc
+  0x00000160 6d700074 65726d69 6e617469 6e675f64 mp.terminating_d
   0x00000170 6563696d 616c5f74 6f5f6672 61637469 ecimal_to_fracti
   0x00000180 6f6e0066 72616374 696f6e5f 746f5f63 on.fraction_to_c
   0x00000190 6f6e7469 6e756564 5f667261 6374696f ontinued_fractio
   0x000001a0 6e00636f 6e74696e 7565645f 66726163 n.continued_frac
   0x000001b0 74696f6e 5f746f5f 66726163 74696f6e tion_to_fraction
   0x000001c0 00616273 5f6d6f64 00657175 616c5f66 .abs_mod.equal_f
   0x000001d0 72616374 696f6e00 6d656d73 65740072 raction.memset.r
```

### Comparing `arithmetica-py-1.0.211/src/python-module/libbasic_math_operations.a` & `arithmetica-py-1.0.212/src/python-module/libbasic_math_operations.a`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.211/src/python-module/module.c` & `arithmetica-py-1.0.212/src/python-module/module.c`

 * *Files identical despite different names*

