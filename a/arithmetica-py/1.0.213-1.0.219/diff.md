# Comparing `tmp/arithmetica-py-1.0.213.tar.gz` & `tmp/arithmetica-py-1.0.219.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetica-py-1.0.213.tar", last modified: Fri Jun  9 08:34:19 2023, max compression
+gzip compressed data, was "arithmetica-py-1.0.219.tar", last modified: Fri Jun  9 12:58:27 2023, max compression
```

## Comparing `arithmetica-py-1.0.213.tar` & `arithmetica-py-1.0.219.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:34:19.112751 arithmetica-py-1.0.213/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-09 08:33:49.000000 arithmetica-py-1.0.213/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-09 08:34:19.112751 arithmetica-py-1.0.213/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-09 08:33:49.000000 arithmetica-py-1.0.213/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:34:19.112751 arithmetica-py-1.0.213/arithmetica_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-09 08:34:18.000000 arithmetica-py-1.0.213/arithmetica_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-09 08:34:19.000000 arithmetica-py-1.0.213/arithmetica_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:34:18.000000 arithmetica-py-1.0.213/arithmetica_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 08:34:18.000000 arithmetica-py-1.0.213/arithmetica_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:34:19.112751 arithmetica-py-1.0.213/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-09 08:33:49.000000 arithmetica-py-1.0.213/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:34:19.112751 arithmetica-py-1.0.213/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:34:19.112751 arithmetica-py-1.0.213/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)   187086 2023-06-09 08:34:18.000000 arithmetica-py-1.0.213/src/python-module/libarithmetica.a
--rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-06-09 08:34:18.000000 arithmetica-py-1.0.213/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-09 08:33:49.000000 arithmetica-py-1.0.213/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 08:34:18.000000 arithmetica-py-1.0.213/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:58:27.716378 arithmetica-py-1.0.219/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-09 12:57:49.000000 arithmetica-py-1.0.219/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-09 12:58:27.716378 arithmetica-py-1.0.219/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-09 12:57:49.000000 arithmetica-py-1.0.219/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:58:27.716378 arithmetica-py-1.0.219/arithmetica_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-09 12:58:27.000000 arithmetica-py-1.0.219/arithmetica_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-09 12:58:27.000000 arithmetica-py-1.0.219/arithmetica_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:58:27.000000 arithmetica-py-1.0.219/arithmetica_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 12:58:27.000000 arithmetica-py-1.0.219/arithmetica_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 12:58:27.716378 arithmetica-py-1.0.219/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-09 12:57:49.000000 arithmetica-py-1.0.219/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:58:27.712378 arithmetica-py-1.0.219/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:58:27.716378 arithmetica-py-1.0.219/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)   187086 2023-06-09 12:58:27.000000 arithmetica-py-1.0.219/src/python-module/libarithmetica.a
+-rw-r--r--   0 runner    (1001) docker     (123)    75064 2023-06-09 12:58:27.000000 arithmetica-py-1.0.219/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-09 12:57:49.000000 arithmetica-py-1.0.219/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 12:58:27.000000 arithmetica-py-1.0.219/src/python-module/version.txt
```

### Comparing `arithmetica-py-1.0.213/LICENSE` & `arithmetica-py-1.0.219/LICENSE`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.213/README.md` & `arithmetica-py-1.0.219/README.md`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.213/setup.py` & `arithmetica-py-1.0.219/setup.py`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.213/src/python-module/libarithmetica.a` & `arithmetica-py-1.0.219/src/python-module/libarithmetica.a`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.213/src/python-module/libbasic_math_operations.a` & `arithmetica-py-1.0.219/src/python-module/libbasic_math_operations.a`

 * *Files 2% similar despite different names*

#### file list

```diff
@@ -1,24 +1,24 @@
 ----------   0        0        0     2012 1970-01-01 00:00:00.000000 /
 ----------   0        0        0        0 1970-01-01 00:00:00.000000 //
 ?rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 basic_math_operations.c.o
 ?rw-r--r--   0        0        0    28944 1970-01-01 00:00:00.000000 basic_math_operations.cpp.o
-?rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 strlen_asm.asm.o
-?rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 remove_leading_zeroes.asm.o
+?rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 strlen_asm.asm.o
+?rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 remove_leading_zeroes.asm.o
 ?rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 add_whole.asm.o
 ?rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 add_whole_same_length.asm.o
 ?rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 add.c.o
 ?rw-r--r--   0        0        0     1632 1970-01-01 00:00:00.000000 subtract_whole.asm.o
 ?rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 subtract_whole_same_length.asm.o
 ?rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 subtractp.c.o
 ?rw-r--r--   0        0        0     1888 1970-01-01 00:00:00.000000 subtract.c.o
 ?rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 _multiply_whole.asm.o
 ?rw-r--r--   0        0        0     2552 1970-01-01 00:00:00.000000 multiplyp.c.o
 ?rw-r--r--   0        0        0     2016 1970-01-01 00:00:00.000000 multiply.c.o
-?rw-r--r--   0        0        0     2896 1970-01-01 00:00:00.000000 _divide_whole_with_remainder.asm.o
+?rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 _divide_whole_with_remainder.asm.o
 ?rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 divide_whole_with_remainder.c.o
 ?rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 divide_whole.c.o
 ?rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 dividep.c.o
 ?rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 divide.c.o
 ?rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 abs_mod.c.o
 ?rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 asmalloc.asm.o
 ?rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 multiply_whole.asm.o
```

#### strlen_asm.asm.o

##### readelf --wide --sections {}

```diff
@@ -2,13 +2,13 @@
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000180 000014 00  AX  0   0 16
   [ 2] .shstrtab         STRTAB          0000000000000000 0001a0 000021 00      0   0  1
   [ 3] .symtab           SYMTAB          0000000000000000 0001d0 000078 18      4   4  8
-  [ 4] .strtab           STRTAB          0000000000000000 000250 000081 00      0   0  1
+  [ 4] .strtab           STRTAB          0000000000000000 000250 00007b 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,8 +1,8 @@
 
 Symbol table '.symtab' contains 5 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/strlen_asm.asm
+     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/strlen_asm.asm
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
      3: 0000000000000009     0 NOTYPE  LOCAL  DEFAULT    1 strlen_asm.loop
      4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT    1 strlen_asm
```

##### strings --all --bytes=8 {}

```diff
@@ -1,4 +1,4 @@
 .shstrtab
-/home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/strlen_asm.asm
+/home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/strlen_asm.asm
 strlen_asm
 strlen_asm.loop
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,12 +1,11 @@
 
 Hex dump of section '.strtab':
   0x00000000 002f686f 6d652f72 756e6e65 722f776f ./home/runner/wo
   0x00000010 726b2f61 72697468 6d657469 63612f61 rk/arithmetica/a
-  0x00000020 72697468 6d657469 63612f73 72632f62 rithmetica/src/b
-  0x00000030 61736963 5f6d6174 685f6f70 65726174 asic_math_operat
-  0x00000040 696f6e73 2f737263 2f6c6962 72617279 ions/src/library
-  0x00000050 2f6c696e 75782f73 74726c65 6e5f6173 /linux/strlen_as
-  0x00000060 6d2e6173 6d007374 726c656e 5f61736d m.asm.strlen_asm
-  0x00000070 00737472 6c656e5f 61736d2e 6c6f6f70 .strlen_asm.loop
-  0x00000080 00                                  .
+  0x00000020 72697468 6d657469 63612f62 75696c64 rithmetica/build
+  0x00000030 2f5f6465 70732f62 6d6f2d73 72632f73 /_deps/bmo-src/s
+  0x00000040 72632f6c 69627261 72792f6c 696e7578 rc/library/linux
+  0x00000050 2f737472 6c656e5f 61736d2e 61736d00 /strlen_asm.asm.
+  0x00000060 7374726c 656e5f61 736d0073 74726c65 strlen_asm.strle
+  0x00000070 6e5f6173 6d2e6c6f 6f7000            n_asm.loop.
```

#### remove_leading_zeroes.asm.o

##### readelf --wide --sections {}

```diff
@@ -2,14 +2,14 @@
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 0001c0 00009b 00  AX  0   0 16
   [ 2] .shstrtab         STRTAB          0000000000000000 000260 00002c 00      0   0  1
   [ 3] .symtab           SYMTAB          0000000000000000 000290 000138 18      4  10  8
