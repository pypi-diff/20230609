# Comparing `tmp/pymisp-2.4.98.tar.gz` & `tmp/pymisp-2.4.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymisp-2.4.98.tar", last modified: Mon Dec  3 16:20:22 2018, max compression
+gzip compressed data, was "dist/pymisp-2.4.99.tar", last modified: Thu Dec  6 14:24:01 2018, max compression
```

## Comparing `pymisp-2.4.98.tar` & `pymisp-2.4.99.tar`

### file list

```diff
@@ -1,425 +1,425 @@
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)    91880 2018-12-03 16:09:58.000000 pymisp-2.4.98/CHANGELOG.txt
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1615 2018-09-06 06:43:41.000000 pymisp-2.4.98/LICENSE
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2301 2018-10-12 13:43:56.000000 pymisp-2.4.98/setup.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      283 2018-09-06 06:43:41.000000 pymisp-2.4.98/MANIFEST.in
--rw-rw-r--   0 raphael   (1000) raphael   (1000)       79 2018-12-03 16:20:22.000000 pymisp-2.4.98/setup.cfg
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/tests/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2053 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/misp_event.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)    14019 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/test_mispevent.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1415 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/search_index_result.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      888 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/new_misp_event.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)        0 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/__init__.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3038 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/57c4445b-c548-4654-af0b-4be3950d210f.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/tests/mispevent_testfiles/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      467 2018-10-12 13:43:56.000000 pymisp-2.4.98/tests/mispevent_testfiles/malware.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)   154735 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/mispevent_testfiles/existing_event.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1577 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/mispevent_testfiles/def_param.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1452 2018-12-03 16:06:16.000000 pymisp-2.4.98/tests/mispevent_testfiles/event_obj_def_param.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     4528 2018-12-03 16:06:16.000000 pymisp-2.4.98/tests/mispevent_testfiles/shadow.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      429 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/mispevent_testfiles/attribute.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1032 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/mispevent_testfiles/misp_custom_obj.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)       21 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/mispevent_testfiles/simple.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)       63 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/mispevent_testfiles/sighting.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      474 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/mispevent_testfiles/attribute_del.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      244 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/mispevent_testfiles/event_tags.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      795 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/mispevent_testfiles/proposals.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)   154729 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/mispevent_testfiles/existing_event_edited.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/tests/mispevent_testfiles/test_object_template/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      578 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/mispevent_testfiles/test_object_template/definition.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1633 2018-12-03 16:06:16.000000 pymisp-2.4.98/tests/mispevent_testfiles/event_obj_attr_tag.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     7511 2018-12-03 16:06:16.000000 pymisp-2.4.98/tests/mispevent_testfiles/malware_exist.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      722 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/mispevent_testfiles/event_obj_tag.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      173 2018-09-06 06:43:41.000000 pymisp-2.4.98/tests/mispevent_testfiles/event.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)    21524 2018-12-03 16:06:16.000000 pymisp-2.4.98/tests/test_offline.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)    16761 2018-10-12 13:43:56.000000 pymisp-2.4.98/tests/test.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2256 2018-12-03 16:06:16.000000 pymisp-2.4.98/tests/sharing_groups.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)    52710 2018-12-03 16:06:16.000000 pymisp-2.4.98/tests/testlive_comprehensive.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     9241 2018-10-12 13:43:56.000000 pymisp-2.4.98/pymisp/abstract.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)    26995 2018-12-03 16:06:16.000000 pymisp-2.4.98/pymisp/aping.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     9178 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/data/schema.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     8561 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/data/schema-lax.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/relationships/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)    23729 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/relationships/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/coin-address/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2861 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/coin-address/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Web-Bookmark/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1691 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Web-Bookmark/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/cap-info/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     5181 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/cap-info/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-system-hive-service-drivers/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2534 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-system-hive-service-drivers/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/email/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     4654 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/email/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-appInit-DLLS/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1490 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-appInit-DLLS/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Web-Downloads/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1456 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Web-Downloads/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-applications-installed/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1623 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-applications-installed/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/ja3/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1421 2018-10-12 13:44:10.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/ja3/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/gtp-attack/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2572 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/gtp-attack/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/timestamp/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1316 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/timestamp/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/malware-config/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1479 2018-10-12 13:44:10.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/malware-config/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/sandbox-report/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2692 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/sandbox-report/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/whois/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2584 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/whois/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/cortex/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1353 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/cortex/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/stix2-pattern/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      837 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/stix2-pattern/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-system-hive-firewall-configuration/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1483 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-system-hive-firewall-configuration/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/script/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1584 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/script/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/ss7-attack/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     4860 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/ss7-attack/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/x509/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3158 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/x509/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/yara/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      982 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/yara/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/credential/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1855 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/credential/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/mactime-timeline-analysis/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1549 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/mactime-timeline-analysis/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/bank-account/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     5219 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/bank-account/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/timesketch-timeline/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      927 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/timesketch-timeline/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/exploit-poc/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1386 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/exploit-poc/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/cap-resource/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1440 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/cap-resource/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/fail2ban/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1601 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/fail2ban/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/elf/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     5016 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/elf/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/cowrie/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3404 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/cowrie/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-application-paths/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1353 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-application-paths/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/ip-port/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2027 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/ip-port/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/report/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      677 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/report/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/phishing/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1898 2018-10-12 13:44:10.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/phishing/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-system-hive-network-information/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3115 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-system-hive-network-information/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/process/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2607 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/process/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/android-permission/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     5020 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/android-permission/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/python-etvx-event-log/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     4858 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/python-etvx-event-log/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-sam-hive-single-user/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2033 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-sam-hive-single-user/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/virustotal-report/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1422 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/virustotal-report/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/network-socket/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     4585 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/network-socket/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-command-shell/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1416 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-command-shell/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Web-Search-Query/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1588 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Web-Search-Query/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/victim/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3051 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/victim/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/asn/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2484 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/asn/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/http-request/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2990 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/http-request/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/cortex-taxonomy/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1561 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/cortex-taxonomy/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/person/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     4469 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/person/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/forensic-evidence/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2275 2018-10-12 13:44:10.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/forensic-evidence/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/annotation/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1748 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/annotation/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/forensic-case/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1282 2018-10-12 13:44:10.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/forensic-case/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/ail-leak/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2182 2018-10-12 13:44:10.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/ail-leak/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/paste/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1933 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/paste/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/cookie/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1519 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/cookie/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/shortened-link/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1114 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/shortened-link/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/elf-section/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     4113 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/elf-section/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/timesketch_message/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      589 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/timesketch_message/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/original-imported-file/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      885 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/original-imported-file/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/transaction/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3161 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/transaction/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/network-connection/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2515 2018-10-12 13:44:10.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/network-connection/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/vehicle/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1311 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/vehicle/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/cap-alert/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     4252 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/cap-alert/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-sam-hive-user-group/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1510 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-sam-hive-user-group/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/diameter-attack/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2388 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/diameter-attack/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/av-signature/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1087 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/av-signature/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/course-of-action/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2688 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/course-of-action/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/short-message-service/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1382 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/short-message-service/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-system-hive-general-configuration/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3027 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-system-hive-general-configuration/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/pe-section/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2891 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/pe-section/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/ais-info/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1591 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/ais-info/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/legal-entity/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1244 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/legal-entity/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/pe/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3625 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/pe/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/mutex/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      745 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/mutex/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/bgp-hijack/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1436 2018-10-12 13:44:10.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/bgp-hijack/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Web-History/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1671 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Web-History/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Web-Cookie/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1705 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Web-Cookie/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/tor-node/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2603 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/tor-node/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-userprofile-winlogon/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     5419 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-userprofile-winlogon/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/geolocation/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3025 2018-10-12 13:44:10.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/geolocation/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/ip-api-address/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2798 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/ip-api-address/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/tracking-id/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1546 2018-10-12 13:44:10.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/tracking-id/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/file/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     4730 2018-10-12 13:44:10.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/file/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-general-windows-info/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3481 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-general-windows-info/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/macho-section/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2551 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/macho-section/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/target-system/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1002 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/target-system/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-BHO/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1689 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-BHO/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-NTUser/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2975 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-NTUser/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/microblog/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1812 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/microblog/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/sb-signature/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1160 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/sb-signature/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-software-run/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1704 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-software-run/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/rtir/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1519 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/rtir/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/timecode/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1489 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/timecode/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/phone/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2742 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/phone/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/ddos/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2447 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/ddos/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/domain-ip/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1271 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/domain-ip/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/r2graphity/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     4597 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/r2graphity/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Chats/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2321 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Chats/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/passive-dns/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3178 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/passive-dns/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/yabin/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1158 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/yabin/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regexp/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1431 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/regexp/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/vulnerability/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3032 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/vulnerability/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/internal-reference/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1043 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/internal-reference/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/credit-card/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1335 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/credit-card/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/registry-key/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2511 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/registry-key/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/macho/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1330 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/macho/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/pcap-metadata/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     5889 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/pcap-metadata/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/suricata/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      953 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/suricata/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/netflow/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3826 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/netflow/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/url/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2743 2018-12-03 16:06:54.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/url/definition.json
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/threatgrid-report/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1700 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/objects/threatgrid-report/definition.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2283 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/schema_objects.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1121 2018-09-06 06:44:38.000000 pymisp-2.4.98/pymisp/data/misp-objects/schema_relationships.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)    27581 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/data/describeTypes.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)    47985 2018-12-03 16:06:16.000000 pymisp-2.4.98/pymisp/mispevent.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp/tools/
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)    14163 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/openioc.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     6265 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/peobject.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2755 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/emailobject.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2379 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/abstractgenerator.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      742 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/sbsignatureobject.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      726 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/fail2banobject.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3910 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/elfobject.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     4096 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/create_misp_object.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3726 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/machoobject.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1294 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/stix.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      829 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/load_warninglists.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1988 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/neo4j.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      906 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/ext_lookups.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      906 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/__init__.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3200 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/fileobject.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1534 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/genericgenerator.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      825 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/domainipobject.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      828 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/geolocationobject.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3157 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/vtreportobject.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      804 2018-09-06 06:43:41.000000 pymisp-2.4.98/pymisp/tools/asnobject.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)   108049 2018-12-03 16:06:16.000000 pymisp-2.4.98/pymisp/api.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1988 2018-12-03 16:08:31.000000 pymisp-2.4.98/pymisp/__init__.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1063 2018-10-12 13:43:56.000000 pymisp-2.4.98/pymisp/exceptions.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/docs/
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/docs/tutorial/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)       48 2018-09-06 06:43:41.000000 pymisp-2.4.98/docs/tutorial/install_notebook.sh
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     9974 2018-12-03 16:06:16.000000 pymisp-2.4.98/docs/tutorial/Search.ipynb
--rw-rw-r--   0 raphael   (1000) raphael   (1000)    23565 2018-12-03 16:06:16.000000 pymisp-2.4.98/docs/tutorial/PyMISP Objects.ipynb
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     9786 2018-12-03 16:06:16.000000 pymisp-2.4.98/docs/tutorial/Search-NG.ipynb
--rw-rw-r--   0 raphael   (1000) raphael   (1000)    12269 2018-12-03 16:06:16.000000 pymisp-2.4.98/docs/tutorial/PyMISP_tutorial.ipynb
--rw-rw-r--   0 raphael   (1000) raphael   (1000)    10305 2018-12-03 16:06:16.000000 pymisp-2.4.98/docs/tutorial/Usage-NG.ipynb
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     7615 2018-09-06 06:43:41.000000 pymisp-2.4.98/docs/Makefile
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/docs/source/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1038 2018-09-06 06:43:41.000000 pymisp-2.4.98/docs/source/modules.rst
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      451 2018-09-06 06:43:41.000000 pymisp-2.4.98/docs/source/index.rst
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      948 2018-09-06 06:43:41.000000 pymisp-2.4.98/docs/source/tools.rst
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     4654 2018-12-03 16:06:16.000000 pymisp-2.4.98/docs/source/README.md
--rw-rw-r--   0 raphael   (1000) raphael   (1000)    12320 2018-09-06 06:43:41.000000 pymisp-2.4.98/docs/source/conf.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     4654 2018-12-03 16:06:16.000000 pymisp-2.4.98/README.md
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/examples/
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1668 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/search.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)        7 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/get_network_activity.event_id
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      757 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/up.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      914 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/add_feed.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1381 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/get_csv.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1488 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/misp2clamav.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      804 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/delete_user.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/examples/suricata_search/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1025 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/suricata_search/README.md
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     6870 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/suricata_search/suricata_search.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     3476 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/add_fail2ban_object.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      228 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/keys.py.sample
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      877 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/add_named_attribute.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1032 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/edit_user_json.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      563 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/stats.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      292 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/cache_all.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/examples/events/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1638 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/events/dummy
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      777 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/events/create_massive_dummy_events.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2975 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/events/tools.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      687 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/events/create_dummy_event.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2777 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/events/README.md
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     7514 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/vt_to_misp.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      793 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/suricata.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1076 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/add_email_object.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      946 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/yara.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     3768 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/yara_dump.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     6744 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/get_network_activity.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      726 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/warninglists.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1022 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/tagstatistics.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1258 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/addtag.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1420 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/add_generic_object.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      817 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/edit_user.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1273 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/search_sighting.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      598 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/sharing_groups.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/examples/ioc-2-misp/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3081 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/ioc-2-misp/keys.py.sample
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      455 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/ioc-2-misp/README.md
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)    11599 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/ioc-2-misp/ioc2misp.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      579 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/ioc-2-misp/taxonomy.csv
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     3991 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/et2misp.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     2554 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/copy_list.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      885 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/del.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/examples/graphdb/
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1516 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/graphdb/make_neo4j.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)       66 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/sighting.json
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1261 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/add_sbsignature.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1223 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/last.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     2361 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/misp2cef.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     2145 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/generate_file_objects.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/__init__.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1531 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/add_file_object.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1141 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/get.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      702 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/sighting.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      713 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/lookup.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1164 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/create_events.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      674 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/get_attachment.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1347 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/search_attributes_yara.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      625 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/freetext.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1614 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/addtag2.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      534 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/tags.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      666 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/fetch_events_feed.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)       38 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/freetext.txt
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      480 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/test_sign.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      885 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/add_user_json.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1244 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/searchall.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/examples/situational-awareness/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1107 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/situational-awareness/bokeh_tools.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2206 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/situational-awareness/pygal_tools.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3761 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/situational-awareness/tags_to_graphs.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1508 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/situational-awareness/attribute_treemap.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)    13236 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/situational-awareness/tools.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2342 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/situational-awareness/tag_scatter.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3082 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/situational-awareness/tag_search.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      608 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/situational-awareness/style.css
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2485 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/situational-awareness/tags_count.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2683 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/situational-awareness/README.md
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      541 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/situational-awareness/style2.css
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      520 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/situational-awareness/test_attribute_treemap.html
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1867 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/situational-awareness/date_tools.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      585 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/users_list.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/examples/feed-generator/
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1375 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/feed-generator/settings.default.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/examples/feed-generator/output/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)        0 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/feed-generator/output/empty
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     5710 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/feed-generator/generate.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      850 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/feed-generator/README.md
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      930 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/openioc_to_misp.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     4224 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/asciidoc_generator.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/examples/feed-generator-from-redis/
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1585 2018-10-12 13:43:56.000000 pymisp-2.4.98/examples/feed-generator-from-redis/settings.default.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      279 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/feed-generator-from-redis/server.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     9830 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/feed-generator-from-redis/generator.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     5224 2018-10-12 13:43:56.000000 pymisp-2.4.98/examples/feed-generator-from-redis/fromredis.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      113 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/feed-generator-from-redis/install.sh
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/examples/feed-generator-from-redis/ObjectConstructor/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1259 2018-10-12 13:43:56.000000 pymisp-2.4.98/examples/feed-generator-from-redis/ObjectConstructor/CowrieMISPObject.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     2260 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/feed-generator-from-redis/README.md
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     3247 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/feed-generator-from-redis/MISPItemToRedis.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/examples/profiles/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      414 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/profiles/weekly_report.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      459 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/profiles/daily_report.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)        0 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/profiles/__init__.py
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)     2270 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/upload.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)       87 2018-09-06 06:43:41.000000 pymisp-2.4.98/examples/user_sample.json
--rwxrwxr-x   0 raphael   (1000) raphael   (1000)      890 2018-12-03 16:06:16.000000 pymisp-2.4.98/examples/add_user.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-03 16:20:22.000000 pymisp-2.4.98/pymisp.egg-info/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      245 2018-12-03 16:20:21.000000 pymisp-2.4.98/pymisp.egg-info/requires.txt
--rw-rw-r--   0 raphael   (1000) raphael   (1000)        1 2018-12-03 16:20:21.000000 pymisp-2.4.98/pymisp.egg-info/dependency_links.txt
--rw-rw-r--   0 raphael   (1000) raphael   (1000)    12567 2018-12-03 16:20:21.000000 pymisp-2.4.98/pymisp.egg-info/SOURCES.txt
--rw-rw-r--   0 raphael   (1000) raphael   (1000)        7 2018-12-03 16:20:21.000000 pymisp-2.4.98/pymisp.egg-info/top_level.txt
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     6924 2018-12-03 16:20:21.000000 pymisp-2.4.98/pymisp.egg-info/PKG-INFO
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     6924 2018-12-03 16:20:22.000000 pymisp-2.4.98/PKG-INFO
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)    92591 2018-12-06 14:22:09.000000 pymisp-2.4.99/CHANGELOG.txt
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1615 2018-09-06 06:43:41.000000 pymisp-2.4.99/LICENSE
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2301 2018-10-12 13:43:56.000000 pymisp-2.4.99/setup.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      283 2018-09-06 06:43:41.000000 pymisp-2.4.99/MANIFEST.in
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)       79 2018-12-06 14:24:01.000000 pymisp-2.4.99/setup.cfg
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/tests/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2053 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/misp_event.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)    14019 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/test_mispevent.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1415 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/search_index_result.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      888 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/new_misp_event.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)        0 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/__init__.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3038 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/57c4445b-c548-4654-af0b-4be3950d210f.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/tests/mispevent_testfiles/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      467 2018-10-12 13:43:56.000000 pymisp-2.4.99/tests/mispevent_testfiles/malware.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)   154735 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/mispevent_testfiles/existing_event.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1577 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/mispevent_testfiles/def_param.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1452 2018-12-03 16:06:16.000000 pymisp-2.4.99/tests/mispevent_testfiles/event_obj_def_param.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     4528 2018-12-03 16:06:16.000000 pymisp-2.4.99/tests/mispevent_testfiles/shadow.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      429 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/mispevent_testfiles/attribute.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1032 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/mispevent_testfiles/misp_custom_obj.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)       21 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/mispevent_testfiles/simple.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)       63 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/mispevent_testfiles/sighting.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      474 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/mispevent_testfiles/attribute_del.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      244 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/mispevent_testfiles/event_tags.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      795 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/mispevent_testfiles/proposals.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)   154729 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/mispevent_testfiles/existing_event_edited.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/tests/mispevent_testfiles/test_object_template/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      578 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/mispevent_testfiles/test_object_template/definition.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1633 2018-12-03 16:06:16.000000 pymisp-2.4.99/tests/mispevent_testfiles/event_obj_attr_tag.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     7511 2018-12-03 16:06:16.000000 pymisp-2.4.99/tests/mispevent_testfiles/malware_exist.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      722 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/mispevent_testfiles/event_obj_tag.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      173 2018-09-06 06:43:41.000000 pymisp-2.4.99/tests/mispevent_testfiles/event.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)    21524 2018-12-03 16:06:16.000000 pymisp-2.4.99/tests/test_offline.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)    16761 2018-10-12 13:43:56.000000 pymisp-2.4.99/tests/test.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2256 2018-12-03 16:06:16.000000 pymisp-2.4.99/tests/sharing_groups.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)    52710 2018-12-03 16:06:16.000000 pymisp-2.4.99/tests/testlive_comprehensive.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     9241 2018-10-12 13:43:56.000000 pymisp-2.4.99/pymisp/abstract.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)    26995 2018-12-03 16:06:16.000000 pymisp-2.4.99/pymisp/aping.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     9178 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/data/schema.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     8561 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/data/schema-lax.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/relationships/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)    23729 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/relationships/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/coin-address/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2861 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/coin-address/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Web-Bookmark/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1691 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Web-Bookmark/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/cap-info/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     5181 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/cap-info/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-system-hive-service-drivers/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2534 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-system-hive-service-drivers/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/email/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     4654 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/email/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-appInit-DLLS/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1490 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-appInit-DLLS/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Web-Downloads/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1456 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Web-Downloads/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-applications-installed/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1623 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-applications-installed/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/ja3/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1421 2018-10-12 13:44:10.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/ja3/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/gtp-attack/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2572 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/gtp-attack/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/timestamp/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1316 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/timestamp/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/malware-config/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1479 2018-10-12 13:44:10.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/malware-config/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/sandbox-report/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2692 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/sandbox-report/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/whois/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2584 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/whois/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/cortex/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1353 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/cortex/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/stix2-pattern/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      837 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/stix2-pattern/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-system-hive-firewall-configuration/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1483 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-system-hive-firewall-configuration/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/script/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1584 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/script/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/ss7-attack/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     4860 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/ss7-attack/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/x509/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3158 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/x509/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/yara/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      982 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/yara/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/credential/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1855 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/credential/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/mactime-timeline-analysis/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1549 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/mactime-timeline-analysis/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/bank-account/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     5219 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/bank-account/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/timesketch-timeline/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      927 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/timesketch-timeline/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/exploit-poc/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1386 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/exploit-poc/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/cap-resource/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1440 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/cap-resource/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/fail2ban/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1601 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/fail2ban/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/elf/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     5016 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/elf/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/cowrie/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3404 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/cowrie/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-application-paths/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1353 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-application-paths/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/ip-port/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2027 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/ip-port/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/report/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      677 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/report/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/phishing/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1898 2018-10-12 13:44:10.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/phishing/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-system-hive-network-information/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3115 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-system-hive-network-information/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/process/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2607 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/process/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/android-permission/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     5020 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/android-permission/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/python-etvx-event-log/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     4858 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/python-etvx-event-log/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-sam-hive-single-user/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2033 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-sam-hive-single-user/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/virustotal-report/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1422 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/virustotal-report/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/network-socket/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     4585 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/network-socket/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-command-shell/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1416 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-command-shell/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Web-Search-Query/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1588 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Web-Search-Query/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/victim/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3051 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/victim/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/asn/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2484 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/asn/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/http-request/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2990 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/http-request/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/cortex-taxonomy/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1561 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/cortex-taxonomy/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/person/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     4763 2018-12-06 14:23:14.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/person/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/forensic-evidence/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2275 2018-10-12 13:44:10.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/forensic-evidence/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/annotation/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1748 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/annotation/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/forensic-case/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1282 2018-10-12 13:44:10.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/forensic-case/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/ail-leak/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2182 2018-10-12 13:44:10.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/ail-leak/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/paste/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1933 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/paste/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/cookie/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1519 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/cookie/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/shortened-link/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1114 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/shortened-link/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/elf-section/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     4113 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/elf-section/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/timesketch_message/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      589 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/timesketch_message/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/original-imported-file/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      885 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/original-imported-file/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/transaction/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3161 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/transaction/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/network-connection/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2515 2018-10-12 13:44:10.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/network-connection/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/vehicle/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1311 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/vehicle/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/cap-alert/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     4252 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/cap-alert/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-sam-hive-user-group/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1510 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-sam-hive-user-group/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/diameter-attack/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2388 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/diameter-attack/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/av-signature/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1087 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/av-signature/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/course-of-action/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2688 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/course-of-action/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/short-message-service/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1382 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/short-message-service/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-system-hive-general-configuration/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3027 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-system-hive-general-configuration/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/pe-section/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2891 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/pe-section/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/ais-info/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1591 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/ais-info/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/legal-entity/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1244 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/legal-entity/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/pe/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3625 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/pe/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/mutex/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      745 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/mutex/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/bgp-hijack/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1436 2018-10-12 13:44:10.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/bgp-hijack/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Web-History/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1671 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Web-History/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Web-Cookie/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1705 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Web-Cookie/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/tor-node/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2603 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/tor-node/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-userprofile-winlogon/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     5419 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-userprofile-winlogon/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/geolocation/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3025 2018-10-12 13:44:10.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/geolocation/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/ip-api-address/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2798 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/ip-api-address/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/tracking-id/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1546 2018-10-12 13:44:10.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/tracking-id/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/file/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     4730 2018-10-12 13:44:10.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/file/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-general-windows-info/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3481 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-general-windows-info/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/macho-section/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2551 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/macho-section/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/target-system/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1002 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/target-system/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-BHO/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1689 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-BHO/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-NTUser/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2975 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-NTUser/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/microblog/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1812 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/microblog/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/sb-signature/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1160 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/sb-signature/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-software-run/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1704 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-software-run/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/rtir/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1519 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/rtir/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/timecode/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1489 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/timecode/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/phone/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2742 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/phone/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/ddos/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2447 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/ddos/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/domain-ip/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1271 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/domain-ip/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/r2graphity/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     4597 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/r2graphity/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Chats/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2321 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Chats/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/passive-dns/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3178 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/passive-dns/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/yabin/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1158 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/yabin/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regexp/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1431 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/regexp/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/vulnerability/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3032 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/vulnerability/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/internal-reference/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1043 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/internal-reference/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/credit-card/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1335 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/credit-card/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/registry-key/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2511 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/registry-key/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/macho/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1330 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/macho/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/pcap-metadata/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     5889 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/pcap-metadata/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/suricata/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      953 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/suricata/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/netflow/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3826 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/netflow/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/url/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2743 2018-12-03 16:06:54.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/url/definition.json
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/threatgrid-report/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1700 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/objects/threatgrid-report/definition.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2283 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/schema_objects.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1121 2018-09-06 06:44:38.000000 pymisp-2.4.99/pymisp/data/misp-objects/schema_relationships.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)    27649 2018-12-06 14:22:09.000000 pymisp-2.4.99/pymisp/data/describeTypes.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)    47985 2018-12-03 16:06:16.000000 pymisp-2.4.99/pymisp/mispevent.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp/tools/
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)    14163 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/openioc.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     6265 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/peobject.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2755 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/emailobject.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2379 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/abstractgenerator.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      742 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/sbsignatureobject.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      726 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/fail2banobject.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3910 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/elfobject.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     4096 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/create_misp_object.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3726 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/machoobject.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1294 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/stix.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      829 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/load_warninglists.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1988 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/neo4j.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      906 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/ext_lookups.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      906 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/__init__.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3200 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/fileobject.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1534 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/genericgenerator.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      825 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/domainipobject.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      828 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/geolocationobject.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3157 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/vtreportobject.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      804 2018-09-06 06:43:41.000000 pymisp-2.4.99/pymisp/tools/asnobject.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)   108627 2018-12-06 14:22:09.000000 pymisp-2.4.99/pymisp/api.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1988 2018-12-06 14:22:09.000000 pymisp-2.4.99/pymisp/__init__.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1063 2018-10-12 13:43:56.000000 pymisp-2.4.99/pymisp/exceptions.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/docs/
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/docs/tutorial/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)       48 2018-09-06 06:43:41.000000 pymisp-2.4.99/docs/tutorial/install_notebook.sh
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     9974 2018-12-03 16:06:16.000000 pymisp-2.4.99/docs/tutorial/Search.ipynb
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)    23565 2018-12-03 16:06:16.000000 pymisp-2.4.99/docs/tutorial/PyMISP Objects.ipynb
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     9786 2018-12-03 16:06:16.000000 pymisp-2.4.99/docs/tutorial/Search-NG.ipynb
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)    12269 2018-12-03 16:06:16.000000 pymisp-2.4.99/docs/tutorial/PyMISP_tutorial.ipynb
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)    10305 2018-12-03 16:06:16.000000 pymisp-2.4.99/docs/tutorial/Usage-NG.ipynb
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     7615 2018-09-06 06:43:41.000000 pymisp-2.4.99/docs/Makefile
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/docs/source/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1152 2018-12-06 14:22:09.000000 pymisp-2.4.99/docs/source/modules.rst
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      451 2018-09-06 06:43:41.000000 pymisp-2.4.99/docs/source/index.rst
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      948 2018-09-06 06:43:41.000000 pymisp-2.4.99/docs/source/tools.rst
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     4654 2018-12-03 16:06:16.000000 pymisp-2.4.99/docs/source/README.md
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)    12320 2018-09-06 06:43:41.000000 pymisp-2.4.99/docs/source/conf.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     4654 2018-12-03 16:06:16.000000 pymisp-2.4.99/README.md
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/examples/
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1668 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/search.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)        7 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/get_network_activity.event_id
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      757 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/up.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      914 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/add_feed.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1381 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/get_csv.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1488 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/misp2clamav.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      804 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/delete_user.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/examples/suricata_search/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1025 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/suricata_search/README.md
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     6870 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/suricata_search/suricata_search.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     3476 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/add_fail2ban_object.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      228 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/keys.py.sample
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      877 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/add_named_attribute.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1032 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/edit_user_json.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      563 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/stats.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      292 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/cache_all.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/examples/events/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1638 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/events/dummy
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      777 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/events/create_massive_dummy_events.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2975 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/events/tools.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      687 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/events/create_dummy_event.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2777 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/events/README.md
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     7514 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/vt_to_misp.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      793 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/suricata.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1076 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/add_email_object.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      946 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/yara.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     3768 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/yara_dump.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     6744 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/get_network_activity.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      726 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/warninglists.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1022 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/tagstatistics.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1258 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/addtag.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1613 2018-12-06 14:22:09.000000 pymisp-2.4.99/examples/add_generic_object.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      817 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/edit_user.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1273 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/search_sighting.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      598 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/sharing_groups.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/examples/ioc-2-misp/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3081 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/ioc-2-misp/keys.py.sample
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      455 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/ioc-2-misp/README.md
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)    11599 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/ioc-2-misp/ioc2misp.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      579 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/ioc-2-misp/taxonomy.csv
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     3991 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/et2misp.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     2554 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/copy_list.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      885 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/del.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/examples/graphdb/
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1516 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/graphdb/make_neo4j.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)       66 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/sighting.json
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1261 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/add_sbsignature.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1223 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/last.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     2361 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/misp2cef.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     2145 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/generate_file_objects.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/__init__.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1531 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/add_file_object.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1141 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/get.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      702 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/sighting.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      713 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/lookup.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1164 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/create_events.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      674 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/get_attachment.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1347 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/search_attributes_yara.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      625 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/freetext.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1614 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/addtag2.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      534 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/tags.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      666 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/fetch_events_feed.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)       38 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/freetext.txt
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      480 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/test_sign.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      885 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/add_user_json.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1244 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/searchall.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/examples/situational-awareness/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1107 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/situational-awareness/bokeh_tools.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2206 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/situational-awareness/pygal_tools.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3761 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/situational-awareness/tags_to_graphs.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1508 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/situational-awareness/attribute_treemap.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)    13236 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/situational-awareness/tools.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2342 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/situational-awareness/tag_scatter.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3082 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/situational-awareness/tag_search.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      608 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/situational-awareness/style.css
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2485 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/situational-awareness/tags_count.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2683 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/situational-awareness/README.md
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      541 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/situational-awareness/style2.css
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      520 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/situational-awareness/test_attribute_treemap.html
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1867 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/situational-awareness/date_tools.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      585 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/users_list.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/examples/feed-generator/
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1375 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/feed-generator/settings.default.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/examples/feed-generator/output/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)        0 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/feed-generator/output/empty
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     5710 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/feed-generator/generate.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      850 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/feed-generator/README.md
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      930 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/openioc_to_misp.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     4224 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/asciidoc_generator.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/examples/feed-generator-from-redis/
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     1585 2018-10-12 13:43:56.000000 pymisp-2.4.99/examples/feed-generator-from-redis/settings.default.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      279 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/feed-generator-from-redis/server.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     9830 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/feed-generator-from-redis/generator.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     5224 2018-10-12 13:43:56.000000 pymisp-2.4.99/examples/feed-generator-from-redis/fromredis.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      113 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/feed-generator-from-redis/install.sh
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/examples/feed-generator-from-redis/ObjectConstructor/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1259 2018-10-12 13:43:56.000000 pymisp-2.4.99/examples/feed-generator-from-redis/ObjectConstructor/CowrieMISPObject.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2260 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/feed-generator-from-redis/README.md
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3247 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/feed-generator-from-redis/MISPItemToRedis.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/examples/profiles/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      414 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/profiles/weekly_report.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      459 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/profiles/daily_report.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)        0 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/profiles/__init__.py
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)     2270 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/upload.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)       87 2018-09-06 06:43:41.000000 pymisp-2.4.99/examples/user_sample.json
+-rwxrwxr-x   0 raphael   (1000) raphael   (1000)      890 2018-12-03 16:06:16.000000 pymisp-2.4.99/examples/add_user.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2018-12-06 14:24:01.000000 pymisp-2.4.99/pymisp.egg-info/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      245 2018-12-06 14:24:00.000000 pymisp-2.4.99/pymisp.egg-info/requires.txt
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)        1 2018-12-06 14:24:00.000000 pymisp-2.4.99/pymisp.egg-info/dependency_links.txt
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)    12567 2018-12-06 14:24:00.000000 pymisp-2.4.99/pymisp.egg-info/SOURCES.txt
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)        7 2018-12-06 14:24:00.000000 pymisp-2.4.99/pymisp.egg-info/top_level.txt
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     6924 2018-12-06 14:24:00.000000 pymisp-2.4.99/pymisp.egg-info/PKG-INFO
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     6924 2018-12-06 14:24:01.000000 pymisp-2.4.99/PKG-INFO
```

### Comparing `pymisp-2.4.98/CHANGELOG.txt` & `pymisp-2.4.99/CHANGELOG.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Changelog
 =========
 
 
