# Comparing `tmp/vbcore-2.0.0rc3.tar.gz` & `tmp/vbcore-2.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbcore-2.0.0rc3.tar", last modified: Mon May 22 22:57:00 2023, max compression
+gzip compressed data, was "vbcore-2.0.0rc4.tar", last modified: Sun Jun  4 21:26:28 2023, max compression
```

## Comparing `vbcore-2.0.0rc3.tar` & `vbcore-2.0.0rc4.tar`

### file list

```diff
@@ -1,142 +1,164 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.908615 vbcore-2.0.0rc3/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      402 2023-05-22 22:57:00.907615 vbcore-2.0.0rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.890615 vbcore-2.0.0rc3/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-all.in
--rw-rw-rw-   0 root         (0) root         (0)     5986 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-all.txt
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-build.in
--rw-rw-rw-   0 root         (0) root         (0)     2068 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-build.txt
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-crypto.in
--rw-rw-rw-   0 root         (0) root         (0)      610 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-crypto.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-db.in
--rw-rw-rw-   0 root         (0) root         (0)      582 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-db.txt
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-dev.in
--rw-rw-rw-   0 root         (0) root         (0)     6394 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-extra.in
--rw-rw-rw-   0 root         (0) root         (0)     1243 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-extra.txt
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-http.in
--rw-rw-rw-   0 root         (0) root         (0)     1173 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-http.txt
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-net.in
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-net.txt
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-scheduler.in
--rw-rw-rw-   0 root         (0) root         (0)      711 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-scheduler.txt
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-test.in
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/requirements/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 22:57:00.908615 vbcore-2.0.0rc3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4745 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.894615 vbcore-2.0.0rc3/vbcore/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1632 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/aio.py
--rw-rw-rw-   0 root         (0) root         (0)     4706 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7460 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     1396 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/configurator.py
--rw-rw-rw-   0 root         (0) root         (0)     7979 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/crc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.896615 vbcore-2.0.0rc3/vbcore/crypto/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/crypto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1266 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/crypto/argon.py
--rw-rw-rw-   0 root         (0) root         (0)      942 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/crypto/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1093 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/crypto/bcrypt.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/crypto/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/crypto/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/crypto/hashes.py
--rw-rw-rw-   0 root         (0) root         (0)     3233 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/csvfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.897615 vbcore-2.0.0rc3/vbcore/datastruct/
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/datastruct/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1108 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/datastruct/buffer.py
--rw-rw-rw-   0 root         (0) root         (0)     6012 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/datastruct/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     2776 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/datastruct/dictionaries.py
--rw-rw-rw-   0 root         (0) root         (0)     2772 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/datastruct/lazy.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/datastruct/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/datastruct/orderer_set.py
--rw-rw-rw-   0 root         (0) root         (0)     4400 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/date_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.899615 vbcore-2.0.0rc3/vbcore/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15794 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/db/events.py
--rw-rw-rw-   0 root         (0) root         (0)     4935 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/db/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/db/listener.py
--rw-rw-rw-   0 root         (0) root         (0)     2840 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/db/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     6775 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/db/mysql_dumper.py
--rw-rw-rw-   0 root         (0) root         (0)     1826 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/db/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4076 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/db/sqla.py
--rw-rw-rw-   0 root         (0) root         (0)     5471 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/db/support.py
--rw-rw-rw-   0 root         (0) root         (0)     2318 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/db/views.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2190 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/enums.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3883 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.901615 vbcore-2.0.0rc3/vbcore/http/
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2938 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/http/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     8176 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/http/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3880 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/http/gql.py
--rw-rw-rw-   0 root         (0) root         (0)     3233 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/http/headers.py
--rw-rw-rw-   0 root         (0) root         (0)     2632 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/http/httpcode.py
--rw-rw-rw-   0 root         (0) root         (0)     4012 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/http/httpdumper.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/http/methods.py
--rw-rw-rw-   0 root         (0) root         (0)     6063 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/http/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/http/rpc.py
--rw-rw-rw-   0 root         (0) root         (0)     2128 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/http/useragent.py
--rw-rw-rw-   0 root         (0) root         (0)     4631 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/importer.py
--rw-rw-rw-   0 root         (0) root         (0)     4808 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.902615 vbcore-2.0.0rc3/vbcore/jsonschema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/jsonschema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.902615 vbcore-2.0.0rc3/vbcore/jsonschema/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/jsonschema/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2118 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/jsonschema/schemas/jsonrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7052 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/jsonschema/support.py
--rw-rw-rw-   0 root         (0) root         (0)     2620 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/lambdas.py
--rw-rw-rw-   0 root         (0) root         (0)     2524 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/loggers.py
--rw-rw-rw-   0 root         (0) root         (0)     4304 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.903615 vbcore-2.0.0rc3/vbcore/net/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/net/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/net/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     5873 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/net/sendmail.py
--rw-rw-rw-   0 root         (0) root         (0)     3541 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/net/sftp.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/net/socks_smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.903615 vbcore-2.0.0rc3/vbcore/rule_engine/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/rule_engine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/rule_engine/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/rule_engine/engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.904615 vbcore-2.0.0rc3/vbcore/standalone/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/standalone/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3335 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/standalone/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     9057 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/standalone/wsgi_gunicorn.py
--rw-rw-rw-   0 root         (0) root         (0)     4449 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.905615 vbcore-2.0.0rc3/vbcore/tester/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tester/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16074 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tester/asserter.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tester/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tester/fetchmail.py
--rw-rw-rw-   0 root         (0) root         (0)     1963 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tester/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     7405 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tester/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.905615 vbcore-2.0.0rc3/vbcore/tester/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tester/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tester/plugins/fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tester/plugins/startup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.907615 vbcore-2.0.0rc3/vbcore/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5840 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tools/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      948 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tools/crypto.py
--rw-rw-rw-   0 root         (0) root         (0)     2227 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tools/database.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tools/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.907615 vbcore-2.0.0rc3/vbcore/tools/initializer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tools/initializer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tools/initializer/init.py
--rw-rw-rw-   0 root         (0) root         (0)      765 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/tools/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/types.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/version.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-05-22 22:56:49.000000 vbcore-2.0.0rc3/vbcore/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 22:57:00.895615 vbcore-2.0.0rc3/vbcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      402 2023-05-22 22:57:00.000000 vbcore-2.0.0rc3/vbcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3144 2023-05-22 22:57:00.000000 vbcore-2.0.0rc3/vbcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 22:57:00.000000 vbcore-2.0.0rc3/vbcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-22 22:57:00.000000 vbcore-2.0.0rc3/vbcore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 22:57:00.000000 vbcore-2.0.0rc3/vbcore.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      542 2023-05-22 22:57:00.000000 vbcore-2.0.0rc3/vbcore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-22 22:57:00.000000 vbcore-2.0.0rc3/vbcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.746931 vbcore-2.0.0rc4/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      402 2023-06-04 21:26:28.746931 vbcore-2.0.0rc4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.731931 vbcore-2.0.0rc4/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-all.in
+-rw-rw-rw-   0 root         (0) root         (0)     5238 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-all.txt
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-build.in
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-crypto.in
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-crypto.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-db.in
+-rw-rw-rw-   0 root         (0) root         (0)      606 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-db.txt
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-dev.in
+-rw-rw-rw-   0 root         (0) root         (0)     5559 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-extra.in
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-extra.txt
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-http.in
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-http.txt
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-net.in
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-net.txt
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-scheduler.in
+-rw-rw-rw-   0 root         (0) root         (0)      694 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-scheduler.txt
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-test.in
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/requirements/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-04 21:26:28.746931 vbcore-2.0.0rc4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4745 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.734931 vbcore-2.0.0rc4/vbcore/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     4713 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7460 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/configurator.py
+-rw-rw-rw-   0 root         (0) root         (0)     7979 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.736931 vbcore-2.0.0rc4/vbcore/crypto/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crypto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crypto/argon.py
+-rw-rw-rw-   0 root         (0) root         (0)      942 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crypto/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crypto/bcrypt.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crypto/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crypto/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/crypto/hashes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3369 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/csvfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.736931 vbcore-2.0.0rc4/vbcore/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.736931 vbcore-2.0.0rc4/vbcore/data/transformations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.737931 vbcore-2.0.0rc4/vbcore/data/transformations/builders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2026 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     5586 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/dicttoxml.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5880 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/data/transformations/builders/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.738931 vbcore-2.0.0rc4/vbcore/datastruct/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/datastruct/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/datastruct/buffer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6012 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/datastruct/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2767 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/datastruct/dictionaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2772 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/datastruct/lazy.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/datastruct/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/datastruct/orderer_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     4400 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/date_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.740931 vbcore-2.0.0rc4/vbcore/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15794 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     4935 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     2861 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     6775 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/mysql_dumper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1826 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4076 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/sqla.py
+-rw-rw-rw-   0 root         (0) root         (0)     5471 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/support.py
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/db/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.740931 vbcore-2.0.0rc4/vbcore/dictutils/
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/dictutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15745 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/dictutils/flatter_dict.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/dictutils/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2190 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.741931 vbcore-2.0.0rc4/vbcore/http/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     8176 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3880 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/gql.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/headers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2632 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/httpcode.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/httpdumper.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     6063 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/rpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2128 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/http/useragent.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6034 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.742931 vbcore-2.0.0rc4/vbcore/jsonschema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/jsonschema/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.742931 vbcore-2.0.0rc4/vbcore/jsonschema/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/jsonschema/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2118 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/jsonschema/schemas/jsonrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7052 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/jsonschema/support.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/lambdas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2524 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/loggers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.743931 vbcore-2.0.0rc4/vbcore/net/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/net/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/net/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5873 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/net/sendmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3541 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/net/sftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/net/socks_smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.743931 vbcore-2.0.0rc4/vbcore/rule_engine/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/rule_engine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/rule_engine/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/rule_engine/engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.743931 vbcore-2.0.0rc4/vbcore/standalone/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/standalone/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3335 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/standalone/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     9057 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/standalone/wsgi_gunicorn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.744931 vbcore-2.0.0rc4/vbcore/stringutils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/stringutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1226 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/stringutils/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2158 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/stringutils/notations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4449 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.745931 vbcore-2.0.0rc4/vbcore/tester/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16074 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/asserter.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/fetchmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7405 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.745931 vbcore-2.0.0rc4/vbcore/tester/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/plugins/fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tester/plugins/startup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.746931 vbcore-2.0.0rc4/vbcore/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5840 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/crypto.py
+-rw-rw-rw-   0 root         (0) root         (0)     2227 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/database.py
+-rw-rw-rw-   0 root         (0) root         (0)      699 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.746931 vbcore-2.0.0rc4/vbcore/tools/initializer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/initializer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/initializer/init.py
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/tools/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2023-06-04 21:26:17.000000 vbcore-2.0.0rc4/vbcore/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 21:26:28.735931 vbcore-2.0.0rc4/vbcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      402 2023-06-04 21:26:28.000000 vbcore-2.0.0rc4/vbcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3800 2023-06-04 21:26:28.000000 vbcore-2.0.0rc4/vbcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 21:26:28.000000 vbcore-2.0.0rc4/vbcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-04 21:26:28.000000 vbcore-2.0.0rc4/vbcore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 21:26:28.000000 vbcore-2.0.0rc4/vbcore.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      584 2023-06-04 21:26:28.000000 vbcore-2.0.0rc4/vbcore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-04 21:26:28.000000 vbcore-2.0.0rc4/vbcore.egg-info/top_level.txt
```

### Comparing `vbcore-2.0.0rc3/requirements/requirements-all.txt` & `vbcore-2.0.0rc4/requirements/requirements-all.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-all.txt requirements/requirements-all.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-all.txt --resolver=backtracking requirements/requirements-all.in
 #
 aiohttp==3.8.4
     # via -r requirements/requirements-http.txt
 aiosignal==1.3.1
     # via
     #   -r requirements/requirements-http.txt
     #   aiohttp
