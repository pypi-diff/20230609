# Comparing `tmp/dnszone-2.0.2.tar.gz` & `tmp/dnszone-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dnszone-2.0.2.tar", last modified: Fri Feb 28 19:51:04 2020, max compression
+gzip compressed data, was "dnszone-3.1.1.tar", last modified: Fri Jun  9 01:18:07 2023, max compression
```

## Comparing `dnszone-2.0.2.tar` & `dnszone-3.1.1.tar`

### file list

```diff
@@ -1,18 +1,35 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-28 19:51:04.000000 dnszone-2.0.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5531 2020-02-28 19:51:04.000000 dnszone-2.0.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2816 2020-02-28 19:50:31.000000 dnszone-2.0.2/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-28 19:51:04.000000 dnszone-2.0.2/dnszone/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10365 2020-02-28 19:50:31.000000 dnszone-2.0.2/dnszone/dnszone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1667 2020-02-28 19:50:31.000000 dnszone-2.0.2/dnszone/zone_reload.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1615 2020-02-28 19:50:31.000000 dnszone-2.0.2/dnszone/zone_check.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1923 2020-02-28 19:50:31.000000 dnszone-2.0.2/dnszone/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-02-28 19:51:04.000000 dnszone-2.0.2/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-28 19:51:04.000000 dnszone-2.0.2/dnszone.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5531 2020-02-28 19:51:04.000000 dnszone-2.0.2/dnszone.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-28 19:51:04.000000 dnszone-2.0.2/dnszone.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-02-28 19:51:04.000000 dnszone-2.0.2/dnszone.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-28 19:51:04.000000 dnszone-2.0.2/dnszone.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      320 2020-02-28 19:51:04.000000 dnszone-2.0.2/dnszone.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2020-02-28 19:51:04.000000 dnszone-2.0.2/dnszone.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2020-02-28 19:51:04.000000 dnszone-2.0.2/dnszone.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3189 2020-02-28 19:50:31.000000 dnszone-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:18:07.830495 dnszone-3.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:18:07.826495 dnszone-3.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-09 01:17:41.000000 dnszone-3.1.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-09 01:17:41.000000 dnszone-3.1.1/.github/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-09 01:17:41.000000 dnszone-3.1.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:18:07.830495 dnszone-3.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-09 01:17:41.000000 dnszone-3.1.1/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-09 01:17:41.000000 dnszone-3.1.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-09 01:17:41.000000 dnszone-3.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-09 01:17:41.000000 dnszone-3.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-09 01:17:41.000000 dnszone-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-09 01:18:07.830495 dnszone-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-09 01:17:41.000000 dnszone-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:18:07.830495 dnszone-3.1.1/dnszone/
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-09 01:17:41.000000 dnszone-3.1.1/dnszone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-06-09 01:17:41.000000 dnszone-3.1.1/dnszone/dnszone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 01:18:07.000000 dnszone-3.1.1/dnszone/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-09 01:17:41.000000 dnszone-3.1.1/dnszone/zone_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-09 01:17:41.000000 dnszone-3.1.1/dnszone/zone_reload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:18:07.830495 dnszone-3.1.1/dnszone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-09 01:18:07.000000 dnszone-3.1.1/dnszone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-09 01:18:07.000000 dnszone-3.1.1/dnszone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:18:07.000000 dnszone-3.1.1/dnszone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 01:18:07.000000 dnszone-3.1.1/dnszone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 01:18:07.000000 dnszone-3.1.1/dnszone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-09 01:17:41.000000 dnszone-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 01:18:07.830495 dnszone-3.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:18:07.830495 dnszone-3.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:17:41.000000 dnszone-3.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15733 2023-06-09 01:17:41.000000 dnszone-3.1.1/tests/dnszone_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:18:07.830495 dnszone-3.1.1/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-09 01:17:41.000000 dnszone-3.1.1/tests/files/example.com
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-09 01:17:41.000000 dnszone-3.1.1/tests/test_zone_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-09 01:17:41.000000 dnszone-3.1.1/tests/test_zone_reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-09 01:17:41.000000 dnszone-3.1.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dnszone-2.0.2/README.md` & `dnszone-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dnszone-2.0.2/dnszone/dnszone.py` & `dnszone-3.1.1/dnszone/dnszone.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,80 +1,83 @@
 # encoding: utf-8
 