-v2.4.98 (2018-12-03)
+v2.4.99 (2018-12-06)
 --------------------
 
 New
 ~~~
+- Auto generate doc for PyMISPExpanded. [Raphaël Vinot]
 - Search_index in ExpandedPyMISP, cleanup, update jupyter. [Raphaël
   Vinot]
 - Add log search. [Raphaël Vinot]
 - Add test for pushing an event to ZMQ. [Raphaël Vinot]
 - Change_distribution method. [Raphaël Vinot]
 - Add test cases for sightings, cleanup. [Raphaël Vinot]
 - [example] Added sighting rest search example. [Sami Mokaddem]
 - [sighting] Added support of sighting REST API. [Sami Mokaddem]
 - Allow to pass csv to return_format in search. [Raphaël Vinot]
 - Page/limit in search. [Raphaël Vinot]
 
 Changes
 ~~~~~~~
+- Bump Changelog. [Raphaël Vinot]
+- Bump version. [Raphaël Vinot]
+- Bump misp-objects & describeTypes. [Raphaël Vinot]
+- Bump Changelog. [Raphaël Vinot]
 - Version bump. [Raphaël Vinot]
 - Bump misp-objects. [Raphaël Vinot]
 - Add test cases for default distribution levels. [Raphaël Vinot]
 - Include proposals in attributes search. [Dawid Czarnecki]
 
   Add includeProposals param to the search method
 - Bump misp-objects. [Raphaël Vinot]