@@ -35,44 +35,38 @@
 bcrypt==4.0.1
     # via
     #   -r requirements/requirements-crypto.txt
     #   -r requirements/requirements-net.txt
     #   paramiko
 certifi==2023.5.7
     # via
-    #   -c requirements/requirements-build.txt
     #   -r requirements/requirements-http.txt
     #   requests
 cffi==1.15.1
     # via
-    #   -c requirements/requirements-build.txt
     #   -r requirements/requirements-crypto.txt
     #   -r requirements/requirements-net.txt
     #   argon2-cffi-bindings
     #   cryptography
     #   pynacl
 chardet==5.1.0
-    # via
-    #   -c requirements/requirements-build.txt
-    #   -r requirements/requirements-extra.txt
+    # via -r requirements/requirements-extra.txt
 charset-normalizer==2.1.1
     # via
-    #   -c requirements/requirements-build.txt
     #   -r requirements/requirements-http.txt
     #   aiohttp
     #   requests
 click==8.1.3
-    # via
-    #   -c requirements/requirements.txt
-    #   -r requirements/requirements.txt
+    # via -r requirements/requirements.txt
 cryptography==40.0.2
     # via
-    #   -c requirements/requirements-build.txt
     #   -r requirements/requirements-net.txt
     #   paramiko
