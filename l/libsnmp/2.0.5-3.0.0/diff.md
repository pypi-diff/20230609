# Comparing `tmp/libsnmp-2.0.5.tar.gz` & `tmp/libsnmp-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsnmp-2.0.5.tar", last modified: Sat Jan 30 00:20:21 2010, max compression, from Unix
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `libsnmp-2.0.5.tar` & `libsnmp-3.0.0.tar`

### file list

```diff
@@ -1,49 +1,44 @@
-drwxr-xr-x   0 daedalus  (1000) daedalus  (1000)        0 2010-01-30 00:20:21.000000 libsnmp-2.0.5/
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)      511 2008-10-18 22:59:45.000000 libsnmp-2.0.5/MANIFEST
-drwxr-xr-x   0 daedalus  (1000) daedalus  (1000)        0 2010-01-30 00:20:21.000000 libsnmp-2.0.5/debian/
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)       12 2008-12-09 05:29:58.000000 libsnmp-2.0.5/debian/pyversions
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)        2 2008-10-18 22:59:45.000000 libsnmp-2.0.5/debian/compat
--rwxr-xr-x   0 daedalus  (1000) daedalus  (1000)     1963 2008-12-09 05:44:18.000000 libsnmp-2.0.5/debian/rules
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)      875 2008-12-09 05:33:57.000000 libsnmp-2.0.5/debian/control
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     1232 2008-10-18 22:59:45.000000 libsnmp-2.0.5/debian/copyright
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     1121 2008-10-25 22:32:18.000000 libsnmp-2.0.5/debian/changelog
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)       59 2010-01-30 00:20:21.000000 libsnmp-2.0.5/setup.cfg
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     1117 2008-10-18 22:59:45.000000 libsnmp-2.0.5/TODO
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)      277 2008-10-18 22:59:45.000000 libsnmp-2.0.5/INSTALL
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     2144 2008-10-18 22:59:45.000000 libsnmp-2.0.5/ChangeLog
--rwxr-xr-x   0 daedalus  (1000) daedalus  (1000)     1469 2010-01-29 23:45:51.000000 libsnmp-2.0.5/trapsender.py
--rwxr-xr-x   0 daedalus  (1000) daedalus  (1000)     1904 2008-10-18 22:59:45.000000 libsnmp-2.0.5/traplistener.py
-drwxr-xr-x   0 daedalus  (1000) daedalus  (1000)        0 2010-01-30 00:20:21.000000 libsnmp-2.0.5/test/
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     3401 2008-10-18 22:59:45.000000 libsnmp-2.0.5/test/test_svt_encoder.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     2023 2008-10-18 22:59:45.000000 libsnmp-2.0.5/test/test_Messages.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     6615 2008-10-18 22:59:45.000000 libsnmp-2.0.5/test/test_rfc1157.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     4497 2008-10-18 22:59:45.000000 libsnmp-2.0.5/test/test_rfc1155.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     9866 2010-01-30 00:19:41.000000 libsnmp-2.0.5/test/test_encoder.py
--rwxr-xr-x   0 daedalus  (1000) daedalus  (1000)     1991 2008-10-18 22:59:45.000000 libsnmp-2.0.5/snmpwalk.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     1152 2008-10-18 22:59:45.000000 libsnmp-2.0.5/LICENSE
--rwxr-xr-x   0 daedalus  (1000) daedalus  (1000)     2074 2008-10-18 22:59:45.000000 libsnmp-2.0.5/snmpget-v2.py
--rwxr-xr-x   0 daedalus  (1000) daedalus  (1000)     1647 2010-01-30 00:19:41.000000 libsnmp-2.0.5/setup.py
-drwxr-xr-x   0 daedalus  (1000) daedalus  (1000)        0 2010-01-30 00:20:21.000000 libsnmp-2.0.5/lib/
-drwxr-xr-x   0 daedalus  (1000) daedalus  (1000)        0 2010-01-30 00:20:21.000000 libsnmp-2.0.5/lib/libsnmp/
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)    12884 2008-10-18 22:59:45.000000 libsnmp-2.0.5/lib/libsnmp/snmpmanager.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     1540 2008-10-18 22:59:45.000000 libsnmp-2.0.5/lib/libsnmp/rfc1902.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)    29506 2010-01-30 00:07:45.000000 libsnmp-2.0.5/lib/libsnmp/rfc1155.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)      709 2008-10-18 22:59:45.000000 libsnmp-2.0.5/lib/libsnmp/util.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     7415 2010-01-29 23:45:51.000000 libsnmp-2.0.5/lib/libsnmp/v2.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)      702 2008-10-18 22:59:45.000000 libsnmp-2.0.5/lib/libsnmp/debug.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     7896 2008-10-18 22:59:45.000000 libsnmp-2.0.5/lib/libsnmp/rfc1157.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)      316 2008-10-18 22:59:45.000000 libsnmp-2.0.5/lib/libsnmp/__init__.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     9122 2008-10-18 22:59:45.000000 libsnmp-2.0.5/lib/libsnmp/v1.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     1543 2008-10-18 22:59:45.000000 libsnmp-2.0.5/lib/libsnmp/role.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     1801 2008-10-18 22:59:45.000000 libsnmp-2.0.5/lib/libsnmp/asynrole.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     6718 2008-10-18 22:59:45.000000 libsnmp-2.0.5/lib/libsnmp/rfc1905.py
-drwxr-xr-x   0 daedalus  (1000) daedalus  (1000)        0 2010-01-30 00:20:21.000000 libsnmp-2.0.5/lib/libsnmp.egg-info/
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)        1 2010-01-30 00:20:21.000000 libsnmp-2.0.5/lib/libsnmp.egg-info/dependency_links.txt
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)        8 2010-01-30 00:20:21.000000 libsnmp-2.0.5/lib/libsnmp.egg-info/top_level.txt
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)      758 2010-01-30 00:20:21.000000 libsnmp-2.0.5/lib/libsnmp.egg-info/SOURCES.txt
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)      911 2010-01-30 00:20:21.000000 libsnmp-2.0.5/lib/libsnmp.egg-info/PKG-INFO
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)     1232 2008-10-18 22:59:45.000000 libsnmp-2.0.5/COPYRIGHT
--rwxr-xr-x   0 daedalus  (1000) daedalus  (1000)     2074 2008-10-18 22:59:45.000000 libsnmp-2.0.5/snmpget-v1.py
--rwxr-xr-x   0 daedalus  (1000) daedalus  (1000)     1986 2008-10-18 22:59:45.000000 libsnmp-2.0.5/snmpset.py
--rwxr-xr-x   0 daedalus  (1000) daedalus  (1000)     1941 2008-10-18 22:59:45.000000 libsnmp-2.0.5/snmpget.py
--rw-r--r--   0 daedalus  (1000) daedalus  (1000)      911 2010-01-30 00:20:21.000000 libsnmp-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 libsnmp-3.0.0/COPYRIGHT
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 libsnmp-3.0.0/ChangeLog
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 libsnmp-3.0.0/INSTALL
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 libsnmp-3.0.0/MANIFEST
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 libsnmp-3.0.0/TODO
+-rwxr-xr-x   0        0        0     1572 2020-02-02 00:00:00.000000 libsnmp-3.0.0/setup.py
+-rwxr-xr-x   0        0        0     1622 2020-02-02 00:00:00.000000 libsnmp-3.0.0/snmpget-v1.py
+-rwxr-xr-x   0        0        0     1622 2020-02-02 00:00:00.000000 libsnmp-3.0.0/snmpget-v2.py
+-rwxr-xr-x   0        0        0     1774 2020-02-02 00:00:00.000000 libsnmp-3.0.0/snmpget.py
+-rwxr-xr-x   0        0        0     1783 2020-02-02 00:00:00.000000 libsnmp-3.0.0/snmpset.py
+-rwxr-xr-x   0        0        0     1853 2020-02-02 00:00:00.000000 libsnmp-3.0.0/snmpwalk.py
+-rwxr-xr-x   0        0        0     1640 2020-02-02 00:00:00.000000 libsnmp-3.0.0/traplistener.py
+-rwxr-xr-x   0        0        0     1399 2020-02-02 00:00:00.000000 libsnmp-3.0.0/trapsender.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 libsnmp-3.0.0/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 libsnmp-3.0.0/debian/changelog
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 libsnmp-3.0.0/debian/compat
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 libsnmp-3.0.0/debian/control
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 libsnmp-3.0.0/debian/copyright
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 libsnmp-3.0.0/debian/pyversions
+-rwxr-xr-x   0        0        0     1963 2020-02-02 00:00:00.000000 libsnmp-3.0.0/debian/rules
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/__init__.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/asynrole.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/debug.py
+-rw-r--r--   0        0        0    27845 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/rfc1155.py
+-rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/rfc1157.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/rfc1902.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/rfc1905.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/role.py
+-rw-r--r--   0        0        0    12662 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/snmpmanager.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/util.py
+-rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/v1.py
+-rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 libsnmp-3.0.0/lib/libsnmp/v2.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 libsnmp-3.0.0/test/test_Messages.py
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 libsnmp-3.0.0/test/test_asynrole.py
+-rw-r--r--   0        0        0     9855 2020-02-02 00:00:00.000000 libsnmp-3.0.0/test/test_encoder.py
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 libsnmp-3.0.0/test/test_rfc1155.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 libsnmp-3.0.0/test/test_rfc1157.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 libsnmp-3.0.0/test/test_snmpmanager.py
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 libsnmp-3.0.0/test/test_svt_encoder.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 libsnmp-3.0.0/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 libsnmp-3.0.0/LICENSE
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 libsnmp-3.0.0/README.md
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 libsnmp-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 libsnmp-3.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `libsnmp-2.0.5/debian/rules` & `libsnmp-3.0.0/debian/rules`

 * *Files identical despite different names*

### Comparing `libsnmp-2.0.5/debian/control` & `libsnmp-3.0.0/debian/control`

 * *Files identical despite different names*

### Comparing `libsnmp-2.0.5/debian/copyright` & `libsnmp-3.0.0/COPYRIGHT`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# $Id: copyright 43 2006-11-06 22:39:17Z daedalus $
-# $Revision: 43 $
-#
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
```

### Comparing `libsnmp-2.0.5/debian/changelog` & `libsnmp-3.0.0/debian/changelog`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+python-libsnmp (2.0.5-1) feisty; urgency=low
+
+  * Updated build rules to support python 2.5 and remove support for
+    python 2.3 and 2.4. Support for python 2.6 will be introduced soon.
+
+ -- Justin Warren <daedalus@eigenmagic.com>  Tue, 09 Dec 2008 09:30:11 +1100
+
 python-libsnmp (2.0.4-1) feisty; urgency=low
 
   * Fixed minor bug with isinstance parameter ordering in rfc1155.py
   * Change API of v2.SNMP.createGetRequestMessage() to support
     multiple OIDs, rather than just one.
 
  -- Justin Warren <daedalus@eigenmagic.com>  Sun, 26 Oct 2008 09:30:11 +1100
```

### Comparing `libsnmp-2.0.5/ChangeLog` & `libsnmp-3.0.0/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-06-09  Justin Warren <daedalus@eigenmagic.com>
+    * Upgrade to support Python 3.x thanks to Jay Zhou
+
 2007-04-11  Justin Warren <daedalus@eigenmagic.com>
 	* Minor bugfix in rfc1905.py after feedback from Phil Mayers
 	* Changed example scripts to use any available python, not just 2.3
 	
 2006-10-07  Justin Warren <daedalus@eigenmagic.com>
 	* Re-assigned copyright to Justin Warren.
 	* License changed to MIT license instead of LGPL.
```

### Comparing `libsnmp-2.0.5/trapsender.py` & `libsnmp-3.0.0/trapsender.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-#!/usr/bin/python
-# $Id: trapsender.py 57 2010-01-29 23:45:50Z daedalus $
-# $Revision: 57 $
+#!/usr/bin/env python
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 
 import logging
 import socket
 import select
```

### Comparing `libsnmp-2.0.5/traplistener.py` & `libsnmp-3.0.0/snmpwalk.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,70 @@
-#!/usr/bin/python
-# $Id: traplistener.py 49 2008-09-29 07:56:45Z daedalus $
-# $Revision: 49 $
+#!/usr/bin/env python
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 
-import logging
-import socket
-import select
-import datetime
-
 import getopt
 import sys
+import logging
 
-from libsnmp import debug
+from libsnmp import snmpmanager
 from libsnmp import util
-from libsnmp import rfc1155
-from libsnmp import rfc1157
 
-from libsnmp import v1
-from libsnmp import v2
+
+log = logging.getLogger(__name__)
 
 def checkResponse(snmpClient, msg):
     """ Quick and dirty print of what the message contains
     """
     pdu = msg.data
-    # We want to log traps in the following format:
-    # fromaddr, genericTrapNum, genericTrapEnumValue,
-    frontbit = ",".join( [
-        str(pdu.enterprise),
-        str(pdu.agentAddr),
-        str(pdu.genericTrap.value),
-        pdu.genericTrap.enum(),
-        str(pdu.specificTrap),
-        str(pdu.timestamp.value),
-        ])
-
-    print frontbit
-
-    for varbind in pdu.varBindList:
-        endbit = "%s,%s" % ( varbind.objectID, varbind.objectValue )
-        print "  %s" % endbit
-        #print ",".join([ frontbit, endbit ])
 
-    #endbit = unwrapVarBinds(pdu.varBindList)
+    if int(pdu.errorStatus) != 0:
+        print('Error: %s' % pdu.errorStatus)
+    else:
+        unwrapVarBinds(pdu.varBindList)
+
+        myClient.snmpGetNext(pdu.varBindList, remotesite, checkResponse, community=args[1])
+
 
 def unwrapVarBinds(varBindList):
+    """ Display a set of varbinds
     """