-  [ 4] .strtab           STRTAB          0000000000000000 0003d0 0001a4 00      0   0  1
-  [ 5] .rela.text        RELA            0000000000000000 000580 000030 18      3   1  8
+  [ 4] .strtab           STRTAB          0000000000000000 0003d0 00019e 00      0   0  1
+  [ 5] .rela.text        RELA            0000000000000000 000570 000030 18      3   1  8
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,12 +1,12 @@
 
 Symbol table '.symtab' contains 13 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/remove_leading_zeroes.asm
+     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/remove_leading_zeroes.asm
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
      3: 0000000000000020     0 NOTYPE  LOCAL  DEFAULT    1 remove_leading_zeroes.loop_1
      4: 0000000000000029     0 NOTYPE  LOCAL  DEFAULT    1 remove_leading_zeroes.after_if_1
      5: 0000000000000043     0 NOTYPE  LOCAL  DEFAULT    1 remove_leading_zeroes.after_if_2
      6: 0000000000000055     0 NOTYPE  LOCAL  DEFAULT    1 remove_leading_zeroes_inplace.loop_1
      7: 0000000000000072     0 NOTYPE  LOCAL  DEFAULT    1 remove_leading_zeroes_inplace.after_if_1
      8: 000000000000008a     0 NOTYPE  LOCAL  DEFAULT    1 remove_leading_zeroes_inplace.loop_2
```

##### readelf --wide --relocs {}

```diff
@@ -1,5 +1,5 @@
 
-Relocation section '.rela.text' at offset 0x580 contains 2 entries:
+Relocation section '.rela.text' at offset 0x570 contains 2 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000001  0000000a00000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 000000000000007d  0000000a00000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 .shstrtab
 .rela.text
-/home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/remove_leading_zeroes.asm
+/home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/remove_leading_zeroes.asm
 strlen_asm
 remove_leading_zeroes
 remove_leading_zeroes.loop_1
 remove_leading_zeroes.after_if_1
 remove_leading_zeroes.after_if_2
 remove_leading_zeroes_inplace
 remove_leading_zeroes_inplace.loop_1
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,30 +1,29 @@
 
 Hex dump of section '.strtab':
   0x00000000 002f686f 6d652f72 756e6e65 722f776f ./home/runner/wo
   0x00000010 726b2f61 72697468 6d657469 63612f61 rk/arithmetica/a
-  0x00000020 72697468 6d657469 63612f73 72632f62 rithmetica/src/b
-  0x00000030 61736963 5f6d6174 685f6f70 65726174 asic_math_operat
-  0x00000040 696f6e73 2f737263 2f6c6962 72617279 ions/src/library
-  0x00000050 2f6c696e 75782f72 656d6f76 655f6c65 /linux/remove_le
-  0x00000060 6164696e 675f7a65 726f6573 2e61736d ading_zeroes.asm
-  0x00000070 00737472 6c656e5f 61736d00 72656d6f .strlen_asm.remo
-  0x00000080 76655f6c 65616469 6e675f7a 65726f65 ve_leading_zeroe
-  0x00000090 73007265 6d6f7665 5f6c6561 64696e67 s.remove_leading
-  0x000000a0 5f7a6572 6f65732e 6c6f6f70 5f310072 _zeroes.loop_1.r
-  0x000000b0 656d6f76 655f6c65 6164696e 675f7a65 emove_leading_ze
-  0x000000c0 726f6573 2e616674 65725f69 665f3100 roes.after_if_1.
-  0x000000d0 72656d6f 76655f6c 65616469 6e675f7a remove_leading_z
-  0x000000e0 65726f65 732e6166 7465725f 69665f32 eroes.after_if_2
-  0x000000f0 0072656d 6f76655f 6c656164 696e675f .remove_leading_
-  0x00000100 7a65726f 65735f69 6e706c61 63650072 zeroes_inplace.r
-  0x00000110 656d6f76 655f6c65 6164696e 675f7a65 emove_leading_ze
-  0x00000120 726f6573 5f696e70 6c616365 2e6c6f6f roes_inplace.loo
-  0x00000130 705f3100 72656d6f 76655f6c 65616469 p_1.remove_leadi
-  0x00000140 6e675f7a 65726f65 735f696e 706c6163 ng_zeroes_inplac
-  0x00000150 652e6166 7465725f 69665f31 0072656d e.after_if_1.rem
-  0x00000160 6f76655f 6c656164 696e675f 7a65726f ove_leading_zero
-  0x00000170 65735f69 6e706c61 63652e6c 6f6f705f es_inplace.loop_
-  0x00000180 32007265 6d6f7665 5f6c6561 64696e67 2.remove_leading
-  0x00000190 5f7a6572 6f65735f 696e706c 6163652e _zeroes_inplace.
-  0x000001a0 656e6400                            end.
+  0x00000020 72697468 6d657469 63612f62 75696c64 rithmetica/build
+  0x00000030 2f5f6465 70732f62 6d6f2d73 72632f73 /_deps/bmo-src/s
+  0x00000040 72632f6c 69627261 72792f6c 696e7578 rc/library/linux
+  0x00000050 2f72656d 6f76655f 6c656164 696e675f /remove_leading_
+  0x00000060 7a65726f 65732e61 736d0073 74726c65 zeroes.asm.strle
+  0x00000070 6e5f6173 6d007265 6d6f7665 5f6c6561 n_asm.remove_lea
+  0x00000080 64696e67 5f7a6572 6f657300 72656d6f ding_zeroes.remo
+  0x00000090 76655f6c 65616469 6e675f7a 65726f65 ve_leading_zeroe
+  0x000000a0 732e6c6f 6f705f31 0072656d 6f76655f s.loop_1.remove_
+  0x000000b0 6c656164 696e675f 7a65726f 65732e61 leading_zeroes.a
+  0x000000c0 66746572 5f69665f 31007265 6d6f7665 fter_if_1.remove
+  0x000000d0 5f6c6561 64696e67 5f7a6572 6f65732e _leading_zeroes.
+  0x000000e0 61667465 725f6966 5f320072 656d6f76 after_if_2.remov
+  0x000000f0 655f6c65 6164696e 675f7a65 726f6573 e_leading_zeroes
+  0x00000100 5f696e70 6c616365 0072656d 6f76655f _inplace.remove_
+  0x00000110 6c656164 696e675f 7a65726f 65735f69 leading_zeroes_i
+  0x00000120 6e706c61 63652e6c 6f6f705f 31007265 nplace.loop_1.re
+  0x00000130 6d6f7665 5f6c6561 64696e67 5f7a6572 move_leading_zer
+  0x00000140 6f65735f 696e706c 6163652e 61667465 oes_inplace.afte
+  0x00000150 725f6966 5f310072 656d6f76 655f6c65 r_if_1.remove_le
+  0x00000160 6164696e 675f7a65 726f6573 5f696e70 ading_zeroes_inp
+  0x00000170 6c616365 2e6c6f6f 705f3200 72656d6f lace.loop_2.remo
+  0x00000180 76655f6c 65616469 6e675f7a 65726f65 ve_leading_zeroe
+  0x00000190 735f696e 706c6163 652e656e 6400     s_inplace.end.
```

#### add_whole.asm.o

##### readelf --wide --sections {}

```diff
@@ -2,14 +2,14 @@
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 0001c0 000092 00  AX  0   0 16
   [ 2] .shstrtab         STRTAB          0000000000000000 000260 00002c 00      0   0  1
   [ 3] .symtab           SYMTAB          0000000000000000 000290 000150 18      4  12  8