+defusedxml==0.7.1
+    # via -r requirements/requirements-extra.txt
 dnspython==2.3.0
     # via
     #   -r requirements/requirements-net.txt
     #   email-validator
 email-validator==2.0.0.post2
     # via -r requirements/requirements-net.txt
 frozenlist==1.3.3
@@ -90,17 +84,15 @@
     # via
     #   -r requirements/requirements-db.txt
     #   sqlalchemy
 gunicorn==20.1.0
     # via -r requirements/requirements-extra.txt
 idna==3.4
     # via
-    #   -c requirements/requirements-build.txt
     #   -r requirements/requirements-extra.txt
-    #   -r requirements/requirements-http.txt
     #   -r requirements/requirements-net.txt
     #   email-validator
     #   requests
     #   yarl
 jsonschema==4.17.3
     # via -r requirements/requirements-extra.txt
 multidict==6.0.4
@@ -112,20 +104,17 @@
 paramiko==3.1.0
     # via -r requirements/requirements-net.txt
 ply==3.11
     # via
     #   -r requirements/requirements-extra.txt
     #   rule-engine
 psutil==5.9.5
-    # via
-    #   -c requirements/requirements.txt
-    #   -r requirements/requirements.txt
+    # via -r requirements/requirements.txt
 pycparser==2.21
     # via