-    Unwrap the varbinds and return a stringified list
-    """
-    print '%s' % varBindList
+    #    print '%s' % varBindList
     #    print '%s' % varBindList[0].objectID
-    #    print '%s' % varBindList[0].objectValue
-    # print '%s = %s: (%s) %s' % ( varBindList[0].objectID, varBindList[0].objectValue.__class__.__name__, varBindList[0].objectValue, varBindList[0].objectValue )
-    return ",".join([ "%s,%s" % (varbind.objectID, varbind.objectValue) for varbind in varBindList ])
+    #    print '%s' % varBindList[0].objectValue.value
+
+    print('%s = %s: %s' % (
+    varBindList[0].objectID, varBindList[0].objectValue.__class__.__name__, varBindList[0].objectValue))
+    if varBindList[0].objectValue.__class__.__name__ == 'OctetString':
+        print("   hex: %s" % util.octetsToHex(varBindList[0].objectValue.value))
+
+    if varBindList[0].objectValue.__class__.__name__ == 'NoSuchObject':
+        log.error("No such object!")
+        sys.exit(0)
+
+    if varBindList[0].objectValue.__class__.__name__ == 'EndOfMibView':
+        log.info("End of MIB View")
+        sys.exit(0)
+
 
 # What to do when we finish
 def whenDone(snmpClient):
     sys.exit(0)
 
+
 # Main bits
 
 # Read command line
 options, args = getopt.getopt(sys.argv[1:], '', [])
 
-# Listen on SNMP trap port
-myClient = v2.SNMP( ('0.0.0.0', 162), trapCallback=checkResponse)
+# Probably replace with something that assigns a random port
+myClient = snmpmanager.snmpManager(whenDone)
+
+if len(args) != 3:
+    print("Usage: snmpget.py <server> <community> <oid>")
+    sys.exit(1)
+else:
+    remotesite = (args[0], 161)
+    myClient.snmpGet(args[2], remotesite, checkResponse, community=args[1])
+
 myClient.run()
```

### Comparing `libsnmp-2.0.5/test/test_svt_encoder.py` & `libsnmp-3.0.0/test/test_svt_encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
-# $Id: test_svt_encoder.py 18 2003-09-21 11:16:40Z daedalus $
-# $Revision: 18 $
+# $Id$
+# $Revision$
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (C) 2003 Unicity Pty Ltd <libsnmp@unicity.com.au>
 #
 #    This library is free software; you can redistribute it and/or
 #    modify it under the terms of the GNU Lesser General Public
 #    License as published by the Free Software Foundation; either
@@ -101,16 +101,16 @@
     
     #    print "Profiling encoding/decoding of %d random integers..." % NUMBER_OF_OBJECTS
     #    profile.run('encodeDecodeRandomIntegers()')
     
     #    print "Profiling encoding of %d random ObjectIDs..." % NUMBER_OF_OBJECTS
     #    profile.run('encodeRandomObjectIDs()')
     
-    print "Profiling encoding/decoding of %d random ObjectIDs..." % NUMBER_OF_OBJECTS
+    print("Profiling encoding/decoding of %d random ObjectIDs..." % NUMBER_OF_OBJECTS)
     profile.run('go()')
     
     #encodeDecodeRandomObjectIDs()  
     
     end = time.time()
     diff = end - start
-    print 'time to run %4.2f seconds' % diff
+    print('time to run %4.2f seconds' % diff)
     logging.shutdown()
```

### Comparing `libsnmp-2.0.5/test/test_Messages.py` & `libsnmp-3.0.0/test/test_Messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
-# $Id: test_Messages.py 18 2003-09-21 11:16:40Z daedalus $
-# $Revision: 18 $
+# $Id$
+# $Revision$
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (C) 2003 Unicity Pty Ltd <libsnmp@unicity.com.au>
 #
 #    This library is free software; you can redistribute it and/or
 #    modify it under the terms of the GNU Lesser General Public
 #    License as published by the Free Software Foundation; either
```

### Comparing `libsnmp-2.0.5/test/test_rfc1157.py` & `libsnmp-3.0.0/test/test_rfc1157.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
-# $Id: test_rfc1157.py 33 2005-06-16 02:55:07Z daedalus $
-# $Revision: 33 $
+# $Id$
+# $Revision$
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (C) 2003 Unicity Pty Ltd <libsnmp@unicity.com.au>
 #
 #    This library is free software; you can redistribute it and/or
 #    modify it under the terms of the GNU Lesser General Public
 #    License as published by the Free Software Foundation; either
```

### Comparing `libsnmp-2.0.5/test/test_rfc1155.py` & `libsnmp-3.0.0/test/test_rfc1155.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
-# $Id: test_rfc1155.py 18 2003-09-21 11:16:40Z daedalus $
-# $Revision: 18 $
+# $Id$
+# $Revision$
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (C) 2003 Unicity Pty Ltd <libsnmp@unicity.com.au>
 #
 #    This library is free software; you can redistribute it and/or
 #    modify it under the terms of the GNU Lesser General Public
 #    License as published by the Free Software Foundation; either
@@ -56,29 +56,29 @@
         b = rfc1155.ObjectID(input_b)
         c = rfc1155.ObjectID(input_c)
         d = rfc1155.ObjectID(input_d)
         e = rfc1155.ObjectID('.1.3')
         f = rfc1155.ObjectID().decode(a.encode())[0]
         g = rfc1155.Asn1Object().decode(a.encode())[0]        
         
-        self.assertEquals(a, a)
-        self.assertEquals(a, b)
-        self.assertEquals(a, c)
-        self.assertEquals(a, d)
-        self.assertNotEquals(a, e)
-        self.assertEquals(a, f)
-        self.assertEquals(a, g)        
-        
-        self.assertEquals(b, a)
-        self.assertEquals(b, b)
-        self.assertEquals(b, c)
-        self.assertEquals(b, d)
-        self.assertNotEquals(b, e)        
-        self.assertEquals(b, f)
-        self.assertEquals(b, g)        
+        self.assertEqual(a, a)
+        self.assertEqual(a, b)
+        self.assertEqual(a, c)
+        self.assertEqual(a, d)
+        self.assertNotEqual(a, e)
+        self.assertEqual(a, f)
+        self.assertEqual(a, g)        
+        
+        self.assertEqual(b, a)
+        self.assertEqual(b, b)
+        self.assertEqual(b, c)
+        self.assertEqual(b, d)
+        self.assertNotEqual(b, e)        
+        self.assertEqual(b, f)
+        self.assertEqual(b, g)        
         
         pass
 
     def test_integer(self):
         
         a = rfc1155.Integer(0)
         b = rfc1155.Integer(0x7FFFFFFF)
@@ -97,15 +97,15 @@
                      ('0.0.0.1',          '@\x04\x00\x00\x00\x01'),
                      ('255.0.0.0',        '@\x04\xff\x00\x00\x00'))
         
         for input, output in addresses:
             a = rfc1155.IPAddress(input)
             raw = a.encode()
             b = rfc1155.Asn1Object().decode(raw)[0]
-            self.assertEquals(a,b)
+            self.assertEqual(a,b)
             pass
         return
     
     
     def test_objectid_length(self):
         
         """test length"""
@@ -117,19 +117,19 @@
         
         a = rfc1155.ObjectID(input_a)
         b = rfc1155.ObjectID(input_b)
         c = rfc1155.ObjectID(input_c)
         d = rfc1155.ObjectID(input_d)
         e = rfc1155.ObjectID('.1.3')
         
-        self.assertEquals(len(a), len(input_a))
-        self.assertEquals(len(b), len(input_a))
-        self.assertEquals(len(c), len(input_a))
-        self.assertEquals(len(d), len(input_a))
-        self.assertNotEquals(len(b), len(e))
+        self.assertEqual(len(a), len(input_a))
+        self.assertEqual(len(b), len(input_a))
+        self.assertEqual(len(c), len(input_a))
+        self.assertEqual(len(d), len(input_a))
+        self.assertNotEqual(len(b), len(e))
         
         return
     
     pass
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `libsnmp-2.0.5/test/test_encoder.py` & `libsnmp-3.0.0/test/test_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
-# $Id: test_encoder.py 58 2010-01-30 00:19:41Z daedalus $
-# $Revision: 58 $
+# $Id$
+# $Revision$
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (C) 2003 Unicity Pty Ltd <libsnmp@unicity.com.au>
 #
 #    This library is free software; you can redistribute it and/or
 #    modify it under the terms of the GNU Lesser General Public
 #    License as published by the Free Software Foundation; either
@@ -48,16 +48,16 @@
 }
 
 # octetstrings are simple, since they stay as they are
 test_octetstrings = [
     'fred',
     'the small frog sat in the well',
     '43 403i 594 5908kjljdfj weljf',
-    u'This is a unicode string',
-    u'This is another unicode string',
+    'This is a unicode string',
+    'This is another unicode string',
 ]
 
 test_objectids = {
     '.1.2.4.5.6':                    '\052\004\005\006',
     '1.2.4.5.6':                     '\052\004\005\006',    
     '.2.3.3':                        '\123\003',
     '.0.2.8.5':                      '\002\010\005',
@@ -114,157 +114,157 @@
 
     def tearDown(self):
         logging.shutdown()
 
     def test_integerEncode(self):
         """ Test encoding of Integer type
         """
-        for item in test_integers.keys():
+        for item in list(test_integers.keys()):
             myobj = rfc1155.Integer(item)
 #            self.log.debug('Encoding int: %s' % myobj() )
             octets = myobj.encodeContents()
 #            self.log.debug('Got value [length %s]: %s, oct: %s' % ( len(octets), util.octetsToHex(octets), util.octetsToOct(octets)) )
 #            self.log.debug('check against handcode: %s [%d] %s' % ( util.octetsToHex(test_integers[item]), len(octets), util.octetsToOct(test_integers[item]) ) )
-            self.assertEquals(test_integers[item], octets)
+            self.assertEqual(test_integers[item], octets)
 
     def test_integerEncodeDecode(self):
         """ Test encode/decode of Integer type
         """
-        for item in test_integers.keys():
+        for item in list(test_integers.keys()):
             myobj = rfc1155.Integer(item)
 #            self.log.debug('Encoding int: %s' % myobj() )
             octets = myobj.encodeContents()
 #            self.log.debug('Got value [length %s]: %s, oct: %s' % ( len(octets), util.octetsToHex(octets), util.octetsToOct(octets)) )
             object = myobj.decodeContents(octets)
 #            self.log.debug('Got value [%s]: %s' % ( object, object.value) )
-            self.assertEquals(item, object.value)
+            self.assertEqual(item, object.value)
 
     def test_octetStringEncode(self):
         """ Test encode of OctetString type
         """
 #        self.log.debug('testing octet string in octal and hex')
         for item in test_octetstrings:
             myobj = rfc1155.OctetString(item)
 #            self.log.debug('as hex: %s' % hex(myobj) )
 #            self.log.debug('as octal: %s' % oct(myobj) )
             octets = myobj.encodeContents()
-            self.assertEquals(item, octets)
+            self.assertEqual(item, octets)
 
     def test_octetStringEncodeDecode(self):
         """ Test encode/decode of OctetString type
         """
         for item in test_octetstrings:
             myobj = rfc1155.OctetString(item)
             octets = myobj.encodeContents()
             object = myobj.decodeContents(octets)
-            self.assertEquals(item, object.value)
+            self.assertEqual(item, object.value)
 
     def test_objectidEncode(self):
         
         """Test encode of ObjectID type"""
         
-        for input, output in test_objectids.items():
+        for input, output in list(test_objectids.items()):
             myobj = rfc1155.ObjectID(input)
             octets = myobj.encodeContents()
-            self.assertEquals(octets, output)
+            self.assertEqual(octets, output)
             pass
         return
     
     def test_objectidEncodeDecode(self):
         
         """Test encode/decode of ObjectID type"""
         
-        for input, output in test_objectids.items():
+        for input, output in list(test_objectids.items()):
             myobj = rfc1155.ObjectID(input)
             octets = myobj.encodeContents()
             object = myobj.decodeContents(octets)
             
             result = []
             
             input_check = input.lstrip('.')
             output_check = '.'.join( [ str(x) for x in object.value ] )
-            self.assertEquals(input_check, output_check)
+            self.assertEqual(input_check, output_check)
             pass
         return
     
     def test_nullEncode(self):
         
         """Test encode of Null type"""
         
         myobj = rfc1155.Null()
         octets = myobj.encodeContents()
-        self.assertEquals(octets, '')
+        self.assertEqual(octets, '')
         return
     
     def test_nullEncodeDecode(self):
         
         """Test encode/decode of Null type"""
         
         myobj = rfc1155.Null()
         octets = myobj.encodeContents()
         object = myobj.decodeContents(octets)
-        self.assertEquals(object.value, None)
+        self.assertEqual(object.value, None)
 
     def test_sequenceEncode(self):
         """ Test encode of Sequence type
         """
-        for item in test_sequences.keys():
+        for item in list(test_sequences.keys()):
             myobj = rfc1155.Sequence(test_sequences[item])
             octets = myobj.encodeContents()
             #self.log.debug('Got value [length %s]: %s, oct: %s' % ( len(octets), util.octetsToHex(octets), util.octetsToOct(octets)) )
-            self.assertEquals(item, octets)
+            self.assertEqual(item, octets)
 
     def test_sequenceEncodeDecode(self):
         """ Test encode/decode of Sequence type
         """
-        for item in test_sequences.keys():
+        for item in list(test_sequences.keys()):
             myobj = rfc1155.Sequence(test_sequences[item])
             octets = myobj.encodeContents()
             object = myobj.decodeContents(octets)
             for x, y in zip(myobj.value, object.value):
-                self.assertEquals(x.__class__, y.__class__)
-                self.assertEquals(x.value, y.value)
+                self.assertEqual(x.__class__, y.__class__)
+                self.assertEqual(x.value, y.value)
 
     def test_sequenceofEncode(self):
         """ Test encode of SequenceOf type
         """
-        for item in test_sequenceOf.keys():
+        for item in list(test_sequenceOf.keys()):
             myobj = rfc1155.SequenceOf(test_sequenceOf[item][0], test_sequenceOf[item][1])
 #            self.log.debug('SequenceOf: %s' % myobj)
 
     def test_sequenceofEncodeDecode(self):
         """ Test encode/decode of SequenceOf type
         """
-        for item in test_sequenceOf.keys():
+        for item in list(test_sequenceOf.keys()):
             myobj = rfc1155.SequenceOf(test_sequenceOf[item][0], test_sequenceOf[item][1])
 #            self.log.debug('SequenceOf: %s' % myobj)
             octets = myobj.encodeContents()
             object = myobj.decodeContents(octets)
             for x, y in zip(myobj.value, object.value):
-                self.assertEquals(x.__class__, y.__class__)
-                self.assertEquals(x.value, y.value)
+                self.assertEqual(x.__class__, y.__class__)
+                self.assertEqual(x.value, y.value)
 
     def test_sequenceofNegativeTest_Type(self):
         """ Test mismatching SequenceOf types
         """
         self.assertRaises(ValueError, rfc1155.SequenceOf, rfc1155.Integer, [rfc1155.OctetString('fhdhd')])
 
     def test_ipAddressEncode(self):
         """ Test encode of IPAddress type
         """
-        for item in test_ipaddresses.keys():
+        for item in list(test_ipaddresses.keys()):
             myobj = rfc1155.IPAddress(test_ipaddresses[item])
 #            self.log.debug('IPAddress: %s' % myobj)
 
 
     def test_octetDecode(self):
         """ Test decoding of multiple object types
         """
         decoder = rfc1155.Asn1Object()
-        for item in test_octets.keys():
+        for item in list(test_octets.keys()):
 #            self.log.debug('decoding octets: %s [%s]' % ( item, util.octetsToHex(item) ))
             objectList = decoder.decode( item )
 
 #            self.log.debug('objectList: %s' % objectList)
 #            for object in objectList:
 #                self.log.debug('object: %s, value: %s' % ( object.__class__.__name__, object) )
```

### Comparing `libsnmp-2.0.5/snmpwalk.py` & `libsnmp-3.0.0/snmpget.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,65 @@
-#!/usr/bin/python
-# $Id: snmpwalk.py 46 2007-04-11 05:00:04Z daedalus $
-# $Revision: 46 $
+#!/usr/bin/env python
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 
-import logging
-import socket
-import select
-
 import getopt
-
 import sys
-from libsnmp import debug
-from libsnmp import util
-from libsnmp import rfc1155
-from libsnmp import rfc1157
 
 from libsnmp import snmpmanager
+from libsnmp import util
+
 
 def checkResponse(snmpClient, msg):
     """ Quick and dirty print of what the message contains
     """
     pdu = msg.data
 
-    if int(pdu.errorStatus) != 0:
-        print 'Error: %s' % pdu.errorStatus
+    if int(msg.data.errorStatus) != 0:
+        print('Error: %s' % msg.data.errorStatus)
     else:
         unwrapVarBinds(pdu.varBindList)
 
-        myClient.snmpGetNext(pdu.varBindList, remotesite, checkResponse, community=args[1])
 
 def unwrapVarBinds(varBindList):
     """ Display a set of varbinds
     """
-#    print '%s' % varBindList
-#    print '%s' % varBindList[0].objectID
-#    print '%s' % varBindList[0].objectValue.value
-
-    print '%s = %s: %s' % ( varBindList[0].objectID, varBindList[0].objectValue.__class__.__name__, varBindList[0].objectValue )
+    #    print '%s' % varBindList
+    #    print '%s' % varBindList[0].objectID
+    #    print '%s' % varBindList[0].objectValue
+    print('%s = %s: (%s) %s' % (
+    varBindList[0].objectID, varBindList[0].objectValue.__class__.__name__, varBindList[0].objectValue,
+    varBindList[0].objectValue))
     if varBindList[0].objectValue.__class__.__name__ == 'OctetString':
-        print "   hex: %s" % util.octetsToHex(varBindList[0].objectValue.value)
-    
-    if varBindList[0].objectValue.__class__.__name__ == 'NoSuchObject':
-        log.error("No such object!")
-        sys.exit(0)
-
-    if varBindList[0].objectValue.__class__.__name__ == 'EndOfMibView':
-        log.info("End of MIB View")
-        sys.exit(0)
-        
+        print("   hex: %s" % util.octetsToHex(varBindList[0].objectValue.value))
+
+
 # What to do when we finish
 def whenDone(snmpClient):
     sys.exit(0)
 
+
 # Main bits
 
+# log = logging.getLogger('ping-snmpd')
+
 # Read command line
 options, args = getopt.getopt(sys.argv[1:], '', [])
 
 # Probably replace with something that assigns a random port
-myClient = snmpmanager.snmpManager( whenDone )
+myClient = snmpmanager.snmpManager(whenDone)
+
+# remotesite = ( 'localhost', 161 )
+# myClient.snmpGet('.1.3.6.1.2.1.1.1.0', remotesite, checkResponse)
+# myClient.snmpGet('.1.3.6.1.2.1.1.3.0', remotesite, checkResponse)
 
 if len(args) != 3:
-    print "Usage: snmpget.py <server> <community> <oid>"
+    print("Usage: snmpget.py <server> <community> <oid>")
     sys.exit(1)
 else:
-    remotesite = ( args[0], 161 )
+    remotesite = (args[0], 161)
     myClient.snmpGet(args[2], remotesite, checkResponse, community=args[1])
 
+# myClient.snmpGet('.1.3.6.1.2.1.1.4.0', remotesite, checkResponse)
+
 myClient.run()
```

### Comparing `libsnmp-2.0.5/LICENSE` & `libsnmp-3.0.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# $Id: LICENSE 43 2006-11-06 22:39:17Z daedalus $
-# $Revision: 43 $
-
 Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
```

### Comparing `libsnmp-2.0.5/snmpget-v2.py` & `libsnmp-3.0.0/snmpget-v1.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,77 +1,64 @@
-#!/usr/bin/python
-# $Id: snmpget-v2.py 46 2007-04-11 05:00:04Z daedalus $
-# $Revision: 46 $
+#!/usr/bin/env python
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 
-import logging
-import socket
-import select
-
 import getopt
-
+import select
 import sys
-from libsnmp import debug
-from libsnmp import util
-from libsnmp import rfc1155
+
 from libsnmp import rfc1157
+from libsnmp import v1
 
-from libsnmp import v2
 
 def checkResponse(snmpClient, msg):
     """ Quick and dirty print of what the message contains
     """
     pdu = msg.data
 
     if int(msg.data.errorStatus) != 0:
-        print 'Error: %s' % msg.data.errorStatus
+        print('Error: %s' % msg.data.errorStatus)
     else:
         unwrapVarBinds(pdu.varBindList)
 
+
 def unwrapVarBinds(varBindList):
     """ Display a set of varbinds
     """
-#    print '%s' % varBindList
-#    print '%s' % varBindList[0].objectID
-#    print '%s' % varBindList[0].objectValue
-    print '%s = %s: (%s) %s' % ( varBindList[0].objectID, varBindList[0].objectValue.__class__.__name__, varBindList[0].objectValue, varBindList[0].objectValue )
-
-def getData():
-    (inlist, outlist, errlist) = select.select( [sock], [], [] )
-    if inlist:
-        data = sock.recv(8096)
-    #    log.debug('got data: %s' % util.octetsToHex(data) )
-        msg = rfc1157.Message().decode(data)
-    #    log.debug('message recvd: %s' % msg)
+    #    print '%s' % varBindList
+    #    print '%s' % varBindList[0].objectID
+    #    print '%s' % varBindList[0].objectValue
+    print('%s = %s: (%s) %s' % (
+        varBindList[0].objectID, varBindList[0].objectValue.__class__.__name__, varBindList[0].objectValue,
+        varBindList[0].objectValue))
 
-        checkResponse(msg)
 
 # What to do when we finish
 def whenDone(snmpClient):
     sys.exit(0)
 
+
 # Main bits
 
-#log = logging.getLogger('ping-snmpd')
+# log = logging.getLogger('ping-snmpd')
 
 # Read command line
 options, args = getopt.getopt(sys.argv[1:], '', [])
 
 # Probably replace with something that assigns a random port
-myClient = v2.SNMP( whenDone )
+myClient = v1.SNMP(whenDone)
 
-#remotesite = ( 'localhost', 161 )
-#myClient.snmpGet('.1.3.6.1.2.1.1.1.0', remotesite, checkResponse)
-#myClient.snmpGet('.1.3.6.1.2.1.1.3.0', remotesite, checkResponse)
+# remotesite = ( 'localhost', 161 )
+# myClient.snmpGet('.1.3.6.1.2.1.1.1.0', remotesite, checkResponse)
+# myClient.snmpGet('.1.3.6.1.2.1.1.3.0', remotesite, checkResponse)
 
 if len(args) != 3:
-    print "Usage: snmpget.py <server> <community> <oid>"
+    print("Usage: snmpget.py <server> <community> <oid>")
     sys.exit(1)
 else:
-    remotesite = ( args[0], 161 )
+    remotesite = (args[0], 161)
     myClient.snmpGet(args[2], remotesite, checkResponse, community=args[1])
 
-#myClient.snmpGet('.1.3.6.1.2.1.1.4.0', remotesite, checkResponse)
+# myClient.snmpGet('.1.3.6.1.2.1.1.4.0', remotesite, checkResponse)
 
 myClient.run()
```

### Comparing `libsnmp-2.0.5/setup.py` & `libsnmp-3.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 #!/usr/bin/python
-# $Id: setup.py 58 2010-01-30 00:19:41Z daedalus $
-# $Revision: 58 $
-#
+
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 
 from setuptools import setup
 #from distutils.core import setup
 
 import time
 
-version_major = 2
+version_major = 3
 version_minor = 0
-version_build = 5
+version_build = 0
 version_devel=''
 #version_devel='-dev-' + time.strftime('%Y-%m-%d-%H%M')
 
 version='%d.%d.%d%s' % (version_major, version_minor, version_build, version_devel)
 
 setup(
     name='libsnmp',
     version=version,
 
     packages=['libsnmp'],
     package_dir = { '':'lib'},
     
-##     scripts = ['snmpget.py', 
-##                'snmpwalk.py',
-##                'snmpset.py',
-##                'traplistener.py', 
-##                'trapsender.py',
-##                ],
+    scripts = ['snmpget.py',
+               'snmpget-v1.py',
+               'snmpget-v2.py',
+               'snmpset.py',
+               'snmpwalk.py',
+               'traplistener.py', 
+               'trapsender.py',
+               ],
 
     description='A Python SNMP library',
     long_description='A pure Python implementation of the Simple Network Management Protocol',
     author='Justin Warren',
     author_email='daedalus@eigenmagic.com',
     license='MIT',
-    url='http://www.eigenmagic.com',
-    download_url='http://www.seafelt.com/software/sources',
+    url='https://github.com/jpwarren/libsnmp',
 
     classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Other Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
```

### Comparing `libsnmp-2.0.5/lib/libsnmp/snmpmanager.py` & `libsnmp-3.0.0/lib/libsnmp/snmpmanager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,23 @@
-# $Id: snmpmanager.py 44 2007-01-16 22:09:56Z daedalus $
-# $Revision: 44 $
+# $Id$
+# $Revision$
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 #
 
 ## An snmpmanager understands SNMPv1 and SNMPv2c messages
 ## and so it can encode and decode both.
 
-import socket
-import select
 import logging
-import Queue
-import time
-import os
-import asyncore
+import queue
 
-from libsnmp import debug
 from libsnmp import asynrole
-
 from libsnmp import rfc1157
 from libsnmp import rfc1905
-
 from libsnmp import v1
 from libsnmp import v2
 
 log = logging.getLogger('snmp-manager')
 
 ## Used in typeSetter()
 ## Demo only, really
@@ -34,35 +26,35 @@
     's': 0x04,  ## String
     'o': 0x06,  ## ObjectID
     't': 0x43,  ## TimeTicks
     'a': 0x40,  ## IPAddress
 
     'c': 0x41,  ## Counter
     'C': 0x46,  ## Counter64
-    
-    }
 
-class snmpManager(asynrole.manager):
+}
+
 
-    nextRequestID = 0L      # global counter of requestIDs
+class snmpManager(asynrole.Manager):
+    nextRequestID = 0  # global counter of requestIDs
 
     def __init__(self, queueEmpty=None, trapCallback=None, interface=('0.0.0.0', 0), timeout=0.25):
         """ Create a new snmpManager bound to interface
             queueEmpty is a callback of what to do if I run out
             of stuff to do. Default is to wait for more stuff.
         """
         self.queueEmpty = queueEmpty
-        self.outbound = Queue.Queue()
+        self.outbound = queue.Queue()
         self.callbacks = {}
 
         # What to do if we get a trap
         self.trapCallback = trapCallback
 
         # initialise as an asynrole manager
-        asynrole.manager.__init__(self, (self.receiveData, None), interface=interface, timeout=timeout )
+        asynrole.Manager.__init__(self, (self.receiveData, None), interface=interface, timeout=timeout)
 
         try:
             # figure out the current system uptime
 
             pass
 
         except:
@@ -75,222 +67,222 @@
         self.nextRequestID += 1
         return reqID
 
     def createGetRequestPDU(self, varbindlist, version=2):
         reqID = self.assignRequestID()
 
         if version == 1:
-            pdu = rfc1157.Get( reqID, varBindList=varbindlist )
+            pdu = rfc1157.Get(reqID, varBindList=varbindlist)
 
         elif version == 2:
-            pdu = rfc1905.Get( reqID, varBindList=varbindlist )            
-            
+            pdu = rfc1905.Get(reqID, varBindList=varbindlist)
+
         return pdu
 
     def createGetNextRequestPDU(self, varbindlist, version=2):
         reqID = self.assignRequestID()
-        
+
         if version == 1:
-            pdu = rfc1157.GetNext( reqID, varBindList=varbindlist )
+            pdu = rfc1157.GetNext(reqID, varBindList=varbindlist)
 
         elif version == 2:
-            pdu = rfc1905.GetNext( reqID, varBindList=varbindlist )
-            
+            pdu = rfc1905.GetNext(reqID, varBindList=varbindlist)
+
         return pdu
 
     def createSetRequestPDU(self, varbindlist, version=2):
         reqID = self.assignRequestID()
 
         if version == 1:
-            pdu = rfc1157.Set( reqID, varBindList=varbindlist )
+            pdu = rfc1157.Set(reqID, varBindList=varbindlist)
 
         elif version == 2:
-            pdu = rfc1905.Set( reqID, varBindList=varbindlist )            
-            
+            pdu = rfc1905.Set(reqID, varBindList=varbindlist)
+
         return pdu
 
     def createGetRequestMessage(self, oid, community='public', version=2):
         """ Creates a message object from a pdu and a
             community string.
         """
         if version == 1:
             objID = rfc1157.ObjectID(oid)
             val = rfc1157.Null()
-            varbindlist = rfc1157.VarBindList( [ rfc1157.VarBind(objID, val) ] )
-            pdu = self.createGetRequestPDU( varbindlist, 1 )
-            message = rfc1157.Message( community=community, data=pdu )
+            varbindlist = rfc1157.VarBindList([rfc1157.VarBind(objID, val)])
+            pdu = self.createGetRequestPDU(varbindlist, 1)
+            message = rfc1157.Message(community=community, data=pdu)
 
         elif version == 2:
             objID = rfc1905.ObjectID(oid)
             val = rfc1905.Null()
-            varbindlist = rfc1905.VarBindList( [ rfc1905.VarBind(objID, val) ] )
-            pdu = self.createGetRequestPDU( varbindlist, 2 )
-            message = rfc1905.Message( community=community, data=pdu )
+            varbindlist = rfc1905.VarBindList([rfc1905.VarBind(objID, val)])
+            pdu = self.createGetRequestPDU(varbindlist, 2)
+            message = rfc1905.Message(community=community, data=pdu)
 
         else:
             raise ValueError('Unknown version %d' % version)
 
         return message
 
     def createGetNextRequestMessage(self, varbindlist, community='public', version=2):
         """ Creates a message object from a pdu and a
             community string.
         """
-        pdu = self.createGetNextRequestPDU( varbindlist, version )
+        pdu = self.createGetNextRequestPDU(varbindlist, version)
 
         if version == 1:
-            return rfc1157.Message( community=community, data=pdu )
+            return rfc1157.Message(community=community, data=pdu)
 
         if version == 2:
-            return rfc1905.Message( community=community, data=pdu )
+            return rfc1905.Message(community=community, data=pdu)
 
     def createSetRequestMessage(self, oid, valtype, value, community='public', version=2):
         """ Creates a message object from a pdu and a
             community string.
         """
         if version == 1:
             objID = rfc1157.ObjectID(oid)
             val = rfc1157.tagDecodeDict[valtype](value)
-            varbindlist = rfc1157.VarBindList( [ rfc1157.VarBind(objID, val) ] )
-            pdu = self.createSetRequestPDU( varbindlist, 1 )
-            message = rfc1157.Message( community=community, data=pdu )
+            varbindlist = rfc1157.VarBindList([rfc1157.VarBind(objID, val)])
+            pdu = self.createSetRequestPDU(varbindlist, 1)
+            message = rfc1157.Message(community=community, data=pdu)
 
         elif version == 2:
             objID = rfc1905.ObjectID(oid)
             val = rfc1905.tagDecodeDict[valtype](value)
-            varbindlist = rfc1905.VarBindList( [ rfc1905.VarBind(objID, val) ] )
-            pdu = self.createSetRequestPDU( varbindlist, 1 )
-            message = rfc1905.Message( community=community, data=pdu )
+            varbindlist = rfc1905.VarBindList([rfc1905.VarBind(objID, val)])
+            pdu = self.createSetRequestPDU(varbindlist, 1)
+            message = rfc1905.Message(community=community, data=pdu)
 
         else:
             raise ValueError('Unknown version %d' % version)
 
         return message
 
     def createTrapMessage(self, pdu, community='public', version=2):
         """ Creates a message object from a pdu and a
             community string.
         """
         if version == 1:
-            return v1.createTrapMessage( community=community, data=pdu )
+            return v1.createTrapMessage(community=community, data=pdu)
         elif version == 2:
-            return v2.createTrapMessage( community=community, data=pdu )
+            return v2.createTrapMessage(community=community, data=pdu)
 
-    def createTrapPDU(self, varbindlist, version=2, enterprise='.1.3.6.1.4', agentAddr=None, genericTrap=6, specificTrap=0):
+    def createTrapPDU(self, varbindlist, version=2, enterprise='.1.3.6.1.4', agentAddr=None, genericTrap=6,
+                      specificTrap=0):
         """ Creates a Trap PDU object from a list of strings and integers
             along with a varBindList to make it a bit easier to build a Trap.
         """
         if agentAddr is None:
             agentAddr = self.getsockname()[0]
             pass
 
         if version == 1:
             ent = rfc1157.ObjectID(enterprise)
             agent = rfc1157.NetworkAddress(agentAddr)
             gTrap = rfc1157.GenericTrap(genericTrap)
             sTrap = rfc1157.Integer(specificTrap)
-            ts = rfc1157.TimeTicks( self.getSysUptime() )
+            ts = rfc1157.TimeTicks(self.getSysUptime())
             pdu = rfc1157.TrapPDU(ent, agent, gTrap, sTrap, ts, varbindlist)
-#        log.debug('v1.trap is %s' % pdu)
+        #        log.debug('v1.trap is %s' % pdu)
 
         elif version == 2:
             ent = rfc1905.ObjectID(enterprise)
             agent = rfc1905.NetworkAddress(agentAddr)
             gTrap = rfc1157.GenericTrap(genericTrap)
             sTrap = rfc1905.Integer(specificTrap)
-            ts = rfc1905.TimeTicks( self.getSysUptime() )
+            ts = rfc1905.TimeTicks(self.getSysUptime())
             pdu = rfc1157.TrapPDU(ent, agent, gTrap, sTrap, ts, varbindlist)
             pass
-        
+
         return pdu
 
     def snmpGet(self, oid, remote, callback, community='public', version=2):
         """ snmpGet issues an SNMP Get Request to remote for
             the object ID oid 
             remote is a tuple of (host, port)
             oid is a dotted string eg: .1.2.6.1.0.1.1.3.0
         """
-        msg = self.createGetRequestMessage( oid, community, version )
+        msg = self.createGetRequestMessage(oid, community, version)
 
         # add this message to the outbound queue as a tuple
-        self.outbound.put( (msg, remote) )
+        self.outbound.put((msg, remote))
         # Add the callback to my dictionary with the requestID
         # as the key for later retrieval
         self.callbacks[msg.data.requestID] = callback
 
         return msg.data.requestID
 
     def snmpGetNext(self, varbindlist, remote, callback, community='public', version=2):
         """ snmpGetNext issues an SNMP Get Next Request to remote for
             the varbindlist that is passed in. It is assumed that you
             have either built a varbindlist yourself or just pass
             one in that was previously returned by an snmpGet or snmpGetNext
         """
-        msg = self.createGetNextRequestMessage( varbindlist, community, version )
+        msg = self.createGetNextRequestMessage(varbindlist, community, version)
 
         # add this message to the outbound queue as a tuple
-        self.outbound.put( (msg, remote) )
+        self.outbound.put((msg, remote))
         # Add the callback to my dictionary with the requestID
         # as the key for later retrieval
         self.callbacks[msg.data.requestID] = callback
         return msg.data.requestID
 
     def snmpSet(self, oid, valtype, value, remote, callback, community='public', version=2):
         """
         snmpSet is slightly more complex in that you need to pass in
         a combination of oid and value in order to set a variable.
         Depending on the version, this will be built into the appropriate
         varbindlist for message creation.
         valtype should be a tagDecodeDict key
         """
-        msg = self.createSetRequestMessage( oid, valtype, value, community, version )
+        msg = self.createSetRequestMessage(oid, valtype, value, community, version)
 
         # add this message to the outbound queue as a tuple
-        self.outbound.put( (msg, remote) )
+        self.outbound.put((msg, remote))
         # Add the callback to my dictionary with the requestID
         # as the key for later retrieval
         self.callbacks[msg.data.requestID] = callback
         return msg.data.requestID
 
     def snmpTrap(self, remote, trapPDU, community='public', version=2):
         """ Queue up a trap for sending
         """
         msg = self.createTrapMessage(trapPDU, community, version)
 
-        self.outbound.put( (msg, remote) )
+        self.outbound.put((msg, remote))
 
-
-    def receiveData(self, manager, cb_ctx, (data, src), (exc_type, exc_value, exc_traceback) ):
+    def receiveData(self, manager, cb_ctx, data_src_tuple, exc_tuple):
         """ This method should be called when data is received
             from a remote host.
         """
-
-        # Exception handling
+        (data, src) = data_src_tuple
+        (exc_type, exc_value, exc_traceback) = exc_tuple
         if exc_type is not None:
             raise exc_type(exc_value)
 
         # perform the action on the message by calling the
         # callback from my list of callbacks, passing it the
         # message and a reference to myself
 
         # Decode the data into a message
         msg = rfc1905.Message().decode(data)
 
         # Decode it based on what version of message it is
         if msg.version == 0:
-#            if __debug__: log.debug('Detected SNMPv1 message')
+            #            if __debug__: log.debug('Detected SNMPv1 message')
             self.handleV1Message(msg)
 
         elif msg.version == 1:
-#            if __debug__: log.debug('Detected SNMPv2 message')
+            #            if __debug__: log.debug('Detected SNMPv2 message')
             self.handleV2Message(msg)
 
         else:
             log.error('Unknown message version %d detected' % msg.version)
-            log.error('version is a %s' % msg.version() )
+            log.error('version is a %s' % msg.version())
             raise ValueError('Unknown message version %d detected' % msg.version)
 
     def handleV1Message(self, msg):
         """ Handle reception of an SNMP version 1 message 
         """
         if isinstance(msg.data, rfc1157.PDU):
             self.callbacks[msg.data.requestID](self, msg)
@@ -335,17 +327,17 @@
         while 1:
             try:
                 # check for inbound messages
                 self.poll()
 
                 # send any pending outbound messages
                 request = self.outbound.get(0)
-                self.send( request[0].encode(), request[1] )
+                self.send(request[0].encode(), request[1])
 
-            except Queue.Empty:
+            except queue.Empty:
                 if self.queueEmpty:
                     self.queueEmpty(self)
                 pass
 
             except:
                 raise
```

### Comparing `libsnmp-2.0.5/lib/libsnmp/rfc1902.py` & `libsnmp-3.0.0/lib/libsnmp/rfc1902.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-# $Id: rfc1902.py 43 2006-11-06 22:39:17Z daedalus $
-# $Revision: 43 $
+# $Id$
+# $Revision$
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 #
 # SNMPv2 stuff from RFC 1902
 
-import util
-import debug
-import logging
-import types
-
-from rfc1155 import *
+from .rfc1155 import *
 
 log = logging.getLogger('rfc1902')
 
 ## change logging level.. options of:
 ##
 ## logging.CRITICAL
 ## logging.ERROR
@@ -24,49 +19,55 @@
 ## logging.DEBUG
 
 log.setLevel(logging.INFO)
 
 # Add a new TagNumber for encoding purposes
 asnTagNumbers['Counter64'] = 0x06
 
+
 class Integer32(Integer):
     """ A 32 bit integer
     """
-    MINVAL = -2147483648L
-    MAXVAL = 2147483648L
+    MINVAL = -2147483648
+    MAXVAL = 2147483648
+
 
 class Counter32(Counter):
     """ A 32 bit counter
     """
     pass
 
+
 class Guage32(Guage):
     """ A 32 bit Guage
     """
     pass
 
+
 class Counter64(Counter):
     """ A 64 bit counter
     """
-    MINVAL = 0L
-    MAXVAL = 18446744073709551615L
+    MINVAL = 0
+    MAXVAL = 18446744073709551615
 
     asnTagClass = asnTagNumbers['Counter64']
 
+
 class OctetString(OctetString):
     """ An SNMP v2 OctetString must be between
         0 and 65535 bytes in length
     """
 
     def __init__(self, value=''):
         if len(value) > 65535:
             raise ValueError('OctetString must be shorter than 65535 bytes')
 
         OctetString.__init__(self, value)
 
+
 ## Modify tag decode lookup table to use SNMPv2 classes
 ## instead of the old SNMPv1 classes. Little actual difference
 ## apart from the class names.
 tagDecodeDict[0x02] = Integer32
 tagDecodeDict[0x41] = Counter32
 tagDecodeDict[0x42] = Guage32
 tagDecodeDict[0x46] = Counter64
```

### Comparing `libsnmp-2.0.5/lib/libsnmp/rfc1155.py` & `libsnmp-3.0.0/lib/libsnmp/rfc1155.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,312 +1,313 @@
-# $Id: rfc1155.py 53 2008-10-25 11:14:55Z daedalus $
-# $Revision: 53 $
+# $Id$
+# $Revision$
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 #
 # This file contains all the base types for SNMP with the abstract
 # ASN1 stuff removed and a 'hardcoded' definition used instead.  This
 # means we don't use an abstract ASN.1 library to figure out what
 # stuff is, which is faster for something that is a dedicated
 # application of ASN.1, like SNMP.
 
 # I've included here all the basic SNMPv1 types, since they are used
 # by SNMPv2 and v3.
 
-import util
-import debug
-import logging
-import types
 import copy
+import logging
+from functools import reduce
+
+from . import util
 
 log = logging.getLogger('Asn1Object')
 
 ## change logging level.. options of:
 ##
 ## logging.CRITICAL
 ## logging.ERROR
 ## logging.WARN
 ## logging.INFO
 ## logging.DEBUG
 ##
 log.setLevel(logging.INFO)
 
 asnTagClasses = {
-    'UNIVERSAL':    0x00,
-    'APPLICATION':  0x40,
-    'CONTEXT':      0x80,
-    'PRIVATE':      0xC0
+    'UNIVERSAL': 0x00,
+    'APPLICATION': 0x40,
+    'CONTEXT': 0x80,
+    'PRIVATE': 0xC0
 }
 
 asnTagFormats = {
-    'PRIMITIVE':    0x00,
-    'CONSTRUCTED':  0x20
+    'PRIMITIVE': 0x00,
+    'CONSTRUCTED': 0x20
 }
 
 asnTagNumbers = {
-    
-    'Integer':      0x02,
-    'OctetString':  0x04,
-    'Null':         0x05,
-    'ObjectID':     0x06,
-    'Sequence':     0x10,
-    
+
+    'Integer': 0x02,
+    'OctetString': 0x04,
+    'Null': 0x05,
+    'ObjectID': 0x06,
+    'Sequence': 0x10,
+
     # Application types
-    
-    'IPAddress':        0x00,
-    'Counter':          0x01,
-    'Guage':            0x02,
-    'TimeTicks':        0x03,
-    'Opaque':           0x04,
+
+    'IPAddress': 0x00,
+    'Counter': 0x01,
+    'Guage': 0x02,
+    'TimeTicks': 0x03,
+    'Opaque': 0x04,
 }
 
 
 class Asn1Object:
-
     """Base class for all Asn1Objects This is only intended to
     support a specific subset of ASN1 stuff as defined by the RFCs to
     keep things as simple as possible."""
-    
+
     ##
     ## The asnTag is a number used with BER to encode/decode the
     ## object.
     ##
     asnTagClass = asnTagClasses['UNIVERSAL']
     asnTagFormat = asnTagFormats['PRIMITIVE']
     asnTagNumber = None
-    
+
     value = None
-    
+
     def __init__(self):
         return
-    
+
     def encode(self):
-        
+
         """ encode() this Asn1Object using BER"""
-        
+
         contents = self.encodeContents()
-        
+
         resultlist = []
         resultlist.append(self.encodeIdentifier())
         resultlist.append(self.encodeLength(len(contents)))
         resultlist.append(contents)
-        
+
         result = ''.join(resultlist)
-        
+
         return result
-    
+
     ##
     ##
     def decodeTag(self, stream):
 
         """Decode a BER tag field, returning the tag and the remainder
         of the stream"""
 
         tag = ord(stream[0])
         n = 1
         if tag & 0x1F == 0x1F:
-            
+
             ## A large tag is encoded using concatenated 7-bit values
             ## over the following octets, ignoring the initial 5 bits
             ## in the first octet.  The 8th bit represents a
             ## follow-on.
-            
+
             tag = 0
             while 1:
                 byte = ord(stream[n])
                 tag = (tag << 7) | (byte & 0x7F)
                 n += 1
                 if not byte & 0x80: break
                 pass
             pass
 
         return tag, stream[n:]
-    
+
     ##
     ##
     def decodeLength(self, stream):
-        
+
         """Decode a BER length field, returing the length and the
         remainder of the stream"""
-        
+
         length = ord(stream[0])
         n = 1
         if length & 0x80:
-            
+
             ## Multi-Octet length encoding.  The first octet
             ## represents the run-length (the number of octets used to
             ## build the length)
-            
+
             run = length & 0x7F
             length = 0
-            for i in xrange(run):
+            for i in range(run):
                 length = (length << 8) | ord(stream[n])
                 n += 1
                 pass
             pass
         return length, stream[n:]
-    
+
     ##
     ##
     def decode(self, stream):
-        
+
         """decode() an octet stream into a sequence of Asn1Objects
         This method should be overridden by subclasses to define how
         to decode one of themselves from a fixed length stream.  This
         general case method looks at the identifier at the beginning
         of a stream of octets and uses the appropriate decode() method
         of that known object.  Attempts to decode() an unknown object
         type result in an error.  """
 
-        if type(stream) != types.StringType:
-            raise TypeError('stream should be of type StringType, not %s' % type(stream) )
-        
+        if type(stream) != str:
+            raise TypeError('stream should be of type StringType, not %s' % type(stream))
+
         objects = []
         while len(stream) > 0:
-            
+
             (tag, stream) = self.decodeTag(stream)
             (length, stream) = self.decodeLength(stream)
 
             objectData = stream[:length]
             stream = stream[length:]
-            
+
             try:
                 decoder = tagDecodeDict[tag]()
             except KeyError:
-                raise ValueError('Unknown ASN.1 Type %d' % (tag) )
-            
-            objects.append( decoder.decodeContents(objectData) )
+                raise ValueError('Unknown ASN.1 Type %d' % (tag))
+
+            objects.append(decoder.decodeContents(objectData))
             pass
-        
+
         return objects
-    
+
     def encodeContents(self):
 
         """encodeContents should be overridden by subclasses to encode
         the contents of a particular type"""
-        
+
         raise NotImplementedError
-    
+
     def encodeIdentifier(self):
 
         """encodeIdentifier() returns encoded identifier octets for
         this object.  Section 6.3 of ITU-T-X.209 """
-        
+
         if self.asnTagNumber < 0x1F:
             result = chr(self.asnTagClass | self.asnTagFormat | self.asnTagNumber)
-            
+
         else:
-            
+
             ## Encode each number of the asnTagNumber from 31 upwards
             ## as a sequence of 7-bit numbers with bit 8 set to 1 for
             ## all but the last octet. Bit 8 set to 0 signifies the
             ## last octet of the Identifier octets
-            
+
             # encode the first octet
             resultlist = []
             resultlist.append(chr(self.asnTagClass | self.asnTagFormat | 0x1F))
-            
+
             # encode each subsequent octet
             integer = self.asnTagNumber
             while integer != -1:
                 resultlist.append(chr(integer & 0xFF))
                 integer = integer >> 8
                 pass
             result = ''.join(resultlist)
             pass
-        
+
         return result
 
     def encodeLength(self, length):
-        
+
         """encodeLength() takes the length of the contents and
         produces the encoding for that length.  Section 6.3 of
         ITU-T-X.209 """
-        
+
         if length < 127:
-            result = chr( length & 0xff )
+            result = chr(length & 0xff)
             pass
-        
+
         else:
-            
+
             # Long form - Octet one is the number of octets used to
             # encode the length It has bit 8 set to 1 and the
             # remaining 7 bits are used to encode the number of octets
             # used to encode the length Each subsequent octet uses all
             # 8 bits to encode the length
-            
+
             if __debug__: log.debug('Long length encoding required for length of %d' % length)
 
             resultlist = []
             numOctets = 0
             while length > 0:
                 resultlist.insert(0, chr(length & 0xff))
                 length = length >> 8
                 numOctets += 1
                 pass
-            
+
             # Add a 1 to the front of the octet
             if __debug__: log.debug('long length encoding of: %d octets' % numOctets)
             numOctets = numOctets | 0x80
             resultlist.insert(0, chr(numOctets & 0xff))
-            
+
             result = ''.join(resultlist)
             pass
-        
+
         return result
-    
+
     def encodeEndOfContents(self):
         return '\000\000'
-    
+
     ##
     ## 
     def __eq__(self, other):
         """
         Compare two instance by comparison of their value fields
         only.
         """
-        
+
         return isinstance(other, self.__class__) and self.value == other.value
-#        return self.value == other.value
-    
+
+    #        return self.value == other.value
+
     ##
     ##
     def __ne__(self, other):
-        
+
         """Compare two objects for inequality"""
-        
+
         return not (self == other)
-    
+
     ##
     ##
     def toObjectID(self):
         raise TypeError
-    
+
     pass
 
+
 class Integer(Asn1Object):
     """An ASN.1 Integer type"""
-    
+
     asnTagClass = asnTagClasses['UNIVERSAL']
     asnTagNumber = asnTagNumbers['Integer']
-    
-    MINVAL = -2147483648L
-    MAXVAL =  2147483647L
-    
-    def __init__(self, value=0L):
+
+    MINVAL = -2147483648
+    MAXVAL = 2147483647
+
+    def __init__(self, value=0):
         Asn1Object.__init__(self)
         if not self.MINVAL <= value <= self.MAXVAL:
             if __debug__: log.debug('minval: %d' % self.MINVAL)
             if __debug__: log.debug('maxval: %d' % self.MAXVAL)
             raise ValueError('Integer value of %d is out of bounds' % value)
-        
+
         self.value = value
         return
-    
+
     def __str__(self):
         return '%d' % self.value
 
     def __int__(self):
         return int(self.value)
 
     def __float__(self):
@@ -325,15 +326,15 @@
         """ Return the value of the Integer when referring to it directly
         """
         return self.value
 
     # Define some handy arithmetic operations
     def __eq__(self, other):
         try:
-            if self.value == long(other):
+            if self.value == int(other):
                 return True
 
         except:
             raise
 
         return False
 
@@ -342,401 +343,397 @@
         """
         if not isinstance(integer, self.__class__):
             integer = self.__class__(integer)
 
         return self.__class__(self.value + integer.value)
 
     def __sub__(self, integer):