@@ -34,32 +39,42 @@
   [Raphaël Vinot]
 - Bump misp-objects. [Raphaël Vinot]
 - Add print in testlive to debug travis. [Raphaël Vinot]
 - Bump objects. [Raphaël Vinot]
 
 Fix
 ~~~
+- Auto generate doc for PyMISPExpanded. [Raphaël Vinot]
 - Test failing on travis... [Raphaël Vinot]
 - Properly handle errors on event creation/update. [Raphaël Vinot]
 - Test case. [Raphaël Vinot]
 - Do not run the zmq test on travis. [Raphaël Vinot]
 - Type of quick_filter. [Raphaël Vinot]
 - Quick_filter was broken. [Raphaël Vinot]
 - Properly initialize the config when jupyter runs on the VM. [Raphaël
   Vinot]
 - Travis run. [Raphaël Vinot]
 - Readme update + python3 + pep8. [Christophe Vandeplas]
 
   align python path to readme specifying python3
 - Feed-generator gitignore. [Christophe Vandeplas]
 - Test cases. [Raphaël Vinot]
-- Test cases sample files. [Raphaël Vinot]
 
 Other
 ~~~~~
+- Merge branch 'master' of github.com:MISP/PyMISP. [Raphaël Vinot]
+- Merge pull request #310 from DragonDev1906/master. [Raphaël Vinot]
+
+  Added get_object & get_attribute (by ID)
+- Dded get_object & get_attribute. [DragonDev1906]
+- Merge pull request #307 from garanews/patch-1. [Raphaël Vinot]
+
+  fix for last pymisp version
+- Fix for last pymisp version. [garanews]
+- Merge branch 'master' of github.com:MISP/PyMISP. [Raphaël Vinot]
 - Merge pull request #305 from dawid-
   czarnecki/feature/include_proposals. [Raphaël Vinot]
 
   chg: Include proposals in attributes search
 - Merge pull request #301 from deralexxx/patch-7. [Raphaël Vinot]
 
   mention virtualenv