-    #   -c requirements/requirements-build.txt
     #   -r requirements/requirements-crypto.txt
     #   -r requirements/requirements-net.txt
     #   cffi
 pydot==1.4.2
     # via
     #   -r requirements/requirements-db.txt
     #   sqlalchemy-schemadisplay
@@ -141,49 +130,37 @@
     # via
     #   -r requirements/requirements-extra.txt
     #   jsonschema
 pysocks==1.7.1
     # via -r requirements/requirements-net.txt
 python-dateutil==2.8.2
     # via
-    #   -c requirements/requirements.txt
     #   -r requirements/requirements-extra.txt
     #   -r requirements/requirements.txt
     #   rule-engine
 python-decouple==3.8
-    # via
-    #   -c requirements/requirements.txt
-    #   -r requirements/requirements.txt
+    # via -r requirements/requirements.txt
 python-dotenv==1.0.0
-    # via
-    #   -c requirements/requirements.txt
-    #   -r requirements/requirements.txt
+    # via -r requirements/requirements.txt
 pytz==2023.3
     # via
     #   -r requirements/requirements-scheduler.txt
     #   apscheduler
 pytz-deprecation-shim==0.1.0.post0
     # via
     #   -r requirements/requirements-scheduler.txt
     #   tzlocal
 pyyaml==6.0
-    # via
-    #   -c requirements/requirements.txt
-    #   -r requirements/requirements.txt
+    # via -r requirements/requirements.txt
 requests==2.30.0
-    # via
-    #   -c requirements/requirements-build.txt
-    #   -r requirements/requirements-http.txt
+    # via -r requirements/requirements-http.txt
 rule-engine==3.5.1
     # via -r requirements/requirements-extra.txt
 six==1.16.0
     # via
-    #   -c requirements/requirements-build.txt
-    #   -c requirements/requirements.txt
-    #   -r requirements/requirements-extra.txt
     #   -r requirements/requirements-scheduler.txt
     #   -r requirements/requirements.txt
     #   apscheduler
     #   python-dateutil
 sqlalchemy==1.4.48
     # via -r requirements/requirements-db.txt
 sqlalchemy-schemadisplay==1.3
@@ -198,19 +175,20 @@
     #   apscheduler
 ua-parser==0.16.1
     # via
     #   -r requirements/requirements-http.txt
     #   user-agents
 urllib3==2.0.2
     # via
-    #   -c requirements/requirements-build.txt
     #   -r requirements/requirements-http.txt
     #   requests
 user-agents==2.2.0
     # via -r requirements/requirements-http.txt
+xmltodict==0.13.0
+    # via -r requirements/requirements-extra.txt
 yarl==1.9.2
     # via
     #   -r requirements/requirements-extra.txt
     #   -r requirements/requirements-http.txt
     #   aiohttp
     #   gql
```

### Comparing `vbcore-2.0.0rc3/requirements/requirements-build.txt` & `vbcore-2.0.0rc4/requirements/requirements-build.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-build.txt requirements/requirements-build.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-build.txt --resolver=backtracking requirements/requirements-build.in
 #
 bleach==6.0.0
     # via readme-renderer
 cachetools==5.3.0
     # via tox
 certifi==2023.5.7
     # via requests
```

### Comparing `vbcore-2.0.0rc3/requirements/requirements-crypto.txt` & `vbcore-2.0.0rc4/requirements/requirements-crypto.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-crypto.txt requirements/requirements-crypto.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-crypto.txt --resolver=backtracking requirements/requirements-crypto.in
 #
 argon2-cffi==21.3.0
     # via -r requirements/requirements-crypto.in
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 bcrypt==4.0.1
     # via -r requirements/requirements-crypto.in
```

### Comparing `vbcore-2.0.0rc3/requirements/requirements-db.txt` & `vbcore-2.0.0rc4/requirements/requirements-db.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-db.txt requirements/requirements-db.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-db.txt --resolver=backtracking requirements/requirements-db.in
 #
 greenlet==2.0.2
     # via sqlalchemy
 pydot==1.4.2
     # via sqlalchemy-schemadisplay
 pyparsing==3.0.9
     # via pydot
```

### Comparing `vbcore-2.0.0rc3/requirements/requirements-extra.txt` & `vbcore-2.0.0rc4/requirements/requirements-extra.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-extra.txt requirements/requirements-extra.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-extra.txt --resolver=backtracking requirements/requirements-extra.in
 #
 attrs==23.1.0
     # via jsonschema
 backoff==2.2.1
     # via gql
 chardet==5.1.0
-    # via
-    #   -c requirements/requirements-build.txt
-    #   -r requirements/requirements-extra.in
+    # via -r requirements/requirements-extra.in
+defusedxml==0.7.1
+    # via -r requirements/requirements-extra.in
 gql==3.4.1
     # via -r requirements/requirements-extra.in
 graphql-core==3.2.3
     # via gql
 gunicorn==20.1.0
     # via -r requirements/requirements-extra.in
 idna==3.4