-'''dnszone
+"""dnszone
 
 A module to manage the common record types of a zone file,
 including SOA records.  This module sits on top of the
 dnspython package and provides a higher level abstraction
 for common zone file manipulation use cases.
-'''
+"""
 
-__author__ = 'Greg Hellings'
-__copyright__ = '(c) Greg Hellings 2019'
-__version__ = '2.0.2'
+__author__ = "Greg Hellings"
+__copyright__ = "(c) Greg Hellings 2019"
+__version__ = "2.0.2"
 
 
 # ---- Imports ----
 
 # - Python Modules -
 from time import localtime, strftime, time
-from six import string_types, integer_types, next
+
+from six import integer_types, next, string_types
 
 # - dnspython Modules - http://www.dnspython.org/
 try:
     import dns.zone
 except ImportError:
     import sys
+
     sys.stderr.write("Requires dns module from http://www.dnspython.org/\n")
     sys.exit(1)
 
 import dns.rdtypes.ANY.CNAME
-import dns.rdtypes.ANY.NS
 import dns.rdtypes.ANY.MX
+import dns.rdtypes.ANY.NS
+import dns.rdtypes.ANY.TXT
 import dns.rdtypes.IN.A
 import dns.rdtypes.IN.AAAA
-import dns.rdtypes.ANY.TXT
-
 
 # ---- Exceptions ----
 
+
 class ZoneError(Exception):
-    '''An error from dnszone.Zone'''
+    """An error from dnszone.Zone"""
 
 
 class NameError(Exception):
-    '''An error from dnszone.Name'''
+    """An error from dnszone.Name"""
 
 
 class RecordsError(Exception):
-    '''An error from dnszone.Records'''
+    """An error from dnszone.Records"""
 
 
 # ---- Classes ----
 
+
 class SOA(object):
-    '''Represents the SOA fields of the root node of a Zone.
-    '''
+    """Represents the SOA fields of the root node of a Zone."""
+
     def __init__(self, soa):
         self._soa = soa
 
     def get_mname(self):
         return str(self._soa.mname)
 
     def set_mname(self, value):
-        name = dns.name.Name(value.split('.'))
+        name = dns.name.Name(value.split("."))
         self._soa.mname = name
 
     mname = property(get_mname, set_mname)
 
     def get_rname(self):
         return str(self._soa.rname)
 
     def set_rname(self, value):
-        name = dns.name.Name(value.split('.'))
+        name = dns.name.Name(value.split("."))
         self._soa.rname = name
 
     rname = property(get_rname, set_rname)
 
     def get_serial(self):
         return self._soa.serial
 
@@ -113,29 +116,30 @@
     def set_minttl(self, value):
         self._soa.minimum = value
 
     minttl = property(get_minttl, set_minttl)
 
 
 class Records(object):
-    '''Represents the records associated with a name node.
+    """Represents the records associated with a name node.
     Record items are common DNS types such as 'A', 'MX',
     'NS', etc.
-    '''
+    """
+
     def __init__(self, rectype, rdataset):
         self.type = rectype
         self._rdataset = rdataset
 
     def add(self, item):
-        if self.type == 'MX':
+        if self.type == "MX":
             assert isinstance(item, tuple)
             assert len(item) == 2
             assert isinstance(item[0], integer_types)
             assert isinstance(item[1], string_types)
-        elif self.type == 'TXT':
+        elif self.type == "TXT":
             assert isinstance(item, string_types)
             if item.startswith('"') and item.endswith('"'):
                 # dns module auto-adds quotation marks
                 item = item[1:-1]
         else:
             assert isinstance(item, string_types)
 
@@ -150,41 +154,43 @@
             raise RecordsError("No such item in record: %s" % item)
 
     def __iter__(self):
         self._item_iter = iter(self._rdataset.items)
         return self
 
     def next(self):
-        if self.type == 'MX':
+        if self.type == "MX":
             r = next(self._item_iter)
             return (r.preference, str(r.exchange))
         else:
             return str(next(self._item_iter))
+
     __next__ = next
 
     def get_items(self):
         return [r for r in self]
 
     items = property(get_items)
 
 
 class Name(object):
-    '''Represents a name node within a zone file.  This could
+    """Represents a name node within a zone file.  This could
     be the root node (the zone itself) or a hostname or subdomain
     node.
 
     Each node can consist of one or more records of various
     types, e.g. 'MX', 'A', 'NS', etc.
 
     If `node` is a dns.node object then the records associated
     with that node will be available as the `records` attribute.
 
     If the node contains SOA fields (i.e. the  root ('@') node)
     then the `soa` attribute points to an SOA object.
-    '''
+    """
+
     def __init__(self, name, node=None, ttl=None):
         self.name = name
         self.soa = None
         self.ttl = ttl
         self._node = node
 
         if node:
@@ -206,150 +212,142 @@
             r.update_ttl(self.ttl)
 
         rec = Records(rectype, r)
 
         return rec
 
     def clear_all_records(self, exclude=None):
-        '''Clear all the records for this name node.
-        '''
+        """Clear all the records for this name node."""
         if exclude is None:
             self._node.rdatasets = []
         else:
             exclude_type = dns.rdatatype._by_text.get(exclude, None)
             if exclude_type is None:
                 raise NameError("Invalid exclude: %s" % exclude)
 
             for r in self._node.rdatasets:
                 if r.rdtype != exclude_type:
                     self._node.rdatasets.remove(r)
 
 
 class Zone(object):
-    '''Represents a DNS zone.
-    '''
+    """Represents a DNS zone."""
+
     def __init__(self, domain):
         if not domain or not isinstance(domain, string_types):
-            raise ZoneError('Invalid domain')
-        if domain[-1] != '.':
-            domain = domain + '.'
+            raise ZoneError("Invalid domain")
+        if domain[-1] != ".":
+            domain = domain + "."
         self.domain = domain
 
         self._zone = None
 
     def load_from_file(self, filename):
-        '''Load the details of a zone from zone file `filename`.
-        '''
+        """Load the details of a zone from zone file `filename`."""
         self.filename = filename
-        self._zone = dns.zone.from_file(filename,
-                                        self.domain,
-                                        relativize=False)
+        self._zone = dns.zone.from_file(filename, self.domain, relativize=False)
 
     def get_root(self):
-        '''Return the root ("@") name of the zone as a Name object.
-        '''
+        """Return the root ("@") name of the zone as a Name object."""
         if not self._zone:
             return None
 
-        return Name('@', self._zone[self.domain])
+        return Name("@", self._zone[self.domain])
+
     root = property(get_root)
 
     def get_names(self):
-        '''Return a dictionary of names, keyed by name as string,
-        with values as corresponding Name objects.'''
+        """Return a dictionary of names, keyed by name as string,
+        with values as corresponding Name objects."""
         if not self._zone:
             return None
 
         default_ttl = soa_from_node(self._zone[self.domain]).minimum
 
         names = {}
         for name in self._zone.keys():
             name = str(name)
             nameobj = Name(name, self._zone[name], default_ttl)
             names[name] = nameobj
 
         return names
+
     names = property(get_names)
 
     def add_name(self, name):
-        '''Add a new name (hostname) to the zone.
+        """Add a new name (hostname) to the zone.
         If a node with the same name already exists it is returned instead.
-        '''
+        """
         node = self._zone.get_node(name, create=True)
         if node is None:
             raise ZoneError("Could not create node named: %s" % name)
 
     def delete_name(self, name):
-        '''Remove all nodes associated with a name (hostname) from the zone.
+        """Remove all nodes associated with a name (hostname) from the zone.
         If no such nodes exist, nothing happens.
-        '''
+        """
         self._zone.delete_node(name)
 
     def save(self, filename=None, autoserial=False):
-        '''Write the zone back to a file.
+        """Write the zone back to a file.
 
         If `filename` is not specified the zone will be written
         over the top of the file it was read from.
 
         if `autoserial`is True then the serial will be updated to the
         current date in common YYYYMMDDxx format.  The serial is
         guaranteed to be larger than the previous number.
-        '''
+        """
         if autoserial:
             soa = self.root.soa