@@ -111,14 +126,15 @@
 - More test cases. [Raphaël Vinot]
 - Update order parameters & doc. [Raphaël Vinot]
 - Add an extra IP from the warninglists. [Raphaël Vinot]
 - Test for event UUID in attribute. [Raphaël Vinot]
 
 Fix
 ~~~
+- Test cases sample files. [Raphaël Vinot]
 - Prevent checking length on a integer. [Sami Mokaddem]
 - Direct call & add example. [Raphaël Vinot]
 - Disable test for travis, take 2. [Raphaël Vinot]
 - Disable test for travis. [Raphaël Vinot]
 - Skip tests that fail on travis for no reason... [Raphaël Vinot]
 - Tentative to fix tests on travis. [Raphaël Vinot]
 - Disable test warning lists. Enabling is not deterministic. [Raphaël
```

### Comparing `pymisp-2.4.98/LICENSE` & `pymisp-2.4.99/LICENSE`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/setup.py` & `pymisp-2.4.99/setup.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/misp_event.json` & `pymisp-2.4.99/tests/misp_event.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/test_mispevent.py` & `pymisp-2.4.99/tests/test_mispevent.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/search_index_result.json` & `pymisp-2.4.99/tests/search_index_result.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/new_misp_event.json` & `pymisp-2.4.99/tests/new_misp_event.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/57c4445b-c548-4654-af0b-4be3950d210f.json` & `pymisp-2.4.99/tests/57c4445b-c548-4654-af0b-4be3950d210f.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/mispevent_testfiles/existing_event.json` & `pymisp-2.4.99/tests/mispevent_testfiles/existing_event.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/mispevent_testfiles/def_param.json` & `pymisp-2.4.99/tests/mispevent_testfiles/def_param.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/mispevent_testfiles/event_obj_def_param.json` & `pymisp-2.4.99/tests/mispevent_testfiles/event_obj_def_param.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/mispevent_testfiles/shadow.json` & `pymisp-2.4.99/tests/mispevent_testfiles/shadow.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/mispevent_testfiles/misp_custom_obj.json` & `pymisp-2.4.99/tests/mispevent_testfiles/misp_custom_obj.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/mispevent_testfiles/proposals.json` & `pymisp-2.4.99/tests/mispevent_testfiles/proposals.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/mispevent_testfiles/existing_event_edited.json` & `pymisp-2.4.99/tests/mispevent_testfiles/existing_event_edited.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/mispevent_testfiles/test_object_template/definition.json` & `pymisp-2.4.99/tests/mispevent_testfiles/test_object_template/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/mispevent_testfiles/event_obj_attr_tag.json` & `pymisp-2.4.99/tests/mispevent_testfiles/event_obj_attr_tag.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/mispevent_testfiles/malware_exist.json` & `pymisp-2.4.99/tests/mispevent_testfiles/malware_exist.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/mispevent_testfiles/event_obj_tag.json` & `pymisp-2.4.99/tests/mispevent_testfiles/event_obj_tag.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/test_offline.py` & `pymisp-2.4.99/tests/test_offline.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/test.py` & `pymisp-2.4.99/tests/test.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/sharing_groups.json` & `pymisp-2.4.99/tests/sharing_groups.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/tests/testlive_comprehensive.py` & `pymisp-2.4.99/tests/testlive_comprehensive.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/abstract.py` & `pymisp-2.4.99/pymisp/abstract.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/aping.py` & `pymisp-2.4.99/pymisp/aping.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/schema.json` & `pymisp-2.4.99/pymisp/data/schema.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/schema-lax.json` & `pymisp-2.4.99/pymisp/data/schema-lax.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/relationships/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/relationships/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/coin-address/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/coin-address/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Web-Bookmark/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Web-Bookmark/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/cap-info/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/cap-info/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-system-hive-service-drivers/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-system-hive-service-drivers/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/email/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/email/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-appInit-DLLS/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-appInit-DLLS/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Web-Downloads/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Web-Downloads/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-applications-installed/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-applications-installed/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/ja3/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/ja3/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/gtp-attack/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/gtp-attack/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/timestamp/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/timestamp/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/malware-config/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/malware-config/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/sandbox-report/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/sandbox-report/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/whois/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/whois/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/cortex/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/cortex/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/stix2-pattern/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/stix2-pattern/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-system-hive-firewall-configuration/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-system-hive-firewall-configuration/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/script/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/script/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/ss7-attack/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/ss7-attack/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/x509/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/x509/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/yara/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/yara/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/credential/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/credential/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/mactime-timeline-analysis/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/mactime-timeline-analysis/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/bank-account/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/bank-account/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/timesketch-timeline/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/timesketch-timeline/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/exploit-poc/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/exploit-poc/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/cap-resource/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/cap-resource/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/fail2ban/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/fail2ban/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/elf/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/elf/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/cowrie/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/cowrie/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-application-paths/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-application-paths/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/ip-port/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/ip-port/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/report/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/report/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/phishing/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/phishing/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-system-hive-network-information/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-system-hive-network-information/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/process/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/process/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/android-permission/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/android-permission/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/python-etvx-event-log/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/python-etvx-event-log/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-sam-hive-single-user/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-sam-hive-single-user/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/virustotal-report/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/virustotal-report/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/network-socket/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/network-socket/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-command-shell/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-command-shell/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Web-Search-Query/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Web-Search-Query/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/victim/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/victim/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/asn/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/asn/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/http-request/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/http-request/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/cortex-taxonomy/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/cortex-taxonomy/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/person/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/person/definition.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9226190476190476%*

 * *Differences: {"'attributes'": "{'birth-certificate-number': OrderedDict([('description', 'Birth Certificate "*

 * *                 "Number'), ('ui-priority', 0), ('misp-attribute', 'text')]), "*

 * *                 "'ofac-identification-number': OrderedDict([('description', 'ofac-identification "*

 * *                 "Number'), ('ui-priority', 0), ('misp-attribute', 'text')])}",*

 * * "'version'": '5'}*

```diff
@@ -8,14 +8,19 @@
         },
         "alias": {
             "description": "Alias name or known as.",
             "misp-attribute": "text",
             "multiple": true,
             "ui-priority": 0
         },
