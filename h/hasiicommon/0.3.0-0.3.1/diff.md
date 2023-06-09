# Comparing `tmp/hasiicommon-0.3.0.tar.gz` & `tmp/hasiicommon-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hasiicommon-0.3.0.tar", last modified: Fri Jun  9 14:44:48 2023, max compression
+gzip compressed data, was "hasiicommon-0.3.1.tar", last modified: Fri Jun  9 16:05:44 2023, max compression
```

## Comparing `hasiicommon-0.3.0.tar` & `hasiicommon-0.3.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 14:44:48.339727 hasiicommon-0.3.0/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-02-08 21:38:24.000000 hasiicommon-0.3.0/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1973 2023-06-09 14:44:48.339610 hasiicommon-0.3.0/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1608 2023-04-11 01:34:23.000000 hasiicommon-0.3.0/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 14:44:48.328193 hasiicommon-0.3.0/hasiicommon/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:24.000000 hasiicommon-0.3.0/hasiicommon/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.3.0/hasiicommon/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 14:44:48.328966 hasiicommon-0.3.0/hasiicommon/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 15:51:36.000000 hasiicommon-0.3.0/hasiicommon/resources/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 14:44:48.329483 hasiicommon-0.3.0/hasiicommon/resources/images/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2774 2021-02-03 02:11:03.000000 hasiicommon-0.3.0/hasiicommon/resources/images/DefaultPreferences.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 16:13:15.000000 hasiicommon-0.3.0/hasiicommon/resources/images/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 14:44:48.329572 hasiicommon-0.3.0/hasiicommon/resources/images/icons/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-10-17 00:02:24.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 14:44:48.333843 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8370 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxActor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1334 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxArrow.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1642 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxClass.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1186 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewClassDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1330 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewProject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1190 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewSequenceDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1170 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewUseCaseDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8522 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1286 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxOpenFile.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1378 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxRedo.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1098 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAggregation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1078 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAssociation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1102 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipComposition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1122 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipInheritance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1066 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1114 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipRealization.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1482 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxSaveDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1162 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramInstance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1162 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramMessage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1046 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxText.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1402 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxUndo.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8346 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxUseCase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1382 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomIn.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1366 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomOut.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 14:44:48.337866 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1190 2021-01-24 17:56:38.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxActor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1522 2021-01-24 17:56:39.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxArrow.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1742 2021-01-24 17:56:39.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxClass.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9478 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewClassDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3210 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewProject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9878 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewSequenceDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9486 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewUseCaseDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      962 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2410 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxOpenFile.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2770 2021-01-24 17:56:44.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxRedo.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8570 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAggregation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8226 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAssociation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      714 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipComposition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8446 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipInheritance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8254 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8446 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipRealization.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2954 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxSaveDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8846 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramInstance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8582 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramMessage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1666 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxText.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2762 2021-01-24 17:56:54.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxUndo.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1662 2021-01-24 17:56:55.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxUseCase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3198 2021-01-25 02:00:22.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomIn.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3166 2021-01-24 17:56:56.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomOut.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2021-01-19 21:01:31.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.3.0/hasiicommon/resources/images/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.3.0/hasiicommon/resources/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 14:44:48.338287 hasiicommon-0.3.0/hasiicommon/ui/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      739 2023-03-26 22:09:23.000000 hasiicommon-0.3.0/hasiicommon/ui/UnitTestBaseW.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:39.000000 hasiicommon-0.3.0/hasiicommon/ui/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.3.0/hasiicommon/ui/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 14:44:48.339472 hasiicommon-0.3.0/hasiicommon/ui/widgets/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2384 2023-03-26 21:09:16.000000 hasiicommon-0.3.0/hasiicommon/ui/widgets/DimensionsControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      224 2022-11-09 03:57:30.000000 hasiicommon-0.3.0/hasiicommon/ui/widgets/DirectionEnum.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4602 2023-02-09 02:19:53.000000 hasiicommon-0.3.0/hasiicommon/ui/widgets/DualSpinnerControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2306 2023-03-26 21:09:22.000000 hasiicommon-0.3.0/hasiicommon/ui/widgets/PositionControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:58.000000 hasiicommon-0.3.0/hasiicommon/ui/widgets/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.3.0/hasiicommon/ui/widgets/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 14:44:48.328764 hasiicommon-0.3.0/hasiicommon.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1973 2023-06-09 14:44:48.000000 hasiicommon-0.3.0/hasiicommon.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4526 2023-06-09 14:44:48.000000 hasiicommon-0.3.0/hasiicommon.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-09 14:44:48.000000 hasiicommon-0.3.0/hasiicommon.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       54 2023-06-09 14:44:48.000000 hasiicommon-0.3.0/hasiicommon.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-06-09 14:44:48.000000 hasiicommon-0.3.0/hasiicommon.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-09 14:44:48.339758 hasiicommon-0.3.0/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1557 2023-06-09 03:00:17.000000 hasiicommon-0.3.0/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 16:05:44.630529 hasiicommon-0.3.1/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-02-08 21:38:24.000000 hasiicommon-0.3.1/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1973 2023-06-09 16:05:44.630409 hasiicommon-0.3.1/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1608 2023-04-11 01:34:23.000000 hasiicommon-0.3.1/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 16:05:44.621689 hasiicommon-0.3.1/hasiicommon/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:24.000000 hasiicommon-0.3.1/hasiicommon/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.3.1/hasiicommon/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 16:05:44.622638 hasiicommon-0.3.1/hasiicommon/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 15:51:36.000000 hasiicommon-0.3.1/hasiicommon/resources/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 16:05:44.622939 hasiicommon-0.3.1/hasiicommon/resources/images/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2774 2021-02-03 02:11:03.000000 hasiicommon-0.3.1/hasiicommon/resources/images/DefaultPreferences.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 16:13:15.000000 hasiicommon-0.3.1/hasiicommon/resources/images/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 16:05:44.623027 hasiicommon-0.3.1/hasiicommon/resources/images/icons/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-10-17 00:02:24.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 16:05:44.626235 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8370 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxActor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1334 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxArrow.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1642 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxClass.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1186 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewClassDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1330 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewProject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1190 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewSequenceDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1170 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewUseCaseDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8522 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1286 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxOpenFile.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1378 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRedo.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1098 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAggregation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1078 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAssociation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1102 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipComposition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1122 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipInheritance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1066 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1114 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipRealization.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1482 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxSaveDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1162 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramInstance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1162 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramMessage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1046 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxText.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1402 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxUndo.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8346 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxUseCase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1382 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomIn.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1366 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomOut.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 16:05:44.629298 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1190 2021-01-24 17:56:38.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxActor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1522 2021-01-24 17:56:39.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxArrow.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1742 2021-01-24 17:56:39.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxClass.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9478 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewClassDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3210 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewProject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9878 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewSequenceDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9486 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewUseCaseDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      962 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2410 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxOpenFile.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2770 2021-01-24 17:56:44.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRedo.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8570 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAggregation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8226 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAssociation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      714 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipComposition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8446 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipInheritance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8254 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8446 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipRealization.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2954 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxSaveDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8846 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramInstance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8582 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramMessage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1666 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxText.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2762 2021-01-24 17:56:54.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxUndo.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1662 2021-01-24 17:56:55.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxUseCase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3198 2021-01-25 02:00:22.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomIn.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3166 2021-01-24 17:56:56.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomOut.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2021-01-19 21:01:31.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.3.1/hasiicommon/resources/images/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.3.1/hasiicommon/resources/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 16:05:44.629583 hasiicommon-0.3.1/hasiicommon/ui/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      739 2023-03-26 22:09:23.000000 hasiicommon-0.3.1/hasiicommon/ui/UnitTestBaseW.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:39.000000 hasiicommon-0.3.1/hasiicommon/ui/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.3.1/hasiicommon/ui/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 16:05:44.630260 hasiicommon-0.3.1/hasiicommon/ui/widgets/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2384 2023-03-26 21:09:16.000000 hasiicommon-0.3.1/hasiicommon/ui/widgets/DimensionsControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      224 2022-11-09 03:57:30.000000 hasiicommon-0.3.1/hasiicommon/ui/widgets/DirectionEnum.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4602 2023-02-09 02:19:53.000000 hasiicommon-0.3.1/hasiicommon/ui/widgets/DualSpinnerControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2306 2023-03-26 21:09:22.000000 hasiicommon-0.3.1/hasiicommon/ui/widgets/PositionControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:58.000000 hasiicommon-0.3.1/hasiicommon/ui/widgets/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.3.1/hasiicommon/ui/widgets/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 16:05:44.622372 hasiicommon-0.3.1/hasiicommon.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1973 2023-06-09 16:05:44.000000 hasiicommon-0.3.1/hasiicommon.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4526 2023-06-09 16:05:44.000000 hasiicommon-0.3.1/hasiicommon.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-09 16:05:44.000000 hasiicommon-0.3.1/hasiicommon.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       54 2023-06-09 16:05:44.000000 hasiicommon-0.3.1/hasiicommon.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-06-09 16:05:44.000000 hasiicommon-0.3.1/hasiicommon.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-09 16:05:44.630566 hasiicommon-0.3.1/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1557 2023-06-09 16:03:48.000000 hasiicommon-0.3.1/setup.py
```

### Comparing `hasiicommon-0.3.0/LICENSE` & `hasiicommon-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/PKG-INFO` & `hasiicommon-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hasiicommon
-Version: 0.3.0
+Version: 0.3.1
 Summary: Humberto`s Common Stuff
 Home-page: https://github.com/hasii2011/hasiicommon
 Author: Humberto A. Sanchez II
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hasiicommon Version: 0.3.0 Summary: Humberto`s
+Metadata-Version: 2.1 Name: hasiicommon Version: 0.3.1 Summary: Humberto`s
 Common Stuff Home-page: https://github.com/hasii2011/hasiicommon Author:
 Humberto A. Sanchez II Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II Maintainer-email:
 humberto.a.sanchez.ii@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./developer/agpl-license-web-badge-version-2-256x48.png]
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/hasiicommon/
 tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/
```