-  [ 4] .strtab           STRTAB          0000000000000000 0003e0 00011c 00      0   0  1
+  [ 4] .strtab           STRTAB          0000000000000000 0003e0 000116 00      0   0  1
   [ 5] .rela.text        RELA            0000000000000000 000500 000030 18      3   1  8
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,12 +1,12 @@
 
 Symbol table '.symtab' contains 14 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/add_whole.asm
+     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/add_whole.asm
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
      3: 000000000000001a     0 NOTYPE  LOCAL  DEFAULT    1 add_whole.no_swap
      4: 000000000000002f     0 NOTYPE  LOCAL  DEFAULT    1 add_whole.loop_a
      5: 0000000000000046     0 NOTYPE  LOCAL  DEFAULT    1 add_whole.char_ok
      6: 0000000000000057     0 NOTYPE  LOCAL  DEFAULT    1 add_whole.no_loop_a
      7: 000000000000005c     0 NOTYPE  LOCAL  DEFAULT    1 add_whole.loop_b
      8: 000000000000006d     0 NOTYPE  LOCAL  DEFAULT    1 add_whole.char_ok_
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 .shstrtab
 .rela.text
-/home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/add_whole.asm
+/home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/add_whole.asm
 strlen_asm
 add_whole
 add_whole.no_swap
 add_whole.loop_a
 add_whole.char_ok
 add_whole.no_loop_a
 add_whole.loop_b
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,21 +1,21 @@
 
 Hex dump of section '.strtab':
   0x00000000 002f686f 6d652f72 756e6e65 722f776f ./home/runner/wo
   0x00000010 726b2f61 72697468 6d657469 63612f61 rk/arithmetica/a
-  0x00000020 72697468 6d657469 63612f73 72632f62 rithmetica/src/b
-  0x00000030 61736963 5f6d6174 685f6f70 65726174 asic_math_operat
-  0x00000040 696f6e73 2f737263 2f6c6962 72617279 ions/src/library
-  0x00000050 2f6c696e 75782f61 64645f77 686f6c65 /linux/add_whole
-  0x00000060 2e61736d 00737472 6c656e5f 61736d00 .asm.strlen_asm.
-  0x00000070 6164645f 77686f6c 65006164 645f7768 add_whole.add_wh
-  0x00000080 6f6c652e 6e6f5f73 77617000 6164645f ole.no_swap.add_
-  0x00000090 77686f6c 652e6c6f 6f705f61 00616464 whole.loop_a.add
-  0x000000a0 5f77686f 6c652e63 6861725f 6f6b0061 _whole.char_ok.a
-  0x000000b0 64645f77 686f6c65 2e6e6f5f 6c6f6f70 dd_whole.no_loop
-  0x000000c0 5f610061 64645f77 686f6c65 2e6c6f6f _a.add_whole.loo
-  0x000000d0 705f6200 6164645f 77686f6c 652e6368 p_b.add_whole.ch
-  0x000000e0 61725f6f 6b5f0061 64645f77 686f6c65 ar_ok_.add_whole
-  0x000000f0 2e6e6f5f 6c6f6f70 5f620061 64645f77 .no_loop_b.add_w
-  0x00000100 686f6c65 2e636f70 795f7570 00616464 hole.copy_up.add
-  0x00000110 5f77686f 6c652e64 6f6e6500          _whole.done.
+  0x00000020 72697468 6d657469 63612f62 75696c64 rithmetica/build
+  0x00000030 2f5f6465 70732f62 6d6f2d73 72632f73 /_deps/bmo-src/s
+  0x00000040 72632f6c 69627261 72792f6c 696e7578 rc/library/linux
+  0x00000050 2f616464 5f77686f 6c652e61 736d0073 /add_whole.asm.s
+  0x00000060 74726c65 6e5f6173 6d006164 645f7768 trlen_asm.add_wh
+  0x00000070 6f6c6500 6164645f 77686f6c 652e6e6f ole.add_whole.no
+  0x00000080 5f737761 70006164 645f7768 6f6c652e _swap.add_whole.
+  0x00000090 6c6f6f70 5f610061 64645f77 686f6c65 loop_a.add_whole
+  0x000000a0 2e636861 725f6f6b 00616464 5f77686f .char_ok.add_who
+  0x000000b0 6c652e6e 6f5f6c6f 6f705f61 00616464 le.no_loop_a.add
+  0x000000c0 5f77686f 6c652e6c 6f6f705f 62006164 _whole.loop_b.ad
+  0x000000d0 645f7768 6f6c652e 63686172 5f6f6b5f d_whole.char_ok_
+  0x000000e0 00616464 5f77686f 6c652e6e 6f5f6c6f .add_whole.no_lo
+  0x000000f0 6f705f62 00616464 5f77686f 6c652e63 op_b.add_whole.c
+  0x00000100 6f70795f 75700061 64645f77 686f6c65 opy_up.add_whole
+  0x00000110 2e646f6e 6500                       .done.
```

#### add_whole_same_length.asm.o

##### readelf --wide --sections {}

```diff
@@ -2,14 +2,14 @@
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 0001c0 000088 00  AX  0   0 16
   [ 2] .shstrtab         STRTAB          0000000000000000 000250 00002c 00      0   0  1
   [ 3] .symtab           SYMTAB          0000000000000000 000280 0000f0 18      4   8  8
-  [ 4] .strtab           STRTAB          0000000000000000 000370 00012f 00      0   0  1
+  [ 4] .strtab           STRTAB          0000000000000000 000370 000129 00      0   0  1
   [ 5] .rela.text        RELA            0000000000000000 0004a0 000018 18      3   1  8
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,12 +1,12 @@
 
 Symbol table '.symtab' contains 10 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/add_whole_same_length.asm
+     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/add_whole_same_length.asm
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
      3: 0000000000000011     0 NOTYPE  LOCAL  DEFAULT    1 add_whole_same_length.loop_1
      4: 0000000000000028     0 NOTYPE  LOCAL  DEFAULT    1 add_whole_same_length.after_if_1
      5: 0000000000000035     0 NOTYPE  LOCAL  DEFAULT    1 add_whole_same_length.after_if_2
      6: 0000000000000055     0 NOTYPE  LOCAL  DEFAULT    1 add_whole_same_length.after_if_3
      7: 000000000000005e     0 NOTYPE  LOCAL  DEFAULT    1 add_whole_same_length.loop_2
      8: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen_asm
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 .shstrtab
 .rela.text
-/home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/add_whole_same_length.asm
+/home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/add_whole_same_length.asm
 strlen_asm
 add_whole_same_length
 add_whole_same_length.loop_1
 add_whole_same_length.after_if_1
 add_whole_same_length.after_if_2
 add_whole_same_length.after_if_3
 add_whole_same_length.loop_2
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,22 +1,22 @@
 
 Hex dump of section '.strtab':
   0x00000000 002f686f 6d652f72 756e6e65 722f776f ./home/runner/wo
   0x00000010 726b2f61 72697468 6d657469 63612f61 rk/arithmetica/a
