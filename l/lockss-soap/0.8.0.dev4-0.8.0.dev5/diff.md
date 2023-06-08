# Comparing `tmp/lockss_soap-0.8.0.dev4.tar.gz` & `tmp/lockss_soap-0.8.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockss_soap-0.8.0.dev4.tar", max compression
+gzip compressed data, was "lockss_soap-0.8.0.dev5.tar", max compression
```

## Comparing `lockss_soap-0.8.0.dev4.tar` & `lockss_soap-0.8.0.dev5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     2084 2023-05-11 16:22:26.475340 lockss_soap-0.8.0.dev4/CHANGELOG.rst
--rw-r--r--   0        0        0     1506 2023-03-07 22:41:03.875719 lockss_soap-0.8.0.dev4/LICENSE
--rw-r--r--   0        0        0     3165 2023-05-02 07:01:49.696347 lockss_soap-0.8.0.dev4/README.rst
--rw-r--r--   0        0        0     1090 2023-05-12 16:45:22.577672 lockss_soap-0.8.0.dev4/pyproject.toml
--rw-r--r--   0        0        0     4174 2023-05-12 16:45:14.201001 lockss_soap-0.8.0.dev4/src/lockss/soap/__init__.py
--rw-r--r--   0        0        0    32056 2023-05-12 16:43:42.587615 lockss_soap-0.8.0.dev4/src/lockss/soap/cli.py
--rw-r--r--   0        0        0    19921 2023-05-12 00:49:56.561767 lockss_soap-0.8.0.dev4/src/lockss/soap/daemon_status_service.py
--rw-r--r--   0        0        0    12108 2023-05-12 16:36:26.113957 lockss_soap-0.8.0.dev4/src/lockss/soap/util.py
--rw-r--r--   0        0        0     4349 1970-01-01 00:00:00.000000 lockss_soap-0.8.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0     2042 2023-06-08 23:05:52.247982 lockss_soap-0.8.0.dev5/CHANGELOG.rst
+-rw-r--r--   0        0        0     1506 2023-03-07 22:41:03.875719 lockss_soap-0.8.0.dev5/LICENSE
+-rw-r--r--   0        0        0     3584 2023-06-08 23:08:46.621804 lockss_soap-0.8.0.dev5/README.rst
+-rw-r--r--   0        0        0     1090 2023-06-08 23:06:13.274708 lockss_soap-0.8.0.dev5/pyproject.toml
+-rw-r--r--   0        0        0     4648 2023-06-08 23:06:20.674729 lockss_soap-0.8.0.dev5/src/lockss/soap/__init__.py
+-rw-r--r--   0        0        0    33247 2023-06-08 23:07:34.504936 lockss_soap-0.8.0.dev5/src/lockss/soap/cli.py
+-rw-r--r--   0        0        0     3010 2023-06-02 23:32:00.073873 lockss_soap-0.8.0.dev5/src/lockss/soap/content_configuration_service.py
+-rw-r--r--   0        0        0    21225 2023-06-08 23:04:06.914351 lockss_soap-0.8.0.dev5/src/lockss/soap/daemon_status_service.py
+-rw-r--r--   0        0        0    12108 2023-05-12 16:36:26.113957 lockss_soap-0.8.0.dev5/src/lockss/soap/util.py
+-rw-r--r--   0        0        0     4768 1970-01-01 00:00:00.000000 lockss_soap-0.8.0.dev5/PKG-INFO
```

### Comparing `lockss_soap-0.8.0.dev4/CHANGELOG.rst` & `lockss_soap-0.8.0.dev5/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 
    *  Initial release.
 
    *  Port of `lockss-daemon <https://gitub.com/lockss/lockss-daemon>`_'s
       ``scripts/ws/daemonstatusservice.py`` into the package
       ``lockss.turtles``:
 