@@ -35,14 +35,15 @@
     #   -c requirements/requirements.txt
     #   rule-engine
 rule-engine==3.5.1
     # via -r requirements/requirements-extra.in
 six==1.16.0
     # via
     #   -c requirements/requirements-build.txt
-    #   -c requirements/requirements.txt
     #   python-dateutil
+xmltodict==0.13.0
+    # via -r requirements/requirements-extra.in
 yarl==1.9.2
     # via gql
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `vbcore-2.0.0rc3/requirements/requirements-http.txt` & `vbcore-2.0.0rc4/requirements/requirements-http.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-http.txt requirements/requirements-http.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-http.txt --resolver=backtracking requirements/requirements-http.in
 #
 aiohttp==3.8.4
     # via -r requirements/requirements-http.in
 aiosignal==1.3.1
     # via aiohttp
 async-timeout==4.0.2
     # via aiohttp
@@ -31,17 +31,15 @@
     #   requests
     #   yarl
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
 requests==2.30.0
-    # via
-    #   -c requirements/requirements-build.txt
-    #   -r requirements/requirements-http.in
+    # via -r requirements/requirements-http.in
 ua-parser==0.16.1
     # via user-agents
 urllib3==2.0.2
     # via
     #   -c requirements/requirements-build.txt
     #   requests
 user-agents==2.2.0
```

### Comparing `vbcore-2.0.0rc3/requirements/requirements-net.txt` & `vbcore-2.0.0rc4/requirements/requirements-net.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-net.txt requirements/requirements-net.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-net.txt --resolver=backtracking requirements/requirements-net.in
 #
 bcrypt==4.0.1
     # via paramiko
 cffi==1.15.1
     # via
     #   -c requirements/requirements-build.txt
     #   cryptography
```

### Comparing `vbcore-2.0.0rc3/requirements/requirements-scheduler.txt` & `vbcore-2.0.0rc4/requirements/requirements-scheduler.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-scheduler.txt requirements/requirements-scheduler.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-scheduler.txt --resolver=backtracking requirements/requirements-scheduler.in
 #
 apscheduler==3.10.1
     # via -r requirements/requirements-scheduler.in
 pytz==2023.3
     # via apscheduler
 pytz-deprecation-shim==0.1.0.post0
     # via tzlocal
 six==1.16.0
     # via
     #   -c requirements/requirements-build.txt
-    #   -c requirements/requirements.txt
     #   apscheduler
 tzdata==2023.3
     # via pytz-deprecation-shim
 tzlocal==4.3
     # via apscheduler
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `vbcore-2.0.0rc3/requirements/requirements-test.txt` & `vbcore-2.0.0rc4/requirements/requirements-test.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-test.txt requirements/requirements-test.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-test.txt --resolver=backtracking requirements/requirements-test.in
 #
 attrs==23.1.0
     # via
     #   -c requirements/requirements-all.txt
     #   hypothesis
 certifi==2023.5.7
     # via
-    #   -c requirements/requirements-all.txt
     #   -c requirements/requirements-build.txt
     #   requests
 charset-normalizer==2.1.1
     # via
-    #   -c requirements/requirements-all.txt
     #   -c requirements/requirements-build.txt
     #   requests
 coverage[toml]==7.2.5
     # via
     #   -r requirements/requirements-test.in
     #   pytest-cov
 exceptiongroup==1.1.1
     # via
     #   hypothesis
     #   pytest
 hypothesis==6.75.2
     # via -r requirements/requirements-test.in
 idna==3.4
     # via
-    #   -c requirements/requirements-all.txt
     #   -c requirements/requirements-build.txt
     #   requests
 iniconfig==2.0.0
     # via pytest
 packaging==23.1
     # via
     #   -c requirements/requirements-build.txt
@@ -51,15 +48,14 @@
     # via -r requirements/requirements-test.in
 pyyaml==6.0
     # via
     #   -c requirements/requirements-all.txt
     #   responses
 requests==2.30.0
     # via
-    #   -c requirements/requirements-all.txt
     #   -c requirements/requirements-build.txt
     #   responses
 responses==0.23.1
     # via -r requirements/requirements-test.in
 sortedcontainers==2.4.0
     # via hypothesis
 tomli==2.0.1
@@ -67,11 +63,10 @@
     #   -c requirements/requirements-build.txt
     #   coverage
     #   pytest
 types-pyyaml==6.0.12.9
     # via responses
 urllib3==2.0.2
     # via
-    #   -c requirements/requirements-all.txt
     #   -c requirements/requirements-build.txt
     #   requests
     #   responses
```

