# Comparing `tmp/coacd-0.0.3-py3-none-win_amd64.whl.zip` & `tmp/coacd-0.0.4-py3-none-win_amd64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                   5714247 (0000000000573147h)
-  Actual end-cent-dir record offset:       5714225 (0000000000573131h)
-  Expected end-cent-dir record offset:     5714225 (0000000000573131h)
+  Zip archive file size:                   5882211 (000000000059C163h)
+  Actual end-cent-dir record offset:       5882189 (000000000059C14Dh)
+  Expected end-cent-dir record offset:     5882189 (000000000059C14Dh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 12 entries.
-  The central directory is 1125 (0000000000000465h) bytes long,
+  central directory contains 15 entries.
+  The central directory is 1403 (000000000000057Bh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 5713100 (0000000000572CCCh).
+  is 5880786 (000000000059BBD2h).
 
 
 Central directory entry #1:
 ---------------------------
 
   coacd/
 
@@ -25,17 +25,17 @@
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 16 21:05:26
-  file last modified on (UT extra field modtime): 2023 May 17 04:05:25 local
-  file last modified on (UT extra field modtime): 2023 May 17 04:05:25 UTC
+  file last modified on (DOS date/time):          2023 Jun 8 23:47:20
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:47:19 local
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:47:19 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             6 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -62,17 +62,17 @@
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 16 21:05:26
-  file last modified on (UT extra field modtime): 2023 May 17 04:05:25 local
-  file last modified on (UT extra field modtime): 2023 May 17 04:05:25 UTC
+  file last modified on (DOS date/time):          2023 Jun 8 23:47:20
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:47:19 local
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:47:19 UTC
   32-bit CRC value (hex):                         31093819
   compressed size:                                5708094 bytes
   uncompressed size:                              25298178 bytes
   length of filename:                             19 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -87,26 +87,63 @@
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  coacd/__init__.py
+  coacd/libgomp-1.dll
 
   offset of local header from start of archive:   5708235
                                                   (00000000005719CBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
+  file last modified on (DOS date/time):          2023 Jun 8 23:47:20
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:47:19 local
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:47:19 UTC
+  32-bit CRC value (hex):                         f531891d
+  compressed size:                                106255 bytes
+  uncompressed size:                              228878 bytes
+  length of filename:                             19 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (100755 octal):            -rwxr-xr-x
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #4:
+---------------------------
+
+  coacd/__init__.py
+
+  offset of local header from start of archive:   5814567
+                                                  (000000000058B927h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
   file last modified on (DOS date/time):          2023 May 16 16:28:14
   file last modified on (UT extra field modtime): 2023 May 16 23:28:14 local
   file last modified on (UT extra field modtime): 2023 May 16 23:28:14 UTC
   32-bit CRC value (hex):                         070a9f8e
   compressed size:                                1168 bytes
   uncompressed size:                              3831 bytes
   length of filename:                             17 characters
@@ -121,31 +158,105 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #4:
+Central directory entry #5:
+---------------------------
+
+  coacd/libgcc_s_seh-1.dll
+
+  offset of local header from start of archive:   5815810
+                                                  (000000000058BE02h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Jun 8 23:47:20
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:47:19 local
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:47:19 UTC
+  32-bit CRC value (hex):                         a217fff6
+  compressed size:                                35609 bytes
+  uncompressed size:                              79374 bytes
+  length of filename:                             24 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (100755 octal):            -rwxr-xr-x
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #6:
+---------------------------
+
+  coacd/libwinpthread-1.dll
+
+  offset of local header from start of archive:   5851501
+                                                  (000000000059496Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Jun 8 23:47:20
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:47:19 local
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:47:19 UTC
+  32-bit CRC value (hex):                         f45a5159
+  compressed size:                                25517 bytes
+  uncompressed size:                              59216 bytes
+  length of filename:                             25 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (100755 octal):            -rwxr-xr-x
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #7:
 ---------------------------
 
-  coacd-0.0.3.data/
+  coacd-0.0.4.data/
 
-  offset of local header from start of archive:   5709478
-                                                  (0000000000571EA6h) bytes
+  offset of local header from start of archive:   5877101
+                                                  (000000000059AD6Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 16 20:53:00
-  file last modified on (UT extra field modtime): 2023 May 17 03:53:00 local
-  file last modified on (UT extra field modtime): 2023 May 17 03:53:00 UTC
+  file last modified on (DOS date/time):          2023 Jun 8 23:44:56
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:55 local
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:55 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             17 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -157,31 +268,31 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #5:
+Central directory entry #8:
 ---------------------------
 
-  coacd-0.0.3.data/scripts/
+  coacd-0.0.4.data/scripts/
 
-  offset of local header from start of archive:   5709553
-                                                  (0000000000571EF1h) bytes
+  offset of local header from start of archive:   5877176
+                                                  (000000000059ADB8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 16 20:53:00
-  file last modified on (UT extra field modtime): 2023 May 17 03:53:00 local
-  file last modified on (UT extra field modtime): 2023 May 17 03:53:00 UTC
+  file last modified on (DOS date/time):          2023 Jun 8 23:44:56
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:55 local
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:55 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             25 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -193,32 +304,32 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #6:
+Central directory entry #9:
 ---------------------------
 
-  coacd-0.0.3.data/scripts/coacd
+  coacd-0.0.4.data/scripts/coacd
 
-  offset of local header from start of archive:   5709636
-                                                  (0000000000571F44h) bytes
+  offset of local header from start of archive:   5877259
+                                                  (000000000059AE0Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 16 20:52:58
-  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 local
-  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 UTC
+  file last modified on (DOS date/time):          2023 Jun 8 23:44:52
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:52 local
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:52 UTC
   32-bit CRC value (hex):                         d4b77592
   compressed size:                                1229 bytes
   uncompressed size:                              3730 bytes
   length of filename:                             30 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -230,31 +341,31 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #7:
+Central directory entry #10:
 ---------------------------
 
-  coacd-0.0.3.dist-info/
+  coacd-0.0.4.dist-info/
 
-  offset of local header from start of archive:   5710953
-                                                  (0000000000572469h) bytes
+  offset of local header from start of archive:   5878576
+                                                  (000000000059B330h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 16 21:24:08
-  file last modified on (UT extra field modtime): 2023 May 17 04:24:08 local
-  file last modified on (UT extra field modtime): 2023 May 17 04:24:08 UTC
+  file last modified on (DOS date/time):          2023 Jun 8 23:44:56
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:55 local
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:55 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             22 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -266,35 +377,35 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #8:
+Central directory entry #11:
 ---------------------------
 
-  coacd-0.0.3.dist-info/RECORD
+  coacd-0.0.4.dist-info/RECORD
 
-  offset of local header from start of archive:   5711033
-                                                  (00000000005724B9h) bytes
+  offset of local header from start of archive:   5878656
+                                                  (000000000059B380h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 16 21:12:50
-  file last modified on (UT extra field modtime): 2023 May 17 04:12:49 local
-  file last modified on (UT extra field modtime): 2023 May 17 04:12:49 UTC
-  32-bit CRC value (hex):                         d7a53d48
-  compressed size:                                414 bytes
-  uncompressed size:                              625 bytes
+  file last modified on (DOS date/time):          2023 Jun 8 23:44:54
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:54 local
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:54 UTC
+  32-bit CRC value (hex):                         6ba8764b
+  compressed size:                                476 bytes
+  uncompressed size:                              720 bytes
   length of filename:                             28 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
@@ -303,34 +414,34 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #9:
+Central directory entry #12:
 ---------------------------
 
-  coacd-0.0.3.dist-info/METADATA
+  coacd-0.0.4.dist-info/METADATA
 
-  offset of local header from start of archive:   5711533
-                                                  (00000000005726ADh) bytes
+  offset of local header from start of archive:   5879218
+                                                  (000000000059B5B2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 16 20:52:58
-  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 local
-  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 UTC
-  32-bit CRC value (hex):                         cc1de6e3
-  compressed size:                                475 bytes
+  file last modified on (DOS date/time):          2023 Jun 8 23:44:52
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:52 local
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:52 UTC
+  32-bit CRC value (hex):                         5738d8b6
+  compressed size:                                476 bytes
   uncompressed size:                              1195 bytes
   length of filename:                             30 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
@@ -340,31 +451,31 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #10:
+Central directory entry #13:
 ---------------------------
 
-  coacd-0.0.3.dist-info/top_level.txt
+  coacd-0.0.4.dist-info/top_level.txt
 
-  offset of local header from start of archive:   5712096
-                                                  (00000000005728E0h) bytes
+  offset of local header from start of archive:   5879782
+                                                  (000000000059B7E6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 16 20:52:58
-  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 local
-  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 UTC
+  file last modified on (DOS date/time):          2023 Jun 8 23:44:52
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:52 local
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:52 UTC
   32-bit CRC value (hex):                         0c8f9e69
   compressed size:                                6 bytes
   uncompressed size:                              6 bytes
   length of filename:                             35 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -376,31 +487,31 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #11:
+Central directory entry #14:
 ---------------------------
 
-  coacd-0.0.3.dist-info/WHEEL
+  coacd-0.0.4.dist-info/WHEEL
 
-  offset of local header from start of archive:   5712195
-                                                  (0000000000572943h) bytes
+  offset of local header from start of archive:   5879881
+                                                  (000000000059B849h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 16 21:24:08
-  file last modified on (UT extra field modtime): 2023 May 17 04:24:08 local
-  file last modified on (UT extra field modtime): 2023 May 17 04:24:08 UTC
+  file last modified on (DOS date/time):          2023 Jun 8 23:46:56
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:46:56 local
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:46:56 UTC
   32-bit CRC value (hex):                         f70794a1
   compressed size:                                98 bytes
   uncompressed size:                              98 bytes
   length of filename:                             27 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -412,32 +523,32 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #12:
+Central directory entry #15:
 ---------------------------
 
-  coacd-0.0.3.dist-info/LICENSE
+  coacd-0.0.4.dist-info/LICENSE
 
-  offset of local header from start of archive:   5712378
-                                                  (00000000005729FAh) bytes
+  offset of local header from start of archive:   5880064
+                                                  (000000000059B900h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 16 20:52:58
-  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 local
-  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 UTC
+  file last modified on (DOS date/time):          2023 Jun 8 23:44:52
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:52 local
+  file last modified on (UT extra field modtime): 2023 Jun 9 06:44:52 UTC
   32-bit CRC value (hex):                         59bd864a
   compressed size:                                635 bytes
   uncompressed size:                              1080 bytes
   length of filename:                             29 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
```

## zipnote {}

```diff
@@ -1,37 +1,46 @@
 Filename: coacd/
 Comment: 
 
 Filename: coacd/lib_coacd.dll
 Comment: 
 
+Filename: coacd/libgomp-1.dll
+Comment: 
+
 Filename: coacd/__init__.py
 Comment: 
 
-Filename: coacd-0.0.3.data/
+Filename: coacd/libgcc_s_seh-1.dll
+Comment: 
+
+Filename: coacd/libwinpthread-1.dll
+Comment: 
+
+Filename: coacd-0.0.4.data/
 Comment: 
 
-Filename: coacd-0.0.3.data/scripts/
+Filename: coacd-0.0.4.data/scripts/
 Comment: 
 
-Filename: coacd-0.0.3.data/scripts/coacd
+Filename: coacd-0.0.4.data/scripts/coacd
 Comment: 
 
-Filename: coacd-0.0.3.dist-info/
+Filename: coacd-0.0.4.dist-info/
 Comment: 
 
-Filename: coacd-0.0.3.dist-info/RECORD
+Filename: coacd-0.0.4.dist-info/RECORD
 Comment: 
 
-Filename: coacd-0.0.3.dist-info/METADATA
+Filename: coacd-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: coacd-0.0.3.dist-info/top_level.txt
+Filename: coacd-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: coacd-0.0.3.dist-info/WHEEL
+Filename: coacd-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: coacd-0.0.3.dist-info/LICENSE
+Filename: coacd-0.0.4.dist-info/LICENSE
 Comment: 
 
 Zip file comment:
```

## Comparing `coacd-0.0.3.data/scripts/coacd` & `coacd-0.0.4.data/scripts/coacd`

 * *Files identical despite different names*

## Comparing `coacd-0.0.3.dist-info/METADATA` & `coacd-0.0.4.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coacd
-Version: 0.0.3
+Version: 0.0.4
 Summary: Approximate Convex Decomposition for 3D Meshes with Collision-Aware Concavity and Tree Search
 Home-page: https://colin97.github.io/CoACD/
 Author-email: xiwei@ucsd.edu
 License: MIT
 Keywords: collision convex decomposition
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
```

## Comparing `coacd-0.0.3.dist-info/LICENSE` & `coacd-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