-      =============================================================== =====
-      0.7.x                                                           0.8.x
-      =============================================================== =====
-      ``import daemonstatusservice`` (with ``PYTHONPATH``)            ``import lockss.soap.daemon_status_service``
-      ``scripts/ws/daemonstatusservice --hosts=... --host=...``       ``daemonstatusservice --nodes=... --node=...``
-      ``--get-au-article-urls``                                       n/a
-      ``--get-au-status``                                             ``get-au-status`` (``gas``)
-      ``--get-au-subst-urls``                                         n/a
-      ``--get-au-urls``                                               ``get-au-urls`` (``gau``)
-      ``--get-auids``                                                 ``get-auids`` (``ga``)
-      ``--get-auids-names``                                           ``get-auids --names`` (``ga --names``)
-      ``--get-peer-agreements``                                       n/a
-      ``--get-platform-configuration``                                ``get-platform-configuration`` (``gpc``)
-      ``--is-daemon-ready``                                           ``is-daemon-ready`` (``idr``)
-      ``--is-daemon-ready-quiet``                                     n/a
-      ``--query-aus``                                                 ``query-aus`` (``qa``)
-      ``--query-crawls``                                              ``query-crawls`` (``qc``)
-      n/a                                                             ``query-polls`` (``qp``)
-      ``--version``                                                   ``version``
-      =============================================================== =====
-
+      ===================================================== =======================
+      0.7.x (``lockss-daemon``)                             0.8.x (``lockss-soap``)
+      ===================================================== =======================
+      ``import daemonstatusservice`` (with ``PYTHONPATH``)  ``import lockss.soap.daemon_status_service``
+      ``scripts/ws/daemonstatusservice --hosts/--host=...`` ``daemonstatusservice --nodes/--node=...``
+      ``--get-au-article-urls``                             n/a
+      ``--get-au-status``                                   ``get-au-status`` (``gas``)
+      ``--get-au-subst-urls``                               n/a
+      ``--get-au-urls``                                     ``get-au-urls`` (``gau``)
+      ``--get-auids``                                       ``get-auids`` (``ga``)
+      ``--get-auids-names``                                 ``get-auids --names`` (``ga --names``)
+      ``--get-peer-agreements``                             n/a
+      ``--get-platform-configuration``                      ``get-platform-configuration`` (``gpc``)
+      ``--is-daemon-ready``                                 ``is-daemon-ready`` (``idr``)
+      ``--is-daemon-ready-quiet``                           n/a
+      ``--query-aus``                                       ``query-aus`` (``qa``)
+      ``--query-crawls``                                    ``query-crawls`` (``qc``)
+      n/a                                                   ``query-polls`` (``qp``)
+      n/a                                                   ``query-repositories`` (``qr``)
+      ``--version``                                        ``version``
+      ===================================================== =======================
```

### Comparing `lockss_soap-0.8.0.dev4/LICENSE` & `lockss_soap-0.8.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `lockss_soap-0.8.0.dev4/README.rst` & `lockss_soap-0.8.0.dev5/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -40,10 +40,14 @@
                                             [HOST:PORT ...]
 
     Usage: daemonstatusservice query-polls [-h] [--output-format FMT] [--node HOST:PORT] [--nodes FILE] [--password PASS]
                                            [--username USER] [--select CSFIELDS] [--where CLAUSE] [--pool-size SIZE]
                                            [--process-pool | --thread-pool]
                                            [HOST:PORT ...]
 
+    Usage: daemonstatusservice query-repositories [-h] [--output-format FMT] [--skip-headers] [--node HOST:PORT] [--nodes FILE]
+                                                  [--password PASS] [--username USER] [--select CSFIELDS] [--where CLAUSE]
+                                                  [--pool-size SIZE] [--process-pool | --thread-pool]
+                                                  [HOST:PORT ...]
     Usage: daemonstatusservice usage [-h]
 
     Usage: daemonstatusservice version [-h]
```

### Comparing `lockss_soap-0.8.0.dev4/pyproject.toml` & `lockss_soap-0.8.0.dev5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lockss-soap"
-version = "0.8.0-dev4"
+version = "0.8.0-dev5"
 description = "Library and command line tools to interact with legacy LOCKSS SOAP interfaces"
 license = "BSD-3-Clause"
 authors = [
     "Thib Guicherd-Callin <thib@cs.stanford.edu>"
 ]
 readme = "README.rst"
 homepage = "https://www.lockss.org/"