-        if not isinstance(value, self.__class__):
-            value = self.__class__(value)
+        if not isinstance(integer, self.__class__):
+            integer = self.__class__(integer)
         return self.__class__(self.value + integer.value)
 
     def __hash__(self):
         """ Standard Python integers are easy to hash
             so we just do the same thing.
         """
         return self.value.__hash__()
 
     def encodeContents(self):
 
         ## We handle two special cases otherwise we handle positive
         ## and negative numbers independently
-        
+
         integer = self.value
-        
+
         if integer == 0:
             return '\000'
-            
+
         elif integer == -1:
             return '\377'
-        
+
         elif integer > 0:
             result = []
             while integer != 0:
                 result.insert(0, integer & 0xff)
                 integer >>= 8
                 pass
-            
+
             if result[0] & 0x80:
                 result.insert(0, 0)
                 pass
-            
+
             return ''.join(map(chr, result))
-        
+
         else:
             result = []
             while integer != -1:
                 result.insert(0, integer & 0xff)
                 integer >>= 8
                 pass
-            
+
             if result[0] & 0x80 != 0x80:
                 result.insert(0, 0)
                 pass
-            
+
             return ''.join(map(chr, result))
-        
+
         pass
-    
-    
+
     def decodeContents(self, stream):
         """ Decode some input octet stream into a signed ASN.1 integer
         """
         ##
         ## This method wins because it's consistently the fastest
         ##