-  0x00000020 72697468 6d657469 63612f73 72632f62 rithmetica/src/b
-  0x00000030 61736963 5f6d6174 685f6f70 65726174 asic_math_operat
-  0x00000040 696f6e73 2f737263 2f6c6962 72617279 ions/src/library
-  0x00000050 2f6c696e 75782f61 64645f77 686f6c65 /linux/add_whole
-  0x00000060 5f73616d 655f6c65 6e677468 2e61736d _same_length.asm
-  0x00000070 00737472 6c656e5f 61736d00 6164645f .strlen_asm.add_
-  0x00000080 77686f6c 655f7361 6d655f6c 656e6774 whole_same_lengt
-  0x00000090 68006164 645f7768 6f6c655f 73616d65 h.add_whole_same
-  0x000000a0 5f6c656e 6774682e 6c6f6f70 5f310061 _length.loop_1.a
-  0x000000b0 64645f77 686f6c65 5f73616d 655f6c65 dd_whole_same_le
-  0x000000c0 6e677468 2e616674 65725f69 665f3100 ngth.after_if_1.
-  0x000000d0 6164645f 77686f6c 655f7361 6d655f6c add_whole_same_l
-  0x000000e0 656e6774 682e6166 7465725f 69665f32 ength.after_if_2
-  0x000000f0 00616464 5f77686f 6c655f73 616d655f .add_whole_same_
-  0x00000100 6c656e67 74682e61 66746572 5f69665f length.after_if_
-  0x00000110 33006164 645f7768 6f6c655f 73616d65 3.add_whole_same
-  0x00000120 5f6c656e 6774682e 6c6f6f70 5f3200   _length.loop_2.
+  0x00000020 72697468 6d657469 63612f62 75696c64 rithmetica/build
+  0x00000030 2f5f6465 70732f62 6d6f2d73 72632f73 /_deps/bmo-src/s
+  0x00000040 72632f6c 69627261 72792f6c 696e7578 rc/library/linux
+  0x00000050 2f616464 5f77686f 6c655f73 616d655f /add_whole_same_
+  0x00000060 6c656e67 74682e61 736d0073 74726c65 length.asm.strle
+  0x00000070 6e5f6173 6d006164 645f7768 6f6c655f n_asm.add_whole_
+  0x00000080 73616d65 5f6c656e 67746800 6164645f same_length.add_
+  0x00000090 77686f6c 655f7361 6d655f6c 656e6774 whole_same_lengt
+  0x000000a0 682e6c6f 6f705f31 00616464 5f77686f h.loop_1.add_who
+  0x000000b0 6c655f73 616d655f 6c656e67 74682e61 le_same_length.a
+  0x000000c0 66746572 5f69665f 31006164 645f7768 fter_if_1.add_wh
+  0x000000d0 6f6c655f 73616d65 5f6c656e 6774682e ole_same_length.
+  0x000000e0 61667465 725f6966 5f320061 64645f77 after_if_2.add_w
+  0x000000f0 686f6c65 5f73616d 655f6c65 6e677468 hole_same_length
+  0x00000100 2e616674 65725f69 665f3300 6164645f .after_if_3.add_
+  0x00000110 77686f6c 655f7361 6d655f6c 656e6774 whole_same_lengt
+  0x00000120 682e6c6f 6f705f32 00                h.loop_2.
```

#### subtract_whole.asm.o

##### readelf --wide --sections {}

```diff
@@ -2,14 +2,14 @@
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 0001c0 000103 00  AX  0   0 16
   [ 2] .shstrtab         STRTAB          0000000000000000 0002d0 00002c 00      0   0  1
   [ 3] .symtab           SYMTAB          0000000000000000 000300 000180 18      4  14  8
-  [ 4] .strtab           STRTAB          0000000000000000 000480 00018b 00      0   0  1
+  [ 4] .strtab           STRTAB          0000000000000000 000480 000185 00      0   0  1
   [ 5] .rela.text        RELA            0000000000000000 000610 000048 18      3   1  8
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,12 +1,12 @@
 
 Symbol table '.symtab' contains 16 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/subtract_whole.asm
+     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/subtract_whole.asm
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
      3: 000000000000002f     0 NOTYPE  LOCAL  DEFAULT    1 subtract_whole.loop_1
      4: 0000000000000044     0 NOTYPE  LOCAL  DEFAULT    1 subtract_whole.after_if_1
      5: 0000000000000054     0 NOTYPE  LOCAL  DEFAULT    1 subtract_whole.after_if_2
      6: 000000000000006b     0 NOTYPE  LOCAL  DEFAULT    1 subtract_whole.else_1
      7: 0000000000000078     0 NOTYPE  LOCAL  DEFAULT    1 subtract_whole.after_else_1
      8: 0000000000000098     0 NOTYPE  LOCAL  DEFAULT    1 subtract_whole.loop_2
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 .shstrtab
 .rela.text
-/home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/subtract_whole.asm
+/home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/subtract_whole.asm
 strlen_asm
 subtract_whole
 subtract_whole.loop_1
 subtract_whole.after_if_1
 subtract_whole.after_if_2
 subtract_whole.else_1
 subtract_whole.after_else_1
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,28 +1,28 @@
 
 Hex dump of section '.strtab':
   0x00000000 002f686f 6d652f72 756e6e65 722f776f ./home/runner/wo
   0x00000010 726b2f61 72697468 6d657469 63612f61 rk/arithmetica/a
-  0x00000020 72697468 6d657469 63612f73 72632f62 rithmetica/src/b
-  0x00000030 61736963 5f6d6174 685f6f70 65726174 asic_math_operat
-  0x00000040 696f6e73 2f737263 2f6c6962 72617279 ions/src/library
-  0x00000050 2f6c696e 75782f73 75627472 6163745f /linux/subtract_
-  0x00000060 77686f6c 652e6173 6d007374 726c656e whole.asm.strlen
-  0x00000070 5f61736d 00737562 74726163 745f7768 _asm.subtract_wh
-  0x00000080 6f6c6500 73756274 72616374 5f77686f ole.subtract_who
-  0x00000090 6c652e6c 6f6f705f 31007375 62747261 le.loop_1.subtra
-  0x000000a0 63745f77 686f6c65 2e616674 65725f69 ct_whole.after_i
-  0x000000b0 665f3100 73756274 72616374 5f77686f f_1.subtract_who
-  0x000000c0 6c652e61 66746572 5f69665f 32007375 le.after_if_2.su
-  0x000000d0 62747261 63745f77 686f6c65 2e656c73 btract_whole.els
-  0x000000e0 655f3100 73756274 72616374 5f77686f e_1.subtract_who
-  0x000000f0 6c652e61 66746572 5f656c73 655f3100 le.after_else_1.
-  0x00000100 73756274 72616374 5f77686f 6c652e6c subtract_whole.l
-  0x00000110 6f6f705f 32007375 62747261 63745f77 oop_2.subtract_w
-  0x00000120 686f6c65 2e616674 65725f69 665f3300 hole.after_if_3.
-  0x00000130 73756274 72616374 5f77686f 6c652e6c subtract_whole.l
-  0x00000140 6f6f705f 33007375 62747261 63745f77 oop_3.subtract_w
-  0x00000150 686f6c65 2e656c73 655f3200 73756274 hole.else_2.subt
-  0x00000160 72616374 5f77686f 6c652e61 66746572 ract_whole.after
-  0x00000170 5f656c73 655f3200 73756274 72616374 _else_2.subtract
-  0x00000180 5f77686f 6c652e72 657400            _whole.ret.
+  0x00000020 72697468 6d657469 63612f62 75696c64 rithmetica/build
+  0x00000030 2f5f6465 70732f62 6d6f2d73 72632f73 /_deps/bmo-src/s
+  0x00000040 72632f6c 69627261 72792f6c 696e7578 rc/library/linux
+  0x00000050 2f737562 74726163 745f7768 6f6c652e /subtract_whole.
+  0x00000060 61736d00 7374726c 656e5f61 736d0073 asm.strlen_asm.s
+  0x00000070 75627472 6163745f 77686f6c 65007375 ubtract_whole.su
+  0x00000080 62747261 63745f77 686f6c65 2e6c6f6f btract_whole.loo
+  0x00000090 705f3100 73756274 72616374 5f77686f p_1.subtract_who
+  0x000000a0 6c652e61 66746572 5f69665f 31007375 le.after_if_1.su
+  0x000000b0 62747261 63745f77 686f6c65 2e616674 btract_whole.aft
+  0x000000c0 65725f69 665f3200 73756274 72616374 er_if_2.subtract
+  0x000000d0 5f77686f 6c652e65 6c73655f 31007375 _whole.else_1.su
+  0x000000e0 62747261 63745f77 686f6c65 2e616674 btract_whole.aft
+  0x000000f0 65725f65 6c73655f 31007375 62747261 er_else_1.subtra
+  0x00000100 63745f77 686f6c65 2e6c6f6f 705f3200 ct_whole.loop_2.
+  0x00000110 73756274 72616374 5f77686f 6c652e61 subtract_whole.a
+  0x00000120 66746572 5f69665f 33007375 62747261 fter_if_3.subtra
+  0x00000130 63745f77 686f6c65 2e6c6f6f 705f3300 ct_whole.loop_3.
+  0x00000140 73756274 72616374 5f77686f 6c652e65 subtract_whole.e
+  0x00000150 6c73655f 32007375 62747261 63745f77 lse_2.subtract_w
+  0x00000160 686f6c65 2e616674 65725f65 6c73655f hole.after_else_
+  0x00000170 32007375 62747261 63745f77 686f6c65 2.subtract_whole
+  0x00000180 2e726574 00                         .ret.
```

#### subtract_whole_same_length.asm.o

##### readelf --wide --sections {}

```diff
@@ -2,14 +2,14 @@
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 0001c0 0000c9 00  AX  0   0 16
   [ 2] .shstrtab         STRTAB          0000000000000000 000290 00002c 00      0   0  1
   [ 3] .symtab           SYMTAB          0000000000000000 0002c0 000150 18      4  12  8