```

### Comparing `lockss_soap-0.8.0.dev4/src/lockss/soap/__init__.py` & `lockss_soap-0.8.0.dev5/src/lockss/soap/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = '0.8.0-dev4'
+__version__ = '0.8.0-dev5'
 
 __copyright__ = '''
 Copyright (c) 2000-2023, Board of Trustees of Leland Stanford Jr. University
 '''.strip()
 
 __license__ = __copyright__ + '\n\n' + '''
 Redistribution and use in source and binary forms, with or without
@@ -64,22 +64,39 @@
 
 import base64
 
 import lockss.soap.util
 
 
 def node(node_reference, username, password):
+    """
+    Creates a node object from a node reference (a string like ``host:8081``,
+    ``http://host:8081``, ``http://host:8081/``, ``https://host:8081``,
+    ``https://host:8081/``; no protocol defaults to ``http://``), a username,
+    and a password.
+
+    .. seealso::
+
+    :param node_reference: A node reference.
+    :param username: A username.
+    :param password: A password.
+    :return: A node object.
+    """
     return _Node(node_reference, username, password)
 
 
 class _Node(object):
+    """
+    Encapsulates a node reference.
+    """
 
     DEFAULT_PROTOCOL = 'http'
 
     def __init__(self, node_reference, username, password):
+
         super().__init__()
         if '://' not in node_reference:
             node_reference = f'{_Node.DEFAULT_PROTOCOL}://{node_reference}'
         if node_reference.endswith('/'):
             node_reference = node_reference[:-1]
         self._url = node_reference
         self._username = username
```

### Comparing `lockss_soap-0.8.0.dev4/src/lockss/soap/cli.py` & `lockss_soap-0.8.0.dev5/src/lockss/soap/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,14 +226,25 @@
     'talliedUrls': ('Tallied URLs', lambda r: '\n'.join(r.get('talliedUrls', []))),
     'tooCloseUrlCount': ('Too Close URL Count', lambda r: r.get('tooCloseUrlCount')),
     'tooCloseUrls': ('Too Close URLs', lambda r: '\n'.join(r.get('tooCloseUrls', []))),
     'voteDeadline': ('Vote Deadline', lambda r: datetime_ms(r.get('voteDeadline')))
 }
 
 
+QUERY_REPOSITORIES = {
+    'auName': ('AU Name', lambda r: r.get('auName')),
+    'directoryName': ('Directory Name', lambda r: r.get('directoryName')),
+    'diskUsage': ('Disk Usage', lambda r: r.get('diskUsage')),
+    'internal': ('Internal', lambda r: r.get('internal')),
+    'params': ('Params', lambda r: f'{{{", ".join(f"{e.key}={e.value}" for e in r.get("params", []))}}}'),
+    'pluginName': ('Plugin Name', lambda r: r.get('pluginName')),
+    'repositorySpaceId': ('Repository Space ID', lambda r: r.get('repositorySpaceId')),
+    'status': ('Status', lambda r: r.get('status')),
+}
+
 class DaemonStatusServiceCli(_BaseCli):
 
     PROG = 'daemonstatusservice'
 
     def __init__(self):
         super().__init__()
         self._auids = None
@@ -394,14 +405,15 @@
         self._make_parser_get_auids(self._subparsers)
         self._make_parser_get_platform_configuration(self._subparsers)
         self._make_parser_is_daemon_ready(self._subparsers)
         self._make_parser_license(self._subparsers)
         self._make_parser_query_aus(self._subparsers)
         self._make_parser_query_crawls(self._subparsers)
         self._make_parser_query_polls(self._subparsers)
+        self._make_parser_query_repositories(self._subparsers)
         self._make_parser_usage(self._subparsers)
         self._make_parser_version(self._subparsers)
 
     def _make_parser_get_au_status(self, container):
         parser = container.add_parser('get-au-status', aliases=['gas'],
                                       description='Output status information about target AUIDs.',
                                       help='output status information about target AUIDs',
@@ -490,14 +502,22 @@
         parser = self._make_parser_query(container,
                                          'query-polls', aliases=['qp'],
                                          description='Perform a query on polls.',
                                          help='perform a query on polls',
                                          target=lockss.soap.daemon_status_service.query_polls,
                                          query_mapping=QUERY_POLLS)
 
+    def _make_parser_query_repositories(self, container):
+        parser = self._make_parser_query(container,
+                                         'query-repositories', aliases=['qr'],
+                                         description='Perform a query on repositories.',
+                                         help='perform a query on repositories',
+                                         target=lockss.soap.daemon_status_service.query_repositories,
+                                         query_mapping=QUERY_REPOSITORIES)
+
     def _do_query(self):
         target = self._args.target
         query_mapping = self._args.query_mapping
         node_objects = [lockss.soap.node(node_ref, self._get_username(), self._get_password()) for node_ref in self._get_nodes()]
         requested_fields = self._args.select if self._args.select and len(self._args.select) > 0 else query_mapping.keys()
         select_minus_auid = list(dict.fromkeys(k.partition(':')[0] for k in requested_fields if k != 'auId'))
         select_auid_first = ['auId', *select_minus_auid]
```

### Comparing `lockss_soap-0.8.0.dev4/src/lockss/soap/daemon_status_service.py` & `lockss_soap-0.8.0.dev5/src/lockss/soap/daemon_status_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -466,52 +466,94 @@
        *  ``url`` (string)
     *  ``deadline`` (numeric)
     *  ``disagreedUrlCount`` (numeric)
     *  ``disagreedUrls`` (list of strings)
     *  ``duration`` (numeric)
     *  ``endTime`` (numeric)
     *  ``errorDetail`` (string)
-    *  ``errorUrls``, a list of records with these attributes:
-       *  ``entry``, a record with these attributes:
+    *  ``errorUrls``, a record with these attributes:
+       *  ``entry``, a list of records with these attributes:
           *  ``key`` (string)
           *  ``value`` (string)
     *  ``hashErrorCount`` (numeric)
     *  ``noQuorumUrlCount`` (numeric)
     *  ``noQuorumUrls`` (list of strings)
     *  ``participantCount`` (numeric)
+    *  ``participants``, a list of records with these attributes:
+       *  ``agreedUrls`` (list of strings)
+       *  ``agreedVoteCount`` (numeric)
+       *  ``bytesHashed`` (numeric)
+       *  ``bytesRead`` (numeric)
+       *  ``currentState`` (string)
+       *  ``disagreedUrls`` (list of strings)
+       *  ``disagreedVoteCount`` (numeric)
+       *  ``hasVoted`` (boolean)
+       *  ``isExParticipant`` (boolean)
+       *  ``lastStateChange`` (numeric)
+       *  ``peerId`` (string)
+       *  ``peerStatus`` (string)
+       *  ``percentAgreement`` (floating point)
+       *  ``pollerOnlyUrls`` (list of strings)
+       *  ``pollerOnlyVoteCount`` (numeric)
+       *  ``voterOnlyUrls`` (list of strings)
+       *  ``voterOnlyVotecount`` (numeric)
+    *  ``percentAgreement`` (floating point)
+    *  ``pollKey`` (string)
+    *  ``pollStatus`` (string)
+    *  ``pollVariant`` (string)
+    *  ``quorum`` (numeric)
+    *  ``remainingTime`` (numeric)
+    *  ``startTime`` (numeric)
+    *  ``talliedUrlCount`` (numeric)
+    *  ``talliedUrls`` (list of strings)
+    *  ``tooCloseUrlCount`` (numeric)
+    *  ``tooCloseUrls`` (list of strings)
+    *  ``voteDeadline`` (numeric)
 
-<xs:element maxOccurs="unbounded" minOccurs="0" name="participants" nillable="true" type="tns:participantWsResult"/>
-<xs:element minOccurs="0" name="percentAgreement" type="xs:float"/>
-<xs:element minOccurs="0" name="pollKey" type="xs:string"/>
-<xs:element minOccurs="0" name="pollStatus" type="xs:string"/>
-<xs:element minOccurs="0" name="pollVariant" type="xs:string"/>
-<xs:element minOccurs="0" name="quorum" type="xs:int"/>
-<xs:element minOccurs="0" name="remainingTime" type="xs:long"/>
-<xs:element minOccurs="0" name="startTime" type="xs:long"/>
-<xs:element minOccurs="0" name="talliedUrlCount" type="xs:int"/>
-<xs:element maxOccurs="unbounded" minOccurs="0" name="talliedUrls" nillable="true" type="xs:string"/>
-<xs:element minOccurs="0" name="tooCloseUrlCount" type="xs:int"/>
-<xs:element maxOccurs="unbounded" minOccurs="0" name="tooCloseUrls" nillable="true" type="xs:string"/>
-<xs:element minOccurs="0" name="voteDeadline" type="xs:long"/>
+    Performs a ``queryPolls`` SOAP operation.
+
+    :param node_object: A node object returned by `lockss.soap.node`.
+    :param select: A list of attribute names, chosen among the ones above.
+    :param where: An optional query string expressed over the attribute names
+        above.
+    :return: A list of objects for polls matching the ``where`` query, each
+        populated with only the attributes requested in the ``select`` list.
+    """
+    client = _make_client(node_object, SERVICE)
+    query = _construct_query(select, where)
+    ret = client.service.queryPolls(pollQuery=query)
+    return zeep.helpers.serialize_object(ret)
 
 
+def query_repositories(node_object, select, where=None):
+    """
+    Performs a query against the repositories of a given node, and returns a
+    record with attributes among these:
 
+    *  ``auName`` (string)
+    *  ``directoryName`` (string)
+    *  ``diskUsage`` (numeric)
+    *  ``internal`` (boolean)
+    *  ``params`` (string)
+    *  ``pluginName`` (string)
+    *  ``repositorySpaceId`` (string)
+    *  ``status`` (string)
 
-    Performs a ``queryPolls`` SOAP operation.
+    Performs a ``queryRepositories`` SOAP operation.
 
     :param node_object: A node object returned by `lockss.soap.node`.
     :param select: A list of attribute names, chosen among the ones above.
     :param where: An optional query string expressed over the attribute names
         above.
     :return: A list of objects for polls matching the ``where`` query, each
         populated with only the attributes requested in the ``select`` list.
     """
     client = _make_client(node_object, SERVICE)
     query = _construct_query(select, where)
-    ret = client.service.queryPolls(pollQuery=query)
+    ret = client.service.queryRepositories(repositoryQuery=query)
     return zeep.helpers.serialize_object(ret)
 
 
 def query_tdb_titles(*args, **kwargs):
     """
     .. warning::
```

### Comparing `lockss_soap-0.8.0.dev4/src/lockss/soap/util.py` & `lockss_soap-0.8.0.dev5/src/lockss/soap/util.py`

 * *Files identical despite different names*

### Comparing `lockss_soap-0.8.0.dev4/PKG-INFO` & `lockss_soap-0.8.0.dev5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockss-soap
-Version: 0.8.0.dev4
+Version: 0.8.0.dev5
 Summary: Library and command line tools to interact with legacy LOCKSS SOAP interfaces
 Home-page: https://www.lockss.org/
 License: BSD-3-Clause
 Author: Thib Guicherd-Callin
 Author-email: thib@cs.stanford.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -69,11 +69,15 @@
                                             [HOST:PORT ...]
 
     Usage: daemonstatusservice query-polls [-h] [--output-format FMT] [--node HOST:PORT] [--nodes FILE] [--password PASS]
                                            [--username USER] [--select CSFIELDS] [--where CLAUSE] [--pool-size SIZE]
                                            [--process-pool | --thread-pool]
                                            [HOST:PORT ...]
 
+    Usage: daemonstatusservice query-repositories [-h] [--output-format FMT] [--skip-headers] [--node HOST:PORT] [--nodes FILE]
+                                                  [--password PASS] [--username USER] [--select CSFIELDS] [--where CLAUSE]
+                                                  [--pool-size SIZE] [--process-pool | --thread-pool]
+                                                  [HOST:PORT ...]
     Usage: daemonstatusservice usage [-h]
 
     Usage: daemonstatusservice version [-h]
```