-        
-        input = map(ord, stream)
-        
-        if __debug__: log.debug('Decoding %s' % util.octetsToHex(stream) )
-        
-        self.value = 0L
+
+        input = list(map(ord, stream))
+
+        if __debug__: log.debug('Decoding %s' % util.octetsToHex(stream))
+
+        self.value = 0
         byte = input[0]
         if (byte & 0x80) == 0x80:
-            negbit = 0x80L
+            negbit = 0x80
             self.value = byte & 0x7f
-            
-            for i in xrange(1, len(input)):
+
+            for i in range(1, len(input)):
                 negbit <<= 8
                 self.value = (self.value << 8) | input[i]
                 pass
-            
+
             self.value = self.value - negbit
-            
+
         else:
-            self.value = long(byte)
-            for i in xrange(1,len(input)):
+            self.value = int(byte)
+            for i in range(1, len(input)):
                 self.value = (self.value << 8) | input[i]
                 pass
             pass
-        
+
         if __debug__: log.debug('decoded as: %d' % self.value)
-        
+
         return self
-    
+
     def decodeTwosInteger1(self, stream):
-        
+
         """ One algorithm for decoding twos complement Integers """
-        
+
         ##
         ## Original pysnmp algorithm
         ##
-        bytes = map(ord, stream)
+        bytes = list(map(ord, stream))
         if bytes[0] & 0x80:
-            bytes.insert(0, -1L)
+            bytes.insert(0, -1)
             pass
-        
-        result = reduce(lambda x,y: x<<8 | y, bytes, 0L)
-        
+
+        result = reduce(lambda x, y: x << 8 | y, bytes, 0)
+
         return result
-    
+
     def decodeTwosInteger2(self, stream):
-        
+
         """A second algorithm for decoding twos complement Integers
         Coded from scratch by jpw """
-        
+
         val = 0
         byte = ord(stream[0])
         if (byte & 0x80) == 0x80:
-            negbit = 0x80L
+            negbit = 0x80
             val = byte & 0x7f
 
-            for i in range(len(stream)-1):
-                byte = ord(stream[i+1])
+            for i in range(len(stream) - 1):
+                byte = ord(stream[i + 1])
                 negbit <<= 8
                 val = (val << 8) | byte
                 pass
-            
+
             val = val - negbit
-            
+
         else:
             val = byte
-            for i in range(len(stream)-1):
-                byte = ord(stream[i+1])
-                val = (val<<8) | byte
+            for i in range(len(stream) - 1):
+                byte = ord(stream[i + 1])
+                val = (val << 8) | byte
                 pass
             pass
         return val
-    
+
     def decodeTwosInteger3(self, stream):
-        
+
         """ A third algorithm for decoding twos complement Integers
         Coded from scratch by jpw """
-        
+
         val = 0
-        bytes = map(ord, stream)
+        bytes = list(map(ord, stream))
 
         if bytes[0] & 0x80:
-            bytes[0] = bytes[0] & 0x7f      # invert bit 8
-            negbit = 0x80L
+            bytes[0] = bytes[0] & 0x7f  # invert bit 8
+            negbit = 0x80
             for i in bytes:
                 negbit <<= 8
                 val = (val << 8) | i
                 pass
             val = val - (negbit >> 8)
-            
+
         else:
             for i in bytes:
                 val = (val << 8) | i
                 pass
             pass
-        
+
         return val
-    
+
     ##
     ##
     def toObjectID(self):
         return ObjectID([self.value])
+
     pass
 
+
 class OctetString(Asn1Object):
-    
     """An ASN.1 Octet String type"""
-    
+
     asnTagClass = asnTagClasses['UNIVERSAL']
     asnTagNumber = asnTagNumbers['OctetString']
-    
+
     def __init__(self, value=''):
         Asn1Object.__init__(self)
         self.value = copy.copy(value)
         return
-    
+
     def __str__(self):
         return self.value
-    
+
     def encodeContents(self):
-        
         """An OctetString is already encoded. Whee!"""
-        
+
         return self.value
-    
+
     def decodeContents(self, stream):
-        
         """An OctetString is already decoded. Whee!  """
-        
+
         self.value = stream
         return self
-    
+
     def __hex__(self):
-        
-        return ''.join( [ '%.2X' % ord(x) for x in self.value ] )
-    
+        return ''.join(['%.2X' % ord(x) for x in self.value])
+
     def __oct__(self):
-        
-        return ''.join( [ '%3o' % ord(x) for x in self.value ] )
-    
+        return ''.join(['%3o' % ord(x) for x in self.value])
+
     def toObjectID(self):
-        return ObjectID([ ord(x) for x in self.value])
+        return ObjectID([ord(x) for x in self.value])
+
     pass
 
 
 class ObjectID(Asn1Object):
-    
     """An ASN.1 Object Identifier type """
-    
+
     asnTagClass = asnTagClasses['UNIVERSAL']
     asnTagFormat = asnTagFormats['PRIMITIVE']
     asnTagNumber = asnTagNumbers['ObjectID']
-    
+
     def __init__(self, value=None):
-        
+
         """Create an ObjectID - value is a list of subids as a string
         or list"""
-        
+
         Asn1Object.__init__(self)
-        
-        if type(value) == types.StringType:
-            
+
+        if type(value) == str:
+
             value = value.strip('.')
             subidlist = value.split('.')
             self.value = []
-            
+
             for subid in subidlist:
                 number = int(subid)
                 if number < 0 or number > 0x7FFFFFFF:
                     raise ValueError("SubID out of range")
                 self.value.append(number)
                 pass
             pass
-        
-        elif type(value) == types.ListType or type(value) == types.NoneType:
+
+        elif type(value) == list or value is None:
             self.value = copy.copy(value)
-            
-        elif type(value) == types.TupleType:
+
+        elif type(value) == tuple:
             self.value = list(value)
-            
-        elif type(value) == types.IntType:
+
+        elif type(value) == int:
             self.value = [value]
 
         elif isinstance(value, ObjectID):
             self.value = value.value[:]
-            
+
         else:
             raise TypeError('unknown type passed as OID')
-        
+
         return
-    
+
     def __str__(self):
 
         if self.value is not None:
             # Prepend a leading '.' to the OID string
-            return '.' + '.'.join( [str(x) for x in self.value] )
+            return '.' + '.'.join([str(x) for x in self.value])
         else:
             return ''
         pass
-    
+
     def __len__(self):
-        
+
         """Return the length of the value field"""
-        
+
         if self.value is None:
             return 0
         else:
             return len(self.value)
         pass
-    
+
     def __getitem__(self, key):
         if isinstance(key, int):
             return self.value.__getitem__(key)
         else:
             return ObjectID(self.value.__getitem__(key))
         pass
-    
+
     def __delitem__(self, key):
         self.value.__delitem__(key)
         return
 
     def copy(self):
         """
         Return a copy of this object as a new object
         """
         return ObjectID(self.value)
-    
+
     def append(self, subid):
-        if type(subid) == types.IntType:
+        if type(subid) == int:
             self.value.append(subid)
         else:
             raise TypeError
-        return 
-    
+        return
+
     def extend(self, other):
         if isinstance(other, self.__class__):
             self.value.extend(other.value)
         else:
             self.value.extend(other)
             pass
         return None
-    
+
     def isPrefixOf(self, other):
 
         """
         Compares this ObjectID with another ObjectID and returns
         non-None if this ObjectID is a prefix of the other one.
         """
-        
+
         if not isinstance(other, self.__class__):
-            raise TypeError('Attempt to compare ObjectID with non-ObjectID: %s' % other.__repr__() )
+            raise TypeError('Attempt to compare ObjectID with non-ObjectID: %s' % other.__repr__())
         if len(other) < len(self):
             return False
         for i in range(len(self)):
             if self.value[i] != other.value[i]:
                 return False
             pass
         return True
-    
+
     def encodeContents(self):
-        
+
         """encode() an objectID into an octet stream """
-        
+
         result = []
         idlist = self.value[:]
-        
+
         # Do the bit with the first 2 subids
         # section 22.4 of X.209
         idlist.reverse()
         subid1 = (idlist.pop() * 40) + idlist.pop()
         idlist.reverse()
         idlist.insert(0, subid1)
-        
+
         for subid in idlist:
             if subid < 128:
                 result.append(chr(subid & 0x7f))
             else:
                 position = len(result)
                 result.append(chr(subid & 0x7f))
-                
+
                 subid = subid >> 7
                 while subid > 0:
                     result.insert(position, chr(0x80 | (subid & 0x7f)))
                     subid = subid >> 7
                     pass
                 pass
             pass
-        
+
         return ''.join(result)
-    
+
     ##
     ##
     def decodeContents(self, stream):
-        
+
         """decode() a stream into an ObjectID()"""
-        
+
         self.value = []
-        
-        bytes = map(ord, stream)
-        
+
+        bytes = list(map(ord, stream))
+
         if len(stream) == 0:
             raise ValueError('stream of zero length in %s' % self.__class__.__name__)
-        
+
         ##
         ## Do the funky decode of the first octet
         ##
 
         if bytes[0] < 128:
-            self.value.append( int(bytes[0] / 40) )
-            self.value.append( int(bytes[0] % 40) )
+            self.value.append(int(bytes[0] / 40))
+            self.value.append(int(bytes[0] % 40))
 
         else:
-            
+
             ## I haven't bothered putting in the convoluted logic here
             ## because the highest likely assignment for the first
             ## octet is 83 according to Annex B of X.208 Those X.209
             ## does give as an example 2.100.3, which is kinda stupid.
             ## Actually, a lot of the space-saving encodings, like
             ## this first octet, are a real PITA later on.  So yeah,
             ## stuff it, we'll just raise an exception.
-            
+
             raise NotImplementedError('First octet is > 128! Unsupported oid detected')
-        
+
         ##
         ## Decode the rest of the octets
         ##
-        
+
         n = 1
-        
+
         while n < len(bytes):
             subid = bytes[n]
             n += 1
             ##
             ## If bit 8 is not set, this is the last octet of this subid
             ## If bit 8 is set, the subid spans this octet and the ones
             ## afterwards, up until bit 8 isn't set.
@@ -749,348 +746,357 @@
                     val = (val << 7) | (subid & 0x7f)
                     pass
                 self.value.append(val)
             else:
                 self.value.append(subid)
                 pass
             pass
-        
+
         return self
-    
+
     def toObjectID(self):
         return ObjectID(copy.copy(self.value))
-    
+
     pass
 
+
 class Null(Asn1Object):
-    
     """An ASN.1 Object Identifier type"""
-    
+
     asnTagClass = asnTagClasses['UNIVERSAL']
     asnTagFormat = asnTagFormats['PRIMITIVE']
     asnTagNumber = asnTagNumbers['Null']
-    
+
     def __str__(self):
         return '<Null>'
-    
+
     def encodeContents(self):
         return ''
-    
+
     def decodeContents(self, stream):
         if len(stream) != 0:
             raise ValueError('Input stream too long for %s' % self.__class__.__name__)
         return self
+
     pass
 
+
 ##
 ##
 class Sequence(Asn1Object):
-    
     """A Sequence is basically a list of name, value pairs with the
     name being an object Type and the value being an instance of an
     Asn1Object of that Type."""
-    
+
     asnTagClass = asnTagClasses['UNIVERSAL']
     asnTagFormat = asnTagFormats['CONSTRUCTED']
     asnTagNumber = asnTagNumbers['Sequence']
-    
+
     value = []
-    
-    def __init__(self, value=[]):
+
+    def __init__(self, value=None):
         Asn1Object.__init__(self)
+        if value is None:
+            value = []
         self.value = value
         return
-    
+
     def __str__(self):
         result = '['
         res = []
         for item in self.value:
-            res.append( '%s' % item )
+            res.append('%s' % item)
             pass
-        
+
         result += ', '.join(res)
-        
+
         result += ']'
         return result
-    
+
     def __len__(self):
         return len(self.value)
-    
+
     def __getitem__(self, index):
         return self.value[index]
-    
+
     ## We want to implement some usual sequence stuff for this type
     ## such as slices, etc.
-    
+
     def append(self, val):
         self.value.append(val)
-        
+
     def encodeContents(self):
 
         """ To encode a Sequence, we simply encode() each sub-object
         in turn."""
-        
+
         if __debug__: log.debug('Encoding sequence contents...')
         resultlist = []
         for elem in self.value:
-            resultlist.append(elem.encode())
+            resultlist.append(elem.encode() if type(elem) is not str else elem)
             pass
-        
+
         result = ''.join(resultlist)
-        
+
         return result
-    
+
     def decodeContents(self, stream):
-        
+
         """decode a sequence of objects"""
-        
+
         objectList = self.decode(stream)
 
         self.value = objectList
-        #return Sequence(objectList)
+        # return Sequence(objectList)
         return self
+
     pass
 
+
 class SequenceOf(Sequence):
-    
     """A SequenceOf is a special kind of sequence that places a
     constraint on the kind of objects it can contain.  It is variable
     in length."""
-    
+
     asnTagClass = asnTagClasses['UNIVERSAL']
     asnTagFormat = asnTagFormats['CONSTRUCTED']
     asnTagNumber = asnTagNumbers['Sequence']
-    
+
     def __init__(self, componentType=Asn1Object, value=None):
         Sequence.__init__(self)
         self.componentType = componentType
-        
+
         ## Add each item in the list to ourselves, which automatically
         ## checks each one to ensure it is of the correct type.
-        
+
         self.value = []
         if value:
             for item in value:
                 self.append(item)
                 pass
             pass
         return
-    
+
     def append(self, value):
-        if not isinstance( value, self.componentType ):
-            raise ValueError('%s: cannot contain components of type: %s' % (self.__class__.__name__, value.__class__.__name__) )
+        if not isinstance(value, self.componentType):
+            raise ValueError(
+                '%s: cannot contain components of type: %s' % (self.__class__.__name__, value.__class__.__name__))
         Sequence.append(self, value)
         return
+
     pass
 
-class IPAddress(OctetString):
 
+class IPAddress(OctetString):
     """An IpAddress is a special type of OctetString.  It represents a
     32-bit internet address as an OctetString of length 4, in network
     byte order.  """
-    
-    asnTagClass = asnTagClasses['APPLICATION']    
+
+    asnTagClass = asnTagClasses['APPLICATION']
     asnTagFormat = asnTagFormats['PRIMITIVE']
     asnTagNumber = asnTagNumbers['IPAddress']
-    
+
     def __init__(self, value=None):
         OctetString.__init__(self, value)
-        
-        if type(value) == types.StringType:
+
+        if type(value) == str:
             self.value = ''
             listform = value.split('.')
-            
+
             if len(listform) != 4:
                 raise ValueError('IPAddress must be of length 4')
-            
+
             for item in listform:
                 self.value += chr(int(item))
                 pass
             pass
-        elif type(value) == types.ListType:
+        elif type(value) == list:
             if len(value) != 4:
                 raise ValueError('IPAddress must be of length 4')
             pass
         else:
             self.value = ''
             pass
         return
-    
+
     def decodeContents(self, stream):
-        
+
         """An IPAddress is already decoded. Whee!"""
-        
+
         self.value = stream
         return self
-    
+
     def __str__(self):
         result = []
         for item in self.value:
-            result.append( '%d' % ord(item) )
+            result.append('%d' % ord(item))
             pass
         return '.'.join(result)
-    
+
     ##
     ##
     def toObjectID(self):
-        return ObjectID( [ ord(x) for x in self.value ] )
-    
+        return ObjectID([ord(x) for x in self.value])
+
     pass
 
+
 class NetworkAddress(IPAddress):
-    
     """ A Network Address is a CHOICE with only one possible value:
         internet
     """
-    
+
     name = 'internet'
     pass
 
-class Counter(Integer):
 
+class Counter(Integer):
     """ A counter starts at zero and keeps going to a maximum integer
         value of 2^32-1 where it wraps back to zero.
     """
-    
+
     asnTagClass = asnTagClasses['APPLICATION']
     asnTagFormat = asnTagFormats['PRIMITIVE']
     asnTagNumber = asnTagNumbers['Counter']
-    
-    MINVAL = 0L
-    MAXVAL = 4294967295L
-    
+
+    MINVAL = 0
+    MAXVAL = 4294967295
+
     def __add__(self, val):
-        
+
         """ We only add to a counter, and we check for a wrap
             condition.
         """
-        
+
         if self.value + val > self.MAXVAL:
-            self.value = val - ( self.MAXVAL - self.value )
+            self.value = val - (self.MAXVAL - self.value)
         else:
             self.value += val
             pass
         return
-    
+
     def decodeContents(self, stream):
-        
+
         result = Integer.decodeContents(self, stream)
