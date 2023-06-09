# Comparing `tmp/ogl-0.70.50.tar.gz` & `tmp/ogl-0.70.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogl-0.70.50.tar", last modified: Fri Jun  9 20:27:39 2023, max compression
+gzip compressed data, was "ogl-0.70.51.tar", last modified: Fri Jun  9 21:01:42 2023, max compression
```

## Comparing `ogl-0.70.50.tar` & `ogl-0.70.51.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 20:27:39.789625 ogl-0.70.50/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 23:19:08.000000 ogl-0.70.50/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-06-09 20:27:39.789489 ogl-0.70.50/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1999 2023-04-12 19:50:00.000000 ogl-0.70.50/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 20:27:39.780038 ogl-0.70.50/miniogl/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5038 2023-03-22 20:23:56.000000 ogl-0.70.50/miniogl/AnchorPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1022 2023-02-21 19:19:18.000000 ogl-0.70.50/miniogl/AttachmentSide.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3100 2023-06-09 19:44:45.000000 ogl-0.70.50/miniogl/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       87 2022-05-18 20:30:08.000000 ogl-0.70.50/miniogl/Constants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1365 2022-05-18 20:30:08.000000 ogl-0.70.50/miniogl/ControlPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3743 2023-05-15 20:23:59.000000 ogl-0.70.50/miniogl/Diagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    40698 2023-05-16 01:00:55.000000 ogl-0.70.50/miniogl/DiagramFrame.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4713 2023-03-22 20:23:56.000000 ogl-0.70.50/miniogl/DlgDebugDiagramFrame.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1669 2022-05-18 20:30:08.000000 ogl-0.70.50/miniogl/LinePoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13202 2023-03-22 20:23:56.000000 ogl-0.70.50/miniogl/LineShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3594 2023-02-21 21:15:44.000000 ogl-0.70.50/miniogl/LollipopLine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1747 2023-02-11 19:23:36.000000 ogl-0.70.50/miniogl/MiniOglColorEnum.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1684 2022-05-18 20:30:08.000000 ogl-0.70.50/miniogl/MiniOglPenStyle.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      170 2022-05-18 20:30:08.000000 ogl-0.70.50/miniogl/MiniOglUtils.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2771 2022-05-18 20:30:08.000000 ogl-0.70.50/miniogl/PointShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10767 2023-05-16 01:00:24.000000 ogl-0.70.50/miniogl/RectangleShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1076 2022-05-18 20:30:08.000000 ogl-0.70.50/miniogl/RectangleShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4772 2022-11-13 14:57:11.000000 ogl-0.70.50/miniogl/RotatableShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2156 2023-03-22 20:23:56.000000 ogl-0.70.50/miniogl/SelectAnchorPoint.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21669 2023-05-15 20:23:15.000000 ogl-0.70.50/miniogl/Shape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2336 2023-05-16 16:52:43.000000 ogl-0.70.50/miniogl/ShapeEventHandler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1632 2023-03-22 20:23:56.000000 ogl-0.70.50/miniogl/ShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1452 2023-05-16 00:57:28.000000 ogl-0.70.50/miniogl/SizerShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7511 2023-03-25 21:42:57.000000 ogl-0.70.50/miniogl/TextShape.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      649 2022-05-18 20:30:08.000000 ogl-0.70.50/miniogl/TextShapeModel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5650 2022-11-13 14:38:42.000000 ogl-0.70.50/miniogl/VShapes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.50/miniogl/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.50/miniogl/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 20:27:39.783883 ogl-0.70.50/ogl/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      126 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/IllegalOperationException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4646 2023-05-16 01:11:07.000000 ogl-0.70.50/ogl/OglActor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1463 2022-11-01 13:15:29.000000 ogl-0.70.50/ogl/OglAggregation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12912 2023-03-25 20:34:07.000000 ogl-0.70.50/ogl/OglAssociation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      328 2023-06-09 20:08:20.000000 ogl-0.70.50/ogl/OglAssociationLabel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    20392 2023-05-16 00:59:29.000000 ogl-0.70.50/ogl/OglClass.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1409 2023-03-22 20:23:56.000000 ogl-0.70.50/ogl/OglComposition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      668 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/OglConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      717 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/OglDimensions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1460 2023-01-31 22:21:10.000000 ogl-0.70.50/ogl/OglInheritance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3541 2023-03-31 00:59:54.000000 ogl-0.70.50/ogl/OglInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6199 2023-02-21 19:19:18.000000 ogl-0.70.50/ogl/OglInterface2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15577 2023-03-22 20:23:56.000000 ogl-0.70.50/ogl/OglLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3115 2023-03-26 22:27:03.000000 ogl-0.70.50/ogl/OglLinkFactory.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2693 2022-08-28 23:27:21.000000 ogl-0.70.50/ogl/OglNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1180 2023-02-19 02:02:00.000000 ogl-0.70.50/ogl/OglNoteLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5529 2023-05-16 16:51:16.000000 ogl-0.70.50/ogl/OglObject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      474 2023-06-09 20:04:54.000000 ogl-0.70.50/ogl/OglPosition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8683 2023-05-15 20:22:45.000000 ogl-0.70.50/ogl/OglText.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      226 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/OglTextFontFamily.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2197 2022-06-08 20:23:03.000000 ogl-0.70.50/ogl/OglUseCase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4349 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/OglUtils.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       37 2023-05-14 21:20:56.000000 ogl-0.70.50/ogl/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       24 2023-06-09 15:00:09.000000 ogl-0.70.50/ogl/_version.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 20:27:39.785521 ogl-0.70.50/ogl/events/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      543 2023-01-15 21:02:48.000000 ogl-0.70.50/ogl/events/IOglEventEngine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/events/InvalidKeywordException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4566 2023-01-15 21:06:24.000000 ogl-0.70.50/ogl/events/OglEventEngine.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      780 2022-11-14 22:52:55.000000 ogl-0.70.50/ogl/events/OglEvents.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      239 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/events/ShapeSelectedEventData.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/events/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.50/ogl/events/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 20:27:39.786135 ogl-0.70.50/ogl/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21282 2023-05-14 20:59:24.000000 ogl-0.70.50/ogl/preferences/OglPreferences.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.50/ogl/preferences/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.50/ogl/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 20:27:39.786240 ogl-0.70.50/ogl/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/resources/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 20:27:39.786869 ogl-0.70.50/ogl/resources/img/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1350 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/resources/img/Display.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1702 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/resources/img/DoNotDisplay.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2238 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/resources/img/UnSpecified.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/resources/img/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.50/ogl/resources/img/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 20:27:39.787276 ogl-0.70.50/ogl/resources/img/textdetails/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1543 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/resources/img/textdetails/DecreaseTextSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1575 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/resources/img/textdetails/IncreaseTextSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/resources/img/textdetails/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.50/ogl/resources/img/textdetails/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 20:27:39.787950 ogl-0.70.50/ogl/sd/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      904 2023-05-12 20:37:54.000000 ogl-0.70.50/ogl/sd/OglInstanceName.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6876 2023-05-16 01:17:51.000000 ogl-0.70.50/ogl/sd/OglSDInstance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6874 2023-05-14 21:08:57.000000 ogl-0.70.50/ogl/sd/OglSDMessage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.50/ogl/sd/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.50/ogl/sd/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 20:27:39.788503 ogl-0.70.50/ogl/ui/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      657 2023-05-16 00:59:48.000000 ogl-0.70.50/ogl/ui/BaseOglPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3967 2023-02-19 20:46:44.000000 ogl-0.70.50/ogl/ui/DefaultValuesPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12232 2023-02-19 22:08:38.000000 ogl-0.70.50/ogl/ui/DiagramPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 14:43:49.000000 ogl-0.70.50/ogl/ui/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.50/ogl/ui/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 20:27:39.789318 ogl-0.70.50/ogl/ui/valuecontrols/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2279 2023-02-11 21:29:46.000000 ogl-0.70.50/ogl/ui/valuecontrols/AssociationAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5065 2023-02-11 20:04:09.000000 ogl-0.70.50/ogl/ui/valuecontrols/ClassAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2987 2023-02-11 20:20:38.000000 ogl-0.70.50/ogl/ui/valuecontrols/DefaultNamesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1943 2023-03-26 22:24:15.000000 ogl-0.70.50/ogl/ui/valuecontrols/NoteAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2686 2023-03-26 22:24:31.000000 ogl-0.70.50/ogl/ui/valuecontrols/SDAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5284 2023-05-14 22:17:09.000000 ogl-0.70.50/ogl/ui/valuecontrols/TextAttributesControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 15:30:26.000000 ogl-0.70.50/ogl/ui/valuecontrols/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 20:27:39.784402 ogl-0.70.50/ogl.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-06-09 20:27:39.000000 ogl-0.70.50/ogl.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2516 2023-06-09 20:27:39.000000 ogl-0.70.50/ogl.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-09 20:27:39.000000 ogl-0.70.50/ogl.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       90 2023-06-09 20:27:39.000000 ogl-0.70.50/ogl.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-06-09 20:27:39.000000 ogl-0.70.50/ogl.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-09 20:27:39.789659 ogl-0.70.50/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     1565 2023-06-09 16:48:31.000000 ogl-0.70.50/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:01:42.138648 ogl-0.70.51/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 23:19:08.000000 ogl-0.70.51/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-06-09 21:01:42.138525 ogl-0.70.51/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1999 2023-04-12 19:50:00.000000 ogl-0.70.51/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:01:42.125048 ogl-0.70.51/miniogl/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5038 2023-03-22 20:23:56.000000 ogl-0.70.51/miniogl/AnchorPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1022 2023-02-21 19:19:18.000000 ogl-0.70.51/miniogl/AttachmentSide.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3100 2023-06-09 19:44:45.000000 ogl-0.70.51/miniogl/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       87 2022-05-18 20:30:08.000000 ogl-0.70.51/miniogl/Constants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1365 2022-05-18 20:30:08.000000 ogl-0.70.51/miniogl/ControlPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3743 2023-05-15 20:23:59.000000 ogl-0.70.51/miniogl/Diagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    40698 2023-05-16 01:00:55.000000 ogl-0.70.51/miniogl/DiagramFrame.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4713 2023-03-22 20:23:56.000000 ogl-0.70.51/miniogl/DlgDebugDiagramFrame.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1669 2022-05-18 20:30:08.000000 ogl-0.70.51/miniogl/LinePoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13202 2023-03-22 20:23:56.000000 ogl-0.70.51/miniogl/LineShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3594 2023-02-21 21:15:44.000000 ogl-0.70.51/miniogl/LollipopLine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1747 2023-02-11 19:23:36.000000 ogl-0.70.51/miniogl/MiniOglColorEnum.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1684 2022-05-18 20:30:08.000000 ogl-0.70.51/miniogl/MiniOglPenStyle.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      170 2022-05-18 20:30:08.000000 ogl-0.70.51/miniogl/MiniOglUtils.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2771 2022-05-18 20:30:08.000000 ogl-0.70.51/miniogl/PointShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10767 2023-05-16 01:00:24.000000 ogl-0.70.51/miniogl/RectangleShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1076 2022-05-18 20:30:08.000000 ogl-0.70.51/miniogl/RectangleShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4772 2022-11-13 14:57:11.000000 ogl-0.70.51/miniogl/RotatableShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2156 2023-03-22 20:23:56.000000 ogl-0.70.51/miniogl/SelectAnchorPoint.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21669 2023-05-15 20:23:15.000000 ogl-0.70.51/miniogl/Shape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2336 2023-05-16 16:52:43.000000 ogl-0.70.51/miniogl/ShapeEventHandler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1632 2023-03-22 20:23:56.000000 ogl-0.70.51/miniogl/ShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1452 2023-05-16 00:57:28.000000 ogl-0.70.51/miniogl/SizerShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7511 2023-03-25 21:42:57.000000 ogl-0.70.51/miniogl/TextShape.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      649 2022-05-18 20:30:08.000000 ogl-0.70.51/miniogl/TextShapeModel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5650 2022-11-13 14:38:42.000000 ogl-0.70.51/miniogl/VShapes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.51/miniogl/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.51/miniogl/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:01:42.130631 ogl-0.70.51/ogl/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      126 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/IllegalOperationException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4646 2023-05-16 01:11:07.000000 ogl-0.70.51/ogl/OglActor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1463 2022-11-01 13:15:29.000000 ogl-0.70.51/ogl/OglAggregation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12912 2023-03-25 20:34:07.000000 ogl-0.70.51/ogl/OglAssociation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      328 2023-06-09 20:08:20.000000 ogl-0.70.51/ogl/OglAssociationLabel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    20392 2023-05-16 00:59:29.000000 ogl-0.70.51/ogl/OglClass.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1409 2023-03-22 20:23:56.000000 ogl-0.70.51/ogl/OglComposition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      668 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/OglConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      717 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/OglDimensions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1460 2023-01-31 22:21:10.000000 ogl-0.70.51/ogl/OglInheritance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3541 2023-03-31 00:59:54.000000 ogl-0.70.51/ogl/OglInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6199 2023-02-21 19:19:18.000000 ogl-0.70.51/ogl/OglInterface2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15577 2023-03-22 20:23:56.000000 ogl-0.70.51/ogl/OglLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3115 2023-03-26 22:27:03.000000 ogl-0.70.51/ogl/OglLinkFactory.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2693 2022-08-28 23:27:21.000000 ogl-0.70.51/ogl/OglNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1180 2023-02-19 02:02:00.000000 ogl-0.70.51/ogl/OglNoteLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5529 2023-05-16 16:51:16.000000 ogl-0.70.51/ogl/OglObject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      474 2023-06-09 20:04:54.000000 ogl-0.70.51/ogl/OglPosition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8683 2023-05-15 20:22:45.000000 ogl-0.70.51/ogl/OglText.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      226 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/OglTextFontFamily.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2197 2022-06-08 20:23:03.000000 ogl-0.70.51/ogl/OglUseCase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4349 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/OglUtils.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       37 2023-05-14 21:20:56.000000 ogl-0.70.51/ogl/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       24 2023-06-09 21:01:24.000000 ogl-0.70.51/ogl/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:01:42.132428 ogl-0.70.51/ogl/events/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      543 2023-01-15 21:02:48.000000 ogl-0.70.51/ogl/events/IOglEventEngine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/events/InvalidKeywordException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4566 2023-01-15 21:06:24.000000 ogl-0.70.51/ogl/events/OglEventEngine.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      780 2022-11-14 22:52:55.000000 ogl-0.70.51/ogl/events/OglEvents.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      239 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/events/ShapeSelectedEventData.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/events/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.51/ogl/events/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:01:42.133144 ogl-0.70.51/ogl/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    21282 2023-05-14 20:59:24.000000 ogl-0.70.51/ogl/preferences/OglPreferences.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.51/ogl/preferences/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.51/ogl/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:01:42.133249 ogl-0.70.51/ogl/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/resources/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:01:42.134071 ogl-0.70.51/ogl/resources/img/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1350 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/resources/img/Display.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1702 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/resources/img/DoNotDisplay.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2238 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/resources/img/UnSpecified.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/resources/img/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.51/ogl/resources/img/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:01:42.134544 ogl-0.70.51/ogl/resources/img/textdetails/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1543 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/resources/img/textdetails/DecreaseTextSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1575 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/resources/img/textdetails/IncreaseTextSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/resources/img/textdetails/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.51/ogl/resources/img/textdetails/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:01:42.135699 ogl-0.70.51/ogl/sd/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      904 2023-05-12 20:37:54.000000 ogl-0.70.51/ogl/sd/OglInstanceName.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6876 2023-05-16 01:17:51.000000 ogl-0.70.51/ogl/sd/OglSDInstance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6874 2023-05-14 21:08:57.000000 ogl-0.70.51/ogl/sd/OglSDMessage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-05-18 20:30:08.000000 ogl-0.70.51/ogl/sd/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.51/ogl/sd/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:01:42.136609 ogl-0.70.51/ogl/ui/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      657 2023-05-16 00:59:48.000000 ogl-0.70.51/ogl/ui/BaseOglPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3967 2023-02-19 20:46:44.000000 ogl-0.70.51/ogl/ui/DefaultValuesPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12232 2023-02-19 22:08:38.000000 ogl-0.70.51/ogl/ui/DiagramPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 14:43:49.000000 ogl-0.70.51/ogl/ui/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 ogl-0.70.51/ogl/ui/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:01:42.138375 ogl-0.70.51/ogl/ui/valuecontrols/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2279 2023-02-11 21:29:46.000000 ogl-0.70.51/ogl/ui/valuecontrols/AssociationAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5065 2023-02-11 20:04:09.000000 ogl-0.70.51/ogl/ui/valuecontrols/ClassAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2987 2023-02-11 20:20:38.000000 ogl-0.70.51/ogl/ui/valuecontrols/DefaultNamesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1943 2023-03-26 22:24:15.000000 ogl-0.70.51/ogl/ui/valuecontrols/NoteAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2686 2023-03-26 22:24:31.000000 ogl-0.70.51/ogl/ui/valuecontrols/SDAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5284 2023-05-14 22:17:09.000000 ogl-0.70.51/ogl/ui/valuecontrols/TextAttributesControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 15:30:26.000000 ogl-0.70.51/ogl/ui/valuecontrols/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-09 21:01:42.131215 ogl-0.70.51/ogl.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2357 2023-06-09 21:01:42.000000 ogl-0.70.51/ogl.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2516 2023-06-09 21:01:42.000000 ogl-0.70.51/ogl.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-09 21:01:42.000000 ogl-0.70.51/ogl.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       90 2023-06-09 21:01:42.000000 ogl-0.70.51/ogl.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-06-09 21:01:42.000000 ogl-0.70.51/ogl.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-09 21:01:42.138683 ogl-0.70.51/setup.cfg
+-rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     1565 2023-06-09 16:48:31.000000 ogl-0.70.51/setup.py
```

### Comparing `ogl-0.70.50/LICENSE` & `ogl-0.70.51/LICENSE`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/PKG-INFO` & `ogl-0.70.51/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogl
-Version: 0.70.50
+Version: 0.70.51
 Summary: External Pyut Graphical Shapes
 Home-page: https://github.com/hasii2011/ogl
 Author: Humberto A. Sanchez II
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ogl Version: 0.70.50 Summary: External Pyut
+Metadata-Version: 2.1 Name: ogl Version: 0.70.51 Summary: External Pyut
 Graphical Shapes Home-page: https://github.com/hasii2011/ogl Author: Humberto
 A. Sanchez II Author-email: Humberto.A.Sanchez.II@gmail.com Maintainer:
 Humberto A. Sanchez II Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown License-File: LICENSE [./developer/
 agpl-license-web-badge-version-2-256x48.png] [![Maintenance](https://
 img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/
 StrapDown.js/graphs/commit-activity) [![CircleCI](https://dl.circleci.com/
```