-  [ 4] .strtab           STRTAB          0000000000000000 000410 0001db 00      0   0  1
+  [ 4] .strtab           STRTAB          0000000000000000 000410 0001d5 00      0   0  1
   [ 5] .rela.text        RELA            0000000000000000 0005f0 000030 18      3   1  8
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,12 +1,12 @@
 
 Symbol table '.symtab' contains 14 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/subtract_whole_same_length.asm
+     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/subtract_whole_same_length.asm
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
      3: 000000000000000b     0 NOTYPE  LOCAL  DEFAULT    1 subtract_whole_same_length.loop_1
      4: 000000000000002b     0 NOTYPE  LOCAL  DEFAULT    1 subtract_whole_same_length.else_1
      5: 000000000000003c     0 NOTYPE  LOCAL  DEFAULT    1 subtract_whole_same_length.after_else_1
      6: 0000000000000061     0 NOTYPE  LOCAL  DEFAULT    1 subtract_whole_same_length.loop_2
      7: 0000000000000079     0 NOTYPE  LOCAL  DEFAULT    1 subtract_whole_same_length.after_if_2
      8: 0000000000000094     0 NOTYPE  LOCAL  DEFAULT    1 subtract_whole_same_length.loop_3
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 .shstrtab
 .rela.text
-/home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/subtract_whole_same_length.asm
+/home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/subtract_whole_same_length.asm
 strlen_asm
 subtract_whole_same_length
 subtract_whole_same_length.loop_1
 subtract_whole_same_length.else_1
 subtract_whole_same_length.after_else_1
 subtract_whole_same_length.loop_2
 subtract_whole_same_length.after_if_2
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,33 +1,33 @@
 
 Hex dump of section '.strtab':
   0x00000000 002f686f 6d652f72 756e6e65 722f776f ./home/runner/wo
   0x00000010 726b2f61 72697468 6d657469 63612f61 rk/arithmetica/a
-  0x00000020 72697468 6d657469 63612f73 72632f62 rithmetica/src/b
-  0x00000030 61736963 5f6d6174 685f6f70 65726174 asic_math_operat
-  0x00000040 696f6e73 2f737263 2f6c6962 72617279 ions/src/library
-  0x00000050 2f6c696e 75782f73 75627472 6163745f /linux/subtract_
-  0x00000060 77686f6c 655f7361 6d655f6c 656e6774 whole_same_lengt
-  0x00000070 682e6173 6d007374 726c656e 5f61736d h.asm.strlen_asm
-  0x00000080 00737562 74726163 745f7768 6f6c655f .subtract_whole_
-  0x00000090 73616d65 5f6c656e 67746800 73756274 same_length.subt
-  0x000000a0 72616374 5f77686f 6c655f73 616d655f ract_whole_same_
-  0x000000b0 6c656e67 74682e6c 6f6f705f 31007375 length.loop_1.su
-  0x000000c0 62747261 63745f77 686f6c65 5f73616d btract_whole_sam
-  0x000000d0 655f6c65 6e677468 2e656c73 655f3100 e_length.else_1.
-  0x000000e0 73756274 72616374 5f77686f 6c655f73 subtract_whole_s
-  0x000000f0 616d655f 6c656e67 74682e61 66746572 ame_length.after
-  0x00000100 5f656c73 655f3100 73756274 72616374 _else_1.subtract
-  0x00000110 5f77686f 6c655f73 616d655f 6c656e67 _whole_same_leng
-  0x00000120 74682e6c 6f6f705f 32007375 62747261 th.loop_2.subtra
-  0x00000130 63745f77 686f6c65 5f73616d 655f6c65 ct_whole_same_le
-  0x00000140 6e677468 2e616674 65725f69 665f3200 ngth.after_if_2.
-  0x00000150 73756274 72616374 5f77686f 6c655f73 subtract_whole_s
-  0x00000160 616d655f 6c656e67 74682e6c 6f6f705f ame_length.loop_
-  0x00000170 33007375 62747261 63745f77 686f6c65 3.subtract_whole
-  0x00000180 5f73616d 655f6c65 6e677468 2e656c73 _same_length.els
-  0x00000190 655f3200 73756274 72616374 5f77686f e_2.subtract_who
-  0x000001a0 6c655f73 616d655f 6c656e67 74682e61 le_same_length.a
-  0x000001b0 66746572 5f656c73 655f3200 73756274 fter_else_2.subt
-  0x000001c0 72616374 5f77686f 6c655f73 616d655f ract_whole_same_
-  0x000001d0 6c656e67 74682e72 657400            length.ret.
+  0x00000020 72697468 6d657469 63612f62 75696c64 rithmetica/build
+  0x00000030 2f5f6465 70732f62 6d6f2d73 72632f73 /_deps/bmo-src/s
+  0x00000040 72632f6c 69627261 72792f6c 696e7578 rc/library/linux
+  0x00000050 2f737562 74726163 745f7768 6f6c655f /subtract_whole_
+  0x00000060 73616d65 5f6c656e 6774682e 61736d00 same_length.asm.
+  0x00000070 7374726c 656e5f61 736d0073 75627472 strlen_asm.subtr
+  0x00000080 6163745f 77686f6c 655f7361 6d655f6c act_whole_same_l
+  0x00000090 656e6774 68007375 62747261 63745f77 ength.subtract_w
+  0x000000a0 686f6c65 5f73616d 655f6c65 6e677468 hole_same_length
+  0x000000b0 2e6c6f6f 705f3100 73756274 72616374 .loop_1.subtract
+  0x000000c0 5f77686f 6c655f73 616d655f 6c656e67 _whole_same_leng
+  0x000000d0 74682e65 6c73655f 31007375 62747261 th.else_1.subtra
+  0x000000e0 63745f77 686f6c65 5f73616d 655f6c65 ct_whole_same_le
+  0x000000f0 6e677468 2e616674 65725f65 6c73655f ngth.after_else_
+  0x00000100 31007375 62747261 63745f77 686f6c65 1.subtract_whole
+  0x00000110 5f73616d 655f6c65 6e677468 2e6c6f6f _same_length.loo
+  0x00000120 705f3200 73756274 72616374 5f77686f p_2.subtract_who
+  0x00000130 6c655f73 616d655f 6c656e67 74682e61 le_same_length.a
+  0x00000140 66746572 5f69665f 32007375 62747261 fter_if_2.subtra
+  0x00000150 63745f77 686f6c65 5f73616d 655f6c65 ct_whole_same_le
+  0x00000160 6e677468 2e6c6f6f 705f3300 73756274 ngth.loop_3.subt
+  0x00000170 72616374 5f77686f 6c655f73 616d655f ract_whole_same_
+  0x00000180 6c656e67 74682e65 6c73655f 32007375 length.else_2.su
+  0x00000190 62747261 63745f77 686f6c65 5f73616d btract_whole_sam
+  0x000001a0 655f6c65 6e677468 2e616674 65725f65 e_length.after_e
+  0x000001b0 6c73655f 32007375 62747261 63745f77 lse_2.subtract_w
+  0x000001c0 686f6c65 5f73616d 655f6c65 6e677468 hole_same_length
+  0x000001d0 2e726574 00                         .ret.
```

#### _multiply_whole.asm.o

##### readelf --wide --sections {}

```diff
@@ -2,14 +2,14 @@
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 0001c0 00011c 00  AX  0   0 16
   [ 2] .shstrtab         STRTAB          0000000000000000 0002e0 00002c 00      0   0  1
   [ 3] .symtab           SYMTAB          0000000000000000 000310 000120 18      4   9  8