-        
+
         ## Some agents encode Counters incorrectly (hello Solaris) as
         ## a negative number.  I'm assuming most SNMP libraries don't
         ## notice the problem because the are written in C and cast
         ## the result to an unsigned int - problem solved (if
         ## accidentally).  This ugly hack on their behalf flips the
         ## value over to the positive world.
-        
+
         if self.value < 0:
-            self.value += 0x100000000L
+            self.value += 0x100000000
             pass
         return self
-    
+
     pass
 
-class Guage(Integer):
 
+class Guage(Integer):
     """ A Guage is a non negative integer.  It may increase or
         decrease. It latches at a maximum value.
     """
-    
+
     asnTagClass = asnTagClasses['APPLICATION']
     asnTagFormat = asnTagFormats['PRIMITIVE']
     asnTagNumber = asnTagNumbers['Guage']
-    
+
     MINVAL = 0
-    MAXVAL = 4294967295L
-    
+    MAXVAL = 4294967295
+
     def __add__(self, val):
-        
+
         """Add to the Guage, latching at the maximum"""
 
-        if self.value + val > MAXVAL:
-            self.value = MAXVAL
+        if self.value + val > self.__class__.MAXVAL:
+            self.value = self.__class__.MAXVAL
         else:
             self.value += val
             pass
         return
-    
+
     def __sub__(self, val):
 
         """Subtract from the Guage, latching at zerod """
-        
+
         if self.value - val < self.MINVAL:
             self.value = self.MINVAL
         else:
             self.value -= val
             pass
         return
-    
+
     pass
 
+
 class TimeTicks(Integer):
-    
     """ TimeTicks is the number of hundredths of a second since an
         epoch, specified at object creation time
     """
-    
+
     asnTagClass = asnTagClasses['APPLICATION']
     asnTagFormat = asnTagFormats['PRIMITIVE']
     asnTagNumber = asnTagNumbers['TimeTicks']
-    
+
     MINVAL = 0
-    MAXVAL = 4294967295L
-    
+    MAXVAL = 4294967295
+
     epoch = None
-    
+
     def __init__(self, value=0, epoch=None):
         Integer.__init__(self, value)
         if epoch:
             self.epoch = epoch
             pass
         return
+
     pass
 
     def _todo__str__(self):
         """
         Format the TimeTicks value into an actual
         time/date stamp based on the epoch.
         """
         # FIXME: Assumes an epoch of 1 Jan 1970
         return ''
 
-class Opaque(OctetString):
 
+class Opaque(OctetString):
     """Opaque is a fun type that allows you to pass arbitrary ASN.1
     encoded stuff in an object. The value is some ASN.1 syntax encoded
     using BER which this object encodes as an OctetString.  We don't
     do any decoding of this object because we don't have to, and that
     makes this all much quicker.  """
 
     pass
 
+
 class DecodeError(Exception):
     def __init__(self, args=None):
         self.args = args
         return
-    
+
     pass
 
+
 ##
 ## Lookup table for object decoding
 ##
 tagDecodeDict = {
-    
-    0x02:   Integer,
-    0x04:   OctetString,
-    0x05:   Null,
-    0x06:   ObjectID,
-    0x30:   Sequence,
-    
+
+    0x02: Integer,
+    0x04: OctetString,
+    0x05: Null,
+    0x06: ObjectID,
+    0x30: Sequence,
+
     # Application types
-    
-    0x40:   IPAddress,
-    0x41:   Counter,
-    0x42:   Guage,
-    0x43:   TimeTicks,
-    0x44:   Opaque,
-    
-    }
+
+    0x40: IPAddress,
+    0x41: Counter,
+    0x42: Guage,
+    0x43: TimeTicks,
+    0x44: Opaque,
+
+}
```

### Comparing `libsnmp-2.0.5/lib/libsnmp/util.py` & `libsnmp-3.0.0/lib/libsnmp/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# $Id: util.py 43 2006-11-06 22:39:17Z daedalus $
-# $Revision: 43 $
+# $Id$
+# $Revision$
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 # 
 # Some utility functions to help make life easier
 
 def octetsToHex(octets):
```

### Comparing `libsnmp-2.0.5/lib/libsnmp/v2.py` & `libsnmp-3.0.0/lib/libsnmp/v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,159 +1,153 @@
-# $Id: v2.py 57 2010-01-29 23:45:50Z daedalus $
-# $Revision: 57 $
+# $Id$
+# $Revision$
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 #
 # SNMPv2 related functions
 
-#import socket
-#import select
-import logging
-#import Queue
-#import time
-#import os
-#import asyncore
 
+import logging
 import traceback
 
-from libsnmp import debug
 from libsnmp import rfc1155
 from libsnmp import rfc1157
-from libsnmp import rfc1902
 from libsnmp import rfc1905
-#from libsnmp import asynrole
-
 from libsnmp import v1
+
+
 log = logging.getLogger('v2.SNMP')
 
 log.setLevel(logging.INFO)
 
+
 class SNMP(v1.SNMP):
 
     def createGetRequestPDU(self, varbindlist):
         reqID = self.assignRequestID()
-        pdu = rfc1905.Get( reqID, varBindList=varbindlist )
+        pdu = rfc1905.Get(reqID, varBindList=varbindlist)
         return pdu
 
     def createGetNextRequestPDU(self, varbindlist):
         reqID = self.assignRequestID()
-        pdu = rfc1905.GetNext( reqID, varBindList=varbindlist )
+        pdu = rfc1905.GetNext(reqID, varBindList=varbindlist)
         return pdu
 
     def createGetRequestMessage(self, oidlist, community='public'):
         """
         Creates a message object from a pdu and a
         community string.
         @param oidlist: a list of oids to place in the message.
         """
         varbinds = []
         for oid in oidlist:
             objID = rfc1155.ObjectID(oid)
             val = rfc1155.Null()
-            varbinds.append( rfc1157.VarBind(objID, val) )
+            varbinds.append(rfc1157.VarBind(objID, val))
             pass
-        varbindlist = rfc1905.VarBindList( varbinds )
-        pdu = self.createGetRequestPDU( varbindlist )
-        return rfc1905.Message( community=community, data=pdu )
+        varbindlist = rfc1905.VarBindList(varbinds)
+        pdu = self.createGetRequestPDU(varbindlist)
+        return rfc1905.Message(community=community, data=pdu)
 
     def createGetNextRequestMessage(self, varbindlist, community='public'):
         """ Creates a message object from a pdu and a
             community string.
         """
-        pdu = self.createGetNextRequest( varbindlist )
-        return rfc1905.Message( community=community, data=pdu )
+        pdu = self.createGetNextRequest(varbindlist)
+        return rfc1905.Message(community=community, data=pdu)
 
     def createTrapMessage(self, pdu, community='public'):
         """ Creates a message object from a pdu and a
             community string.
         """
-        return rfc1905.Message( community=community, data=pdu )
+        return rfc1905.Message(community=community, data=pdu)
 
     def createTrap(self, varbindlist, enterprise='.1.3.6.1.4', agentAddr=None, genericTrap=6, specificTrap=0):
         """ Creates a Trap PDU object from a list of strings and integers
             along with a varBindList to make it a bit easier to build a Trap.
         """
         ent = rfc1155.ObjectID(enterprise)
         if not agentAddr:
             agentAddr = self.getsockname()[0]
         agent = rfc1155.NetworkAddress(agentAddr)
         gTrap = rfc1157.GenericTrap(genericTrap)
         sTrap = rfc1155.Integer(specificTrap)
-        ts = rfc1155.TimeTicks( self.getSysUptime() )
+        ts = rfc1155.TimeTicks(self.getSysUptime())
 
         pdu = rfc1157.TrapPDU(ent, agent, gTrap, sTrap, ts, varbindlist)
         return pdu
 
     def snmpGet(self, oid, remote, callback, community='public'):
         """ snmpGet issues an SNMP Get Request to remote for
             the object ID oid 
             remote is a tuple of (host, port)
             oid is a dotted string eg: .1.2.6.1.0.1.1.3.0
         """
-        msg = self.createGetRequestMessage( oid, community )
+        msg = self.createGetRequestMessage(oid, community)
         # log.debug('sending message: %s' % msg)
 
         # add this message to the outbound queue as a tuple
-        self.outbound.put( (msg, remote) )
+        self.outbound.put((msg, remote))
         # Add the callback to my dictionary with the requestID
         # as the key for later retrieval
         self.callbacks[int(msg.data.requestID)] = callback
         return msg.data.requestID
 
     def snmpGetNext(self, varbindlist, remote, callback, community='public'):
         """ snmpGetNext issues an SNMP Get Next Request to remote for
             the varbindlist that is passed in. It is assumed that you
             have either built a varbindlist yourself or just pass
             one in that was previously returned by an snmpGet or snmpGetNext
         """
-        msg = self.createGetNextRequestMessage( varbindlist, community )
+        msg = self.createGetNextRequestMessage(varbindlist, community)
 
         # add this message to the outbound queue as a tuple
-        self.outbound.put( (msg, remote) )
+        self.outbound.put((msg, remote))
         # Add the callback to my dictionary with the requestID
         # as the key for later retrieval
         self.callbacks[int(msg.data.requestID)] = callback
         return msg.data.requestID
 
     def snmpSet(self, varbindlist, remote, callback, community='public'):
         """ An snmpSet requires a bit more up front smarts, in that
             you need to pass in a varbindlist of matching OIDs and
             values so that the value type matches that expected for the
             OID. This library does not care about any of that stuff.
 
         """
         reqID = self.assignRequestID()
-        pdu = rfc1157.GetNextRequestPDU( reqID, varBindList=varbindlist )
-        msg = rfc1905.Message( community=community, data=pdu )
+        pdu = rfc1157.GetNextRequestPDU(reqID, varBindList=varbindlist)
+        msg = rfc1905.Message(community=community, data=pdu)
 
         # add this message to the outbound queue as a tuple
-        self.outbound.put( (msg, remote) )
+        self.outbound.put((msg, remote))
         # Add the callback to my dictionary with the requestID
         # as the key for later retrieval
         self.callbacks[int(msg.data.requestID)] = callback
         return msg.data.requestID
 
     def snmpTrap(self, remote, trapPDU, community='public'):
         """ Queue up a trap for sending
         """
         msg = self.createTrapMessage(trapPDU, community)
 
-        self.outbound.put( (msg, remote) )
+        self.outbound.put((msg, remote))
 
     def createSetRequestMessage(self, varBindList, community='public'):
         """ Creates a message object from a pdu and a
             community string.
         """
 
-    def receiveData(self, manager, cb_ctx, (data, src), (exc_type, exc_value, exc_traceback) ):
+    def receiveData(self, manager, cb_ctx, data_src_tuple, exc_tuple):
         """ This method should be called when data is received
             from a remote host.
         """
-        # Exception handling
+        (data, src) = data_src_tuple
+        (exc_type, exc_value, exc_traceback) = exc_tuple
         if exc_type is not None:
             raise exc_type(exc_value)
 
         # perform the action on the message by calling the
         # callback from my list of callbacks, passing it the
         # message and a reference to myself
 
@@ -166,31 +160,31 @@
                 if __debug__: log.debug('Detected SNMPv1 message')
 
             elif msg.version == 1:
                 if __debug__: log.debug('Detected SNMPv2 message')
 
             else:
                 log.error('Unknown message version %d detected' % msg.version)
-                log.error('version is a %s' % msg.version() )
+                log.error('version is a %s' % msg.version())
                 raise ValueError('Unknown message version %d detected' % msg.version)
 
             # Figure out what kind of PDU the message contains
             if isinstance(msg.data, rfc1157.PDU):
-#               if __debug__: log.debug('response to requestID: %d' % msg.data.requestID)
+                #               if __debug__: log.debug('response to requestID: %d' % msg.data.requestID)
                 self.callbacks[int(msg.data.requestID)](self, msg)
 
                 # remove the callback from my list once it's done
                 del self.callbacks[int(msg.data.requestID)]
 
             elif isinstance(msg.data, rfc1157.TrapPDU):
                 if __debug__: log.debug('Detected an inbound Trap')
                 self.trapCallback(self, msg)
 
             else:
                 log.debug('Unknown message type')
 
         # log any errors in callback
-        except Exception, e:
-#            log.error('Exception in callback: %s: %s' % (self.callbacks[int(msg.data.requestID)].__name__, e) )
-            log.error('Exception in receiveData: %s' % e )
+        except Exception as e:
+            #            log.error('Exception in callback: %s: %s' % (self.callbacks[int(msg.data.requestID)].__name__, e) )
+            log.error('Exception in receiveData: %s' % e)
             traceback.print_exc()
-            #raise
+            # raise
```

### Comparing `libsnmp-2.0.5/lib/libsnmp/debug.py` & `libsnmp-3.0.0/lib/libsnmp/debug.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# $Id: debug.py 43 2006-11-06 22:39:17Z daedalus $
-# $Revision: 43 $
-#
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 #
 # Customised logging stuff
 
 import logging
 import os
```

### Comparing `libsnmp-2.0.5/lib/libsnmp/rfc1157.py` & `libsnmp-3.0.0/lib/libsnmp/rfc1157.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-# $Id: rfc1157.py 47 2008-09-25 05:07:01Z daedalus $
-# $Revision: 47 $
+# $Id$
+# $Revision$
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 
 import logging
-import debug
+
 log = logging.getLogger('rfc1157')
 
-from rfc1155 import *
+from .rfc1155 import *
 
 asnTagNumbers['Get'] = 0x00
 asnTagNumbers['GetNext'] = 0x01
 asnTagNumbers['Response'] = 0x02
 asnTagNumbers['Set'] = 0x03
 asnTagNumbers['Trap'] = 0x04
 
+
 class ErrorStatus(Integer):
     """ Error Status
     """
     # define a dictionary of error codes