-            new_serial = int(strftime('%Y%m%d00', localtime(time())))
+            new_serial = int(strftime("%Y%m%d00", localtime(time())))
             if new_serial <= soa.serial:
                 new_serial = soa.serial + 1
             soa.serial = new_serial
 
         if not filename:
             filename = self.filename
         self._zone.to_file(filename, relativize=False)
 
 
 # ---- Module Functions ----
 
+
 def zone_from_file(domain, filename):
-    '''Read a zone file and return the contents as a Zone object.
-    '''
+    """Read a zone file and return the contents as a Zone object."""
     zone = Zone(domain)
     zone.load_from_file(filename)
     return zone
 
 
 def _new_rdata(rectype, *args):
-    '''Create a new rdata type of `rectype`.
+    """Create a new rdata type of `rectype`.
     rectype must be one of: 'NS', 'MX', 'A', 'CNAME', 'TXT', 'AAAA'
     Extra arguments are as required by the rectype.
-    '''
-    if rectype == 'NS':
-        name = dns.name.Name(args[0].split('.'))
+    """
+    if rectype == "NS":
+        name = dns.name.Name(args[0].split("."))
         rd = dns.rdtypes.ANY.NS.NS(dns.rdataclass.IN, dns.rdatatype.NS, name)
-    elif rectype == 'MX':
+    elif rectype == "MX":
         preference = args[0][0]
-        exchange = dns.name.Name(args[0][1].split('.'))
-        rd = dns.rdtypes.ANY.MX.MX(dns.rdataclass.IN, dns.rdatatype.MX,
-                                   preference, exchange)
-    elif rectype == 'A':
+        exchange = dns.name.Name(args[0][1].split("."))
+        rd = dns.rdtypes.ANY.MX.MX(
+            dns.rdataclass.IN, dns.rdatatype.MX, preference, exchange
+        )
+    elif rectype == "A":
         # name = dns.name.Name( args[0].split('.') )
         name = args[0]
         rd = dns.rdtypes.IN.A.A(dns.rdataclass.IN, dns.rdatatype.A, name)
-    elif rectype == 'CNAME':
-        name = dns.name.Name(args[0].split('.'))
-        rd = dns.rdtypes.ANY.CNAME.CNAME(dns.rdataclass.IN,
-                                         dns.rdatatype.CNAME,
-                                         name)
-    elif rectype == 'TXT':
-        rd = dns.rdtypes.ANY.TXT.TXT(dns.rdataclass.IN,
-                                     dns.rdatatype.TXT,
-                                     args[0])
-    elif rectype == 'AAAA':
-        rd = dns.rdtypes.IN.AAAA.AAAA(dns.rdataclass.IN,
-                                      dns.rdatatype.AAAA,
-                                      args[0])
+    elif rectype == "CNAME":
+        name = dns.name.Name(args[0].split("."))
+        rd = dns.rdtypes.ANY.CNAME.CNAME(dns.rdataclass.IN, dns.rdatatype.CNAME, name)
+    elif rectype == "TXT":
+        rd = dns.rdtypes.ANY.TXT.TXT(dns.rdataclass.IN, dns.rdatatype.TXT, args[0])
+    elif rectype == "AAAA":
+        rd = dns.rdtypes.IN.AAAA.AAAA(dns.rdataclass.IN, dns.rdatatype.AAAA, args[0])
     else:
         raise ValueError("rectype not supported: %s" % rectype)
 
     return rd
 
 
 def soa_from_node(node):
```

### Comparing `dnszone-2.0.2/dnszone/zone_reload.py` & `dnszone-3.1.1/dnszone/zone_reload.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 
-'''zone_reload
+"""zone_reload
 
 A wrapper around 'rndc' for requesting zone reloads from named.
 
 Example::
 
     >>> from dnszone.zone_reload import ZoneReload
     >>> r = ZoneReload()
@@ -18,55 +18,52 @@
         raise ZoneReloadError("rndc failed with return code %d" % r)
     dnszone.zone_reload.ZoneReloadError: rndc failed with return code 1
     >>>
     >>> r = ZoneReload(rndc='/usr/sbin/rndc')
     >>> r.reload('example.com')
     zone reload up-to-date
     >>>
