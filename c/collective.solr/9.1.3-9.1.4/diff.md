# Comparing `tmp/collective.solr-9.1.3.tar.gz` & `tmp/collective.solr-9.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.solr-9.1.3.tar", last modified: Tue Apr 11 15:54:21 2023, max compression
+gzip compressed data, was "collective.solr-9.1.4.tar", last modified: Fri Jun  9 18:52:31 2023, max compression
```

## Comparing `collective.solr-9.1.3.tar` & `collective.solr-9.1.4.tar`

### file list

```diff
@@ -1,244 +1,244 @@
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.113390 collective.solr-9.1.3/
--rw-r--r--   0 timo       (501) staff       (20)    36845 2023-04-11 15:54:20.000000 collective.solr-9.1.3/CHANGES.rst
--rw-r--r--   0 timo       (501) staff       (20)      358 2023-04-11 15:54:20.000000 collective.solr-9.1.3/MANIFEST.in
--rw-r--r--   0 timo       (501) staff       (20)    44460 2023-04-11 15:54:21.113064 collective.solr-9.1.3/PKG-INFO
--rw-r--r--   0 timo       (501) staff       (20)     6395 2023-04-11 15:54:20.000000 collective.solr-9.1.3/README.rst
--rw-r--r--   0 timo       (501) staff       (20)     2312 2023-04-11 15:54:20.000000 collective.solr-9.1.3/SOLR-7.rst
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.062764 collective.solr-9.1.3/docs/
--rw-r--r--   0 timo       (501) staff       (20)    15220 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/LICENSE.GPL
--rw-r--r--   0 timo       (501) staff       (20)      668 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/LICENSE.txt
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.063013 collective.solr-9.1.3/docs/_static/
--rw-r--r--   0 timo       (501) staff       (20)       81 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/_static/README.txt
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.063974 collective.solr-9.1.3/docs/base/
--rw-r--r--   0 timo       (501) staff       (20)      652 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/base/dependencies.rst
--rw-r--r--   0 timo       (501) staff       (20)      428 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/base/index.rst
--rw-r--r--   0 timo       (501) staff       (20)     3739 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/base/indexing.rst
--rw-r--r--   0 timo       (501) staff       (20)     5141 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/base/searching.rst
--rw-r--r--   0 timo       (501) staff       (20)     8015 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/conf.py
--rw-r--r--   0 timo       (501) staff       (20)      671 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/contributors.rst
--rw-r--r--   0 timo       (501) staff       (20)      355 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/credits.rst
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.064704 collective.solr-9.1.3/docs/development/
--rw-r--r--   0 timo       (501) staff       (20)     1064 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/development/TODO.rst
--rw-r--r--   0 timo       (501) staff       (20)      578 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/development/index.rst
--rw-r--r--   0 timo       (501) staff       (20)      770 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/development/search_widget.rst
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.066923 collective.solr-9.1.3/docs/features/
--rw-r--r--   0 timo       (501) staff       (20)      962 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/features/atomic_updates.rst
--rw-r--r--   0 timo       (501) staff       (20)     1031 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/features/binary.rst
--rw-r--r--   0 timo       (501) staff       (20)      908 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/features/exclude.rst
--rw-r--r--   0 timo       (501) staff       (20)      539 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/features/facets.rst
--rw-r--r--   0 timo       (501) staff       (20)      749 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/features/highlighting.rst
--rw-r--r--   0 timo       (501) staff       (20)      517 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/features/index.rst
--rw-r--r--   0 timo       (501) staff       (20)     1528 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/features/languages.rst
--rw-r--r--   0 timo       (501) staff       (20)      500 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/features/suggestions.rst
--rw-r--r--   0 timo       (501) staff       (20)      842 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/features/wildcard.rst
--rw-r--r--   0 timo       (501) staff       (20)      827 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/index.rst
--rw-r--r--   0 timo       (501) staff       (20)      531 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/indexes.rst
--rw-r--r--   0 timo       (501) staff       (20)      907 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/introduction.rst
--rw-r--r--   0 timo       (501) staff       (20)      967 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/status.rst
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.069502 collective.solr-9.1.3/docs/usage/
--rw-r--r--   0 timo       (501) staff       (20)     2700 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/usage/autocomplete.rst
--rw-r--r--   0 timo       (501) staff       (20)     2413 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/usage/config.rst
--rw-r--r--   0 timo       (501) staff       (20)      196 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/usage/index.rst
--rw-r--r--   0 timo       (501) staff       (20)     2056 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/usage/install.rst
--rw-r--r--   0 timo       (501) staff       (20)      800 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/usage/java_settings.rst
--rw-r--r--   0 timo       (501) staff       (20)      444 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/usage/maintenance.rst
--rw-r--r--   0 timo       (501) staff       (20)     2446 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/usage/monitoring.rst
--rw-r--r--   0 timo       (501) staff       (20)      195 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/usage/production.rst
--rw-r--r--   0 timo       (501) staff       (20)     1691 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/usage/replication.rst
--rw-r--r--   0 timo       (501) staff       (20)      169 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/usage/setup.rst
--rw-r--r--   0 timo       (501) staff       (20)      166 2023-04-11 15:54:20.000000 collective.solr-9.1.3/docs/usage/solrcloud.rst
--rw-r--r--   0 timo       (501) staff       (20)       38 2023-04-11 15:54:21.113485 collective.solr-9.1.3/setup.cfg
--rw-r--r--   0 timo       (501) staff       (20)     3191 2023-04-11 15:54:20.000000 collective.solr-9.1.3/setup.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.056197 collective.solr-9.1.3/src/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.069736 collective.solr-9.1.3/src/collective/
--rw-r--r--   0 timo       (501) staff       (20)       56 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/__init__.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.079658 collective.solr-9.1.3/src/collective/solr/
--rw-r--r--   0 timo       (501) staff       (20)      195 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/__init__.py
--rw-r--r--   0 timo       (501) staff       (20)      595 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/attributes.py
--rw-r--r--   0 timo       (501) staff       (20)     1203 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/behaviors.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.083046 collective.solr-9.1.3/src/collective/solr/browser/
--rw-r--r--   0 timo       (501) staff       (20)       53 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/__init__.py
--rw-r--r--   0 timo       (501) staff       (20)     2021 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/configure.zcml
--rw-r--r--   0 timo       (501) staff       (20)     1886 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/controlpanel.pt
--rw-r--r--   0 timo       (501) staff       (20)     2473 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/controlpanel.py
--rw-r--r--   0 timo       (501) staff       (20)     2187 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/errors.pt
--rw-r--r--   0 timo       (501) staff       (20)      906 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/errors.py
--rw-r--r--   0 timo       (501) staff       (20)     1149 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/facets.pt
--rw-r--r--   0 timo       (501) staff       (20)     6417 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/facets.py
--rw-r--r--   0 timo       (501) staff       (20)      276 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/hiddenfields.pt
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.083281 collective.solr-9.1.3/src/collective/solr/browser/images/
--rw-r--r--   0 timo       (501) staff       (20)      515 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/images/icon.png
--rw-r--r--   0 timo       (501) staff       (20)      134 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/interfaces.py
--rw-r--r--   0 timo       (501) staff       (20)    15486 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/maintenance.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.083518 collective.solr-9.1.3/src/collective/solr/browser/resources/
--rw-r--r--   0 timo       (501) staff       (20)     1007 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/resources/style.css
--rw-r--r--   0 timo       (501) staff       (20)     1998 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/search.pt
--rw-r--r--   0 timo       (501) staff       (20)     1902 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/searchbox.pt
--rw-r--r--   0 timo       (501) staff       (20)     2748 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/browser/suggest.py
--rw-r--r--   0 timo       (501) staff       (20)     3880 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/commands.py
--rw-r--r--   0 timo       (501) staff       (20)     3606 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/configure.zcml
--rw-r--r--   0 timo       (501) staff       (20)     5433 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/contentlisting.py
--rw-r--r--   0 timo       (501) staff       (20)     4162 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/dispatcher.py
--rw-r--r--   0 timo       (501) staff       (20)      652 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/events.py
--rw-r--r--   0 timo       (501) staff       (20)     1032 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/exceptions.py
--rw-r--r--   0 timo       (501) staff       (20)     3040 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/extender.py
--rw-r--r--   0 timo       (501) staff       (20)      493 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/extender.zcml
--rw-r--r--   0 timo       (501) staff       (20)     3225 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/flare.py
--rw-r--r--   0 timo       (501) staff       (20)    15176 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/indexer.py
--rw-r--r--   0 timo       (501) staff       (20)    18353 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/interfaces.py
--rw-r--r--   0 timo       (501) staff       (20)      172 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/lingua.py
--rw-r--r--   0 timo       (501) staff       (20)      489 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/local.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.084002 collective.solr-9.1.3/src/collective/solr/locales/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.057043 collective.solr-9.1.3/src/collective/solr/locales/de/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.084247 collective.solr-9.1.3/src/collective/solr/locales/de/LC_MESSAGES/
--rw-r--r--   0 timo       (501) staff       (20)    16813 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/locales/de/LC_MESSAGES/solr.po
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.057258 collective.solr-9.1.3/src/collective/solr/locales/en/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.084536 collective.solr-9.1.3/src/collective/solr/locales/en/LC_MESSAGES/
--rw-r--r--   0 timo       (501) staff       (20)    11026 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/locales/en/LC_MESSAGES/solr.po
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.057467 collective.solr-9.1.3/src/collective/solr/locales/it/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.084788 collective.solr-9.1.3/src/collective/solr/locales/it/LC_MESSAGES/
--rw-r--r--   0 timo       (501) staff       (20)    11112 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/locales/it/LC_MESSAGES/solr.po
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.057683 collective.solr-9.1.3/src/collective/solr/locales/nl/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.085037 collective.solr-9.1.3/src/collective/solr/locales/nl/LC_MESSAGES/
--rw-r--r--   0 timo       (501) staff       (20)    11152 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/locales/nl/LC_MESSAGES/solr.po
--rwxr-xr-x   0 timo       (501) staff       (20)      218 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/locales/rebuildPo.sh
--rw-r--r--   0 timo       (501) staff       (20)    11042 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/locales/solr.pot
--rw-r--r--   0 timo       (501) staff       (20)     6756 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/manager.py
--rw-r--r--   0 timo       (501) staff       (20)    11780 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/mangler.py
--rw-r--r--   0 timo       (501) staff       (20)      430 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/meta.zcml
--rw-r--r--   0 timo       (501) staff       (20)     1123 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/monkey.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.090757 collective.solr-9.1.3/src/collective/solr/munin_config/
--rw-r--r--   0 timo       (501) staff       (20)      287 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_admin_file_requests.conf
--rw-r--r--   0 timo       (501) staff       (20)      328 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_avg_extract_requests.conf
--rw-r--r--   0 timo       (501) staff       (20)      310 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_avg_extract_time.conf
--rw-r--r--   0 timo       (501) staff       (20)      299 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_avg_query_requests.conf
--rw-r--r--   0 timo       (501) staff       (20)      281 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_avg_query_time.conf
--rw-r--r--   0 timo       (501) staff       (20)      304 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_avg_update_requests.conf
--rw-r--r--   0 timo       (501) staff       (20)      286 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_avg_update_time.conf
--rw-r--r--   0 timo       (501) staff       (20)      332 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_avg_updatehandler_autocommits.conf
--rw-r--r--   0 timo       (501) staff       (20)      306 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_avg_updatehandler_commits.conf
--rw-r--r--   0 timo       (501) staff       (20)      318 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_avg_updatehandler_optimizes.conf
--rw-r--r--   0 timo       (501) staff       (20)      694 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_cpu.conf
--rw-r--r--   0 timo       (501) staff       (20)      329 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_doccache_hitratio.conf
--rw-r--r--   0 timo       (501) staff       (20)      241 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_doccache_size.conf
--rw-r--r--   0 timo       (501) staff       (20)      231 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_doccount.conf
--rw-r--r--   0 timo       (501) staff       (20)      340 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_filtercache_hitratio.conf
--rw-r--r--   0 timo       (501) staff       (20)      246 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_filtercache_size.conf
--rw-r--r--   0 timo       (501) staff       (20)      280 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_filtercache_warmuptime.conf
--rw-r--r--   0 timo       (501) staff       (20)     1898 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_memory.conf
--rw-r--r--   0 timo       (501) staff       (20)      346 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_querycache_hitratio.conf
--rw-r--r--   0 timo       (501) staff       (20)      254 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_querycache_size.conf
--rw-r--r--   0 timo       (501) staff       (20)      282 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_querycache_warmuptime.conf
--rw-r--r--   0 timo       (501) staff       (20)      269 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_searcher_warmuptime.conf
--rw-r--r--   0 timo       (501) staff       (20)      412 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/munin_config/solr_threads.conf
--rw-r--r--   0 timo       (501) staff       (20)     7449 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/parser.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.058395 collective.solr-9.1.3/src/collective/solr/profiles/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.092921 collective.solr-9.1.3/src/collective/solr/profiles/default/
--rw-r--r--   0 timo       (501) staff       (20)      348 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/actionicons.xml
--rw-r--r--   0 timo       (501) staff       (20)      126 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/browserlayer.xml
--rw-r--r--   0 timo       (501) staff       (20)      512 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/componentregistry.xml
--rw-r--r--   0 timo       (501) staff       (20)      522 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/controlpanel.xml
--rw-r--r--   0 timo       (501) staff       (20)      286 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/cssregistry.xml
--rw-r--r--   0 timo       (501) staff       (20)      157 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/jsregistry.xml
--rw-r--r--   0 timo       (501) staff       (20)      225 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/metadata.xml
--rw-r--r--   0 timo       (501) staff       (20)     1319 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/registry.xml
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.094900 collective.solr-9.1.3/src/collective/solr/profiles/default/types/
--rw-r--r--   0 timo       (501) staff       (20)      253 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/types/Collection.xml
--rw-r--r--   0 timo       (501) staff       (20)      251 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/types/Document.xml
--rw-r--r--   0 timo       (501) staff       (20)      248 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/types/Event.xml
--rw-r--r--   0 timo       (501) staff       (20)      247 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/types/File.xml
--rw-r--r--   0 timo       (501) staff       (20)      249 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/types/Folder.xml
--rw-r--r--   0 timo       (501) staff       (20)      248 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/types/Image.xml
--rw-r--r--   0 timo       (501) staff       (20)      247 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/types/Link.xml
--rw-r--r--   0 timo       (501) staff       (20)      252 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/types/News_Item.xml
--rw-r--r--   0 timo       (501) staff       (20)      512 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/default/types.xml
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.096855 collective.solr-9.1.3/src/collective/solr/profiles/plone4/
--rw-r--r--   0 timo       (501) staff       (20)      348 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/plone4/actionicons.xml
--rw-r--r--   0 timo       (501) staff       (20)      126 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/plone4/browserlayer.xml
--rw-r--r--   0 timo       (501) staff       (20)      512 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/plone4/componentregistry.xml
--rw-r--r--   0 timo       (501) staff       (20)      522 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/plone4/controlpanel.xml
--rw-r--r--   0 timo       (501) staff       (20)      286 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/plone4/cssregistry.xml
--rw-r--r--   0 timo       (501) staff       (20)      157 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/plone4/jsregistry.xml
--rw-r--r--   0 timo       (501) staff       (20)      226 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/plone4/metadata.xml
--rw-r--r--   0 timo       (501) staff       (20)     1013 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/plone4/registry.xml
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.097101 collective.solr-9.1.3/src/collective/solr/profiles/uninstall/
--rw-r--r--   0 timo       (501) staff       (20)      156 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 timo       (501) staff       (20)      804 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/profiles.zcml
--rw-r--r--   0 timo       (501) staff       (20)    10578 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/queryparser.py
--rw-r--r--   0 timo       (501) staff       (20)     9649 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/search.py
--rw-r--r--   0 timo       (501) staff       (20)      496 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/serializer.py
--rw-r--r--   0 timo       (501) staff       (20)     5145 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/setuphandlers.py
--rw-r--r--   0 timo       (501) staff       (20)    15118 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/solr.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.097603 collective.solr-9.1.3/src/collective/solr/static/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.097868 collective.solr-9.1.3/src/collective/solr/static/dist/
--rw-r--r--   0 timo       (501) staff       (20)   529728 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/static/dist/search.min.js
--rw-r--r--   0 timo       (501) staff       (20)     1001 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/static/package.json
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.098980 collective.solr-9.1.3/src/collective/solr/static/src/
--rw-r--r--   0 timo       (501) staff       (20)      660 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/static/src/index.html
--rw-r--r--   0 timo       (501) staff       (20)    17412 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/static/src/index.jsx
--rw-r--r--   0 timo       (501) staff       (20)     1408 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/static/webpack.config.js
--rw-r--r--   0 timo       (501) staff       (20)     9259 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/testing.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.105680 collective.solr-9.1.3/src/collective/solr/tests/
--rw-r--r--   0 timo       (501) staff       (20)       53 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/__init__.py
--rw-r--r--   0 timo       (501) staff       (20)     7045 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/configlet.txt
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.112293 collective.solr-9.1.3/src/collective/solr/tests/data/
--rw-r--r--   0 timo       (501) staff       (20)      240 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/add_request.txt
--rw-r--r--   0 timo       (501) staff       (20)      247 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/add_request_with_boost_values.txt
--rw-r--r--   0 timo       (501) staff       (20)      268 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/add_response.txt
--rw-r--r--   0 timo       (501) staff       (20)      142 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/commit_request.txt
--rw-r--r--   0 timo       (501) staff       (20)      184 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/commit_request_authentication.txt
--rw-r--r--   0 timo       (501) staff       (20)      164 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/commit_request_no_wait_searcher.txt
--rw-r--r--   0 timo       (501) staff       (20)      245 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/commit_response.txt
--rw-r--r--   0 timo       (501) staff       (20)     1935 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/complex_xml_response.txt
--rw-r--r--   0 timo       (501) staff       (20)     1094 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/date_facet_xml_response.txt
--rw-r--r--   0 timo       (501) staff       (20)      163 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/delete_request.txt
--rw-r--r--   0 timo       (501) staff       (20)      244 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/delete_response.txt
--rw-r--r--   0 timo       (501) staff       (20)      185 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/dummy_response.txt
--rw-r--r--   0 timo       (501) staff       (20)      760 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/facet_xml_response.txt
--rw-r--r--   0 timo       (501) staff       (20)       96 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/not_found.txt
--rw-r--r--   0 timo       (501) staff       (20)      145 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/optimize_request.txt
--rw-r--r--   0 timo       (501) staff       (20)     1444 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/plone_schema.xml
--rw-r--r--   0 timo       (501) staff       (20)    17909 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/quirky_response.txt
--rw-r--r--   0 timo       (501) staff       (20)     7259 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/schema.xml
--rw-r--r--   0 timo       (501) staff       (20)      266 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/search_request.txt
--rw-r--r--   0 timo       (501) staff       (20)      266 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/search_request_py2.txt
--rw-r--r--   0 timo       (501) staff       (20)      657 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/search_response.txt
--rw-r--r--   0 timo       (501) staff       (20)      620 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/data/simple_schema.xml
--rw-r--r--   0 timo       (501) staff       (20)     5700 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/errors.txt
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.112557 collective.solr-9.1.3/src/collective/solr/tests/robot/
--rw-r--r--   0 timo       (501) staff       (20)    10691 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/robot/test_search.robot
--rw-r--r--   0 timo       (501) staff       (20)     1173 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_behavior.py
--rw-r--r--   0 timo       (501) staff       (20)     5795 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_browser_suggest.py
--rw-r--r--   0 timo       (501) staff       (20)     1526 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_collections.py
--rw-r--r--   0 timo       (501) staff       (20)     2332 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_conflicts.py
--rw-r--r--   0 timo       (501) staff       (20)     5808 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_contentlisting.py
--rw-r--r--   0 timo       (501) staff       (20)      986 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_doctests.py
--rw-r--r--   0 timo       (501) staff       (20)    16050 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_facethelpers.py
--rw-r--r--   0 timo       (501) staff       (20)    10637 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_facets.py
--rw-r--r--   0 timo       (501) staff       (20)      498 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_flare.py
--rw-r--r--   0 timo       (501) staff       (20)    19335 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_indexer.py
--rw-r--r--   0 timo       (501) staff       (20)     9850 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_integration.py
--rw-r--r--   0 timo       (501) staff       (20)    20927 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_mangler.py
--rw-r--r--   0 timo       (501) staff       (20)     4984 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_multicore.py
--rw-r--r--   0 timo       (501) staff       (20)     9659 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_parser.py
--rw-r--r--   0 timo       (501) staff       (20)    18924 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_query.py
--rw-r--r--   0 timo       (501) staff       (20)      771 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_robot.py
--rw-r--r--   0 timo       (501) staff       (20)    82941 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_server.py
--rw-r--r--   0 timo       (501) staff       (20)     8564 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_solr.py
--rw-r--r--   0 timo       (501) staff       (20)     7754 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_spatial.py
--rw-r--r--   0 timo       (501) staff       (20)      980 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_subjects.py
--rw-r--r--   0 timo       (501) staff       (20)    10138 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/test_utils.py
--rw-r--r--   0 timo       (501) staff       (20)     5360 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/tests/utils.py
--rw-r--r--   0 timo       (501) staff       (20)     1824 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/upgrades.zcml
--rw-r--r--   0 timo       (501) staff       (20)     6788 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/utils.py
--rw-r--r--   0 timo       (501) staff       (20)     1851 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/vocabularies.py
--rw-r--r--   0 timo       (501) staff       (20)      998 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective/solr/zcml.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-04-11 15:54:21.071815 collective.solr-9.1.3/src/collective.solr.egg-info/
--rw-r--r--   0 timo       (501) staff       (20)    44460 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective.solr.egg-info/PKG-INFO
--rw-r--r--   0 timo       (501) staff       (20)     8546 2023-04-11 15:54:21.000000 collective.solr-9.1.3/src/collective.solr.egg-info/SOURCES.txt
--rw-r--r--   0 timo       (501) staff       (20)        1 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective.solr.egg-info/dependency_links.txt
--rw-r--r--   0 timo       (501) staff       (20)      442 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective.solr.egg-info/entry_points.txt
--rw-r--r--   0 timo       (501) staff       (20)       11 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective.solr.egg-info/namespace_packages.txt
--rw-r--r--   0 timo       (501) staff       (20)        1 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective.solr.egg-info/not-zip-safe
--rw-r--r--   0 timo       (501) staff       (20)      518 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective.solr.egg-info/requires.txt
--rw-r--r--   0 timo       (501) staff       (20)       11 2023-04-11 15:54:20.000000 collective.solr-9.1.3/src/collective.solr.egg-info/top_level.txt
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.207638 collective.solr-9.1.4/
+-rw-r--r--   0 timo       (501) staff       (20)    36959 2023-06-09 18:52:30.000000 collective.solr-9.1.4/CHANGES.rst
+-rw-r--r--   0 timo       (501) staff       (20)      358 2023-06-09 18:52:30.000000 collective.solr-9.1.4/MANIFEST.in
+-rw-r--r--   0 timo       (501) staff       (20)    44574 2023-06-09 18:52:31.207473 collective.solr-9.1.4/PKG-INFO
+-rw-r--r--   0 timo       (501) staff       (20)     6395 2023-06-09 18:52:30.000000 collective.solr-9.1.4/README.rst
+-rw-r--r--   0 timo       (501) staff       (20)     2312 2023-06-09 18:52:30.000000 collective.solr-9.1.4/SOLR-7.rst
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.180107 collective.solr-9.1.4/docs/
+-rw-r--r--   0 timo       (501) staff       (20)    15220 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/LICENSE.GPL
+-rw-r--r--   0 timo       (501) staff       (20)      668 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/LICENSE.txt
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.180246 collective.solr-9.1.4/docs/_static/
+-rw-r--r--   0 timo       (501) staff       (20)       81 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/_static/README.txt
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.180762 collective.solr-9.1.4/docs/base/
+-rw-r--r--   0 timo       (501) staff       (20)      652 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/base/dependencies.rst
+-rw-r--r--   0 timo       (501) staff       (20)      428 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/base/index.rst
+-rw-r--r--   0 timo       (501) staff       (20)     3739 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/base/indexing.rst
+-rw-r--r--   0 timo       (501) staff       (20)     5141 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/base/searching.rst
+-rw-r--r--   0 timo       (501) staff       (20)     8015 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/conf.py
+-rw-r--r--   0 timo       (501) staff       (20)      671 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/contributors.rst
+-rw-r--r--   0 timo       (501) staff       (20)      355 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/credits.rst
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.181157 collective.solr-9.1.4/docs/development/
+-rw-r--r--   0 timo       (501) staff       (20)     1064 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/development/TODO.rst
+-rw-r--r--   0 timo       (501) staff       (20)      578 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/development/index.rst
+-rw-r--r--   0 timo       (501) staff       (20)      770 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/development/search_widget.rst
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.182319 collective.solr-9.1.4/docs/features/
+-rw-r--r--   0 timo       (501) staff       (20)      962 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/features/atomic_updates.rst
+-rw-r--r--   0 timo       (501) staff       (20)     1031 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/features/binary.rst
+-rw-r--r--   0 timo       (501) staff       (20)      908 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/features/exclude.rst
+-rw-r--r--   0 timo       (501) staff       (20)      539 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/features/facets.rst
+-rw-r--r--   0 timo       (501) staff       (20)      749 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/features/highlighting.rst
+-rw-r--r--   0 timo       (501) staff       (20)      517 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/features/index.rst
+-rw-r--r--   0 timo       (501) staff       (20)     1528 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/features/languages.rst
+-rw-r--r--   0 timo       (501) staff       (20)      500 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/features/suggestions.rst
+-rw-r--r--   0 timo       (501) staff       (20)      842 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/features/wildcard.rst
+-rw-r--r--   0 timo       (501) staff       (20)      827 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/index.rst
+-rw-r--r--   0 timo       (501) staff       (20)      531 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/indexes.rst
+-rw-r--r--   0 timo       (501) staff       (20)      907 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/introduction.rst
+-rw-r--r--   0 timo       (501) staff       (20)      967 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/status.rst
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.183745 collective.solr-9.1.4/docs/usage/
+-rw-r--r--   0 timo       (501) staff       (20)     2700 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/usage/autocomplete.rst
+-rw-r--r--   0 timo       (501) staff       (20)     2413 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/usage/config.rst
+-rw-r--r--   0 timo       (501) staff       (20)      196 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/usage/index.rst
+-rw-r--r--   0 timo       (501) staff       (20)     2056 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/usage/install.rst
+-rw-r--r--   0 timo       (501) staff       (20)      800 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/usage/java_settings.rst
+-rw-r--r--   0 timo       (501) staff       (20)      444 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/usage/maintenance.rst
+-rw-r--r--   0 timo       (501) staff       (20)     2446 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/usage/monitoring.rst
+-rw-r--r--   0 timo       (501) staff       (20)      195 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/usage/production.rst
+-rw-r--r--   0 timo       (501) staff       (20)     1691 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/usage/replication.rst
+-rw-r--r--   0 timo       (501) staff       (20)      169 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/usage/setup.rst
+-rw-r--r--   0 timo       (501) staff       (20)      166 2023-06-09 18:52:30.000000 collective.solr-9.1.4/docs/usage/solrcloud.rst
+-rw-r--r--   0 timo       (501) staff       (20)       38 2023-06-09 18:52:31.207677 collective.solr-9.1.4/setup.cfg
+-rw-r--r--   0 timo       (501) staff       (20)     3191 2023-06-09 18:52:30.000000 collective.solr-9.1.4/setup.py
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.176086 collective.solr-9.1.4/src/
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.183871 collective.solr-9.1.4/src/collective/
+-rw-r--r--   0 timo       (501) staff       (20)       56 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/__init__.py
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.189988 collective.solr-9.1.4/src/collective/solr/
+-rw-r--r--   0 timo       (501) staff       (20)      195 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/__init__.py
+-rw-r--r--   0 timo       (501) staff       (20)      595 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/attributes.py
+-rw-r--r--   0 timo       (501) staff       (20)     1203 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/behaviors.py
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.191782 collective.solr-9.1.4/src/collective/solr/browser/
+-rw-r--r--   0 timo       (501) staff       (20)       53 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/__init__.py
+-rw-r--r--   0 timo       (501) staff       (20)     2021 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/configure.zcml
+-rw-r--r--   0 timo       (501) staff       (20)     1886 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/controlpanel.pt
+-rw-r--r--   0 timo       (501) staff       (20)     2473 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/controlpanel.py
+-rw-r--r--   0 timo       (501) staff       (20)     2187 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/errors.pt
+-rw-r--r--   0 timo       (501) staff       (20)      906 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/errors.py
+-rw-r--r--   0 timo       (501) staff       (20)     1149 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/facets.pt
+-rw-r--r--   0 timo       (501) staff       (20)     6417 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/facets.py
+-rw-r--r--   0 timo       (501) staff       (20)      276 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/hiddenfields.pt
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.191923 collective.solr-9.1.4/src/collective/solr/browser/images/
+-rw-r--r--   0 timo       (501) staff       (20)      515 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/images/icon.png
+-rw-r--r--   0 timo       (501) staff       (20)      134 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/interfaces.py
+-rw-r--r--   0 timo       (501) staff       (20)    15486 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/maintenance.py
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.192054 collective.solr-9.1.4/src/collective/solr/browser/resources/
+-rw-r--r--   0 timo       (501) staff       (20)     1007 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/resources/style.css
+-rw-r--r--   0 timo       (501) staff       (20)     1998 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/search.pt
+-rw-r--r--   0 timo       (501) staff       (20)     1902 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/searchbox.pt
+-rw-r--r--   0 timo       (501) staff       (20)     2748 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/browser/suggest.py
+-rw-r--r--   0 timo       (501) staff       (20)     3880 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/commands.py
+-rw-r--r--   0 timo       (501) staff       (20)     3606 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/configure.zcml
+-rw-r--r--   0 timo       (501) staff       (20)     5433 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/contentlisting.py
+-rw-r--r--   0 timo       (501) staff       (20)     4162 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/dispatcher.py
+-rw-r--r--   0 timo       (501) staff       (20)      652 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/events.py
+-rw-r--r--   0 timo       (501) staff       (20)     1032 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/exceptions.py
+-rw-r--r--   0 timo       (501) staff       (20)     3040 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/extender.py
+-rw-r--r--   0 timo       (501) staff       (20)      493 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/extender.zcml
+-rw-r--r--   0 timo       (501) staff       (20)     3225 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/flare.py
+-rw-r--r--   0 timo       (501) staff       (20)    15176 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/indexer.py
+-rw-r--r--   0 timo       (501) staff       (20)    18353 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/interfaces.py
+-rw-r--r--   0 timo       (501) staff       (20)      172 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/lingua.py
+-rw-r--r--   0 timo       (501) staff       (20)      489 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/local.py
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.192365 collective.solr-9.1.4/src/collective/solr/locales/
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.176602 collective.solr-9.1.4/src/collective/solr/locales/de/
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.192503 collective.solr-9.1.4/src/collective/solr/locales/de/LC_MESSAGES/
+-rw-r--r--   0 timo       (501) staff       (20)    16813 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/locales/de/LC_MESSAGES/solr.po
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.176751 collective.solr-9.1.4/src/collective/solr/locales/en/
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.192671 collective.solr-9.1.4/src/collective/solr/locales/en/LC_MESSAGES/
+-rw-r--r--   0 timo       (501) staff       (20)    11026 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/locales/en/LC_MESSAGES/solr.po
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.176908 collective.solr-9.1.4/src/collective/solr/locales/it/
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.192821 collective.solr-9.1.4/src/collective/solr/locales/it/LC_MESSAGES/
+-rw-r--r--   0 timo       (501) staff       (20)    11112 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/locales/it/LC_MESSAGES/solr.po
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.177088 collective.solr-9.1.4/src/collective/solr/locales/nl/
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.192993 collective.solr-9.1.4/src/collective/solr/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 timo       (501) staff       (20)    11152 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/locales/nl/LC_MESSAGES/solr.po
+-rwxr-xr-x   0 timo       (501) staff       (20)      218 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/locales/rebuildPo.sh
+-rw-r--r--   0 timo       (501) staff       (20)    11042 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/locales/solr.pot
+-rw-r--r--   0 timo       (501) staff       (20)     6756 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/manager.py
+-rw-r--r--   0 timo       (501) staff       (20)    11780 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/mangler.py
+-rw-r--r--   0 timo       (501) staff       (20)      430 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/meta.zcml
+-rw-r--r--   0 timo       (501) staff       (20)     1123 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/monkey.py
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.198025 collective.solr-9.1.4/src/collective/solr/munin_config/
+-rw-r--r--   0 timo       (501) staff       (20)      287 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_admin_file_requests.conf
+-rw-r--r--   0 timo       (501) staff       (20)      328 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_avg_extract_requests.conf
+-rw-r--r--   0 timo       (501) staff       (20)      310 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_avg_extract_time.conf
+-rw-r--r--   0 timo       (501) staff       (20)      299 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_avg_query_requests.conf
+-rw-r--r--   0 timo       (501) staff       (20)      281 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_avg_query_time.conf
+-rw-r--r--   0 timo       (501) staff       (20)      304 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_avg_update_requests.conf
+-rw-r--r--   0 timo       (501) staff       (20)      286 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_avg_update_time.conf
+-rw-r--r--   0 timo       (501) staff       (20)      332 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_avg_updatehandler_autocommits.conf
+-rw-r--r--   0 timo       (501) staff       (20)      306 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_avg_updatehandler_commits.conf
+-rw-r--r--   0 timo       (501) staff       (20)      318 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_avg_updatehandler_optimizes.conf
+-rw-r--r--   0 timo       (501) staff       (20)      694 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_cpu.conf
+-rw-r--r--   0 timo       (501) staff       (20)      329 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_doccache_hitratio.conf
+-rw-r--r--   0 timo       (501) staff       (20)      241 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_doccache_size.conf
+-rw-r--r--   0 timo       (501) staff       (20)      231 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_doccount.conf
+-rw-r--r--   0 timo       (501) staff       (20)      340 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_filtercache_hitratio.conf
+-rw-r--r--   0 timo       (501) staff       (20)      246 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_filtercache_size.conf
+-rw-r--r--   0 timo       (501) staff       (20)      280 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_filtercache_warmuptime.conf
+-rw-r--r--   0 timo       (501) staff       (20)     1898 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_memory.conf
+-rw-r--r--   0 timo       (501) staff       (20)      346 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_querycache_hitratio.conf
+-rw-r--r--   0 timo       (501) staff       (20)      254 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_querycache_size.conf
+-rw-r--r--   0 timo       (501) staff       (20)      282 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_querycache_warmuptime.conf
+-rw-r--r--   0 timo       (501) staff       (20)      269 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_searcher_warmuptime.conf
+-rw-r--r--   0 timo       (501) staff       (20)      412 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/munin_config/solr_threads.conf
+-rw-r--r--   0 timo       (501) staff       (20)     7449 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/parser.py
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.177636 collective.solr-9.1.4/src/collective/solr/profiles/
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.199045 collective.solr-9.1.4/src/collective/solr/profiles/default/
+-rw-r--r--   0 timo       (501) staff       (20)      348 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/actionicons.xml
+-rw-r--r--   0 timo       (501) staff       (20)      126 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/browserlayer.xml
+-rw-r--r--   0 timo       (501) staff       (20)      512 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/componentregistry.xml
+-rw-r--r--   0 timo       (501) staff       (20)      522 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/controlpanel.xml
+-rw-r--r--   0 timo       (501) staff       (20)      286 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/cssregistry.xml
+-rw-r--r--   0 timo       (501) staff       (20)      157 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/jsregistry.xml
+-rw-r--r--   0 timo       (501) staff       (20)      225 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/metadata.xml
+-rw-r--r--   0 timo       (501) staff       (20)     1319 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/registry.xml
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.199937 collective.solr-9.1.4/src/collective/solr/profiles/default/types/
+-rw-r--r--   0 timo       (501) staff       (20)      253 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/types/Collection.xml
+-rw-r--r--   0 timo       (501) staff       (20)      251 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/types/Document.xml
+-rw-r--r--   0 timo       (501) staff       (20)      248 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/types/Event.xml
+-rw-r--r--   0 timo       (501) staff       (20)      247 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/types/File.xml
+-rw-r--r--   0 timo       (501) staff       (20)      249 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/types/Folder.xml
+-rw-r--r--   0 timo       (501) staff       (20)      248 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/types/Image.xml
+-rw-r--r--   0 timo       (501) staff       (20)      247 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/types/Link.xml
+-rw-r--r--   0 timo       (501) staff       (20)      252 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/types/News_Item.xml
+-rw-r--r--   0 timo       (501) staff       (20)      512 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/default/types.xml
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.200828 collective.solr-9.1.4/src/collective/solr/profiles/plone4/
+-rw-r--r--   0 timo       (501) staff       (20)      348 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/plone4/actionicons.xml
+-rw-r--r--   0 timo       (501) staff       (20)      126 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/plone4/browserlayer.xml
+-rw-r--r--   0 timo       (501) staff       (20)      512 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/plone4/componentregistry.xml
+-rw-r--r--   0 timo       (501) staff       (20)      522 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/plone4/controlpanel.xml
+-rw-r--r--   0 timo       (501) staff       (20)      286 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/plone4/cssregistry.xml
+-rw-r--r--   0 timo       (501) staff       (20)      157 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/plone4/jsregistry.xml
+-rw-r--r--   0 timo       (501) staff       (20)      226 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/plone4/metadata.xml
+-rw-r--r--   0 timo       (501) staff       (20)     1013 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/plone4/registry.xml
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.200947 collective.solr-9.1.4/src/collective/solr/profiles/uninstall/
+-rw-r--r--   0 timo       (501) staff       (20)      156 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 timo       (501) staff       (20)      804 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/profiles.zcml
+-rw-r--r--   0 timo       (501) staff       (20)    10578 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/queryparser.py
+-rw-r--r--   0 timo       (501) staff       (20)     9649 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/search.py
+-rw-r--r--   0 timo       (501) staff       (20)      496 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/serializer.py
+-rw-r--r--   0 timo       (501) staff       (20)     5145 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/setuphandlers.py
+-rw-r--r--   0 timo       (501) staff       (20)    15118 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/solr.py
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.201167 collective.solr-9.1.4/src/collective/solr/static/
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.201276 collective.solr-9.1.4/src/collective/solr/static/dist/
+-rw-r--r--   0 timo       (501) staff       (20)   529728 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/static/dist/search.min.js
+-rw-r--r--   0 timo       (501) staff       (20)     1001 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/static/package.json
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.201747 collective.solr-9.1.4/src/collective/solr/static/src/
+-rw-r--r--   0 timo       (501) staff       (20)      660 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/static/src/index.html
+-rw-r--r--   0 timo       (501) staff       (20)    17412 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/static/src/index.jsx
+-rw-r--r--   0 timo       (501) staff       (20)     1408 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/static/webpack.config.js
+-rw-r--r--   0 timo       (501) staff       (20)     9259 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/testing.py
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.204614 collective.solr-9.1.4/src/collective/solr/tests/
+-rw-r--r--   0 timo       (501) staff       (20)       53 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/__init__.py
+-rw-r--r--   0 timo       (501) staff       (20)     7045 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/configlet.txt
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.207119 collective.solr-9.1.4/src/collective/solr/tests/data/
+-rw-r--r--   0 timo       (501) staff       (20)      240 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/add_request.txt
+-rw-r--r--   0 timo       (501) staff       (20)      247 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/add_request_with_boost_values.txt
+-rw-r--r--   0 timo       (501) staff       (20)      268 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/add_response.txt
+-rw-r--r--   0 timo       (501) staff       (20)      142 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/commit_request.txt
+-rw-r--r--   0 timo       (501) staff       (20)      184 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/commit_request_authentication.txt
+-rw-r--r--   0 timo       (501) staff       (20)      164 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/commit_request_no_wait_searcher.txt
+-rw-r--r--   0 timo       (501) staff       (20)      245 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/commit_response.txt
+-rw-r--r--   0 timo       (501) staff       (20)     1935 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/complex_xml_response.txt
+-rw-r--r--   0 timo       (501) staff       (20)     1094 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/date_facet_xml_response.txt
+-rw-r--r--   0 timo       (501) staff       (20)      163 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/delete_request.txt
+-rw-r--r--   0 timo       (501) staff       (20)      244 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/delete_response.txt
+-rw-r--r--   0 timo       (501) staff       (20)      185 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/dummy_response.txt
+-rw-r--r--   0 timo       (501) staff       (20)      760 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/facet_xml_response.txt
+-rw-r--r--   0 timo       (501) staff       (20)       96 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/not_found.txt
+-rw-r--r--   0 timo       (501) staff       (20)      145 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/optimize_request.txt
+-rw-r--r--   0 timo       (501) staff       (20)     1444 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/plone_schema.xml
+-rw-r--r--   0 timo       (501) staff       (20)    17909 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/quirky_response.txt
+-rw-r--r--   0 timo       (501) staff       (20)     7259 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/schema.xml
+-rw-r--r--   0 timo       (501) staff       (20)      266 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/search_request.txt
+-rw-r--r--   0 timo       (501) staff       (20)      266 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/search_request_py2.txt
+-rw-r--r--   0 timo       (501) staff       (20)      657 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/search_response.txt
+-rw-r--r--   0 timo       (501) staff       (20)      620 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/data/simple_schema.xml
+-rw-r--r--   0 timo       (501) staff       (20)     5700 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/errors.txt
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.207249 collective.solr-9.1.4/src/collective/solr/tests/robot/
+-rw-r--r--   0 timo       (501) staff       (20)    10691 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/robot/test_search.robot
+-rw-r--r--   0 timo       (501) staff       (20)     1173 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_behavior.py
+-rw-r--r--   0 timo       (501) staff       (20)     5795 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_browser_suggest.py
+-rw-r--r--   0 timo       (501) staff       (20)     1526 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_collections.py
+-rw-r--r--   0 timo       (501) staff       (20)     2332 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_conflicts.py
+-rw-r--r--   0 timo       (501) staff       (20)     5808 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_contentlisting.py
+-rw-r--r--   0 timo       (501) staff       (20)      986 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_doctests.py
+-rw-r--r--   0 timo       (501) staff       (20)    16050 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_facethelpers.py
+-rw-r--r--   0 timo       (501) staff       (20)    10637 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_facets.py
+-rw-r--r--   0 timo       (501) staff       (20)      498 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_flare.py
+-rw-r--r--   0 timo       (501) staff       (20)    19335 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_indexer.py
+-rw-r--r--   0 timo       (501) staff       (20)     9850 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_integration.py
+-rw-r--r--   0 timo       (501) staff       (20)    20927 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_mangler.py
+-rw-r--r--   0 timo       (501) staff       (20)     4984 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_multicore.py
+-rw-r--r--   0 timo       (501) staff       (20)     9659 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_parser.py
+-rw-r--r--   0 timo       (501) staff       (20)    19047 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_query.py
+-rw-r--r--   0 timo       (501) staff       (20)      771 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_robot.py
+-rw-r--r--   0 timo       (501) staff       (20)    82941 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_server.py
+-rw-r--r--   0 timo       (501) staff       (20)     8564 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_solr.py
+-rw-r--r--   0 timo       (501) staff       (20)     7754 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_spatial.py
+-rw-r--r--   0 timo       (501) staff       (20)      980 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_subjects.py
+-rw-r--r--   0 timo       (501) staff       (20)    10408 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/test_utils.py
+-rw-r--r--   0 timo       (501) staff       (20)     5360 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/tests/utils.py
+-rw-r--r--   0 timo       (501) staff       (20)     1824 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/upgrades.zcml
+-rw-r--r--   0 timo       (501) staff       (20)     6972 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/utils.py
+-rw-r--r--   0 timo       (501) staff       (20)     1851 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/vocabularies.py
+-rw-r--r--   0 timo       (501) staff       (20)      998 2023-06-09 18:52:30.000000 collective.solr-9.1.4/src/collective/solr/zcml.py
+drwxr-xr-x   0 timo       (501) staff       (20)        0 2023-06-09 18:52:31.185156 collective.solr-9.1.4/src/collective.solr.egg-info/
+-rw-r--r--   0 timo       (501) staff       (20)    44574 2023-06-09 18:52:31.000000 collective.solr-9.1.4/src/collective.solr.egg-info/PKG-INFO
+-rw-r--r--   0 timo       (501) staff       (20)     8546 2023-06-09 18:52:31.000000 collective.solr-9.1.4/src/collective.solr.egg-info/SOURCES.txt
+-rw-r--r--   0 timo       (501) staff       (20)        1 2023-06-09 18:52:31.000000 collective.solr-9.1.4/src/collective.solr.egg-info/dependency_links.txt
+-rw-r--r--   0 timo       (501) staff       (20)      442 2023-06-09 18:52:31.000000 collective.solr-9.1.4/src/collective.solr.egg-info/entry_points.txt
+-rw-r--r--   0 timo       (501) staff       (20)       11 2023-06-09 18:52:31.000000 collective.solr-9.1.4/src/collective.solr.egg-info/namespace_packages.txt
+-rw-r--r--   0 timo       (501) staff       (20)        1 2023-06-09 18:52:31.000000 collective.solr-9.1.4/src/collective.solr.egg-info/not-zip-safe
+-rw-r--r--   0 timo       (501) staff       (20)      518 2023-06-09 18:52:31.000000 collective.solr-9.1.4/src/collective.solr.egg-info/requires.txt
+-rw-r--r--   0 timo       (501) staff       (20)       11 2023-06-09 18:52:31.000000 collective.solr-9.1.4/src/collective.solr.egg-info/top_level.txt
```

### Comparing `collective.solr-9.1.3/CHANGES.rst` & `collective.solr-9.1.4/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+9.1.4 (2023-06-09)
+------------------
+
+- Strip standalone wildcards from the searchable text (#362) [reebalazs]
+
+
 9.1.3 (2023-04-11)
 ------------------
 
 - Fix indexing of set values in multivalue fields [reebalazs]
 
 
 9.1.2 (2023-03-20)
```

### Comparing `collective.solr-9.1.3/PKG-INFO` & `collective.solr-9.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.solr
-Version: 9.1.3
+Version: 9.1.4
 Summary: Solr integration for external indexing and searching.
 Home-page: https://github.com/collective/collective.solr
 Author: Plone Community
 Author-email: plone-developers@lists.sourceforge.net
 Maintainer: Timo Stollenwerk
 Maintainer-email: tisto@plone.org
 License: GPL version 2
@@ -213,14 +213,20 @@
   .. _`Solr`: https://lucene.apache.org/solr/
   .. _`Plone`: https://www.plone.org/
 
 
 Changelog
 =========
 
+9.1.4 (2023-06-09)
+------------------
+
+- Strip standalone wildcards from the searchable text (#362) [reebalazs]
+
+
 9.1.3 (2023-04-11)
 ------------------
 
 - Fix indexing of set values in multivalue fields [reebalazs]
 
 
 9.1.2 (2023-03-20)
```

### Comparing `collective.solr-9.1.3/README.rst` & `collective.solr-9.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/SOLR-7.rst` & `collective.solr-9.1.4/SOLR-7.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/LICENSE.GPL` & `collective.solr-9.1.4/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/LICENSE.txt` & `collective.solr-9.1.4/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/base/dependencies.rst` & `collective.solr-9.1.4/docs/base/dependencies.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/base/indexing.rst` & `collective.solr-9.1.4/docs/base/indexing.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/base/searching.rst` & `collective.solr-9.1.4/docs/base/searching.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/conf.py` & `collective.solr-9.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/contributors.rst` & `collective.solr-9.1.4/docs/contributors.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/development/TODO.rst` & `collective.solr-9.1.4/docs/development/TODO.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/development/index.rst` & `collective.solr-9.1.4/docs/development/index.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/development/search_widget.rst` & `collective.solr-9.1.4/docs/development/search_widget.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/features/atomic_updates.rst` & `collective.solr-9.1.4/docs/features/atomic_updates.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/features/binary.rst` & `collective.solr-9.1.4/docs/features/binary.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/features/exclude.rst` & `collective.solr-9.1.4/docs/features/exclude.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/features/facets.rst` & `collective.solr-9.1.4/docs/features/facets.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/features/highlighting.rst` & `collective.solr-9.1.4/docs/features/highlighting.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/features/index.rst` & `collective.solr-9.1.4/docs/features/index.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/features/languages.rst` & `collective.solr-9.1.4/docs/features/languages.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/features/wildcard.rst` & `collective.solr-9.1.4/docs/features/wildcard.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/index.rst` & `collective.solr-9.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/indexes.rst` & `collective.solr-9.1.4/docs/indexes.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/introduction.rst` & `collective.solr-9.1.4/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/status.rst` & `collective.solr-9.1.4/docs/status.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/usage/autocomplete.rst` & `collective.solr-9.1.4/docs/usage/autocomplete.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/usage/config.rst` & `collective.solr-9.1.4/docs/usage/config.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/usage/install.rst` & `collective.solr-9.1.4/docs/usage/install.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/usage/java_settings.rst` & `collective.solr-9.1.4/docs/usage/java_settings.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/usage/monitoring.rst` & `collective.solr-9.1.4/docs/usage/monitoring.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/docs/usage/replication.rst` & `collective.solr-9.1.4/docs/usage/replication.rst`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/setup.py` & `collective.solr-9.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 from setuptools import find_packages, setup
 
-version = "9.1.3"
+version = "9.1.4"
 
 assert sys.version_info >= (
     3,
     6,
     0,
 ), "collective.solr 9 requires Python 3.8.0+. Please downgrade to collective.solr 8 for Python 2 and Plone 4.3/5.1."
```

### Comparing `collective.solr-9.1.3/src/collective/solr/attributes.py` & `collective.solr-9.1.4/src/collective/solr/attributes.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/behaviors.py` & `collective.solr-9.1.4/src/collective/solr/behaviors.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/browser/configure.zcml` & `collective.solr-9.1.4/src/collective/solr/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/browser/controlpanel.pt` & `collective.solr-9.1.4/src/collective/solr/browser/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/browser/controlpanel.py` & `collective.solr-9.1.4/src/collective/solr/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/browser/errors.pt` & `collective.solr-9.1.4/src/collective/solr/browser/errors.pt`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/browser/errors.py` & `collective.solr-9.1.4/src/collective/solr/browser/errors.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/browser/facets.pt` & `collective.solr-9.1.4/src/collective/solr/browser/facets.pt`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/browser/facets.py` & `collective.solr-9.1.4/src/collective/solr/browser/facets.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/browser/images/icon.png` & `collective.solr-9.1.4/src/collective/solr/browser/images/icon.png`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/browser/maintenance.py` & `collective.solr-9.1.4/src/collective/solr/browser/maintenance.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/browser/resources/style.css` & `collective.solr-9.1.4/src/collective/solr/browser/resources/style.css`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/browser/search.pt` & `collective.solr-9.1.4/src/collective/solr/browser/search.pt`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/browser/searchbox.pt` & `collective.solr-9.1.4/src/collective/solr/browser/searchbox.pt`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/browser/suggest.py` & `collective.solr-9.1.4/src/collective/solr/browser/suggest.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/commands.py` & `collective.solr-9.1.4/src/collective/solr/commands.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/configure.zcml` & `collective.solr-9.1.4/src/collective/solr/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/contentlisting.py` & `collective.solr-9.1.4/src/collective/solr/contentlisting.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/dispatcher.py` & `collective.solr-9.1.4/src/collective/solr/dispatcher.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/events.py` & `collective.solr-9.1.4/src/collective/solr/events.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/exceptions.py` & `collective.solr-9.1.4/src/collective/solr/exceptions.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/extender.py` & `collective.solr-9.1.4/src/collective/solr/extender.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/flare.py` & `collective.solr-9.1.4/src/collective/solr/flare.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/indexer.py` & `collective.solr-9.1.4/src/collective/solr/indexer.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/interfaces.py` & `collective.solr-9.1.4/src/collective/solr/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/locales/de/LC_MESSAGES/solr.po` & `collective.solr-9.1.4/src/collective/solr/locales/de/LC_MESSAGES/solr.po`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/locales/en/LC_MESSAGES/solr.po` & `collective.solr-9.1.4/src/collective/solr/locales/en/LC_MESSAGES/solr.po`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/locales/it/LC_MESSAGES/solr.po` & `collective.solr-9.1.4/src/collective/solr/locales/it/LC_MESSAGES/solr.po`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/locales/nl/LC_MESSAGES/solr.po` & `collective.solr-9.1.4/src/collective/solr/locales/nl/LC_MESSAGES/solr.po`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/locales/solr.pot` & `collective.solr-9.1.4/src/collective/solr/locales/solr.pot`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/manager.py` & `collective.solr-9.1.4/src/collective/solr/manager.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/mangler.py` & `collective.solr-9.1.4/src/collective/solr/mangler.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/monkey.py` & `collective.solr-9.1.4/src/collective/solr/monkey.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/munin_config/solr_cpu.conf` & `collective.solr-9.1.4/src/collective/solr/munin_config/solr_cpu.conf`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/munin_config/solr_memory.conf` & `collective.solr-9.1.4/src/collective/solr/munin_config/solr_memory.conf`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/parser.py` & `collective.solr-9.1.4/src/collective/solr/parser.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/profiles/default/componentregistry.xml` & `collective.solr-9.1.4/src/collective/solr/profiles/default/componentregistry.xml`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/profiles/default/controlpanel.xml` & `collective.solr-9.1.4/src/collective/solr/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/profiles/default/registry.xml` & `collective.solr-9.1.4/src/collective/solr/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/profiles/default/types.xml` & `collective.solr-9.1.4/src/collective/solr/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/profiles/plone4/componentregistry.xml` & `collective.solr-9.1.4/src/collective/solr/profiles/plone4/componentregistry.xml`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/profiles/plone4/controlpanel.xml` & `collective.solr-9.1.4/src/collective/solr/profiles/plone4/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/profiles/plone4/registry.xml` & `collective.solr-9.1.4/src/collective/solr/profiles/plone4/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/profiles.zcml` & `collective.solr-9.1.4/src/collective/solr/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/queryparser.py` & `collective.solr-9.1.4/src/collective/solr/queryparser.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/search.py` & `collective.solr-9.1.4/src/collective/solr/search.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/setuphandlers.py` & `collective.solr-9.1.4/src/collective/solr/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/solr.py` & `collective.solr-9.1.4/src/collective/solr/solr.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/static/dist/search.min.js` & `collective.solr-9.1.4/src/collective/solr/static/dist/search.min.js`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/static/package.json` & `collective.solr-9.1.4/src/collective/solr/static/package.json`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/static/src/index.html` & `collective.solr-9.1.4/src/collective/solr/static/src/index.html`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/static/src/index.jsx` & `collective.solr-9.1.4/src/collective/solr/static/src/index.jsx`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/static/webpack.config.js` & `collective.solr-9.1.4/src/collective/solr/static/webpack.config.js`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/testing.py` & `collective.solr-9.1.4/src/collective/solr/testing.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/configlet.txt` & `collective.solr-9.1.4/src/collective/solr/tests/configlet.txt`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/data/complex_xml_response.txt` & `collective.solr-9.1.4/src/collective/solr/tests/data/complex_xml_response.txt`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/data/date_facet_xml_response.txt` & `collective.solr-9.1.4/src/collective/solr/tests/data/date_facet_xml_response.txt`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/data/facet_xml_response.txt` & `collective.solr-9.1.4/src/collective/solr/tests/data/facet_xml_response.txt`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/data/plone_schema.xml` & `collective.solr-9.1.4/src/collective/solr/tests/data/plone_schema.xml`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/data/quirky_response.txt` & `collective.solr-9.1.4/src/collective/solr/tests/data/quirky_response.txt`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/data/schema.xml` & `collective.solr-9.1.4/src/collective/solr/tests/data/schema.xml`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/data/search_response.txt` & `collective.solr-9.1.4/src/collective/solr/tests/data/search_response.txt`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/data/simple_schema.xml` & `collective.solr-9.1.4/src/collective/solr/tests/data/simple_schema.xml`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/errors.txt` & `collective.solr-9.1.4/src/collective/solr/tests/errors.txt`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/robot/test_search.robot` & `collective.solr-9.1.4/src/collective/solr/tests/robot/test_search.robot`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_behavior.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_behavior.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_browser_suggest.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_browser_suggest.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_collections.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_conflicts.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_conflicts.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_contentlisting.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_contentlisting.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_doctests.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_facethelpers.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_facethelpers.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_facets.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_facets.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_indexer.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_integration.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_mangler.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_mangler.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_multicore.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_multicore.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_parser.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_query.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,17 @@
         self.assertEqual(quote("te*t"), "te*t")
         self.assertEqual(quote("?test"), "test")
         self.assertEqual(quote("*test"), "test")
         self.assertEqual(quote("*test", prefix_wildcard=True), "*test")
         self.assertEqual(quote("?test", prefix_wildcard=True), "?test")
         self.assertEqual(quote("**test", prefix_wildcard=True), "*test")
         self.assertEqual(quote("??test", prefix_wildcard=True), "?test")
+        ## standalone wildcard stripped
+        self.assertEqual(quote("*"), "")
+        self.assertEqual(quote("**"), "")
 
     def testQuotingFuzzySearches(self):
         self.assertEqual(quote("roam~"), "roam~")
         self.assertEqual(quote("roam~0.8"), "roam~0.8")
 
     def testQuotingProximitySearches(self):
         self.assertEqual(quote('"jakarta apache"~10'), '"jakarta apache"~10')
```

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_robot.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_server.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_solr.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_solr.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_spatial.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_spatial.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_subjects.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_subjects.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/test_utils.py` & `collective.solr-9.1.4/src/collective/solr/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,14 +122,19 @@
     def testSplitSimpleSearch(self):
         self.assertEqual(splitSimpleSearch("foo bar"), ["foo", "bar"])
         self.assertEqual(
             splitSimpleSearch('foo "bar foobar" baz'), ["foo", '"bar foobar"', "baz"]
         )
         self.assertRaises(AssertionError, splitSimpleSearch, "foo AND bar")
         self.assertEqual(splitSimpleSearch("foo 42"), ["foo", "42"])
+        # standalone wildcard stripped
+        self.assertEqual(splitSimpleSearch("foo *"), ["foo"])
+        self.assertEqual(splitSimpleSearch("foo **"), ["foo"])
+        # connected wildcard not stripped
+        self.assertEqual(splitSimpleSearch("foo**"), ["foo**"])
 
     def testIsWildCard(self):
         self.assertTrue(isWildCard("foo*"))
         self.assertTrue(isWildCard("fo?"))
         self.assertTrue(isWildCard("fo?o"))
         self.assertTrue(isWildCard("fo*oo"))
         self.assertTrue(isWildCard("fo?o*"))
```

### Comparing `collective.solr-9.1.3/src/collective/solr/tests/utils.py` & `collective.solr-9.1.4/src/collective/solr/tests/utils.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/upgrades.zcml` & `collective.solr-9.1.4/src/collective/solr/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/utils.py` & `collective.solr-9.1.4/src/collective/solr/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,15 +148,20 @@
     if not isSimpleSearch(term):
         raise AssertionError("term is not a simple search")
     parts = term.split('"')
     tokens = []
     for i in range(0, len(parts)):
         if i % 2 == 0:
             # unquoted text
-            words = [word for word in parts[i].split() if word]
+            # note, make sure that both empty words and standalone wildcards are omitted
+            words = [
+                word
+                for word in parts[i].split()
+                if word and word != "*" and word != "**"
+            ]
             tokens.extend(words)
         else:
             # The uneven parts are those inside quotes.
             if parts[i]:
                 tokens.append('"%s"' % parts[i])
     return tokens
```

### Comparing `collective.solr-9.1.3/src/collective/solr/vocabularies.py` & `collective.solr-9.1.4/src/collective/solr/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective/solr/zcml.py` & `collective.solr-9.1.4/src/collective/solr/zcml.py`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective.solr.egg-info/PKG-INFO` & `collective.solr-9.1.4/src/collective.solr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.solr
-Version: 9.1.3
+Version: 9.1.4
 Summary: Solr integration for external indexing and searching.
 Home-page: https://github.com/collective/collective.solr
 Author: Plone Community
 Author-email: plone-developers@lists.sourceforge.net
 Maintainer: Timo Stollenwerk
 Maintainer-email: tisto@plone.org
 License: GPL version 2
@@ -213,14 +213,20 @@
   .. _`Solr`: https://lucene.apache.org/solr/
   .. _`Plone`: https://www.plone.org/
 
 
 Changelog
 =========
 
+9.1.4 (2023-06-09)
+------------------
+
+- Strip standalone wildcards from the searchable text (#362) [reebalazs]
+
+
 9.1.3 (2023-04-11)
 ------------------
 
 - Fix indexing of set values in multivalue fields [reebalazs]
 
 
 9.1.2 (2023-03-20)
```

### Comparing `collective.solr-9.1.3/src/collective.solr.egg-info/SOURCES.txt` & `collective.solr-9.1.4/src/collective.solr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.solr-9.1.3/src/collective.solr.egg-info/requires.txt` & `collective.solr-9.1.4/src/collective.solr.egg-info/requires.txt`

 * *Files identical despite different names*