-    errString = { 
-        0:      'No Error',
-        1:      'Response message would have been too large',
-        2:      'There is no such variable name in this MIB',
-        3:      'The value given has the wrong type',
-        4:      'Object is Read Only',
-        5:      'An unknown error occurred'
+    errString = {
+        0: 'No Error',
+        1: 'Response message would have been too large',
+        2: 'There is no such variable name in this MIB',
+        3: 'The value given has the wrong type',
+        4: 'Object is Read Only',
+        5: 'An unknown error occurred'
     }
 
     errNum = {
-        'noError':      0,
-        'tooBig':       1,
-        'noSuchName':   2,
-        'badValue':     3,
-        'readOnly':     4,
-        'genErr':       5,
+        'noError': 0,
+        'tooBig': 1,
+        'noSuchName': 2,
+        'badValue': 3,
+        'readOnly': 4,
+        'genErr': 5,
     }
-    
+
     def __str__(self):
         """ Return a nicer looking error
         """
         return '%d: %s' % (self.value, self.errString[self.value])
 
     def enum(self, num=None):
         """
@@ -49,38 +50,44 @@
         If a specific number is passed in, use that,
         otherwise, use my current value.
         """
         if num is None:
             num = self.value
         return self.errNum(num)
 
+
 class VarBind(Sequence):
     """ Variable Binding
         This binds a name to an object
     """
+
     def __init__(self, name=None, value=None):
         if name:
-            if not isinstance( name, ObjectID ):
+            if not isinstance(name, ObjectID):
                 raise ValueError('name must be an ObjectID')
         if value:
-            if not isinstance( value, Asn1Object ):
+            if not isinstance(value, Asn1Object):
                 raise ValueError('name must be an Asn1Object')
 
         self.objectID = name
         self.objectValue = value
-        Sequence.__init__(self, [ self.objectID, self.objectValue ] )
+        Sequence.__init__(self, [self.objectID, self.objectValue])
+
 
 class VarBindList(SequenceOf):
     """ A Sequence of VarBinds
     """
+
     def __init__(self, value=[]):
         SequenceOf.__init__(self, VarBind, value)
         return
+
     pass
 
+
 class Message(Sequence):
     """ A Message is the base comms type for all SNMP messages
     """
 
     def __init__(self, version=0, community='public', data=None):
         Sequence.__init__(self)
         self.version = Integer(version)
@@ -101,30 +108,32 @@
         return Sequence.encodeContents(self)
 
     def decode(self, stream):
         objectList = Sequence().decode(stream)
 
         # Should return a single Sequence
         if len(objectList) != 1:
-            raise MessageError('Malformed Message: More than one object decoded.' % len(self.value) )
+            raise MessageError('Malformed Message: More than one object decoded.' % len(self.value))
 
         # Sequence should contain 3 objects
         if len(objectList[0]) != 3:
-            raise MessageError('Malformed Message: Incorrect sequence length %d' % len(self.value) )
+            raise MessageError('Malformed Message: Incorrect sequence length %d' % len(self.value))
 
         self.version = objectList[0][0]
         self.community = objectList[0][1]
         self.data = objectList[0][2]
 
         return self
 
+
 class MessageError(Exception):
     def __init__(self, args=None):
         self.args = args
 
+
 class PDU(Sequence):
     """ Base class for a non-trap PDU
     """
     asnTagClass = asnTagClasses['CONTEXT']
 
     def __init__(self, requestID=0, errorStatus=0, errorIndex=0, varBindList=[]):
         """ __init__ allows you to create a new object with no arguments,
@@ -135,66 +144,72 @@
         Sequence.__init__(self)
 
         self.requestID = Integer(requestID)
         self.errorStatus = ErrorStatus(errorStatus)
         self.errorIndex = Integer(errorIndex)
         self.varBindList = VarBindList(varBindList)
 
-        self.value = [ self.requestID, self.errorStatus, self.errorIndex, self.varBindList ]
+        self.value = [self.requestID, self.errorStatus, self.errorIndex, self.varBindList]
 
     def decodeContents(self, stream):
         """ Decode into a Get PDU Object
         """
         objectList = Sequence.decodeContents(self, stream)
         if len(self.value) != 4:
-            raise PDUError('Malformed PDU: Incorrect length %d' % len(self.value) )
+            raise PDUError('Malformed PDU: Incorrect length %d' % len(self.value))
 
         # Build things with the correct type
         myVarList = VarBindList()
         for item in objectList[3]:
-            myVarList.append( VarBind(item[0], item[1]) )
+            myVarList.append(VarBind(item[0], item[1]))
+
+        return self.__class__(int(objectList[0]), int(objectList[1]), int(objectList[2]), myVarList)
+
 
-        return self.__class__( int(objectList[0]), int(objectList[1]), int(objectList[2]), myVarList)
-        
 class PDUError(Exception):
     def __init__(self, args=None):
         self.args = args
 
+
 class Get(PDU):
     """ A Get Request PDU
     """
     asnTagNumber = asnTagNumbers['Get']
 
+
 class GetNext(PDU):
     """ A GetNext PDU
     """
     asnTagNumber = asnTagNumbers['GetNext']
 
+
 class Response(PDU):
     """ A Response PDU
     """
     asnTagNumber = asnTagNumbers['Get']
 
+
 class Set(PDU):
     """ A Set PDU
     """
     asnTagNumber = asnTagNumbers['Set']
 
+
 class GenericTrap(Integer):
     """
     Generic Trap type
     """
     genericTraps = {
-        0:      'coldStart',
-        1:      'warmStart',
-        2:      'linkDown',
-        3:      'linkUp',
-        4:      'authenticationFailure',
-        5:      'egpNeighborLoss',
-        6:      'enterpriseSpecific',
+        0: 'coldStart',
+        1: 'warmStart',
+        2: 'linkDown',
+        3: 'linkUp',
+        4: 'authenticationFailure',
+        5: 'egpNeighborLoss',
+        6: 'enterpriseSpecific',
     }
 
     def __str__(self):
         """ Return an informative string instead of just a number
         """
         return '%s: %d (%s)' % (self.__class__.__name__, self.value, self.genericTraps[self.value])
 
@@ -204,55 +219,59 @@
         If a specific number is passed in, use that,
         otherwise, use my current value.
         """
         if num is None:
             num = self.value
         return self.genericTraps[num]
 
+
 class TrapPDU(Sequence):
     """ A Trap PDU
     """
     asnTagClass = asnTagClasses['CONTEXT']
     asnTagNumber = asnTagNumbers['Trap']
 
-    def __init__(self, enterprise=None, agentAddr=None, genericTrap=None, specificTrap=None, timestamp=None, varBindList=None):
+    def __init__(self, enterprise=None, agentAddr=None, genericTrap=None, specificTrap=None, timestamp=None,
+                 varBindList=None):
         Sequence.__init__(self)
 
-        self.enterprise = enterprise        # ObjectID
-        self.agentAddr = agentAddr          # NetworkAddress
-        self.genericTrap = genericTrap      # GenericTrap
-        self.specificTrap = specificTrap    # Integer
-        self.timestamp = timestamp          # TimeTicks
-        self.varBindList = varBindList      # VarBindList
-        
+        self.enterprise = enterprise  # ObjectID
+        self.agentAddr = agentAddr  # NetworkAddress
+        self.genericTrap = genericTrap  # GenericTrap
+        self.specificTrap = specificTrap  # Integer
+        self.timestamp = timestamp  # TimeTicks
+        self.varBindList = varBindList  # VarBindList
+
         self.value = []
         self.value.append(self.enterprise)
         self.value.append(self.agentAddr)
         self.value.append(self.genericTrap)
         self.value.append(self.specificTrap)
         self.value.append(self.timestamp)
         self.value.append(self.varBindList)
 
-#    def encodeContents(self):
-#        return Sequence.encodeContents(self)
+    #    def encodeContents(self):
+    #        return Sequence.encodeContents(self)
 
     def decodeContents(self, stream):
         """ Decode into a Get PDU Object
         """
         objectList = Sequence.decodeContents(self, stream)
 
         if len(self.value) != 6:
-            raise PDUError('Malformed TrapPDU: Incorrect length %d' % len(self.value) )
+            raise PDUError('Malformed TrapPDU: Incorrect length %d' % len(self.value))
 
         # Build things with the correct type
         myVarList = VarBindList()
         for item in objectList[5]:
-            myVarList.append( VarBind(item[0], item[1]) )
+            myVarList.append(VarBind(item[0], item[1]))
+
+        return self.__class__(objectList[0], objectList[1], GenericTrap(int(objectList[2])), objectList[3],
+                              objectList[4], myVarList)
 
-        return self.__class__( objectList[0], objectList[1], GenericTrap(int(objectList[2])), objectList[3], objectList[4], myVarList)
 
 # Add some new decode types
 tagDecodeDict[0xa0] = Get
 tagDecodeDict[0xa1] = GetNext
 tagDecodeDict[0xa2] = Response
 tagDecodeDict[0xa3] = Set
 tagDecodeDict[0xa4] = TrapPDU
```

### Comparing `libsnmp-2.0.5/lib/libsnmp/v1.py` & `libsnmp-3.0.0/lib/libsnmp/v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,44 @@
-# $Id: v1.py 43 2006-11-06 22:39:17Z daedalus $
-# $Revision: 43 $
+# $Id$
+# $Revision$
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 #
 # SNMPv1 related functions
 
-import socket
-import select
-import logging
-import Queue
+import queue
 import time
-import os
-import asyncore
 
-from libsnmp import debug
 from libsnmp import asynrole
-
 from libsnmp.rfc1157 import *
 
 log = logging.getLogger('v1.SNMP')
 log.setLevel(logging.INFO)
 
-class SNMP(asynrole.manager):
 
-    nextRequestID = 0L      # global counter of requestIDs
+class SNMP(asynrole.Manager):
+    nextRequestID = 0  # global counter of requestIDs
 
     def __init__(self, interface=('0.0.0.0', 0), queueEmpty=None, trapCallback=None, timeout=0.25):
         """ Create a new SNMPv1 object bound to localaddr
             where localaddr is an address tuple of the form
             ('server', port)
             queueEmpty is a callback of what to do if I run out
             of stuff to do. Default is to wait for more stuff.
         """
         self.queueEmpty = queueEmpty
-        self.outbound = Queue.Queue()
+        self.outbound = queue.Queue()
         self.callbacks = {}
 
         # What to do if we get a trap
         self.trapCallback = trapCallback
 
         # initialise as an asynrole manager
-        asynrole.manager.__init__(self, (self.receiveData, None), interface=interface, timeout=timeout )
+        asynrole.Manager.__init__(self, (self.receiveData, None), interface=interface, timeout=timeout)
 
         try:
             # figure out the current system uptime
 
             pass
 
         except:
@@ -56,126 +49,127 @@
         """
         reqID = self.nextRequestID
         self.nextRequestID += 1
         return reqID
 
     def createGetRequestPDU(self, varbindlist):
         reqID = self.assignRequestID()
-        pdu = Get( reqID, varBindList=varbindlist )
+        pdu = Get(reqID, varBindList=varbindlist)
         return pdu
 
     def createGetNextRequestPDU(self, varbindlist):
         reqID = self.assignRequestID()
-        pdu = GetNext( reqID, varBindList=varbindlist )
+        pdu = GetNext(reqID, varBindList=varbindlist)
         return pdu
 
     def createGetRequestMessage(self, oid, community='public'):
         """ Creates a message object from a pdu and a
             community string.
         """
         objID = ObjectID(oid)
         val = Null()
-        varbindlist = VarBindList( [ VarBind(objID, val) ] )
-        pdu = self.createGetRequestPDU( varbindlist )
-        return Message( community=community, data=pdu )
+        varbindlist = VarBindList([VarBind(objID, val)])
+        pdu = self.createGetRequestPDU(varbindlist)
+        return Message(community=community, data=pdu)
 
     def createGetNextRequestMessage(self, varbindlist, community='public'):
         """ Creates a message object from a pdu and a
             community string.
         """
-        pdu = self.createGetNextRequestPDU( varbindlist )
-        return Message( community=community, data=pdu )
+        pdu = self.createGetNextRequestPDU(varbindlist)
+        return Message(community=community, data=pdu)
 
     def createTrapMessage(self, pdu, community='public'):
         """ Creates a message object from a pdu and a
             community string.
         """
-        return Message( community=community, data=pdu )
+        return Message(community=community, data=pdu)
 
     def createTrapPDU(self, varbindlist, enterprise='.1.3.6.1.4', agentAddr=None, genericTrap=6, specificTrap=0):
         """ Creates a Trap PDU object from a list of strings and integers
             along with a varBindList to make it a bit easier to build a Trap.
         """
         ent = ObjectID(enterprise)
         if not agentAddr:
             agentAddr = self.getsockname()[0]
         agent = NetworkAddress(agentAddr)
         gTrap = GenericTrap(genericTrap)
         sTrap = Integer(specificTrap)
-        ts = TimeTicks( self.getSysUptime() )
+        ts = TimeTicks(self.getSysUptime())
 
         pdu = TrapPDU(ent, agent, gTrap, sTrap, ts, varbindlist)
-#        log.debug('v1.trap is %s' % pdu)
+        #        log.debug('v1.trap is %s' % pdu)
         return pdu
 
     def snmpGet(self, oid, remote, callback, community='public'):
         """ snmpGet issues an SNMP Get Request to remote for
             the object ID oid 
             remote is a tuple of (host, port)
             oid is a dotted string eg: .1.2.6.1.0.1.1.3.0
         """
-        msg = self.createGetRequestMessage( oid, community )
+        msg = self.createGetRequestMessage(oid, community)
 
         # add this message to the outbound queue as a tuple
-        self.outbound.put( (msg, remote) )
+        self.outbound.put((msg, remote))
         # Add the callback to my dictionary with the requestID
         # as the key for later retrieval
         self.callbacks[int(msg.data.requestID)] = callback
         return msg.data.requestID
 
     def snmpGetNext(self, varbindlist, remote, callback, community='public'):
         """ snmpGetNext issues an SNMP Get Next Request to remote for
             the varbindlist that is passed in. It is assumed that you
             have either built a varbindlist yourself or just pass
             one in that was previously returned by an snmpGet or snmpGetNext
         """
-        msg = self.createGetNextRequestMessage( varbindlist, community )
+        msg = self.createGetNextRequestMessage(varbindlist, community)
 
         # add this message to the outbound queue as a tuple
-        self.outbound.put( (msg, remote) )
+        self.outbound.put((msg, remote))
         # Add the callback to my dictionary with the requestID
         # as the key for later retrieval
         self.callbacks[int(msg.data.requestID)] = callback
         return msg.data.requestID
 
     def snmpSet(self, varbindlist, remote, callback, community='public'):
         """ An snmpSet requires a bit more up front smarts, in that
             you need to pass in a varbindlist of matching OIDs and
             values so that the value type matches that expected for the
             OID. This library does not care about any of that stuff.
 
         """
         reqID = self.assignRequestID()
-        pdu = GetNext( reqID, varBindList=varbindlist )
-        msg = Message( community=community, data=pdu )
+        pdu = GetNext(reqID, varBindList=varbindlist)
+        msg = Message(community=community, data=pdu)
 
         # add this message to the outbound queue as a tuple
-        self.outbound.put( (msg, remote) )
+        self.outbound.put((msg, remote))
         # Add the callback to my dictionary with the requestID
         # as the key for later retrieval
         self.callbacks[int(msg.data.requestID)] = callback
         return msg.data.requestID
 
     def snmpTrap(self, remote, trapPDU, community='public'):
         """ Queue up a trap for sending
         """
         msg = self.createTrapMessage(trapPDU, community)
 
-        self.outbound.put( (msg, remote) )
+        self.outbound.put((msg, remote))
 
     def createSetRequestMessage(self, varBindList, community='public'):
         """ Creates a message object from a pdu and a
             community string.
         """
 
-    def receiveData(self, manager, cb_ctx, (data, src), (exc_type, exc_value, exc_traceback) ):
+    def receiveData(self, manager, cb_ctx, data_src_tuple, exc_tuple):
         """ This method should be called when data is received
             from a remote host.
         """
-        # Exception handling
+        (data, src) = data_src_tuple
+        (exc_type, exc_value, exc_traceback) = exc_tuple
         if exc_type is not None:
             raise exc_type(exc_value)
 
         # perform the action on the message by calling the
         # callback from my list of callbacks, passing it the
         # message and a reference to myself
 
@@ -185,36 +179,36 @@
 
             # Decode it based on what version of message it is
             if msg.version == 0:
                 if __debug__: log.debug('Detected SNMPv1 message')
 
             else:
                 log.error('Unknown message version %d detected' % msg.version)
-                log.error('version is a %s' % msg.version() )
+                log.error('version is a %s' % msg.version())
                 raise ValueError('Unknown message version %d detected' % msg.version)
 
             # Figure out what kind of PDU the message contains
             if isinstance(msg.data, PDU):
-#               if __debug__: log.debug('response to requestID: %d' % msg.data.requestID)
+                #               if __debug__: log.debug('response to requestID: %d' % msg.data.requestID)
                 self.callbacks[int(msg.data.requestID)](self, msg)
 
                 # remove the callback from my list once it's done
                 del self.callbacks[int(msg.data.requestID)]
 
             elif isinstance(msg.data, TrapPDU):
                 if __debug__: log.debug('Detected an inbound Trap')
                 self.trapCallback(self, msg)
 
             else:
                 if __debug__: log.debug('Unknown message type')
 
         # log any errors in callback
-        except Exception, e:
-#            log.error('Exception in callback: %s: %s' % (self.callbacks[int(msg.data.requestID)].__name__, e) )
-            log.error('Exception in receiveData: %s' % e )
+        except Exception as e:
+            #            log.error('Exception in callback: %s: %s' % (self.callbacks[int(msg.data.requestID)].__name__, e) )
+            log.error('Exception in receiveData: %s' % e)
             raise
 
     def enterpriseOID(self, partialOID):
         """ A convenience method to automagically prepend the
             'enterprise' prefix to the partial OID
         """
         return '.1.3.6.1.2.1.' + partialOID
@@ -223,17 +217,17 @@
         """ Listen for incoming request thingies
             and send pending requests
         """
         while True:
             try:
                 # send any pending outbound messages
                 request = self.outbound.get(0)
-                self.send( request[0].encode(), request[1] )
+                self.send(request[0].encode(), request[1])
 
-            except Queue.Empty:
+            except queue.Empty:
                 if self.queueEmpty is not None:
                     self.queueEmpty(self)
                 pass
 
                 # check for inbound messages
                 self.poll()
```

### Comparing `libsnmp-2.0.5/lib/libsnmp/role.py` & `libsnmp-3.0.0/lib/libsnmp/role.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,62 @@
-# $Id: role.py 43 2006-11-06 22:39:17Z daedalus $
-# $Revision: 43 $
+# $Id$
+# $Revision$
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 
-import socket
 import logging
-import time
-
-from libsnmp import debug
-from libsnmp import rfc1155
-from libsnmp import rfc1157
+import socket
 
 log = logging.getLogger('v1.SNMP')
 
+
 class manager:
-    
+
     def __init__(self, dest, interface=('0.0.0.0', 0), socksize=0x10000):
-        
+
         self.dest = dest
         self.interface = interface
         self.socket = None
         self.socksize = socksize
         self.request_id = 1
-        
+
         return
-    
+
     def __del__(self):
         self.close()
         return
-    
+
     def get_socket(self):
         return self.socket
-    
+
     def open(self):
-        
+
         self.socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self.socket.bind(self.interface)
         self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_RCVBUF, self.socksize)
-        
+
         return self.socket
-    
+
     def send(self, request, dst=(None, 0)):
         if not self.socket:
             self.open()
             pass
         self.socket.sendto(request, dst)
         return
-    
+
     def read(self):
         if not self.socket:
             raise ValueError('Socket not initialized')
-        
+
         (message, src) = self.socket.recvfrom(self.socksize)
-        
+
         return (message, src)
-    
+
     def close(self):
         if self.socket:
             self.socket.close()
             pass
-        self.socket = None  
+        self.socket = None
         return
-    
+
     pass
```

### Comparing `libsnmp-2.0.5/lib/libsnmp/asynrole.py` & `libsnmp-3.0.0/lib/libsnmp/asynrole.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-# $Id: asynrole.py 43 2006-11-06 22:39:17Z daedalus $
-# $Revision: 43 $
+# $Id$
+# $Revision$
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 
-import sys
 import asyncore
-import types
+import sys
 
-from libsnmp import rfc1155
-from libsnmp import rfc1157
 from libsnmp import role
 
-class manager(asyncore.dispatcher):
-    
-    def __init__(self, (cb_fun, cb_ctx), dst=(None, 0), interface=('0.0.0.0', 0), timeout=0.25):
-        
+
+class Manager(asyncore.dispatcher):
+
+    def __init__(self, callback_tuple, dst=(None, 0), interface=('0.0.0.0', 0), timeout=0.25):
+
+        (cb_fun, cb_ctx) = callback_tuple
         if not callable(cb_fun):
             raise ValueError('Non-callable callback function')
-        
+
         self.cb_fun = cb_fun
         self.cb_ctx = cb_ctx
 
         self.timeout = timeout
-        
+
         asyncore.dispatcher.__init__(self)
-        
+
         self.manager = role.manager(dst, interface)
-        
+
         self.set_socket(self.manager.open())
         return
-    
+
     def send(self, req, dst=(None, 0)):
         self.manager.send(req, dst)
         return
-    
+
     def handle_read(self):
         (response, src) = self.manager.read()
         self.cb_fun(self, self.cb_ctx, (response, src), (None, None, None))
         return
-    
+
     def writable(self):
         return 0
-    
+
     def handle_connect(self):
         return
-    
+
     def handle_close(self):
         self.manager.close()
         return
-    
+
     def handle_error(self, exc_type=None, exc_value=None, exc_traceback=None):
         if exc_type is None or exc_value is None or exc_traceback is None:
             exc_type, exc_value, exc_traceback = sys.exc_info()
             pass
-        if type(exc_type) == types.ClassType and issubclass(exc_type, ValueError):
+        if type(exc_type) == type and issubclass(exc_type, ValueError):
             self.cb_fun(self, self.cb_ctx, (None, None), (exc_type, exc_value, exc_traceback))
         else:
             raise
-        
+
         return
+
     pass
 
     def poll(self):
         asyncore.poll(self.timeout)
```

### Comparing `libsnmp-2.0.5/lib/libsnmp/rfc1905.py` & `libsnmp-3.0.0/lib/libsnmp/rfc1905.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,68 +1,74 @@
-# $Id: rfc1905.py 46 2007-04-11 05:00:04Z daedalus $
-# $Revision: 46 $
+# $Id$
+# $Revision$
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 #
 # SNMPv2 protocol parts
 
-import logging
-import debug
-
-import rfc1157
-from rfc1902 import *
+from . import rfc1157
+from .rfc1902 import *
 
 log = logging.getLogger('rfc1905')
 
 asnTagNumbers['GetBulk'] = 0x05
 asnTagNumbers['Inform'] = 0x06
 asnTagNumbers['TrapV2'] = 0x07
 asnTagNumbers['Report'] = 0x08
 
-max_bindings = 2147483647L
+max_bindings = 2147483647
+
 
 class VarBind(rfc1157.VarBind):
     """ VarBind redefined here to place it in the same namespace
     """
     pass
 
+
 ## We need to add some special types because ucd-snmp uses
 ## context specific values for the CHOICE within a VarBind
 class NoSuchObject(rfc1157.Null):
 
     def __str__(self):
-        return('No Such Object')
+        return ('No Such Object')
+
 
 class NoSuchInstance(rfc1157.Null):
 
     def __str__(self):
-        return('No Such Instance')
+        return ('No Such Instance')
+
 
 class EndOfMibView(rfc1157.Null):
 
     def __str__(self):
-        return('EndOfMibView')
+        return ('EndOfMibView')
+
 
 class VarBindList(rfc1157.VarBindList):
     """ An SNMPv2 VarBindList has a maximum size of max_bindings
     """
+
     def __init__(self, value=[]):
         if len(value) > max_bindings:
             raise ValueError('A VarBindList must be shorter than %d' % max_bindings)
         rfc1157.VarBindList.__init__(self, value)
 
+
 class Message(rfc1157.Message):
 
     def __init__(self, version=1, community='public', data=None):
         rfc1157.Message.__init__(self, version, community, data)
 
+
 class ErrorStatus(rfc1157.ErrorStatus):
     """ An SNMPv2 Error status
     """
+
     def __init__(self, value):
         rfc1157.ErrorStatus.__init__(self, value)
         # add to the SNMPv1 error strings
         self.errString[6] = 'Access is not permitted'
         self.errString[7] = 'Type is incorrect'
         self.errString[8] = 'Length is incorrect'
         self.errString[9] = 'Encoding is incorrect'
@@ -86,14 +92,15 @@
         self.errNum[13] = 'resourceUnavailable'
         self.errNum[14] = 'commitFailed'
         self.errNum[15] = 'undoFailed'
         self.errNum[16] = 'authorizationError'
         self.errNum[17] = 'notWritable'
         self.errNum[18] = 'inconsistentName'
 
+
 class PDU(rfc1157.PDU):
     """ SNMPv2 PDUs are very similar to SNMPv1 PDUs
     """
     asnTagClass = asnTagClasses['CONTEXT']
 
     def __init__(self, requestID=0, errorStatus=0, errorIndex=0, varBindList=[]):
         rfc1157.PDU.__init__(self)
@@ -109,14 +116,15 @@
         self.value = [
             self.requestID,
             self.errorStatus,
             self.errorIndex,
             self.varBindList,
         ]
 
+
 #    def decodeContents(self, stream):
 #        """ Decode into a PDU object
 #        """
 #        objectList = Sequence.decodeContents(self, stream)
 #        if len(self.value) != 4:
 #            raise PDUError('Malformed PDU: Incorrect length %d' % len(self.value) )
 #
@@ -154,66 +162,77 @@
         ]
 
     def decodeContents(self, stream):
         """ Decode into a BulkPDU object
         """
         objectList = Sequence.decodeContents(self, stream)
         if len(self.value) != 4:
-            raise PDUError('Malformed BulkPDU: Incorrect length %d' % len(self.value) )
+            raise PDUError('Malformed BulkPDU: Incorrect length %d' % len(self.value))
 
         # Build things with the correct types
+        myVarList = []
         for item in objectList[3]:
-            myVarList.append( VarBind(item[0], item[1]) )
+            myVarList.append(VarBind(item[0], item[1]))
+
+        return self.__class__(int(objectList[0]), int(objectList[1]), int(objectList[2]), myVarList)
 
-        return self.__class__( int(objectList[0]), int(objectList[1]), int(objectList[2]), myVarList)
 
 class Get(PDU):
     """ An SNMPv2 Get Request PDU
     """
     asnTagNumber = asnTagNumbers['Get']
 
+
 class GetNext(PDU):
     """ An SNMPv2 Get Next Request PDU
     """
     asnTagNumber = asnTagNumbers['GetNext']
 
+
 class Response(PDU):
     """ An SNMPv2 Response PDU
     """
     asnTagNumber = asnTagNumbers['Response']
 
+
 class Set(PDU):
     """ An SNMPv2 Set Request PDU
     """
     asnTagNumber = asnTagNumbers['Set']
 
+
 class GetBulk(BulkPDU):
     """ An SNMPv2 Get Next Request PDU
     """
     asnTagNumber = asnTagNumbers['GetBulk']
 
+
 class Inform(PDU):
     """ An SNMPv2 Get Next Request PDU
     """
     asnTagNumber = asnTagNumbers['Inform']
 
+
 class TrapV2(PDU):
     """ An SNMPv2 Trap PDU
     """
     asnTagNumber = asnTagNumbers['TrapV2']
 
+
 class Report(PDU):
     """ An SNMPv2 Report PDU
     """
     asnTagNumber = asnTagNumbers['Report']
 
+
 class PDUError(Exception):
     def __init__(self, args=None):
         self.args = args
 
+
 ## Add some new decode types
 
 tagDecodeDict[0xa2] = Response
 tagDecodeDict[0xa5] = GetBulk
 tagDecodeDict[0xa6] = Inform
 tagDecodeDict[0xa7] = TrapV2
 tagDecodeDict[0xa8] = Report
```

### Comparing `libsnmp-2.0.5/COPYRIGHT` & `libsnmp-3.0.0/debian/copyright`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# $Id: COPYRIGHT 43 2006-11-06 22:39:17Z daedalus $
-# $Revision: 43 $
-#
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
```

### Comparing `libsnmp-2.0.5/snmpget-v1.py` & `libsnmp-3.0.0/snmpget-v2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,64 @@
-#!/usr/bin/python
-# $Id: snmpget-v1.py 46 2007-04-11 05:00:04Z daedalus $
-# $Revision: 46 $
+#!/usr/bin/env python
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 
-import logging
-import socket
-import select
-
 import getopt
-
+import select
 import sys
-from libsnmp import debug
-from libsnmp import util
-from libsnmp import rfc1155
+
 from libsnmp import rfc1157
+from libsnmp import v2
 
-from libsnmp import v1
 
 def checkResponse(snmpClient, msg):
     """ Quick and dirty print of what the message contains
     """
     pdu = msg.data
 
     if int(msg.data.errorStatus) != 0:
-        print 'Error: %s' % msg.data.errorStatus
+        print('Error: %s' % msg.data.errorStatus)
     else:
         unwrapVarBinds(pdu.varBindList)
 
+
 def unwrapVarBinds(varBindList):
     """ Display a set of varbinds
     """
-#    print '%s' % varBindList
-#    print '%s' % varBindList[0].objectID
-#    print '%s' % varBindList[0].objectValue
-    print '%s = %s: (%s) %s' % ( varBindList[0].objectID, varBindList[0].objectValue.__class__.__name__, varBindList[0].objectValue, varBindList[0].objectValue )
-
-def getData():
-    (inlist, outlist, errlist) = select.select( [sock], [], [] )
-    if inlist:
-        data = sock.recv(8096)
-    #    log.debug('got data: %s' % util.octetsToHex(data) )
-        msg = rfc1157.Message().decode(data)
-    #    log.debug('message recvd: %s' % msg)
+    #    print '%s' % varBindList
+    #    print '%s' % varBindList[0].objectID
+    #    print '%s' % varBindList[0].objectValue
+    print('%s = %s: (%s) %s' % (
+        varBindList[0].objectID, varBindList[0].objectValue.__class__.__name__, varBindList[0].objectValue,
+        varBindList[0].objectValue))
 
-        checkResponse(msg)
 
 # What to do when we finish
 def whenDone(snmpClient):
     sys.exit(0)
 
+
 # Main bits
 
-#log = logging.getLogger('ping-snmpd')
+# log = logging.getLogger('ping-snmpd')
 
 # Read command line
 options, args = getopt.getopt(sys.argv[1:], '', [])
 
 # Probably replace with something that assigns a random port
-myClient = v1.SNMP( whenDone )
+myClient = v2.SNMP(whenDone)
 
-#remotesite = ( 'localhost', 161 )
-#myClient.snmpGet('.1.3.6.1.2.1.1.1.0', remotesite, checkResponse)
-#myClient.snmpGet('.1.3.6.1.2.1.1.3.0', remotesite, checkResponse)
+# remotesite = ( 'localhost', 161 )
+# myClient.snmpGet('.1.3.6.1.2.1.1.1.0', remotesite, checkResponse)
+# myClient.snmpGet('.1.3.6.1.2.1.1.3.0', remotesite, checkResponse)
 
 if len(args) != 3:
-    print "Usage: snmpget.py <server> <community> <oid>"
+    print("Usage: snmpget.py <server> <community> <oid>")
     sys.exit(1)
 else:
-    remotesite = ( args[0], 161 )
+    remotesite = (args[0], 161)
     myClient.snmpGet(args[2], remotesite, checkResponse, community=args[1])
 
-#myClient.snmpGet('.1.3.6.1.2.1.1.4.0', remotesite, checkResponse)
+# myClient.snmpGet('.1.3.6.1.2.1.1.4.0', remotesite, checkResponse)
 
 myClient.run()
```

### Comparing `libsnmp-2.0.5/snmpset.py` & `libsnmp-3.0.0/snmpset.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,71 @@
-#!/usr/bin/env python2.3
-# $Id: snmpset.py 43 2006-11-06 22:39:17Z daedalus $
-# $Revision: 43 $
+#!/usr/bin/env python
 #
 #    libsnmp - a Python SNMP library
 #    Copyright (c) 2003 Justin Warren <daedalus@eigenmagic.com>
 
-import logging
-import socket
-import select
-
 import getopt
 
 import sys
+
 sys.path.append('lib')
-from libsnmp import debug
-from libsnmp import util
-from libsnmp import rfc1155
-from libsnmp import rfc1157
 
 from libsnmp import snmpmanager
 
+
 def checkResponse(snmpClient, msg):
     """ Quick and dirty print of what the message contains
     """
     pdu = msg.data
 
     if int(msg.data.errorStatus) != 0:
-        print 'Error: %s' % msg.data.errorStatus
+        print('Error: %s' % msg.data.errorStatus)
     else:
         unwrapVarBinds(pdu.varBindList)
 
+
 def unwrapVarBinds(varBindList):
     """ Display a set of varbinds
     """
-#    print '%s' % varBindList
-#    print '%s' % varBindList[0].objectID
-#    print '%s' % varBindList[0].objectValue
-    print '%s = %s: (%s) %s' % ( varBindList[0].objectID, varBindList[0].objectValue.__class__.__name__, varBindList[0].objectValue, varBindList[0].objectValue )
+    #    print '%s' % varBindList
+    #    print '%s' % varBindList[0].objectID
+    #    print '%s' % varBindList[0].objectValue
+    print('%s = %s: (%s) %s' % (
+    varBindList[0].objectID, varBindList[0].objectValue.__class__.__name__, varBindList[0].objectValue,
+    varBindList[0].objectValue))
+
 
 # What to do when we finish
 def whenDone(snmpClient):
     sys.exit(0)
 
+
 # Main bits
 
-#log = logging.getLogger('ping-snmpd')
+# log = logging.getLogger('ping-snmpd')
 
 # Read command line
 options, args = getopt.getopt(sys.argv[1:], '', [])
 
 # Probably replace with something that assigns a random port
-myClient = snmpmanager.snmpManager( whenDone )
+myClient = snmpmanager.snmpManager(whenDone)
 
-#remotesite = ( 'localhost', 161 )
-#myClient.snmpGet('.1.3.6.1.2.1.1.1.0', remotesite, checkResponse)
-#myClient.snmpGet('.1.3.6.1.2.1.1.3.0', remotesite, checkResponse)
+# remotesite = ( 'localhost', 161 )
+# myClient.snmpGet('.1.3.6.1.2.1.1.1.0', remotesite, checkResponse)
+# myClient.snmpGet('.1.3.6.1.2.1.1.3.0', remotesite, checkResponse)
 
 if len(args) != 5:
-    print "Usage: snmpset.py <server> <community> <oid> <type> <value>"
+    print("Usage: snmpset.py <server> <community> <oid> <type> <value>")
     sys.exit(1)
 else:
-    remotesite = ( args[0], 161 )
-    typeval = myClient.typeSetter( args[3] )
+    remotesite = (args[0], 161)
+    typeval = myClient.typeSetter(args[3])
     if args[3] == 'i':
         value = int(args[4])
     else:
         value = args[4]
-    
+
     myClient.snmpSet(args[2], typeval, value, remotesite, checkResponse, community=args[1])
 
-#myClient.snmpGet('.1.3.6.1.2.1.1.4.0', remotesite, checkResponse)
+# myClient.snmpGet('.1.3.6.1.2.1.1.4.0', remotesite, checkResponse)
 
 myClient.run()
```

