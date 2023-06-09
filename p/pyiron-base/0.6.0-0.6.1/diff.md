# Comparing `tmp/pyiron_base-0.6.0.tar.gz` & `tmp/pyiron_base-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_base-0.6.0.tar", last modified: Wed Jun  7 22:23:35 2023, max compression
+gzip compressed data, was "pyiron_base-0.6.1.tar", last modified: Fri Jun  9 04:58:54 2023, max compression
```

## Comparing `pyiron_base-0.6.0.tar` & `pyiron_base-0.6.1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.688014 pyiron_base-0.6.0/pyiron_base/
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-07 22:23:35.688014 pyiron_base-0.6.0/pyiron_base/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.672012 pyiron_base-0.6.0/pyiron_base/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/reloadfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.676013 pyiron_base-0.6.0/pyiron_base/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24337 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/database/filetable.py
--rw-r--r--   0 runner    (1001) docker     (123)    45395 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/database/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/database/jobtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/database/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/database/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/database/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.676013 pyiron_base-0.6.0/pyiron_base/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/interfaces/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/interfaces/has_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/interfaces/has_hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/interfaces/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/interfaces/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.676013 pyiron_base-0.6.0/pyiron_base/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27613 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/datamining.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.676013 pyiron_base-0.6.0/pyiron_base/jobs/job/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.680013 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/jobstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.680013 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/queuestatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/runmode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    55900 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/jobtype.py
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    20133 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/runfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.680013 pyiron_base-0.6.0/pyiron_base/jobs/master/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/flexible.py
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    32308 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/submissionstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.680013 pyiron_base-0.6.0/pyiron_base/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.680013 pyiron_base-0.6.0/pyiron_base/project/archiving/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/archiving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/archiving/export_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/archiving/import_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/archiving/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/external.py
--rw-r--r--   0 runner    (1001) docker     (123)    68931 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    12732 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.680013 pyiron_base-0.6.0/pyiron_base/project/update/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/update/pyiron_base_03x_to_04x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/pyiron_base/state/
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/publications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/queue_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    25086 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/pyiron_base/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32693 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/datacontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/filedata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)    38762 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/flattenedstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/has_stored_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/hdfio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/hdfstub.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/inputlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    32625 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/pyiron_base/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/jedi.py
--rw-r--r--   0 runner    (1001) docker     (123)    29090 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/safetar.py
--rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.672012 pyiron_base-0.6.0/pyiron_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-07 22:23:35.000000 pyiron_base-0.6.0/pyiron_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-07 22:23:35.000000 pyiron_base-0.6.0/pyiron_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:23:35.000000 pyiron_base-0.6.0/pyiron_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 22:23:35.000000 pyiron_base-0.6.0/pyiron_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 22:23:35.000000 pyiron_base-0.6.0/pyiron_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 22:23:35.000000 pyiron_base-0.6.0/pyiron_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-07 22:23:35.000000 pyiron_base-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/test_benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/test_benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/test_benchmarks/generic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/test_benchmarks/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/test_benchmarks/generic/test_filehdfio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/tests/test_testwithproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/tests/test_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.671112 pyiron_base-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-09 04:58:54.671112 pyiron_base-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.671112 pyiron_base-0.6.1/pyiron_base/
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-09 04:58:54.671112 pyiron_base-0.6.1/pyiron_base/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.635112 pyiron_base-0.6.1/pyiron_base/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/reloadfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.639112 pyiron_base-0.6.1/pyiron_base/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24337 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/database/filetable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45395 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/database/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/database/jobtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/database/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/database/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/database/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.643112 pyiron_base-0.6.1/pyiron_base/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/interfaces/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/interfaces/has_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/interfaces/has_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/interfaces/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/interfaces/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.643112 pyiron_base-0.6.1/pyiron_base/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27613 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.647112 pyiron_base-0.6.1/pyiron_base/jobs/job/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.647112 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/jobstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.651112 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/queuestatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/runmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55900 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/jobtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20443 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/runfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.655112 pyiron_base-0.6.1/pyiron_base/jobs/master/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/flexible.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32308 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/submissionstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.655112 pyiron_base-0.6.1/pyiron_base/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.659112 pyiron_base-0.6.1/pyiron_base/project/archiving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/archiving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/archiving/export_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/archiving/import_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/archiving/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68931 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12732 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.659112 pyiron_base-0.6.1/pyiron_base/project/update/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/update/pyiron_base_03x_to_04x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.663112 pyiron_base-0.6.1/pyiron_base/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/publications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/queue_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25086 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.667112 pyiron_base-0.6.1/pyiron_base/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32693 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/datacontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/filedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38762 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/flattenedstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/has_stored_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/hdfio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/hdfstub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/inputlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32625 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.667112 pyiron_base-0.6.1/pyiron_base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/jedi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29090 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/safetar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.635112 pyiron_base-0.6.1/pyiron_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-09 04:58:54.000000 pyiron_base-0.6.1/pyiron_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-09 04:58:54.000000 pyiron_base-0.6.1/pyiron_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 04:58:54.000000 pyiron_base-0.6.1/pyiron_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 04:58:54.000000 pyiron_base-0.6.1/pyiron_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-09 04:58:54.000000 pyiron_base-0.6.1/pyiron_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 04:58:54.000000 pyiron_base-0.6.1/pyiron_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-09 04:58:54.671112 pyiron_base-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-09 04:58:54.000000 pyiron_base-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.667112 pyiron_base-0.6.1/test_benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/test_benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.667112 pyiron_base-0.6.1/test_benchmarks/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/test_benchmarks/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/test_benchmarks/generic/test_filehdfio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.671112 pyiron_base-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/tests/test_testwithproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/tests/test_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/versioneer.py
```

### Comparing `pyiron_base-0.6.0/LICENSE` & `pyiron_base-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/PKG-INFO` & `pyiron_base-0.6.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_base
-Version: 0.6.0
+Version: 0.6.1
 Summary: pyiron_base - an integrated development environment (IDE) for computational science.
 Home-page: https://github.com/pyiron/pyiron_base
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyiron_base-0.6.0/README.rst` & `pyiron_base-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/__init__.py` & `pyiron_base-0.6.1/pyiron_base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/_tests.py` & `pyiron_base-0.6.1/pyiron_base/_tests.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/cli/control.py` & `pyiron_base-0.6.1/pyiron_base/cli/control.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/cli/install.py` & `pyiron_base-0.6.1/pyiron_base/cli/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/cli/ls.py` & `pyiron_base-0.6.1/pyiron_base/cli/ls.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/cli/reloadfile.py` & `pyiron_base-0.6.1/pyiron_base/cli/reloadfile.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/cli/rm.py` & `pyiron_base-0.6.1/pyiron_base/cli/rm.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/cli/wrapper.py` & `pyiron_base-0.6.1/pyiron_base/cli/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/database/filetable.py` & `pyiron_base-0.6.1/pyiron_base/database/filetable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/database/generic.py` & `pyiron_base-0.6.1/pyiron_base/database/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/database/jobtable.py` & `pyiron_base-0.6.1/pyiron_base/database/jobtable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/database/manager.py` & `pyiron_base-0.6.1/pyiron_base/database/manager.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/database/performance.py` & `pyiron_base-0.6.1/pyiron_base/database/performance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/database/tables.py` & `pyiron_base-0.6.1/pyiron_base/database/tables.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/interfaces/factory.py` & `pyiron_base-0.6.1/pyiron_base/interfaces/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/interfaces/has_groups.py` & `pyiron_base-0.6.1/pyiron_base/interfaces/has_groups.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/interfaces/has_hdf.py` & `pyiron_base-0.6.1/pyiron_base/interfaces/has_hdf.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/interfaces/object.py` & `pyiron_base-0.6.1/pyiron_base/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/interfaces/singleton.py` & `pyiron_base-0.6.1/pyiron_base/interfaces/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/datamining.py` & `pyiron_base-0.6.1/pyiron_base/jobs/datamining.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/dynamic.py` & `pyiron_base-0.6.1/pyiron_base/jobs/dynamic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/core.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/core.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/extension/executable.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/extension/executable.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,40 +213,37 @@
         self.storage.version = new_path
         self._executable_path = new_path
         if new_path and "mpi" in new_path:
             self.storage.mpi = True
         else:
             self.storage.mpi = False
 