### Comparing `vbcore-2.0.0rc3/requirements/requirements.txt` & `vbcore-2.0.0rc4/requirements/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements.txt requirements/requirements.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements.txt --resolver=backtracking requirements/requirements.in
 #
 click==8.1.3
     # via -r requirements/requirements.in
 psutil==5.9.5
     # via -r requirements/requirements.in
 python-dateutil==2.8.2
     # via -r requirements/requirements.in
```

### Comparing `vbcore-2.0.0rc3/setup.py` & `vbcore-2.0.0rc4/setup.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/aio.py` & `vbcore-2.0.0rc4/vbcore/aio.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,11 +47,13 @@
     It should be used as a main entry point for asyncio programs
     and should ideally only be called once
     """
     if sys.version_info < (3, 11):
         return asyncio.run(main, debug=debug or None)
 
     _loop_factory = loop_factory or get_event_loop
+    # only for py3.10
+    # pylint: disable=no-member
     with asyncio.Runner(loop_factory=_loop_factory, debug=debug) as service:
         if signals_handler is not None:
             signals_handler(service.get_loop())
         return service.run(main)
```

### Comparing `vbcore-2.0.0rc3/vbcore/base.py` & `vbcore-2.0.0rc4/vbcore/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
     >>> class MyStaticClass(metaclass=Static):
     ...     pass
     ...
     >>> MyStaticClass()
     Traceback (most recent call last):
         ...
-    TypeError: Can't instantiate class MyStaticClass
+    TypeError: Can't instantiate Static class MyStaticClass
     """
 
     def __call__(cls):
         raise TypeError(f"Can't instantiate Static class {cls.__name__}")
 
 
 class Decorator:
```

### Comparing `vbcore-2.0.0rc3/vbcore/batch.py` & `vbcore-2.0.0rc4/vbcore/batch.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/configurator.py` & `vbcore-2.0.0rc4/vbcore/configurator.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/crc.py` & `vbcore-2.0.0rc4/vbcore/crc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/crypto/argon.py` & `vbcore-2.0.0rc4/vbcore/crypto/argon.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/crypto/base.py` & `vbcore-2.0.0rc4/vbcore/crypto/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/crypto/bcrypt.py` & `vbcore-2.0.0rc4/vbcore/crypto/bcrypt.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/crypto/factory.py` & `vbcore-2.0.0rc4/vbcore/crypto/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/crypto/hashes.py` & `vbcore-2.0.0rc4/vbcore/crypto/hashes.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/csvfile.py` & `vbcore-2.0.0rc4/vbcore/csvfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,25 @@
 
 from vbcore.files import FileHandler, OptStr
 
 RecordType = t.Union[dict, t.Iterable[dict]]
 WriterCoroutineType = t.Generator[None, RecordType, None]
 
 
+class VBCoreDialect(csv.unix_dialect):
+    delimiter = "|"
+    quoting = csv.QUOTE_NONE
+
+
 class CustomUnixDialect(csv.unix_dialect):
     delimiter = ";"
     quoting = csv.QUOTE_MINIMAL
 
 