### Comparing `hasiicommon-0.3.0/README.md` & `hasiicommon-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/DefaultPreferences.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/DefaultPreferences.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxActor.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxActor.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxArrow.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxArrow.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxClass.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxClass.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewClassDiagram.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewClassDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewProject.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewProject.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewSequenceDiagram.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewSequenceDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewUseCaseDiagram.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewUseCaseDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxNote.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNote.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxOpenFile.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxOpenFile.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxRedo.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRedo.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAggregation.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAggregation.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAssociation.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAssociation.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipComposition.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipComposition.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipInheritance.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipInheritance.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipNote.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipNote.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipRealization.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipRealization.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxSaveDiagram.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxSaveDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramInstance.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramInstance.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramMessage.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramMessage.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxText.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxText.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxUndo.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxUndo.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxUseCase.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxUseCase.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomIn.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomIn.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomOut.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomOut.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxActor.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxActor.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxArrow.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxArrow.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxClass.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxClass.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewClassDiagram.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewClassDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewProject.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewProject.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewSequenceDiagram.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewSequenceDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewUseCaseDiagram.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewUseCaseDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxNote.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNote.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxOpenFile.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxOpenFile.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxRedo.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRedo.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAggregation.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAggregation.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAssociation.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAssociation.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipComposition.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipComposition.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipInheritance.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipInheritance.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipNote.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipNote.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipRealization.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipRealization.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxSaveDiagram.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxSaveDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramInstance.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramInstance.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramMessage.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramMessage.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxText.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxText.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxUndo.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxUndo.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxUseCase.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxUseCase.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomIn.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomIn.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomOut.py` & `hasiicommon-0.3.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomOut.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/ui/UnitTestBaseW.py` & `hasiicommon-0.3.1/hasiicommon/ui/UnitTestBaseW.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/ui/widgets/DimensionsControl.py` & `hasiicommon-0.3.1/hasiicommon/ui/widgets/DimensionsControl.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/ui/widgets/DualSpinnerControl.py` & `hasiicommon-0.3.1/hasiicommon/ui/widgets/DualSpinnerControl.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon/ui/widgets/PositionControl.py` & `hasiicommon-0.3.1/hasiicommon/ui/widgets/PositionControl.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/hasiicommon.egg-info/PKG-INFO` & `hasiicommon-0.3.1/hasiicommon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hasiicommon
-Version: 0.3.0
+Version: 0.3.1
 Summary: Humberto`s Common Stuff
 Home-page: https://github.com/hasii2011/hasiicommon
 Author: Humberto A. Sanchez II
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hasiicommon Version: 0.3.0 Summary: Humberto`s
+Metadata-Version: 2.1 Name: hasiicommon Version: 0.3.1 Summary: Humberto`s
 Common Stuff Home-page: https://github.com/hasii2011/hasiicommon Author:
 Humberto A. Sanchez II Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II Maintainer-email:
 humberto.a.sanchez.ii@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./developer/agpl-license-web-badge-version-2-256x48.png]
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/hasiicommon/
 tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/
```

### Comparing `hasiicommon-0.3.0/hasiicommon.egg-info/SOURCES.txt` & `hasiicommon-0.3.1/hasiicommon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.3.0/setup.py` & `hasiicommon-0.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
 
 setup(
     name="hasiicommon",
-    version="0.3.0",
+    version="0.3.1",
     author='Humberto A. Sanchez II',
     author_email='Humberto.A.Sanchez.II@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='Humberto`s Common Stuff',
     long_description=README,
     long_description_content_type="text/markdown",
@@ -36,9 +36,9 @@
         'hasiicommon.resources',
         'hasiicommon.resources.images',
         'hasiicommon.resources.images.icons',
         'hasiicommon.resources.images.icons.embedded16',
         'hasiicommon.resources.images.icons.embedded32',
         'hasiicommon.ui', 'hasiicommon.ui.widgets'
     ],
-    install_requires=['hasiihelper==0.2.0', 'Deprecated~=1.2.13', 'wxPython~=4.2.1'],
+    install_requires=['hasiihelper==0.2.1', 'Deprecated~=1.2.14', 'wxPython~=4.2.1'],
 )
```