-    def get_input_for_subprocess_call(self, cores, threads):
+    def get_input_for_subprocess_call(self, cores, threads, gpus=None):
         """
         Get the input parameters for the subprocess call to execute the job
 
         Args:
             cores (int): number of cores
             threads (int): number of threads
+            gpus (int/None): number of gpus
 
         Returns:
             str/ list, boolean:  executable and shell variables
         """
         if cores == 1 or not self.mpi:
             executable = self.__str__()
             shell = True
-        elif isinstance(self.executable_path, list):
-            executable = self.executable_path[:] + [
-                str(cores),
-                str(threads),
-            ]
-            shell = False
         else:
-            executable = [
-                self.executable_path,
-                str(cores),
-                str(threads),
-            ]
+            if isinstance(self.executable_path, list):
+                executable = self.executable_path[:]
+            else:
+                executable = [self.executable_path]
+            executable += [str(cores), str(threads)]
+            if gpus is not None:
+                executable += [str(gpus)]
             shell = False
         return executable, shell
 
     def __repr__(self):
         """
         Executable path
         """
```

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/extension/jobstatus.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/extension/jobstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/generic.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,18 +70,26 @@
 
         .. attribute:: new_hdf
 
             defines whether a subjob should be stored in the same HDF5 file or in a new one.
     """
 
     def __init__(
-        self, host=None, queue=None, cores=1, threads=1, run_mode="modal", new_hdf=True
+        self,
+        host=None,
+        queue=None,
+        cores=1,
+        threads=1,
+        gpus=None,
+        run_mode="modal",
+        new_hdf=True,
     ):
         self._cores = cores
         self._threads = threads
+        self._gpus = None
         self._run_time = None
         self._memory_limit = None
         self._host = self._init_host(host=host)
         self._run_mode = Runmode()
 
         self.queue = queue
 
@@ -227,14 +235,22 @@
         return self._threads
 
     @threads.setter
     def threads(self, number_of_threads):
         self._threads = number_of_threads
 
     @property
+    def gpus(self):
+        return self._gpus
+
+    @gpus.setter
+    def gpus(self, number_of_gpus):
+        self._gpus = number_of_gpus
+
+    @property
     def cores(self):
         """
         The number of cores selected for the current simulation
 
         Returns:
             (int): number of cores
         """
@@ -443,14 +459,16 @@
         hdf_dict["new_h5"] = self.new_hdf
         hdf_dict["structure_id"] = self.structure_id
         hdf_dict["run_time"] = self.run_time
         hdf_dict["memory_limit"] = self.memory_limit
         hdf_dict["accept_crash"] = self.accept_crash
         if len(self.additional_arguments) > 0:
             hdf_dict["additional_arguments"] = self.additional_arguments
+        if self._gpus is not None:
+            hdf_dict["accept_crash"] = self._gpus
 
         if group_name is not None:
             with hdf.open(group_name) as hdf_group:
                 hdf_group["server"] = hdf_dict
         else:
             hdf["server"] = hdf_dict
 
@@ -486,14 +504,16 @@
             self._memory_limit = hdf_dict["memory_limit"]
         if "accept_crash" in hdf_dict.keys():
             self._accept_crash = hdf_dict["accept_crash"] == 1
         if "threads" in hdf_dict.keys():
             self._threads = hdf_dict["threads"]
         if "additional_arguments" in hdf_dict.keys():
             self.additional_arguments = hdf_dict["additional_arguments"]
+        if "gpus" in hdf_dict.keys():
+            self._gpus = hdf_dict["accept_crash"]
         self._new_hdf = hdf_dict["new_h5"] == 1
 
     def db_entry(self):
         """
         connect all the info regarding the server into a single word that can be used e.g. as entry in a database
 
         Returns:
```

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/queuestatus.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/queuestatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/runmode.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/runmode.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/factory.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/generic.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/interactive.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/jobtype.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/jobtype.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/path.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/runfunction.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/runfunction.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,23 @@
     elif job.server.run_mode.worker:
         run_job_with_runmode_manually(job=job, _manually_print=True)
     elif job.server.run_mode.modal:
         job.run_static()
     elif job.server.run_mode.srun:
         run_job_with_runmode_srun(job=job)
     elif job.server.run_mode.flux:
-        return run_job_with_runmode_flux(job=job, executor=job.flux_executor)
+        if job.server.gpus is not None:
+            gpus_per_slot = int(job.server.gpus / job.server.cores)
+        else:
+            gpus_per_slot = None
+        return run_job_with_runmode_flux(
+            job=job,
+            executor=job.flux_executor,
+            gpus_per_slot=gpus_per_slot,
+        )
     elif (
         job.server.run_mode.non_modal
         or job.server.run_mode.thread
         or job.server.run_mode.worker
     ):
         run_job_with_runmode_non_modal(job=job)
     elif job.server.run_mode.queue:
@@ -439,15 +447,15 @@
         shell=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         universal_newlines=True,
     )
 
 
-def run_job_with_runmode_flux(job, executor):
+def run_job_with_runmode_flux(job, executor, gpus_per_slot=None):
     if not flux_available:
         raise ModuleNotFoundError(
             "No module named 'flux'. No linux you can install flux via conda."
             + "'conda install -c conda-forge flux'"
         )
     if not state.database.database_is_disabled:
         executable_template = Template(
@@ -476,14 +484,15 @@
         job_name = "pi_" + job.job_name
 
     jobspec = flux.job.JobspecV1.from_batch_command(
         jobname=job_name,
         script=exeuctable_str,
         num_nodes=1,
         cores_per_slot=1,
+        gpus_per_slot=gpus_per_slot,
         num_slots=job.server.cores,
     )
     jobspec.cwd = job.project_hdf5.working_directory
     jobspec.environment = dict(os.environ)
     return executor.submit(jobspec)
 
 
@@ -511,15 +520,15 @@
         "{}, status: {}, run job (modal)".format(job.job_info_str, job.status)
     )
     if job.executable.executable_path == "":
         job.status.aborted = True
         raise ValueError("No executable set!")
     job.status.running = True
     executable, shell = job.executable.get_input_for_subprocess_call(
-        cores=job.server.cores, threads=job.server.threads
+        cores=job.server.cores, threads=job.server.threads, gpus=job.server.gpus
     )
     job_crashed, out = False, None
     try:
         out = subprocess.run(
             executable,
             cwd=job.project_hdf5.working_directory,
             shell=shell,
```

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/template.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/template.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/toolkit.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/util.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/util.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/job/wrapper.py` & `pyiron_base-0.6.1/pyiron_base/jobs/job/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/master/flexible.py` & `pyiron_base-0.6.1/pyiron_base/jobs/master/flexible.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/master/generic.py` & `pyiron_base-0.6.1/pyiron_base/jobs/master/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/master/interactivewrapper.py` & `pyiron_base-0.6.1/pyiron_base/jobs/master/interactivewrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/master/list.py` & `pyiron_base-0.6.1/pyiron_base/jobs/master/list.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/master/parallel.py` & `pyiron_base-0.6.1/pyiron_base/jobs/master/parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/master/serial.py` & `pyiron_base-0.6.1/pyiron_base/jobs/master/serial.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/master/submissionstatus.py` & `pyiron_base-0.6.1/pyiron_base/jobs/master/submissionstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/script.py` & `pyiron_base-0.6.1/pyiron_base/jobs/script.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/jobs/worker.py` & `pyiron_base-0.6.1/pyiron_base/jobs/worker.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/project/archiving/export_archive.py` & `pyiron_base-0.6.1/pyiron_base/project/archiving/export_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/project/archiving/import_archive.py` & `pyiron_base-0.6.1/pyiron_base/project/archiving/import_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/project/data.py` & `pyiron_base-0.6.1/pyiron_base/project/data.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/project/external.py` & `pyiron_base-0.6.1/pyiron_base/project/external.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/project/generic.py` & `pyiron_base-0.6.1/pyiron_base/project/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/project/gui.py` & `pyiron_base-0.6.1/pyiron_base/project/gui.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/project/maintenance.py` & `pyiron_base-0.6.1/pyiron_base/project/maintenance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/project/path.py` & `pyiron_base-0.6.1/pyiron_base/project/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/project/update/pyiron_base_03x_to_04x.py` & `pyiron_base-0.6.1/pyiron_base/project/update/pyiron_base_03x_to_04x.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/state/__init__.py` & `pyiron_base-0.6.1/pyiron_base/state/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/state/install.py` & `pyiron_base-0.6.1/pyiron_base/state/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/state/logger.py` & `pyiron_base-0.6.1/pyiron_base/state/logger.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/state/publications.py` & `pyiron_base-0.6.1/pyiron_base/state/publications.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/state/queue_adapter.py` & `pyiron_base-0.6.1/pyiron_base/state/queue_adapter.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/state/settings.py` & `pyiron_base-0.6.1/pyiron_base/state/settings.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/state/signal.py` & `pyiron_base-0.6.1/pyiron_base/state/signal.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/state/update.py` & `pyiron_base-0.6.1/pyiron_base/state/update.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/storage/datacontainer.py` & `pyiron_base-0.6.1/pyiron_base/storage/datacontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/storage/filedata.py` & `pyiron_base-0.6.1/pyiron_base/storage/filedata.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/storage/fileio.py` & `pyiron_base-0.6.1/pyiron_base/storage/fileio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/storage/flattenedstorage.py` & `pyiron_base-0.6.1/pyiron_base/storage/flattenedstorage.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/storage/has_stored_traits.py` & `pyiron_base-0.6.1/pyiron_base/storage/has_stored_traits.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/storage/hdfio.py` & `pyiron_base-0.6.1/pyiron_base/storage/hdfio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/storage/hdfstub.py` & `pyiron_base-0.6.1/pyiron_base/storage/hdfstub.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/storage/helper_functions.py` & `pyiron_base-0.6.1/pyiron_base/storage/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/storage/parameters.py` & `pyiron_base-0.6.1/pyiron_base/storage/parameters.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/utils/deprecate.py` & `pyiron_base-0.6.1/pyiron_base/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/utils/error.py` & `pyiron_base-0.6.1/pyiron_base/utils/error.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/utils/instance.py` & `pyiron_base-0.6.1/pyiron_base/utils/instance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/utils/jedi.py` & `pyiron_base-0.6.1/pyiron_base/utils/jedi.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/utils/parser.py` & `pyiron_base-0.6.1/pyiron_base/utils/parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/utils/safetar.py` & `pyiron_base-0.6.1/pyiron_base/utils/safetar.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base/utils/units.py` & `pyiron_base-0.6.1/pyiron_base/utils/units.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/pyiron_base.egg-info/PKG-INFO` & `pyiron_base-0.6.1/pyiron_base.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron-base
-Version: 0.6.0
+Version: 0.6.1
 Summary: pyiron_base - an integrated development environment (IDE) for computational science.
 Home-page: https://github.com/pyiron/pyiron_base
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyiron_base-0.6.0/pyiron_base.egg-info/SOURCES.txt` & `pyiron_base-0.6.1/pyiron_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/setup.py` & `pyiron_base-0.6.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,14 @@
                  'Programming Language :: Python :: 3.11'
                 ],
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
     install_requires=[
         'dill>=0.3.6',
-        'future>=0.18.3',
         'gitpython>=3.1.31',
         'h5io>=0.1.7',
         'h5py>=3.8.0',
         'numpy>=1.24.3',
         'pandas>=2.0.2',
         'pathlib2>=2.3.7.post1',
         'pint>=0.22',
```

### Comparing `pyiron_base-0.6.0/test_benchmarks/generic/test_filehdfio.py` & `pyiron_base-0.6.1/test_benchmarks/generic/test_filehdfio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/tests/test_testwithproject.py` & `pyiron_base-0.6.1/tests/test_testwithproject.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/tests/test_toolkit.py` & `pyiron_base-0.6.1/tests/test_toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.0/versioneer.py` & `pyiron_base-0.6.1/versioneer.py`

 * *Files identical despite different names*