+csv.register_dialect("vbcore", VBCoreDialect)
 csv.register_dialect("custom-unix", CustomUnixDialect)
 
 
 class CSVHandler(FileHandler):
     def __init__(
         self,
         filename: OptStr = None,
```

### Comparing `vbcore-2.0.0rc3/vbcore/datastruct/buffer.py` & `vbcore-2.0.0rc4/vbcore/datastruct/buffer.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/datastruct/cache.py` & `vbcore-2.0.0rc4/vbcore/datastruct/cache.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/datastruct/dictionaries.py` & `vbcore-2.0.0rc4/vbcore/datastruct/dictionaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self[name] = self.normalize(value, raise_exc=False)
 
     def __delattr__(self, name):
         if name in self:
             del self[name]
 
     @classmethod
-    def normalize(cls, data, raise_exc=True) -> t.Any:
+    def normalize(cls, data, raise_exc=True):
         # TODO using cls instead of ObjectDict
         def normalize_iterable(_data: t.Any):
             for r in _data:
                 yield ObjectDict(**r) if isinstance(r, t.Mapping) else r
 
         try:
             if isinstance(data, t.Mapping):
```

### Comparing `vbcore-2.0.0rc3/vbcore/datastruct/lazy.py` & `vbcore-2.0.0rc4/vbcore/datastruct/lazy.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/datastruct/orderer_set.py` & `vbcore-2.0.0rc4/vbcore/datastruct/orderer_set.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/date_helper.py` & `vbcore-2.0.0rc4/vbcore/date_helper.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/db/events.py` & `vbcore-2.0.0rc4/vbcore/db/events.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/db/exceptions.py` & `vbcore-2.0.0rc4/vbcore/db/exceptions.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/db/listener.py` & `vbcore-2.0.0rc4/vbcore/db/listener.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/db/mixins.py` & `vbcore-2.0.0rc4/vbcore/db/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     def check_password(self, password):
         return self.hasher_instance.verify(self._password, password)
 
 
 class ExtraMixin(BaseMixin):
     _json_class = json
-    _extra = sa.Column(sa.Text())
+    _extra: str = sa.Column(sa.Text())  # type: ignore
 
     @property
     def extra(self) -> t.Dict[str, t.Any]:
         return self._json_class.loads(self._extra) if self._extra else {}
 
     @extra.setter
     def extra(self, value: t.Optional[StrDict]):
```

### Comparing `vbcore-2.0.0rc3/vbcore/db/mysql_dumper.py` & `vbcore-2.0.0rc4/vbcore/db/mysql_dumper.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/db/schema.py` & `vbcore-2.0.0rc4/vbcore/db/schema.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/db/sqla.py` & `vbcore-2.0.0rc4/vbcore/db/sqla.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/db/support.py` & `vbcore-2.0.0rc4/vbcore/db/support.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/db/views.py` & `vbcore-2.0.0rc4/vbcore/db/views.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/dispatcher.py` & `vbcore-2.0.0rc4/vbcore/dispatcher.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/enums.py` & `vbcore-2.0.0rc4/vbcore/enums.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/exceptions.py` & `vbcore-2.0.0rc4/vbcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/factory.py` & `vbcore-2.0.0rc4/vbcore/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/files.py` & `vbcore-2.0.0rc4/vbcore/files.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/http/batch.py` & `vbcore-2.0.0rc4/vbcore/http/batch.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/http/client.py` & `vbcore-2.0.0rc4/vbcore/http/client.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/http/gql.py` & `vbcore-2.0.0rc4/vbcore/http/gql.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/http/headers.py` & `vbcore-2.0.0rc4/vbcore/http/headers.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 class ContentTypeEnum(StrEnum):
     CSS = f"{TypeEnum.TEXT}/css"
     CSV = f"{TypeEnum.TEXT}/csv"
     HTML = f"{TypeEnum.TEXT}/html"
     PLAIN = f"{TypeEnum.TEXT}/plain"
     EXCEL = f"{TypeEnum.APPLICATION}/vnd.ms-excel"
+    BASE64 = f"{TypeEnum.APPLICATION}/base64"
+    YAML = f"{TypeEnum.APPLICATION}/yaml"
+    JS = f"{TypeEnum.APPLICATION}/javascript"
     JAR = f"{TypeEnum.APPLICATION}/java-archive"
     JSON = f"{TypeEnum.APPLICATION}/json"
     PDF = f"{TypeEnum.APPLICATION}/pdf"
     STREAM = f"{TypeEnum.APPLICATION}/octet-stream"
     XML = f"{TypeEnum.APPLICATION}/xml"
     ZIP = f"{TypeEnum.APPLICATION}/zip"
     TAR = f"{TypeEnum.APPLICATION}/x-tar"
@@ -28,16 +31,16 @@
     PNG = f"{TypeEnum.IMAGE}/png"
     SVG = f"{TypeEnum.IMAGE}/svg+xml"
     WEBP = f"{TypeEnum.IMAGE}/webp"
     WAV = f"{TypeEnum.AUDIO}/wav"
     JSON_PROBLEM = f"{TypeEnum.APPLICATION}/problem+json"
     XML_PROBLEM = f"{TypeEnum.APPLICATION}/problem+xml"
     JSON_HEALTH = f"{TypeEnum.APPLICATION}/health+json"
-    FORM_DATA = "multipart/form-data"
     FORM_URLENCODED = f"{TypeEnum.APPLICATION}/x-www-form-urlencoded"
+    FORM_DATA = "multipart/form-data"
 
 
 class HeaderEnum(IStrEnum):
     def _generate_next_value_(self, *_):
         return self.lower().replace("_", "-")
 
     ACCEPT = enum.auto()
```

### Comparing `vbcore-2.0.0rc3/vbcore/http/httpcode.py` & `vbcore-2.0.0rc4/vbcore/http/httpcode.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/http/httpdumper.py` & `vbcore-2.0.0rc4/vbcore/http/httpdumper.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/http/proxy.py` & `vbcore-2.0.0rc4/vbcore/http/proxy.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/http/rpc.py` & `vbcore-2.0.0rc4/vbcore/http/rpc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/http/useragent.py` & `vbcore-2.0.0rc4/vbcore/http/useragent.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/importer.py` & `vbcore-2.0.0rc4/vbcore/importer.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/jsonschema/schemas/jsonrpc.py` & `vbcore-2.0.0rc4/vbcore/jsonschema/schemas/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/jsonschema/support.py` & `vbcore-2.0.0rc4/vbcore/jsonschema/support.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/lambdas.py` & `vbcore-2.0.0rc4/vbcore/lambdas.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import operator as op
 import typing as t
-from decimal import Decimal
 
 from vbcore.types import CoupleAny
 
 T = t.TypeVar("T")
 
 
+def identity(item: t.Any) -> t.Any:
+    return item
+
+
 def op_in(a, b) -> bool:
     return a in b
 
 
 def op_not_in(a, b) -> bool:
     return a not in b
 
@@ -59,14 +62,18 @@
 class OpMeta(type):
     def __getattr__(cls, item):
         return getattr(op, item)
 
 
 class Op(metaclass=OpMeta):
     @classmethod
+    def identity(cls, a, *_, **__) -> bool:
+        return identity(a)
+
+    @classmethod
     def is_true(cls, a, *_, **__) -> bool:
         return op_is_true(a)
 
     @classmethod
     def is_false(cls, a, *_, **__) -> bool:
         return op_is_false(a)
 
@@ -114,15 +121,7 @@
             for _ in range(chunk_size):
                 chunk.append(next(_iterable))
             yield chunk
         except StopIteration:
             if chunk:
                 yield chunk
             break
-
-
-def format_decimal(value: Decimal, precision: int = 8) -> str:
-    if value.is_zero():
-        return "0"
-
-    str_fmt = f"{{:.{precision}f}}"
-    return str_fmt.format(value).rstrip("0").rstrip(".")
```

### Comparing `vbcore-2.0.0rc3/vbcore/loggers.py` & `vbcore-2.0.0rc4/vbcore/loggers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/misc.py` & `vbcore-2.0.0rc4/vbcore/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import functools
 import math
 import re
 import signal
-import string
 import sys
 import typing as t
-from random import SystemRandom
 from threading import Lock
 
 
 class Printer:
     function = print
     thread_lock = Lock()
 
@@ -104,18 +102,14 @@
             return func(*args, **kwargs)
 
         return inner
 
     return wrapper
 
 
-def random_string(length: int, alphabet: str = string.printable) -> str:
-    return "".join(SystemRandom().choice(alphabet) for _ in range(length))
-
-
 class Signal:
     @classmethod
     def handle_terminate(cls, signum, frame, callback: t.Callable = lambda: None):
         Printer.error(f"received signal: {signum} at frame: {frame}")
         callback()
         sys.exit(signum)
```

### Comparing `vbcore-2.0.0rc3/vbcore/net/helpers.py` & `vbcore-2.0.0rc4/vbcore/net/helpers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/net/sendmail.py` & `vbcore-2.0.0rc4/vbcore/net/sendmail.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/net/sftp.py` & `vbcore-2.0.0rc4/vbcore/net/sftp.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/net/socks_smtp.py` & `vbcore-2.0.0rc4/vbcore/net/socks_smtp.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/rule_engine/base.py` & `vbcore-2.0.0rc4/vbcore/rule_engine/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/rule_engine/engine.py` & `vbcore-2.0.0rc4/vbcore/rule_engine/engine.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/standalone/scheduler.py` & `vbcore-2.0.0rc4/vbcore/standalone/scheduler.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/standalone/wsgi_gunicorn.py` & `vbcore-2.0.0rc4/vbcore/standalone/wsgi_gunicorn.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/system.py` & `vbcore-2.0.0rc4/vbcore/system.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/tester/asserter.py` & `vbcore-2.0.0rc4/vbcore/tester/asserter.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/tester/fetchmail.py` & `vbcore-2.0.0rc4/vbcore/tester/fetchmail.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/tester/helpers.py` & `vbcore-2.0.0rc4/vbcore/tester/helpers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/tester/http.py` & `vbcore-2.0.0rc4/vbcore/tester/http.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/tools/cli.py` & `vbcore-2.0.0rc4/vbcore/tools/cli.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/tools/crypto.py` & `vbcore-2.0.0rc4/vbcore/tools/crypto.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/tools/database.py` & `vbcore-2.0.0rc4/vbcore/tools/database.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/tools/entrypoint.py` & `vbcore-2.0.0rc4/vbcore/tools/entrypoint.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/tools/initializer/init.py` & `vbcore-2.0.0rc4/vbcore/tools/initializer/init.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/tools/scheduler.py` & `vbcore-2.0.0rc4/vbcore/tools/scheduler.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/types.py` & `vbcore-2.0.0rc4/vbcore/types.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/uuid.py` & `vbcore-2.0.0rc4/vbcore/uuid.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore/yaml.py` & `vbcore-2.0.0rc4/vbcore/yaml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.0.0rc3/vbcore.egg-info/requires.txt` & `vbcore-2.0.0rc4/vbcore.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 paramiko
 apscheduler
 chardet
 jsonschema
 rule_engine
 gql
 gunicorn
+defusedxml
+xmltodict
 
 [crypto]
 argon2-cffi
 bcrypt
 
 [db]
 sqlalchemy<2
@@ -39,14 +41,16 @@
 
 [extra]
 chardet
 jsonschema
 rule_engine
 gql
 gunicorn
+defusedxml
+xmltodict
 
 [http]
 aiohttp
 requests
 user_agents
 
 [net]
```