### Comparing `ogl-0.70.50/README.md` & `ogl-0.70.51/README.md`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/AnchorPoint.py` & `ogl-0.70.51/miniogl/AnchorPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/AttachmentSide.py` & `ogl-0.70.51/miniogl/AttachmentSide.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/Common.py` & `ogl-0.70.51/miniogl/Common.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/ControlPoint.py` & `ogl-0.70.51/miniogl/ControlPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/Diagram.py` & `ogl-0.70.51/miniogl/Diagram.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/DiagramFrame.py` & `ogl-0.70.51/miniogl/DiagramFrame.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/DlgDebugDiagramFrame.py` & `ogl-0.70.51/miniogl/DlgDebugDiagramFrame.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/LinePoint.py` & `ogl-0.70.51/miniogl/LinePoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/LineShape.py` & `ogl-0.70.51/miniogl/LineShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/LollipopLine.py` & `ogl-0.70.51/miniogl/LollipopLine.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/MiniOglColorEnum.py` & `ogl-0.70.51/miniogl/MiniOglColorEnum.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/MiniOglPenStyle.py` & `ogl-0.70.51/miniogl/MiniOglPenStyle.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/PointShape.py` & `ogl-0.70.51/miniogl/PointShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/RectangleShape.py` & `ogl-0.70.51/miniogl/RectangleShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/RectangleShapeModel.py` & `ogl-0.70.51/miniogl/RectangleShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/RotatableShape.py` & `ogl-0.70.51/miniogl/RotatableShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/SelectAnchorPoint.py` & `ogl-0.70.51/miniogl/SelectAnchorPoint.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/Shape.py` & `ogl-0.70.51/miniogl/Shape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/ShapeEventHandler.py` & `ogl-0.70.51/miniogl/ShapeEventHandler.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/ShapeModel.py` & `ogl-0.70.51/miniogl/ShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/SizerShape.py` & `ogl-0.70.51/miniogl/SizerShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/TextShape.py` & `ogl-0.70.51/miniogl/TextShape.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/TextShapeModel.py` & `ogl-0.70.51/miniogl/TextShapeModel.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/miniogl/VShapes.py` & `ogl-0.70.51/miniogl/VShapes.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglActor.py` & `ogl-0.70.51/ogl/OglActor.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglAggregation.py` & `ogl-0.70.51/ogl/OglAggregation.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglAssociation.py` & `ogl-0.70.51/ogl/OglAssociation.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglClass.py` & `ogl-0.70.51/ogl/OglClass.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglComposition.py` & `ogl-0.70.51/ogl/OglComposition.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglConstants.py` & `ogl-0.70.51/ogl/OglConstants.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglDimensions.py` & `ogl-0.70.51/ogl/OglDimensions.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglInheritance.py` & `ogl-0.70.51/ogl/OglInheritance.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglInterface.py` & `ogl-0.70.51/ogl/OglInterface.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglInterface2.py` & `ogl-0.70.51/ogl/OglInterface2.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglLink.py` & `ogl-0.70.51/ogl/OglLink.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglLinkFactory.py` & `ogl-0.70.51/ogl/OglLinkFactory.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglNote.py` & `ogl-0.70.51/ogl/OglNote.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglNoteLink.py` & `ogl-0.70.51/ogl/OglNoteLink.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglObject.py` & `ogl-0.70.51/ogl/OglObject.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglText.py` & `ogl-0.70.51/ogl/OglText.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglUseCase.py` & `ogl-0.70.51/ogl/OglUseCase.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/OglUtils.py` & `ogl-0.70.51/ogl/OglUtils.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/events/IOglEventEngine.py` & `ogl-0.70.51/ogl/events/IOglEventEngine.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/events/OglEventEngine.py` & `ogl-0.70.51/ogl/events/OglEventEngine.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/events/OglEvents.py` & `ogl-0.70.51/ogl/events/OglEvents.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/preferences/OglPreferences.py` & `ogl-0.70.51/ogl/preferences/OglPreferences.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/resources/img/Display.py` & `ogl-0.70.51/ogl/resources/img/Display.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/resources/img/DoNotDisplay.py` & `ogl-0.70.51/ogl/resources/img/DoNotDisplay.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/resources/img/UnSpecified.py` & `ogl-0.70.51/ogl/resources/img/UnSpecified.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/resources/img/textdetails/DecreaseTextSize.py` & `ogl-0.70.51/ogl/resources/img/textdetails/DecreaseTextSize.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/resources/img/textdetails/IncreaseTextSize.py` & `ogl-0.70.51/ogl/resources/img/textdetails/IncreaseTextSize.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/sd/OglInstanceName.py` & `ogl-0.70.51/ogl/sd/OglInstanceName.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/sd/OglSDInstance.py` & `ogl-0.70.51/ogl/sd/OglSDInstance.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/sd/OglSDMessage.py` & `ogl-0.70.51/ogl/sd/OglSDMessage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/ui/BaseOglPreferencesPage.py` & `ogl-0.70.51/ogl/ui/BaseOglPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/ui/DefaultValuesPreferencesPage.py` & `ogl-0.70.51/ogl/ui/DefaultValuesPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/ui/DiagramPreferencesPage.py` & `ogl-0.70.51/ogl/ui/DiagramPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/ui/valuecontrols/AssociationAttributesControl.py` & `ogl-0.70.51/ogl/ui/valuecontrols/AssociationAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/ui/valuecontrols/ClassAttributesControl.py` & `ogl-0.70.51/ogl/ui/valuecontrols/ClassAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/ui/valuecontrols/DefaultNamesControl.py` & `ogl-0.70.51/ogl/ui/valuecontrols/DefaultNamesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/ui/valuecontrols/NoteAttributesControl.py` & `ogl-0.70.51/ogl/ui/valuecontrols/NoteAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/ui/valuecontrols/SDAttributesControl.py` & `ogl-0.70.51/ogl/ui/valuecontrols/SDAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl/ui/valuecontrols/TextAttributesControl.py` & `ogl-0.70.51/ogl/ui/valuecontrols/TextAttributesControl.py`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/ogl.egg-info/PKG-INFO` & `ogl-0.70.51/ogl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogl
-Version: 0.70.50
+Version: 0.70.51
 Summary: External Pyut Graphical Shapes
 Home-page: https://github.com/hasii2011/ogl
 Author: Humberto A. Sanchez II
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ogl Version: 0.70.50 Summary: External Pyut
+Metadata-Version: 2.1 Name: ogl Version: 0.70.51 Summary: External Pyut
 Graphical Shapes Home-page: https://github.com/hasii2011/ogl Author: Humberto
 A. Sanchez II Author-email: Humberto.A.Sanchez.II@gmail.com Maintainer:
 Humberto A. Sanchez II Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown License-File: LICENSE [./developer/
 agpl-license-web-badge-version-2-256x48.png] [![Maintenance](https://
 img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/
 StrapDown.js/graphs/commit-activity) [![CircleCI](https://dl.circleci.com/
```

### Comparing `ogl-0.70.50/ogl.egg-info/SOURCES.txt` & `ogl-0.70.51/ogl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogl-0.70.50/setup.py` & `ogl-0.70.51/setup.py`

 * *Files identical despite different names*