+        "birth-certificate-number": {
+            "description": "Birth Certificate Number",
+            "misp-attribute": "text",
+            "ui-priority": 0
+        },
         "date-of-birth": {
             "description": "Date of birth of a natural person (in YYYY-MM-DD format).",
             "misp-attribute": "date-of-birth",
             "ui-priority": 0
         },
         "e-mail": {
             "description": "Email address of the person.",
@@ -76,14 +81,19 @@
         },
         "nic-hdl": {
             "description": "NIC Handle (Network Information Centre handle) of the person.",
             "misp-attribute": "text",
             "multiple": true,
             "ui-priority": 10
         },
+        "ofac-identification-number": {
+            "description": "ofac-identification Number",
+            "misp-attribute": "text",
+            "ui-priority": 0
+        },
         "passport-country": {
             "description": "The country in which the passport was issued.",
             "disable_correlation": true,
             "misp-attribute": "passport-country",
             "ui-priority": 0
         },
         "passport-expiration": {
@@ -136,9 +146,9 @@
     "meta-category": "misc",
     "name": "person",
     "requiredOneOf": [
         "first-name",
         "last-name"
     ],
     "uuid": "a15b0477-e9d1-4b9c-9546-abe78a4f4248",
-    "version": 4
+    "version": 5
 }