-'''
+"""
 
-__author__ = 'Greg Hellings'
-__copyright__ = '(c) Greg Hellings 2019'
-__id__ = '$Id$'
-__url__ = '$URL$'
-__version__ = '1.0'
+__author__ = "Greg Hellings"
+__copyright__ = "(c) Greg Hellings 2019"
+__id__ = "$Id$"
+__url__ = "$URL$"
+__version__ = "1.0"
 
 
 # ---- Imports ----
 
 # - Python Modules -
 import subprocess
 
-
 # ---- Exceptions ----
 
+
 class ZoneReloadError(Exception):
-    '''An error occurred within ZoneReload.
-    '''
+    """An error occurred within ZoneReload."""
 
 
 # ---- Classes ----
 
+
 class ZoneReload(object):
-    '''A wrapper around bind's rndc utility, used for reloading a modified
+    """A wrapper around bind's rndc utility, used for reloading a modified
     DNS zone.
 
     `rndc` : string containing path to rndc binary.  Or leave as "rndc"
     to search with default PATH.
-    '''
-    def __init__(self, rndc='rndc'):
+    """
+
+    def __init__(self, rndc="rndc"):
         self.rndc = rndc
 
     def reload(self, zone):
-        '''Ask named to perform a zone reload by calling the
+        """Ask named to perform a zone reload by calling the
         rndc commmand.
-        '''
-        cmd = [
-            self.rndc,
-            'reload',
-            zone
-        ]
+        """
+        cmd = [self.rndc, "reload", zone]
 
         r = subprocess.call(cmd)
 
         if r != 0:
             raise ZoneReloadError("rndc failed with return code %d" % r)
```

### Comparing `dnszone-2.0.2/dnszone/zone_check.py` & `dnszone-3.1.1/dnszone/zone_check.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 
-'''zone_check
+"""zone_check
 
 A wrapper around 'named-checkzone' for checking the validity and syntax of
 zone files.
 
 Example::
 
     >>> from dnszone.zone_check import ZoneCheck
@@ -16,58 +16,54 @@
     >>> c.error
     'Bad syntax'
     >>>
     >>> c = ZoneCheck(checkzone='/usr/sbin/named-checkzone')
     >>> c.isValid('example.com', '/var/named/zones/example.com')
     True
     >>>
-'''
+"""
 
-__author__ = 'Greg Hellings'
-__copyright__ = '(c) Greg Hellings 2019'
-__id__ = '$Id$'
-__url__ = '$URL$'
-__version__ = '1.0'
+__author__ = "Greg Hellings"
+__copyright__ = "(c) Greg Hellings 2019"
+__id__ = "$Id$"
+__url__ = "$URL$"
+__version__ = "1.0"
 
 
 # ---- Imports ----
 
 # - Python Modules -
 import subprocess
 
-
 # ---- Exceptions ----
 
 
 # ---- Classes ----
 
+
 class ZoneCheck(object):
-    '''A wrapper around bind's named-checkzone utility, used for checking the
+    """A wrapper around bind's named-checkzone utility, used for checking the
     syntax of a zone file.
 
     `checkzone` : string containing path to named-checkzone binary.  Or leave
     as "named-checkzone" to search with default PATH.
-    '''
-    def __init__(self, checkzone='checkzone'):
+    """
+
+    def __init__(self, checkzone="checkzone"):
         self.checkzone = checkzone
         self.error = None
 
     def isValid(self, zonename, filename):
-        '''Ask named to check the syntax of a zone file by calling the
+        """Ask named to check the syntax of a zone file by calling the
         named-checkzone commmand.
-        '''
-        cmd = [
-            self.checkzone,
-            '-q',
-            zonename,
-            filename
-        ]
+        """
+        cmd = [self.checkzone, "-q", zonename, filename]
 
         r = subprocess.call(cmd)
 
         if r != 0:
-            self.error = 'Bad syntax'
+            self.error = "Bad syntax"
             return False
 
         else:
             self.error = None
             return True
```

### Comparing `dnszone-2.0.2/dnszone/__init__.py` & `dnszone-3.1.1/dnszone/__init__.py`

 * *Files identical despite different names*