-  [ 4] .strtab           STRTAB          0000000000000000 000430 000120 00      0   0  1
+  [ 4] .strtab           STRTAB          0000000000000000 000430 00011a 00      0   0  1
   [ 5] .rela.text        RELA            0000000000000000 000550 000078 18      3   1  8
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,12 +1,12 @@
 
 Symbol table '.symtab' contains 12 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/_multiply_whole.asm
+     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/_multiply_whole.asm
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
      3: 0000000000000033     0 NOTYPE  LOCAL  DEFAULT    1 _multiply_whole.loop_1
      4: 0000000000000044     0 NOTYPE  LOCAL  DEFAULT    1 _multiply_whole.loop_2
      5: 000000000000008a     0 NOTYPE  LOCAL  DEFAULT    1 _multiply_whole.loop_3
      6: 000000000000009a     0 NOTYPE  LOCAL  DEFAULT    1 _multiply_whole.after_loop_3
      7: 00000000000000ca     0 NOTYPE  LOCAL  DEFAULT    1 _multiply_whole.loop_4
      8: 00000000000000e2     0 NOTYPE  LOCAL  DEFAULT    1 _multiply_whole.loop_5
```

##### strings --all --bytes=8 {}

```diff
@@ -1,12 +1,12 @@
 SATAUAVAWI
 A_A^A]A\[
 .shstrtab
 .rela.text
-/home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/_multiply_whole.asm
+/home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/_multiply_whole.asm
 add_whole
 strlen_asm
 _multiply_whole
 _multiply_whole.loop_1
 _multiply_whole.loop_2
 _multiply_whole.loop_3
 _multiply_whole.after_loop_3
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,21 +1,21 @@
 
 Hex dump of section '.strtab':
   0x00000000 002f686f 6d652f72 756e6e65 722f776f ./home/runner/wo
   0x00000010 726b2f61 72697468 6d657469 63612f61 rk/arithmetica/a
-  0x00000020 72697468 6d657469 63612f73 72632f62 rithmetica/src/b
-  0x00000030 61736963 5f6d6174 685f6f70 65726174 asic_math_operat
-  0x00000040 696f6e73 2f737263 2f6c6962 72617279 ions/src/library
-  0x00000050 2f6c696e 75782f5f 6d756c74 69706c79 /linux/_multiply
-  0x00000060 5f77686f 6c652e61 736d0061 64645f77 _whole.asm.add_w
-  0x00000070 686f6c65 00737472 6c656e5f 61736d00 hole.strlen_asm.
-  0x00000080 5f6d756c 7469706c 795f7768 6f6c6500 _multiply_whole.
-  0x00000090 5f6d756c 7469706c 795f7768 6f6c652e _multiply_whole.
-  0x000000a0 6c6f6f70 5f31005f 6d756c74 69706c79 loop_1._multiply
-  0x000000b0 5f77686f 6c652e6c 6f6f705f 32005f6d _whole.loop_2._m
-  0x000000c0 756c7469 706c795f 77686f6c 652e6c6f ultiply_whole.lo
-  0x000000d0 6f705f33 005f6d75 6c746970 6c795f77 op_3._multiply_w
-  0x000000e0 686f6c65 2e616674 65725f6c 6f6f705f hole.after_loop_
-  0x000000f0 33005f6d 756c7469 706c795f 77686f6c 3._multiply_whol
-  0x00000100 652e6c6f 6f705f34 005f6d75 6c746970 e.loop_4._multip
-  0x00000110 6c795f77 686f6c65 2e6c6f6f 705f3500 ly_whole.loop_5.
+  0x00000020 72697468 6d657469 63612f62 75696c64 rithmetica/build
+  0x00000030 2f5f6465 70732f62 6d6f2d73 72632f73 /_deps/bmo-src/s
+  0x00000040 72632f6c 69627261 72792f6c 696e7578 rc/library/linux
+  0x00000050 2f5f6d75 6c746970 6c795f77 686f6c65 /_multiply_whole
+  0x00000060 2e61736d 00616464 5f77686f 6c650073 .asm.add_whole.s
+  0x00000070 74726c65 6e5f6173 6d005f6d 756c7469 trlen_asm._multi
+  0x00000080 706c795f 77686f6c 65005f6d 756c7469 ply_whole._multi
+  0x00000090 706c795f 77686f6c 652e6c6f 6f705f31 ply_whole.loop_1
+  0x000000a0 005f6d75 6c746970 6c795f77 686f6c65 ._multiply_whole
+  0x000000b0 2e6c6f6f 705f3200 5f6d756c 7469706c .loop_2._multipl
+  0x000000c0 795f7768 6f6c652e 6c6f6f70 5f33005f y_whole.loop_3._
+  0x000000d0 6d756c74 69706c79 5f77686f 6c652e61 multiply_whole.a
+  0x000000e0 66746572 5f6c6f6f 705f3300 5f6d756c fter_loop_3._mul
+  0x000000f0 7469706c 795f7768 6f6c652e 6c6f6f70 tiply_whole.loop
+  0x00000100 5f34005f 6d756c74 69706c79 5f77686f _4._multiply_who
+  0x00000110 6c652e6c 6f6f705f 3500              le.loop_5.
```

#### _divide_whole_with_remainder.asm.o

##### readelf --wide --sections {}

```diff
@@ -2,14 +2,14 @@
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 0001c0 00031f 00  AX  0   0 16
   [ 2] .shstrtab         STRTAB          0000000000000000 0004e0 00002c 00      0   0  1
   [ 3] .symtab           SYMTAB          0000000000000000 000510 000228 18      4  18  8
-  [ 4] .strtab           STRTAB          0000000000000000 000740 000311 00      0   0  1
-  [ 5] .rela.text        RELA            0000000000000000 000a60 0000f0 18      3   1  8
+  [ 4] .strtab           STRTAB          0000000000000000 000740 00030b 00      0   0  1
+  [ 5] .rela.text        RELA            0000000000000000 000a50 0000f0 18      3   1  8
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,12 +1,12 @@
 
 Symbol table '.symtab' contains 23 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/_divide_whole_with_remainder.asm
+     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/_divide_whole_with_remainder.asm
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
      3: 0000000000000033     0 NOTYPE  LOCAL  DEFAULT    1 _divide_whole_with_remainder.loop_1
      4: 00000000000000bb     0 NOTYPE  LOCAL  DEFAULT    1 _divide_whole_with_remainder.loop_2
      5: 00000000000000df     0 NOTYPE  LOCAL  DEFAULT    1 _divide_whole_with_remainder.after_if_1
      6: 00000000000000e2     0 NOTYPE  LOCAL  DEFAULT    1 _divide_whole_with_remainder.loop_3
      7: 000000000000011e     0 NOTYPE  LOCAL  DEFAULT    1 _divide_whole_with_remainder.loop_4
      8: 0000000000000126     0 NOTYPE  LOCAL  DEFAULT    1 _divide_whole_with_remainder.loop_5
```

##### readelf --wide --relocs {}

```diff
@@ -1,9 +1,9 @@
 
-Relocation section '.rela.text' at offset 0xa60 contains 10 entries:
+Relocation section '.rela.text' at offset 0xa50 contains 10 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 000000000000000b  0000001400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 0000000000000017  0000001400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 0000000000000078  0000001200000004 R_X86_64_PLT32         0000000000000000 _multiply_whole - 4
 0000000000000080  0000001400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 0000000000000173  0000001500000004 R_X86_64_PLT32         0000000000000000 subtract_whole - 4
 000000000000018f  0000001300000004 R_X86_64_PLT32         0000000000000000 remove_leading_zeroes - 4
```

##### strings --all --bytes=8 {}

```diff
@@ -4,15 +4,15 @@
 AWWVRPSAQASAPQH
 YA[AY[XZ^_E1
 0WVRPSQAPAQASH
 A[AYAXY[XZ^_E1
 A_A^A]A\[
 .shstrtab
 .rela.text
-/home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/_divide_whole_with_remainder.asm
+/home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/_divide_whole_with_remainder.asm
 _multiply_whole
 remove_leading_zeroes
 strlen_asm
 subtract_whole
 _divide_whole_with_remainder
 _divide_whole_with_remainder.loop_1
 _divide_whole_with_remainder.loop_2
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,53 +1,52 @@
 
 Hex dump of section '.strtab':
   0x00000000 002f686f 6d652f72 756e6e65 722f776f ./home/runner/wo
   0x00000010 726b2f61 72697468 6d657469 63612f61 rk/arithmetica/a
-  0x00000020 72697468 6d657469 63612f73 72632f62 rithmetica/src/b
-  0x00000030 61736963 5f6d6174 685f6f70 65726174 asic_math_operat
-  0x00000040 696f6e73 2f737263 2f6c6962 72617279 ions/src/library
-  0x00000050 2f6c696e 75782f5f 64697669 64655f77 /linux/_divide_w
-  0x00000060 686f6c65 5f776974 685f7265 6d61696e hole_with_remain
-  0x00000070 6465722e 61736d00 5f6d756c 7469706c der.asm._multipl
-  0x00000080 795f7768 6f6c6500 72656d6f 76655f6c y_whole.remove_l
-  0x00000090 65616469 6e675f7a 65726f65 73007374 eading_zeroes.st
-  0x000000a0 726c656e 5f61736d 00737562 74726163 rlen_asm.subtrac
-  0x000000b0 745f7768 6f6c6500 5f646976 6964655f t_whole._divide_
-  0x000000c0 77686f6c 655f7769 74685f72 656d6169 whole_with_remai
-  0x000000d0 6e646572 005f6469 76696465 5f77686f nder._divide_who
-  0x000000e0 6c655f77 6974685f 72656d61 696e6465 le_with_remainde
-  0x000000f0 722e6c6f 6f705f31 005f6469 76696465 r.loop_1._divide
-  0x00000100 5f77686f 6c655f77 6974685f 72656d61 _whole_with_rema
-  0x00000110 696e6465 722e6c6f 6f705f32 005f6469 inder.loop_2._di
-  0x00000120 76696465 5f77686f 6c655f77 6974685f vide_whole_with_
-  0x00000130 72656d61 696e6465 722e6166 7465725f remainder.after_
-  0x00000140 69665f31 005f6469 76696465 5f77686f if_1._divide_who
-  0x00000150 6c655f77 6974685f 72656d61 696e6465 le_with_remainde
-  0x00000160 722e6c6f 6f705f33 005f6469 76696465 r.loop_3._divide
-  0x00000170 5f77686f 6c655f77 6974685f 72656d61 _whole_with_rema
-  0x00000180 696e6465 722e6c6f 6f705f34 005f6469 inder.loop_4._di
-  0x00000190 76696465 5f77686f 6c655f77 6974685f vide_whole_with_
-  0x000001a0 72656d61 696e6465 722e6c6f 6f705f35 remainder.loop_5
-  0x000001b0 005f6469 76696465 5f77686f 6c655f77 ._divide_whole_w
-  0x000001c0 6974685f 72656d61 696e6465 722e6c6f ith_remainder.lo
-  0x000001d0 6f705f36 005f6469 76696465 5f77686f op_6._divide_who
-  0x000001e0 6c655f77 6974685f 72656d61 696e6465 le_with_remainde
-  0x000001f0 722e6c6f 6f705f37 005f6469 76696465 r.loop_7._divide
-  0x00000200 5f77686f 6c655f77 6974685f 72656d61 _whole_with_rema
-  0x00000210 696e6465 722e6c6f 6f705f38 005f6469 inder.loop_8._di
-  0x00000220 76696465 5f77686f 6c655f77 6974685f vide_whole_with_
-  0x00000230 72656d61 696e6465 722e6c6f 6f705f39 remainder.loop_9
-  0x00000240 005f6469 76696465 5f77686f 6c655f77 ._divide_whole_w
-  0x00000250 6974685f 72656d61 696e6465 722e6166 ith_remainder.af
-  0x00000260 7465725f 6c6f6f70 5f35005f 64697669 ter_loop_5._divi
-  0x00000270 64655f77 686f6c65 5f776974 685f7265 de_whole_with_re
-  0x00000280 6d61696e 6465722e 6c6f6f70 5f313000 mainder.loop_10.
-  0x00000290 5f646976 6964655f 77686f6c 655f7769 _divide_whole_wi
-  0x000002a0 74685f72 656d6169 6e646572 2e6c6f6f th_remainder.loo
-  0x000002b0 705f3131 005f6469 76696465 5f77686f p_11._divide_who
-  0x000002c0 6c655f77 6974685f 72656d61 696e6465 le_with_remainde
-  0x000002d0 722e6164 645f7768 6f6c655f 656c7365 r.add_whole_else
-  0x000002e0 5f31005f 64697669 64655f77 686f6c65 _1._divide_whole
-  0x000002f0 5f776974 685f7265 6d61696e 6465722e _with_remainder.
-  0x00000300 61667465 725f6164 645f656c 73655f31 after_add_else_1
-  0x00000310 00                                  .
+  0x00000020 72697468 6d657469 63612f62 75696c64 rithmetica/build
+  0x00000030 2f5f6465 70732f62 6d6f2d73 72632f73 /_deps/bmo-src/s
+  0x00000040 72632f6c 69627261 72792f6c 696e7578 rc/library/linux
+  0x00000050 2f5f6469 76696465 5f77686f 6c655f77 /_divide_whole_w
+  0x00000060 6974685f 72656d61 696e6465 722e6173 ith_remainder.as
+  0x00000070 6d005f6d 756c7469 706c795f 77686f6c m._multiply_whol
+  0x00000080 65007265 6d6f7665 5f6c6561 64696e67 e.remove_leading
+  0x00000090 5f7a6572 6f657300 7374726c 656e5f61 _zeroes.strlen_a
+  0x000000a0 736d0073 75627472 6163745f 77686f6c sm.subtract_whol
+  0x000000b0 65005f64 69766964 655f7768 6f6c655f e._divide_whole_
+  0x000000c0 77697468 5f72656d 61696e64 6572005f with_remainder._
+  0x000000d0 64697669 64655f77 686f6c65 5f776974 divide_whole_wit
+  0x000000e0 685f7265 6d61696e 6465722e 6c6f6f70 h_remainder.loop
+  0x000000f0 5f31005f 64697669 64655f77 686f6c65 _1._divide_whole
+  0x00000100 5f776974 685f7265 6d61696e 6465722e _with_remainder.
+  0x00000110 6c6f6f70 5f32005f 64697669 64655f77 loop_2._divide_w
+  0x00000120 686f6c65 5f776974 685f7265 6d61696e hole_with_remain
+  0x00000130 6465722e 61667465 725f6966 5f31005f der.after_if_1._
+  0x00000140 64697669 64655f77 686f6c65 5f776974 divide_whole_wit
+  0x00000150 685f7265 6d61696e 6465722e 6c6f6f70 h_remainder.loop
+  0x00000160 5f33005f 64697669 64655f77 686f6c65 _3._divide_whole
+  0x00000170 5f776974 685f7265 6d61696e 6465722e _with_remainder.
+  0x00000180 6c6f6f70 5f34005f 64697669 64655f77 loop_4._divide_w
+  0x00000190 686f6c65 5f776974 685f7265 6d61696e hole_with_remain
+  0x000001a0 6465722e 6c6f6f70 5f35005f 64697669 der.loop_5._divi
+  0x000001b0 64655f77 686f6c65 5f776974 685f7265 de_whole_with_re
+  0x000001c0 6d61696e 6465722e 6c6f6f70 5f36005f mainder.loop_6._
+  0x000001d0 64697669 64655f77 686f6c65 5f776974 divide_whole_wit
+  0x000001e0 685f7265 6d61696e 6465722e 6c6f6f70 h_remainder.loop
+  0x000001f0 5f37005f 64697669 64655f77 686f6c65 _7._divide_whole
+  0x00000200 5f776974 685f7265 6d61696e 6465722e _with_remainder.
+  0x00000210 6c6f6f70 5f38005f 64697669 64655f77 loop_8._divide_w
+  0x00000220 686f6c65 5f776974 685f7265 6d61696e hole_with_remain
+  0x00000230 6465722e 6c6f6f70 5f39005f 64697669 der.loop_9._divi
+  0x00000240 64655f77 686f6c65 5f776974 685f7265 de_whole_with_re
+  0x00000250 6d61696e 6465722e 61667465 725f6c6f mainder.after_lo
+  0x00000260 6f705f35 005f6469 76696465 5f77686f op_5._divide_who
+  0x00000270 6c655f77 6974685f 72656d61 696e6465 le_with_remainde
+  0x00000280 722e6c6f 6f705f31 30005f64 69766964 r.loop_10._divid
+  0x00000290 655f7768 6f6c655f 77697468 5f72656d e_whole_with_rem
+  0x000002a0 61696e64 65722e6c 6f6f705f 3131005f ainder.loop_11._
+  0x000002b0 64697669 64655f77 686f6c65 5f776974 divide_whole_wit
+  0x000002c0 685f7265 6d61696e 6465722e 6164645f h_remainder.add_
+  0x000002d0 77686f6c 655f656c 73655f31 005f6469 whole_else_1._di
+  0x000002e0 76696465 5f77686f 6c655f77 6974685f vide_whole_with_
+  0x000002f0 72656d61 696e6465 722e6166 7465725f remainder.after_
+  0x00000300 6164645f 656c7365 5f3100            add_else_1.
```

#### asmalloc.asm.o

##### readelf --wide --sections {}

```diff
@@ -2,13 +2,13 @@
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000180 000022 00  AX  0   0 16
   [ 2] .shstrtab         STRTAB          0000000000000000 0001b0 000021 00      0   0  1
   [ 3] .symtab           SYMTAB          0000000000000000 0001e0 000060 18      4   3  8
-  [ 4] .strtab           STRTAB          0000000000000000 000240 00006d 00      0   0  1
+  [ 4] .strtab           STRTAB          0000000000000000 000240 000067 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,7 +1,7 @@
 
 Symbol table '.symtab' contains 4 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/asmalloc.asm
+     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/asmalloc.asm
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
      3: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT    1 asmalloc
```

##### strings --all --bytes=8 {}

```diff
@@ -1,3 +1,3 @@
 .shstrtab
-/home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/asmalloc.asm
+/home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/asmalloc.asm
 asmalloc
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,10 +1,10 @@
 
 Hex dump of section '.strtab':
   0x00000000 002f686f 6d652f72 756e6e65 722f776f ./home/runner/wo
   0x00000010 726b2f61 72697468 6d657469 63612f61 rk/arithmetica/a
-  0x00000020 72697468 6d657469 63612f73 72632f62 rithmetica/src/b
-  0x00000030 61736963 5f6d6174 685f6f70 65726174 asic_math_operat
-  0x00000040 696f6e73 2f737263 2f6c6962 72617279 ions/src/library
-  0x00000050 2f6c696e 75782f61 736d616c 6c6f632e /linux/asmalloc.
-  0x00000060 61736d00 61736d61 6c6c6f63 00       asm.asmalloc.
+  0x00000020 72697468 6d657469 63612f62 75696c64 rithmetica/build
+  0x00000030 2f5f6465 70732f62 6d6f2d73 72632f73 /_deps/bmo-src/s
+  0x00000040 72632f6c 69627261 72792f6c 696e7578 rc/library/linux
+  0x00000050 2f61736d 616c6c6f 632e6173 6d006173 /asmalloc.asm.as
+  0x00000060 6d616c6c 6f6300                     malloc.
```

#### multiply_whole.asm.o

##### readelf --wide --sections {}

```diff
@@ -2,14 +2,14 @@
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 0001c0 000070 00  AX  0   0 16
   [ 2] .shstrtab         STRTAB          0000000000000000 000230 00002c 00      0   0  1
   [ 3] .symtab           SYMTAB          0000000000000000 000260 0000a8 18      4   3  8
-  [ 4] .strtab           STRTAB          0000000000000000 000310 00009d 00      0   0  1
+  [ 4] .strtab           STRTAB          0000000000000000 000310 000097 00      0   0  1
   [ 5] .rela.text        RELA            0000000000000000 0003b0 000078 18      3   1  8
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,10 +1,10 @@
 
 Symbol table '.symtab' contains 7 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/multiply_whole.asm
+     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS /home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/multiply_whole.asm
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
      3: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _multiply_whole
      4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND asmalloc
      5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen_asm
      6: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT    1 multiply_whole
```

##### strings --all --bytes=8 {}

```diff
@@ -1,7 +1,7 @@
 .shstrtab
 .rela.text
-/home/runner/work/arithmetica/arithmetica/src/basic_math_operations/src/library/linux/multiply_whole.asm
+/home/runner/work/arithmetica/arithmetica/build/_deps/bmo-src/src/library/linux/multiply_whole.asm
 _multiply_whole
 asmalloc
 strlen_asm
 multiply_whole
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,13 +1,13 @@
 
 Hex dump of section '.strtab':
   0x00000000 002f686f 6d652f72 756e6e65 722f776f ./home/runner/wo
   0x00000010 726b2f61 72697468 6d657469 63612f61 rk/arithmetica/a
-  0x00000020 72697468 6d657469 63612f73 72632f62 rithmetica/src/b
-  0x00000030 61736963 5f6d6174 685f6f70 65726174 asic_math_operat
-  0x00000040 696f6e73 2f737263 2f6c6962 72617279 ions/src/library
-  0x00000050 2f6c696e 75782f6d 756c7469 706c795f /linux/multiply_
-  0x00000060 77686f6c 652e6173 6d005f6d 756c7469 whole.asm._multi
-  0x00000070 706c795f 77686f6c 65006173 6d616c6c ply_whole.asmall
-  0x00000080 6f630073 74726c65 6e5f6173 6d006d75 oc.strlen_asm.mu
-  0x00000090 6c746970 6c795f77 686f6c65 00       ltiply_whole.
+  0x00000020 72697468 6d657469 63612f62 75696c64 rithmetica/build
+  0x00000030 2f5f6465 70732f62 6d6f2d73 72632f73 /_deps/bmo-src/s
+  0x00000040 72632f6c 69627261 72792f6c 696e7578 rc/library/linux
+  0x00000050 2f6d756c 7469706c 795f7768 6f6c652e /multiply_whole.
+  0x00000060 61736d00 5f6d756c 7469706c 795f7768 asm._multiply_wh
+  0x00000070 6f6c6500 61736d61 6c6c6f63 00737472 ole.asmalloc.str
+  0x00000080 6c656e5f 61736d00 6d756c74 69706c79 len_asm.multiply
+  0x00000090 5f77686f 6c6500                     _whole.
```

### Comparing `arithmetica-py-1.0.213/src/python-module/module.c` & `arithmetica-py-1.0.219/src/python-module/module.c`

 * *Files identical despite different names*