```

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/forensic-evidence/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/forensic-evidence/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/annotation/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/annotation/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/forensic-case/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/forensic-case/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/ail-leak/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/ail-leak/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/paste/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/paste/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/cookie/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/cookie/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/shortened-link/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/shortened-link/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/elf-section/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/elf-section/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/timesketch_message/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/timesketch_message/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/original-imported-file/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/original-imported-file/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/transaction/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/transaction/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/network-connection/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/network-connection/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/vehicle/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/vehicle/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/cap-alert/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/cap-alert/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-sam-hive-user-group/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-sam-hive-user-group/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/diameter-attack/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/diameter-attack/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/av-signature/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/av-signature/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/course-of-action/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/course-of-action/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/short-message-service/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/short-message-service/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-system-hive-general-configuration/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-system-hive-general-configuration/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/pe-section/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/pe-section/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/ais-info/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/ais-info/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/legal-entity/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/legal-entity/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/pe/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/pe/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/mutex/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/mutex/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/bgp-hijack/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/bgp-hijack/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Web-History/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Web-History/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Web-Cookie/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Web-Cookie/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/tor-node/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/tor-node/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-userprofile-winlogon/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-userprofile-winlogon/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/geolocation/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/geolocation/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/ip-api-address/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/ip-api-address/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/tracking-id/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/tracking-id/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/file/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/file/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-general-windows-info/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-general-windows-info/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/macho-section/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/macho-section/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/target-system/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/target-system/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-BHO/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-BHO/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-NTUser/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-NTUser/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/microblog/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/microblog/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/sb-signature/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/sb-signature/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regripper-software-hive-software-run/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regripper-software-hive-software-run/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/rtir/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/rtir/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/timecode/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/timecode/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/phone/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/phone/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/ddos/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/ddos/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/domain-ip/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/domain-ip/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/r2graphity/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/r2graphity/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/TSK-Chats/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/TSK-Chats/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/passive-dns/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/passive-dns/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/yabin/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/yabin/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/regexp/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/regexp/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/vulnerability/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/vulnerability/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/internal-reference/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/internal-reference/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/credit-card/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/credit-card/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/registry-key/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/registry-key/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/macho/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/macho/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/pcap-metadata/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/pcap-metadata/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/suricata/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/suricata/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/netflow/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/netflow/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/url/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/url/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/objects/threatgrid-report/definition.json` & `pymisp-2.4.99/pymisp/data/misp-objects/objects/threatgrid-report/definition.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/schema_objects.json` & `pymisp-2.4.99/pymisp/data/misp-objects/schema_objects.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/misp-objects/schema_relationships.json` & `pymisp-2.4.99/pymisp/data/misp-objects/schema_relationships.json`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/data/describeTypes.json` & `pymisp-2.4.99/pymisp/data/describeTypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8946542117157037%*

 * *Differences: {"'result'": "{'categories': {insert: [(0, 'Internal reference'), (1, 'Targeting data'), (3, "*

 * *             "'Payload delivery'), (5, 'Payload installation'), (6, 'Persistence mechanism'), (7, "*

 * *             "'Network activity'), (8, 'Payload type'), (13, 'Social network'), (14, 'Person'), "*

 * *             "(15, 'Other')], delete: [15, 13, 12, 11, 10, 9, 8, 7, 6, 5]}, "*

 * *             "'category_type_mappings': {'Network activity': {insert: [(23, "*

 * *             "'x509-fingerprint-md5'), (25, 'x509-fingerprint-s […]*

```diff
@@ -1,26 +1,26 @@
 {
     "result": {
         "categories": [
+            "Internal reference",
+            "Targeting data",
             "Antivirus detection",
+            "Payload delivery",
             "Artifacts dropped",
+            "Payload installation",
+            "Persistence mechanism",
+            "Network activity",
+            "Payload type",
             "Attribution",
             "External analysis",
             "Financial fraud",
-            "Internal reference",
-            "Network activity",
-            "Other",
-            "Payload delivery",
-            "Payload installation",
-            "Payload type",
-            "Persistence mechanism",
-            "Person",
-            "Social network",
             "Support Tool",
-            "Targeting data"
+            "Social network",
+            "Person",
+            "Other"
         ],
         "category_type_mappings": {
             "Antivirus detection": [
                 "link",
                 "comment",
                 "text",
                 "hex",
@@ -182,15 +182,17 @@
                 "snort",
                 "pattern-in-file",
                 "stix2-pattern",
                 "pattern-in-traffic",
                 "attachment",
                 "comment",
                 "text",
+                "x509-fingerprint-md5",
                 "x509-fingerprint-sha1",
+                "x509-fingerprint-sha256",
                 "other",
                 "hex",
                 "cookie",
                 "hostname|port",
                 "bro"
             ],
             "Other": [
@@ -1015,162 +1017,162 @@
             },
             "yara": {
                 "default_category": "Payload installation",
                 "to_ids": 1
             }
         },
         "types": [
+            "md5",
+            "sha1",
+            "sha256",
+            "filename",
+            "pdb",
+            "filename|md5",
+            "filename|sha1",
+            "filename|sha256",
+            "ip-src",
+            "ip-dst",
+            "hostname",
+            "domain",
+            "domain|ip",
+            "email-src",
+            "email-dst",
+            "email-subject",
+            "email-attachment",
+            "email-body",
+            "float",
+            "url",
+            "http-method",
+            "user-agent",
+            "regkey",
+            "regkey|value",
             "AS",
-            "aba-rtn",
+            "snort",
+            "bro",
+            "pattern-in-file",
+            "pattern-in-traffic",
+            "pattern-in-memory",
+            "yara",
+            "stix2-pattern",
+            "sigma",
+            "gene",
+            "mime-type",
+            "identity-card-number",
+            "cookie",
+            "vulnerability",
             "attachment",
-            "authentihash",
-            "bank-account-nr",
+            "malware-sample",
+            "link",
+            "comment",
+            "text",
+            "hex",
+            "other",
+            "named pipe",
+            "mutex",
+            "target-user",
+            "target-email",
+            "target-machine",
+            "target-org",
+            "target-location",
+            "target-external",
+            "btc",
+            "xmr",
+            "iban",
             "bic",
+            "bank-account-nr",
+            "aba-rtn",
             "bin",
-            "boolean",
-            "bro",
-            "btc",
-            "campaign-id",
-            "campaign-name",
             "cc-number",
-            "comment",
-            "cookie",
-            "cortex",
-            "counter",
-            "country-of-residence",
-            "cpe",
-            "date-of-birth",
-            "datetime",
-            "dns-soa-email",
-            "domain",
-            "domain|ip",
-            "email-attachment",
-            "email-body",
-            "email-dst",
-            "email-dst-display-name",
-            "email-header",
-            "email-message-id",
-            "email-mime-boundary",
-            "email-reply-to",
-            "email-src",
-            "email-src-display-name",
-            "email-subject",
-            "email-thread-index",
-            "email-x-mailer",
-            "filename",
+            "prtn",
+            "phone-number",
+            "threat-actor",
+            "campaign-name",
+            "campaign-id",
+            "malware-type",
+            "uri",
+            "authentihash",
+            "ssdeep",
+            "imphash",
+            "pehash",
+            "impfuzzy",
+            "sha224",
+            "sha384",
+            "sha512",
+            "sha512/224",
+            "sha512/256",
+            "tlsh",
             "filename|authentihash",
-            "filename|impfuzzy",
+            "filename|ssdeep",
             "filename|imphash",
-            "filename|md5",
+            "filename|impfuzzy",
             "filename|pehash",
-            "filename|sha1",
             "filename|sha224",
-            "filename|sha256",
             "filename|sha384",
             "filename|sha512",
             "filename|sha512/224",
             "filename|sha512/256",
-            "filename|ssdeep",
             "filename|tlsh",
-            "first-name",
-            "float",
-            "frequent-flyer-number",
-            "gender",
-            "gene",
-            "github-organisation",
-            "github-repository",
-            "github-username",
-            "hex",
-            "hostname",
-            "hostname|port",
-            "http-method",
-            "iban",
-            "identity-card-number",
-            "impfuzzy",
-            "imphash",
-            "ip-dst",
+            "windows-scheduled-task",
+            "windows-service-name",
+            "windows-service-displayname",
+            "whois-registrant-email",
+            "whois-registrant-phone",
+            "whois-registrant-name",
+            "whois-registrant-org",
+            "whois-registrar",
+            "whois-creation-date",
+            "x509-fingerprint-sha1",
+            "x509-fingerprint-md5",
+            "x509-fingerprint-sha256",
+            "dns-soa-email",
+            "size-in-bytes",
+            "counter",
+            "datetime",
+            "cpe",
+            "port",
             "ip-dst|port",
-            "ip-src",
             "ip-src|port",
-            "issue-date-of-the-visa",
-            "jabber-id",
-            "last-name",
-            "link",
+            "hostname|port",
             "mac-address",
             "mac-eui-64",
-            "malware-sample",
-            "malware-type",
-            "md5",
+            "email-dst-display-name",
+            "email-src-display-name",
+            "email-header",
+            "email-reply-to",
+            "email-x-mailer",
+            "email-mime-boundary",
+            "email-thread-index",
+            "email-message-id",
+            "github-username",
+            "github-repository",
+            "github-organisation",
+            "jabber-id",
+            "twitter-id",
+            "first-name",
             "middle-name",
-            "mime-type",
-            "mobile-application-id",
-            "mutex",
-            "named pipe",
-            "nationality",
-            "other",
-            "passenger-name-record-locator-number",
+            "last-name",
+            "date-of-birth",
+            "place-of-birth",
+            "gender",
+            "passport-number",
             "passport-country",
             "passport-expiration",
-            "passport-number",
-            "pattern-in-file",
-            "pattern-in-memory",
-            "pattern-in-traffic",
-            "payment-details",
-            "pdb",
-            "pehash",
-            "phone-number",
-            "place-of-birth",
-            "place-port-of-clearance",
-            "place-port-of-onward-foreign-destination",
-            "place-port-of-original-embarkation",
-            "port",
-            "primary-residence",
-            "prtn",
             "redress-number",
-            "regkey",
-            "regkey|value",
-            "sha1",
-            "sha224",
-            "sha256",
-            "sha384",
-            "sha512",
-            "sha512/224",
-            "sha512/256",
-            "sigma",
-            "size-in-bytes",
-            "snort",
+            "nationality",
+            "visa-number",
+            "issue-date-of-the-visa",
+            "primary-residence",
+            "country-of-residence",
             "special-service-request",
-            "ssdeep",
-            "stix2-pattern",
-            "target-email",
-            "target-external",
-            "target-location",
-            "target-machine",
-            "target-org",
-            "target-user",
-            "text",
-            "threat-actor",
-            "tlsh",
+            "frequent-flyer-number",
             "travel-details",
-            "twitter-id",
-            "uri",
-            "url",
-            "user-agent",
-            "visa-number",
-            "vulnerability",
-            "whois-creation-date",
-            "whois-registrant-email",
-            "whois-registrant-name",
-            "whois-registrant-org",
-            "whois-registrant-phone",
-            "whois-registrar",
-            "windows-scheduled-task",
-            "windows-service-displayname",
-            "windows-service-name",
-            "x509-fingerprint-md5",
-            "x509-fingerprint-sha1",
-            "x509-fingerprint-sha256",
-            "xmr",
-            "yara"
+            "payment-details",
+            "place-port-of-original-embarkation",
+            "place-port-of-clearance",
+            "place-port-of-onward-foreign-destination",
+            "passenger-name-record-locator-number",
+            "mobile-application-id",
+            "cortex",
+            "boolean"
         ]
     }
 }
```

### Comparing `pymisp-2.4.98/pymisp/mispevent.py` & `pymisp-2.4.99/pymisp/mispevent.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/openioc.py` & `pymisp-2.4.99/pymisp/tools/openioc.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/peobject.py` & `pymisp-2.4.99/pymisp/tools/peobject.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/emailobject.py` & `pymisp-2.4.99/pymisp/tools/emailobject.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/abstractgenerator.py` & `pymisp-2.4.99/pymisp/tools/abstractgenerator.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/sbsignatureobject.py` & `pymisp-2.4.99/pymisp/tools/sbsignatureobject.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/fail2banobject.py` & `pymisp-2.4.99/pymisp/tools/fail2banobject.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/elfobject.py` & `pymisp-2.4.99/pymisp/tools/elfobject.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/create_misp_object.py` & `pymisp-2.4.99/pymisp/tools/create_misp_object.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/machoobject.py` & `pymisp-2.4.99/pymisp/tools/machoobject.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/stix.py` & `pymisp-2.4.99/pymisp/tools/stix.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/load_warninglists.py` & `pymisp-2.4.99/pymisp/tools/load_warninglists.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/neo4j.py` & `pymisp-2.4.99/pymisp/tools/neo4j.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/ext_lookups.py` & `pymisp-2.4.99/pymisp/tools/ext_lookups.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/__init__.py` & `pymisp-2.4.99/pymisp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/fileobject.py` & `pymisp-2.4.99/pymisp/tools/fileobject.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/genericgenerator.py` & `pymisp-2.4.99/pymisp/tools/genericgenerator.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/domainipobject.py` & `pymisp-2.4.99/pymisp/tools/domainipobject.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/geolocationobject.py` & `pymisp-2.4.99/pymisp/tools/geolocationobject.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/vtreportobject.py` & `pymisp-2.4.99/pymisp/tools/vtreportobject.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/tools/asnobject.py` & `pymisp-2.4.99/pymisp/tools/asnobject.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp/api.py` & `pymisp-2.4.99/pymisp/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,14 +332,32 @@
 
         :param event_id: Event id to get
         """
         url = urljoin(self.root_url, 'events/{}'.format(event_id))
         response = self._prepare_request('GET', url)
         return self._check_response(response)
 
+    def get_object(self, obj_id):
+        """Get an object
+
+        :param obj_id: Object id to get
+        """
+        url = urljoin(self.root_url, 'objects/view/{}'.format(obj_id))
+        response = self._prepare_request('GET', url)
+        return self._check_response(response)
+
+    def get_attribute(self, att_id):
+        """Get an attribute
+
+        :param att_id: Attribute id to get
+        """
+        url = urljoin(self.root_url, 'attributes/view/{}'.format(att_id))
+        response = self._prepare_request('GET', url)
+        return self._check_response(response)
+
     def add_event(self, event):
         """Add a new event
 
         :param event: Event as JSON object / string to add
         """
         url = urljoin(self.root_url, 'events')
         if isinstance(event, MISPEvent):
```

### Comparing `pymisp-2.4.98/pymisp/__init__.py` & `pymisp-2.4.99/pymisp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.4.98'
+__version__ = '2.4.99'
 import logging
 import functools
 import warnings
 import sys
 
 FORMAT = "%(levelname)s [%(filename)s:%(lineno)s - %(funcName)s() ] %(message)s"
 formatter = logging.Formatter(FORMAT)
```

### Comparing `pymisp-2.4.98/pymisp/exceptions.py` & `pymisp-2.4.99/pymisp/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/docs/tutorial/Search.ipynb` & `pymisp-2.4.99/docs/tutorial/Search.ipynb`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/docs/tutorial/PyMISP Objects.ipynb` & `pymisp-2.4.99/docs/tutorial/PyMISP Objects.ipynb`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/docs/tutorial/Search-NG.ipynb` & `pymisp-2.4.99/docs/tutorial/Search-NG.ipynb`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/docs/tutorial/PyMISP_tutorial.ipynb` & `pymisp-2.4.99/docs/tutorial/PyMISP_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/docs/tutorial/Usage-NG.ipynb` & `pymisp-2.4.99/docs/tutorial/Usage-NG.ipynb`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/docs/Makefile` & `pymisp-2.4.99/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/docs/source/modules.rst` & `pymisp-2.4.99/docs/source/modules.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 
 PyMISP
 ------
 
 .. autoclass:: PyMISP
     :members:
 
+PyMISPExpanded (Python 3.6+ only)
+---------------------------------
+
+.. autoclass:: PyMISPExpanded
+    :members:
+
 MISPAbstract
 ------------
 
 .. autoclass:: AbstractMISP
     :members:
 
 MISPEncode
```

### Comparing `pymisp-2.4.98/docs/source/tools.rst` & `pymisp-2.4.99/docs/source/tools.rst`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/docs/source/README.md` & `pymisp-2.4.99/docs/source/README.md`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/docs/source/conf.py` & `pymisp-2.4.99/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/README.md` & `pymisp-2.4.99/README.md`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/search.py` & `pymisp-2.4.99/examples/search.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/up.py` & `pymisp-2.4.99/examples/up.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/add_feed.py` & `pymisp-2.4.99/examples/add_feed.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/get_csv.py` & `pymisp-2.4.99/examples/get_csv.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/misp2clamav.py` & `pymisp-2.4.99/examples/misp2clamav.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/delete_user.py` & `pymisp-2.4.99/examples/delete_user.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/suricata_search/README.md` & `pymisp-2.4.99/examples/suricata_search/README.md`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/suricata_search/suricata_search.py` & `pymisp-2.4.99/examples/suricata_search/suricata_search.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/add_fail2ban_object.py` & `pymisp-2.4.99/examples/add_fail2ban_object.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/add_named_attribute.py` & `pymisp-2.4.99/examples/add_named_attribute.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/edit_user_json.py` & `pymisp-2.4.99/examples/edit_user_json.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/stats.py` & `pymisp-2.4.99/examples/stats.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/events/create_massive_dummy_events.py` & `pymisp-2.4.99/examples/events/create_massive_dummy_events.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/events/tools.py` & `pymisp-2.4.99/examples/events/tools.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/events/create_dummy_event.py` & `pymisp-2.4.99/examples/events/create_dummy_event.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/events/README.md` & `pymisp-2.4.99/examples/events/README.md`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/vt_to_misp.py` & `pymisp-2.4.99/examples/vt_to_misp.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/suricata.py` & `pymisp-2.4.99/examples/suricata.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/add_email_object.py` & `pymisp-2.4.99/examples/add_email_object.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/yara.py` & `pymisp-2.4.99/examples/yara.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/yara_dump.py` & `pymisp-2.4.99/examples/yara_dump.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/get_network_activity.py` & `pymisp-2.4.99/examples/get_network_activity.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/warninglists.py` & `pymisp-2.4.99/examples/warninglists.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/tagstatistics.py` & `pymisp-2.4.99/examples/tagstatistics.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/addtag.py` & `pymisp-2.4.99/examples/addtag.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/add_generic_object.py` & `pymisp-2.4.99/examples/add_generic_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,17 +16,24 @@
     parser = argparse.ArgumentParser(description='Create a MISP Object selectable by type starting from a dictionary')
     parser.add_argument("-e", "--event", required=True, help="Event ID to update")
     parser.add_argument("-t", "--type", required=True, help="Type of the generic object")
     parser.add_argument("-l", "--attr_list", required=True, help="List of attributes")
     args = parser.parse_args()
 
     pymisp = PyMISP(misp_url, misp_key, misp_verifycert)
+    template = pymisp.get_object_templates_list()
+    if 'response' in template.keys():
+        template = template['response']
     try:
-        template_id = [x['ObjectTemplate']['id'] for x in pymisp.get_object_templates_list() if x['ObjectTemplate']['name'] == args.type][0]
+        template_ids = [x['ObjectTemplate']['id'] for x in template if x['ObjectTemplate']['name'] == args.type]
+        if len(template_ids) > 0:
+            template_id = template_ids[0]
+        else:
+            raise IndexError
     except IndexError:
-        valid_types = ", ".join([x['ObjectTemplate']['name'] for x in pymisp.get_object_templates_list()])
+        valid_types = ", ".join([x['ObjectTemplate']['name'] for x in template])
         print ("Template for type %s not found! Valid types are: %s" % (args.type, valid_types))
         exit()
 
     misp_object = GenericObjectGenerator(args.type.replace("|", "-"))
     misp_object.generate_attributes(json.loads(args.attr_list))
     r = pymisp.add_object(args.event, template_id, misp_object)
```

### Comparing `pymisp-2.4.98/examples/edit_user.py` & `pymisp-2.4.99/examples/edit_user.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/search_sighting.py` & `pymisp-2.4.99/examples/search_sighting.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/sharing_groups.py` & `pymisp-2.4.99/examples/sharing_groups.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/ioc-2-misp/keys.py.sample` & `pymisp-2.4.99/examples/ioc-2-misp/keys.py.sample`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/ioc-2-misp/ioc2misp.py` & `pymisp-2.4.99/examples/ioc-2-misp/ioc2misp.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/ioc-2-misp/taxonomy.csv` & `pymisp-2.4.99/examples/ioc-2-misp/taxonomy.csv`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/et2misp.py` & `pymisp-2.4.99/examples/et2misp.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/copy_list.py` & `pymisp-2.4.99/examples/copy_list.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/del.py` & `pymisp-2.4.99/examples/del.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/graphdb/make_neo4j.py` & `pymisp-2.4.99/examples/graphdb/make_neo4j.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/add_sbsignature.py` & `pymisp-2.4.99/examples/add_sbsignature.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/last.py` & `pymisp-2.4.99/examples/last.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/misp2cef.py` & `pymisp-2.4.99/examples/misp2cef.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/generate_file_objects.py` & `pymisp-2.4.99/examples/generate_file_objects.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/add_file_object.py` & `pymisp-2.4.99/examples/add_file_object.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/get.py` & `pymisp-2.4.99/examples/get.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/sighting.py` & `pymisp-2.4.99/examples/sighting.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/lookup.py` & `pymisp-2.4.99/examples/lookup.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/create_events.py` & `pymisp-2.4.99/examples/create_events.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/get_attachment.py` & `pymisp-2.4.99/examples/get_attachment.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/search_attributes_yara.py` & `pymisp-2.4.99/examples/search_attributes_yara.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/freetext.py` & `pymisp-2.4.99/examples/freetext.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/addtag2.py` & `pymisp-2.4.99/examples/addtag2.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/tags.py` & `pymisp-2.4.99/examples/tags.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/fetch_events_feed.py` & `pymisp-2.4.99/examples/fetch_events_feed.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/add_user_json.py` & `pymisp-2.4.99/examples/add_user_json.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/searchall.py` & `pymisp-2.4.99/examples/searchall.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/situational-awareness/bokeh_tools.py` & `pymisp-2.4.99/examples/situational-awareness/bokeh_tools.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/situational-awareness/pygal_tools.py` & `pymisp-2.4.99/examples/situational-awareness/pygal_tools.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/situational-awareness/tags_to_graphs.py` & `pymisp-2.4.99/examples/situational-awareness/tags_to_graphs.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/situational-awareness/attribute_treemap.py` & `pymisp-2.4.99/examples/situational-awareness/attribute_treemap.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/situational-awareness/tools.py` & `pymisp-2.4.99/examples/situational-awareness/tools.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/situational-awareness/tag_scatter.py` & `pymisp-2.4.99/examples/situational-awareness/tag_scatter.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/situational-awareness/tag_search.py` & `pymisp-2.4.99/examples/situational-awareness/tag_search.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/situational-awareness/style.css` & `pymisp-2.4.99/examples/situational-awareness/style.css`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/situational-awareness/tags_count.py` & `pymisp-2.4.99/examples/situational-awareness/tags_count.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/situational-awareness/README.md` & `pymisp-2.4.99/examples/situational-awareness/README.md`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/situational-awareness/style2.css` & `pymisp-2.4.99/examples/situational-awareness/style2.css`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/situational-awareness/test_attribute_treemap.html` & `pymisp-2.4.99/examples/situational-awareness/test_attribute_treemap.html`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/situational-awareness/date_tools.py` & `pymisp-2.4.99/examples/situational-awareness/date_tools.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/users_list.py` & `pymisp-2.4.99/examples/users_list.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/feed-generator/settings.default.py` & `pymisp-2.4.99/examples/feed-generator/settings.default.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/feed-generator/generate.py` & `pymisp-2.4.99/examples/feed-generator/generate.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/feed-generator/README.md` & `pymisp-2.4.99/examples/feed-generator/README.md`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/openioc_to_misp.py` & `pymisp-2.4.99/examples/openioc_to_misp.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/asciidoc_generator.py` & `pymisp-2.4.99/examples/asciidoc_generator.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/feed-generator-from-redis/settings.default.py` & `pymisp-2.4.99/examples/feed-generator-from-redis/settings.default.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/feed-generator-from-redis/generator.py` & `pymisp-2.4.99/examples/feed-generator-from-redis/generator.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/feed-generator-from-redis/fromredis.py` & `pymisp-2.4.99/examples/feed-generator-from-redis/fromredis.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/feed-generator-from-redis/ObjectConstructor/CowrieMISPObject.py` & `pymisp-2.4.99/examples/feed-generator-from-redis/ObjectConstructor/CowrieMISPObject.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/feed-generator-from-redis/README.md` & `pymisp-2.4.99/examples/feed-generator-from-redis/README.md`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/feed-generator-from-redis/MISPItemToRedis.py` & `pymisp-2.4.99/examples/feed-generator-from-redis/MISPItemToRedis.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/upload.py` & `pymisp-2.4.99/examples/upload.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/examples/add_user.py` & `pymisp-2.4.99/examples/add_user.py`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp.egg-info/SOURCES.txt` & `pymisp-2.4.99/pymisp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymisp-2.4.98/pymisp.egg-info/PKG-INFO` & `pymisp-2.4.99/pymisp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymisp
-Version: 2.4.98
+Version: 2.4.99
 Summary: Python API for MISP.
 Home-page: https://github.com/MISP/PyMISP
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Maintainer: Raphaël Vinot
 License: UNKNOWN
 Project-URL: Source, https://github.com/MISP/PyMISP
```

### Comparing `pymisp-2.4.98/PKG-INFO` & `pymisp-2.4.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymisp
-Version: 2.4.98
+Version: 2.4.99
 Summary: Python API for MISP.
 Home-page: https://github.com/MISP/PyMISP
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Maintainer: Raphaël Vinot
 License: UNKNOWN
 Project-URL: Source, https://github.com/MISP/PyMISP
```

