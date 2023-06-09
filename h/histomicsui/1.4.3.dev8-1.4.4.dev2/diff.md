# Comparing `tmp/histomicsui-1.4.3.dev8.tar.gz` & `tmp/histomicsui-1.4.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histomicsui-1.4.3.dev8.tar", last modified: Tue Apr 11 17:13:22 2023, max compression
+gzip compressed data, was "histomicsui-1.4.4.dev2.tar", last modified: Fri Jun  9 19:20:39 2023, max compression
```

## Comparing `histomicsui-1.4.3.dev8.tar` & `histomicsui-1.4.4.dev2.tar`

### file list

```diff
@@ -1,210 +1,211 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.897448 histomicsui-1.4.3.dev8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.873448 histomicsui-1.4.3.dev8/.circleci/
--rw-r--r--   0 root         (0) root         (0)     3793 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)      303 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/.editorconfig
--rw-r--r--   0 root         (0) root         (0)      419 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/.git-blame-ignore-revs
--rw-r--r--   0 root         (0) root         (0)      556 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/.gitignore
--rw-r--r--   0 root         (0) root         (0)      690 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/.travis.yml
--rw-r--r--   0 root         (0) root         (0)    10173 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      150 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      585 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6974 2023-04-11 17:13:22.897448 histomicsui-1.4.3.dev8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6076 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/README.rst
--rw-r--r--   0 root         (0) root         (0)      460 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/codecov.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.873448 histomicsui-1.4.3.dev8/docs/
--rw-r--r--   0 root         (0) root         (0)     2399 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/docs/config_options.rst
--rw-r--r--   0 root         (0) root         (0)     5901 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/docs/controls.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.873448 histomicsui-1.4.3.dev8/docs/images/
--rwxr-xr-x   0 root         (0) root         (0)   133796 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/docs/images/difference.gif
--rwxr-xr-x   0 root         (0) root         (0)   133603 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/docs/images/intersect.gif
--rwxr-xr-x   0 root         (0) root         (0)   154141 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/docs/images/union.gif
--rwxr-xr-x   0 root         (0) root         (0)   168255 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/docs/images/xor.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.873448 histomicsui-1.4.3.dev8/histomicsui/
--rw-r--r--   0 root         (0) root         (0)    17578 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/__init__.py
--rw-r--r--   0 root         (0) root         (0)      917 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/constants.py
--rw-r--r--   0 root         (0) root         (0)    10635 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.877448 histomicsui-1.4.3.dev8/histomicsui/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/aperio.py
--rw-r--r--   0 root         (0) root         (0)     1832 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/case.py
--rw-r--r--   0 root         (0) root         (0)     1057 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/cohort.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/image.py
--rw-r--r--   0 root         (0) root         (0)     8504 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/meta.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/pathology.py
--rw-r--r--   0 root         (0) root         (0)     1549 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/slide.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.877448 histomicsui-1.4.3.dev8/histomicsui/rest/
--rw-r--r--   0 root         (0) root         (0)      512 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3728 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/rest/aperio.py
--rw-r--r--   0 root         (0) root         (0)     9313 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/rest/hui_resource.py
--rw-r--r--   0 root         (0) root         (0)     4584 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/rest/image_browse_resource.py
--rw-r--r--   0 root         (0) root         (0)    15298 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/rest/system.py
--rw-r--r--   0 root         (0) root         (0)    28968 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/rest/tcga.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.877448 histomicsui-1.4.3.dev8/histomicsui/web_client/
--rw-r--r--   0 root         (0) root         (0)     2450 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/app.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.881448 histomicsui-1.4.3.dev8/histomicsui/web_client/collections/
--rw-r--r--   0 root         (0) root         (0)      308 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/collections/StyleCollection.js
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/collections/index.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.881448 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/
--rw-r--r--   0 root         (0) root         (0)     1326 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/confirmDialog.js
--rw-r--r--   0 root         (0) root         (0)     3936 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/editElement.js
--rw-r--r--   0 root         (0) root         (0)     6663 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/editRegionOfInterest.js
--rw-r--r--   0 root         (0) root         (0)    11184 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/editStyleGroups.js
--rw-r--r--   0 root         (0) root         (0)      478 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/index.js
--rw-r--r--   0 root         (0) root         (0)     1153 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/metadataPlot.js
--rw-r--r--   0 root         (0) root         (0)     4936 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/openAnnotatedImage.js
--rw-r--r--   0 root         (0) root         (0)     2588 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/openImage.js
--rw-r--r--   0 root         (0) root         (0)    22740 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/saveAnnotation.js
--rw-r--r--   0 root         (0) root         (0)       78 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/events.js
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/index.js
--rw-r--r--   0 root         (0) root         (0)      787 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/main.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.881448 histomicsui-1.4.3.dev8/histomicsui/web_client/models/
--rw-r--r--   0 root         (0) root         (0)      221 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/models/StyleModel.js
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/models/index.js
--rw-r--r--   0 root         (0) root         (0)     5686 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.881448 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/
--rw-r--r--   0 root         (0) root         (0)    23413 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/AnnotationSelector.js
--rw-r--r--   0 root         (0) root         (0)    43398 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/DrawWidget.js
--rw-r--r--   0 root         (0) root         (0)    14204 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/MetadataPlot.js
--rw-r--r--   0 root         (0) root         (0)    22033 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/MetadataWidget.js
--rw-r--r--   0 root         (0) root         (0)     8115 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/OverviewWidget.js
--rw-r--r--   0 root         (0) root         (0)     1121 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/RegionSelector.js
--rw-r--r--   0 root         (0) root         (0)     9946 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/ZoomWidget.js
--rw-r--r--   0 root         (0) root         (0)      146 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/index.js
--rw-r--r--   0 root         (0) root         (0)     1485 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/router.js
--rw-r--r--   0 root         (0) root         (0)      292 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/routes.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.881448 histomicsui-1.4.3.dev8/histomicsui/web_client/static/
--rwxr-xr-x   0 root         (0) root         (0)     5072 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/static/favicon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.869448 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.881448 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/body/
--rw-r--r--   0 root         (0) root         (0)      504 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/body/configView.styl
--rw-r--r--   0 root         (0) root         (0)      883 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/body/frontPage.styl
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/body/image.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.885448 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/dialogs/
--rw-r--r--   0 root         (0) root         (0)      191 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/dialogs/editStyleGroups.styl
--rw-r--r--   0 root         (0) root         (0)      238 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/dialogs/openAnnotatedImage.styl
--rw-r--r--   0 root         (0) root         (0)      769 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.885448 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/layout/
--rw-r--r--   0 root         (0) root         (0)      976 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/layout/header.styl
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/layout/headerAnalyses.styl
--rw-r--r--   0 root         (0) root         (0)      150 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/layout/headerImage.styl
--rw-r--r--   0 root         (0) root         (0)     1386 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/layout/layout.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.885448 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/
--rw-r--r--   0 root         (0) root         (0)     1666 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/annotationSelector.styl
--rw-r--r--   0 root         (0) root         (0)     2747 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/drawWidget.styl
--rw-r--r--   0 root         (0) root         (0)      430 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/metadataPlot.styl
--rw-r--r--   0 root         (0) root         (0)      865 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/metadataWidget.styl
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/overviewWidget.styl
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/regionSelector.styl
--rw-r--r--   0 root         (0) root         (0)      877 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/zoomWidget.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.885448 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/popover/
--rw-r--r--   0 root         (0) root         (0)      112 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/popover/annotationContextMenu.styl
--rw-r--r--   0 root         (0) root         (0)     1847 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/popover/annotationPopover.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.885448 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/views/
--rw-r--r--   0 root         (0) root         (0)      222 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/views/itemList.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.869448 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.885448 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/body/
--rw-r--r--   0 root         (0) root         (0)     5608 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/body/configView.pug
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/body/frontPage.pug
--rw-r--r--   0 root         (0) root         (0)      723 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/body/image.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.889448 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/
--rw-r--r--   0 root         (0) root         (0)      501 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/annotatedImageList.pug
--rw-r--r--   0 root         (0) root         (0)      428 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/confirmDialog.pug
--rw-r--r--   0 root         (0) root         (0)     2079 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/editElement.pug
--rw-r--r--   0 root         (0) root         (0)     1730 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug
--rw-r--r--   0 root         (0) root         (0)     3201 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/editStyleGroups.pug
--rw-r--r--   0 root         (0) root         (0)     1541 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/metadataPlot.pug
--rw-r--r--   0 root         (0) root         (0)      838 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug
--rw-r--r--   0 root         (0) root         (0)      353 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/openImage.pug
--rw-r--r--   0 root         (0) root         (0)     5392 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/saveAnnotation.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.889448 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/
--rw-r--r--   0 root         (0) root         (0)      925 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/header.pug
--rw-r--r--   0 root         (0) root         (0)      865 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/headerAnalyses.pug
--rw-r--r--   0 root         (0) root         (0)     1467 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/headerImage.pug
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/headerUser.pug
--rw-r--r--   0 root         (0) root         (0)      157 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/layout.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.889448 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/
--rw-r--r--   0 root         (0) root         (0)     3961 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/annotationSelector.pug
--rw-r--r--   0 root         (0) root         (0)     5673 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/drawWidget.pug
--rw-r--r--   0 root         (0) root         (0)     2166 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/drawWidgetElement.pug
--rw-r--r--   0 root         (0) root         (0)      347 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/metadataPlot.pug
--rw-r--r--   0 root         (0) root         (0)      815 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/metadataWidget.pug
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/overviewWidget.pug
--rw-r--r--   0 root         (0) root         (0)      398 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/panel.pug
--rw-r--r--   0 root         (0) root         (0)      345 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/regionSelector.pug
--rw-r--r--   0 root         (0) root         (0)     1281 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/zoomWidget.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.889448 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/popover/
--rw-r--r--   0 root         (0) root         (0)      576 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/popover/annotationContextMenu.pug
--rw-r--r--   0 root         (0) root         (0)     1404 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/popover/annotationPopover.pug
--rw-r--r--   0 root         (0) root         (0)      204 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/popover/pixelmapContextMenu.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.889448 histomicsui-1.4.3.dev8/histomicsui/web_client/views/
--rw-r--r--   0 root         (0) root         (0)      525 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/HierarchyWidget.js
--rw-r--r--   0 root         (0) root         (0)     2263 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/View.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.893448 histomicsui-1.4.3.dev8/histomicsui/web_client/views/body/
--rw-r--r--   0 root         (0) root         (0)     7205 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/body/ConfigView.js
--rw-r--r--   0 root         (0) root         (0)      776 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/body/FrontPageView.js
--rw-r--r--   0 root         (0) root         (0)    68106 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/body/ImageView.js
--rw-r--r--   0 root         (0) root         (0)      183 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/body/index.js
--rw-r--r--   0 root         (0) root         (0)      190 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/index.js
--rw-r--r--   0 root         (0) root         (0)     3436 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/itemList.js
--rw-r--r--   0 root         (0) root         (0)     2375 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/itemPage.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.893448 histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/
--rw-r--r--   0 root         (0) root         (0)     1658 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/HeaderAnalysesView.js
--rw-r--r--   0 root         (0) root         (0)     2861 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/HeaderImageView.js
--rw-r--r--   0 root         (0) root         (0)      421 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/HeaderUserView.js
--rw-r--r--   0 root         (0) root         (0)     1621 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/HeaderView.js
--rw-r--r--   0 root         (0) root         (0)      134 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/index.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.893448 histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/
--rw-r--r--   0 root         (0) root         (0)     4493 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/AnnotationContextMenu.js
--rw-r--r--   0 root         (0) root         (0)    10799 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/AnnotationPopover.js
--rw-r--r--   0 root         (0) root         (0)     1231 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/PixelmapContextMenu.js
--rw-r--r--   0 root         (0) root         (0)      176 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/index.js
--rw-r--r--   0 root         (0) root         (0)     2847 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/utils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.869448 histomicsui-1.4.3.dev8/histomicsui/web_client/vue/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.893448 histomicsui-1.4.3.dev8/histomicsui/web_client/vue/components/
--rw-r--r--   0 root         (0) root         (0)     2650 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/vue/components/ColorPickerInput.vue
--rw-r--r--   0 root         (0) root         (0)    12531 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue
--rw-r--r--   0 root         (0) root         (0)      745 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue
--rw-r--r--   0 root         (0) root         (0)      947 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/webpack.helper.js
--rw-r--r--   0 root         (0) root         (0)     1538 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/webroot.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.877448 histomicsui-1.4.3.dev8/histomicsui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6974 2023-04-11 17:13:22.000000 histomicsui-1.4.3.dev8/histomicsui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7281 2023-04-11 17:13:22.000000 histomicsui-1.4.3.dev8/histomicsui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 17:13:22.000000 histomicsui-1.4.3.dev8/histomicsui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-11 17:13:22.000000 histomicsui-1.4.3.dev8/histomicsui.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 17:12:29.000000 histomicsui-1.4.3.dev8/histomicsui.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      182 2023-04-11 17:13:22.000000 histomicsui-1.4.3.dev8/histomicsui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-11 17:13:22.000000 histomicsui-1.4.3.dev8/histomicsui.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-11 17:13:22.897448 histomicsui-1.4.3.dev8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2289 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.893448 histomicsui-1.4.3.dev8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/datastore.py
--rw-r--r--   0 root         (0) root         (0)     2202 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/girder_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.897448 histomicsui-1.4.3.dev8/tests/test_files/
--rw-r--r--   0 root         (0) root         (0)     1286 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_files/.histomicsui_config.yaml
--rw-r--r--   0 root         (0) root         (0)      424 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_files/sample.anot
--rw-r--r--   0 root         (0) root         (0)      101 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_files/sample.meta
--rw-r--r--   0 root         (0) root         (0)      493 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_files/sample_girder_id.anot
--rw-r--r--   0 root         (0) root         (0)     8928 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_files/test_analysis_detection.xml
--rw-r--r--   0 root         (0) root         (0)    12017 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_files/test_analysis_features.xml
--rw-r--r--   0 root         (0) root         (0)     5257 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_handlers.py
--rw-r--r--   0 root         (0) root         (0)    19443 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_hui_rest.py
--rw-r--r--   0 root         (0) root         (0)     4365 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_image_browse_endpoints.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_load.py
--rw-r--r--   0 root         (0) root         (0)    32496 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_tcga.py
--rw-r--r--   0 root         (0) root         (0)     5993 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_web_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.897448 histomicsui-1.4.3.dev8/tests/web_client_specs/
--rw-r--r--   0 root         (0) root         (0)      237 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/.eslintrc
--rw-r--r--   0 root         (0) root         (0)     6591 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/analysisSpec.js
--rw-r--r--   0 root         (0) root         (0)    81677 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/annotationSpec.js
--rw-r--r--   0 root         (0) root         (0)     1923 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/girderUISpec.js
--rw-r--r--   0 root         (0) root         (0)     4037 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/huiSpec.js
--rw-r--r--   0 root         (0) root         (0)     4336 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/huiTest.js
--rw-r--r--   0 root         (0) root         (0)     4387 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/itemSpec.js
--rw-r--r--   0 root         (0) root         (0)     4390 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/metadataPanelSpec.js
--rw-r--r--   0 root         (0) root         (0)     6526 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/metadataPlotSpec.js
--rw-r--r--   0 root         (0) root         (0)     6175 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/overviewPanelSpec.js
--rw-r--r--   0 root         (0) root         (0)     2917 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/panelLayoutSpec.js
--rw-r--r--   0 root         (0) root         (0)    13890 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/pixelmapCategorySpec.js
--rw-r--r--   0 root         (0) root         (0)     2944 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.874526 histomicsui-1.4.4.dev2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.834526 histomicsui-1.4.4.dev2/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     3884 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/.editorconfig
+-rw-r--r--   0 root         (0) root         (0)      532 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/.git-blame-ignore-revs
+-rw-r--r--   0 root         (0) root         (0)      556 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      690 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/.travis.yml
+-rw-r--r--   0 root         (0) root         (0)    10173 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      585 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6974 2023-06-09 19:20:39.874526 histomicsui-1.4.4.dev2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6076 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/codecov.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.838526 histomicsui-1.4.4.dev2/docs/
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/docs/config_options.rst
+-rw-r--r--   0 root         (0) root         (0)     6059 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/docs/controls.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.838526 histomicsui-1.4.4.dev2/docs/images/
+-rwxr-xr-x   0 root         (0) root         (0)   133796 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/docs/images/difference.gif
+-rwxr-xr-x   0 root         (0) root         (0)   133603 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/docs/images/intersect.gif
+-rwxr-xr-x   0 root         (0) root         (0)   154141 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/docs/images/union.gif
+-rwxr-xr-x   0 root         (0) root         (0)   168255 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/docs/images/xor.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.838526 histomicsui-1.4.4.dev2/histomicsui/
+-rw-r--r--   0 root         (0) root         (0)    17578 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      917 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/constants.py
+-rw-r--r--   0 root         (0) root         (0)    10489 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.842526 histomicsui-1.4.4.dev2/histomicsui/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/models/aperio.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/models/case.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/models/cohort.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/models/image.py
+-rw-r--r--   0 root         (0) root         (0)     8504 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/models/meta.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/models/pathology.py
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/models/slide.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.846526 histomicsui-1.4.4.dev2/histomicsui/rest/
+-rw-r--r--   0 root         (0) root         (0)      512 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3728 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/rest/aperio.py
+-rw-r--r--   0 root         (0) root         (0)     9313 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/rest/hui_resource.py
+-rw-r--r--   0 root         (0) root         (0)     4584 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/rest/image_browse_resource.py
+-rw-r--r--   0 root         (0) root         (0)    15298 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/rest/system.py
+-rw-r--r--   0 root         (0) root         (0)    28968 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/rest/tcga.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.846526 histomicsui-1.4.4.dev2/histomicsui/web_client/
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/app.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.850526 histomicsui-1.4.4.dev2/histomicsui/web_client/collections/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/collections/StyleCollection.js
+-rw-r--r--   0 root         (0) root         (0)      405 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/collections/UserCollection.js
+-rw-r--r--   0 root         (0) root         (0)      149 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/collections/index.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.850526 histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/
+-rw-r--r--   0 root         (0) root         (0)     1326 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/confirmDialog.js
+-rw-r--r--   0 root         (0) root         (0)     3936 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/editElement.js
+-rw-r--r--   0 root         (0) root         (0)     6663 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/editRegionOfInterest.js
+-rw-r--r--   0 root         (0) root         (0)    11184 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/editStyleGroups.js
+-rw-r--r--   0 root         (0) root         (0)      478 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/index.js
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/metadataPlot.js
+-rw-r--r--   0 root         (0) root         (0)     4936 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/openAnnotatedImage.js
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/openImage.js
+-rw-r--r--   0 root         (0) root         (0)    22740 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/saveAnnotation.js
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/events.js
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/index.js
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/main.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.850526 histomicsui-1.4.4.dev2/histomicsui/web_client/models/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/models/StyleModel.js
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/models/index.js
+-rw-r--r--   0 root         (0) root         (0)     3631 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.854526 histomicsui-1.4.4.dev2/histomicsui/web_client/panels/
+-rw-r--r--   0 root         (0) root         (0)    23413 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/panels/AnnotationSelector.js
+-rw-r--r--   0 root         (0) root         (0)    43398 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/panels/DrawWidget.js
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/panels/FrameSelectorWidget.js
+-rw-r--r--   0 root         (0) root         (0)    14204 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/panels/MetadataPlot.js
+-rw-r--r--   0 root         (0) root         (0)    22033 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/panels/MetadataWidget.js
+-rw-r--r--   0 root         (0) root         (0)     8115 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/panels/OverviewWidget.js
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/panels/RegionSelector.js
+-rw-r--r--   0 root         (0) root         (0)     9946 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/panels/ZoomWidget.js
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/panels/index.js
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/router.js
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/routes.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.854526 histomicsui-1.4.4.dev2/histomicsui/web_client/static/
+-rwxr-xr-x   0 root         (0) root         (0)     5072 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/static/favicon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.830526 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.854526 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/body/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/body/configView.styl
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/body/image.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.854526 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/dialogs/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/dialogs/editStyleGroups.styl
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/dialogs/openAnnotatedImage.styl
+-rw-r--r--   0 root         (0) root         (0)      775 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.858526 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/layout/
+-rw-r--r--   0 root         (0) root         (0)      986 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/layout/header.styl
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/layout/headerAnalyses.styl
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/layout/headerImage.styl
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/layout/layout.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.858526 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/panels/
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/panels/annotationSelector.styl
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/panels/drawWidget.styl
+-rw-r--r--   0 root         (0) root         (0)      605 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/panels/frameSelectorWidget.styl
+-rw-r--r--   0 root         (0) root         (0)      430 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/panels/metadataPlot.styl
+-rw-r--r--   0 root         (0) root         (0)      866 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/panels/metadataWidget.styl
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/panels/overviewWidget.styl
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/panels/regionSelector.styl
+-rw-r--r--   0 root         (0) root         (0)      878 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/panels/zoomWidget.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.858526 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/popover/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/popover/annotationContextMenu.styl
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/popover/annotationPopover.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.858526 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/views/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/views/itemList.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.830526 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.862526 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/body/
+-rw-r--r--   0 root         (0) root         (0)     5608 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/body/configView.pug
+-rw-r--r--   0 root         (0) root         (0)      783 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/body/image.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.862526 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/annotatedImageList.pug
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/confirmDialog.pug
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/editElement.pug
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/editStyleGroups.pug
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/metadataPlot.pug
+-rw-r--r--   0 root         (0) root         (0)      838 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug
+-rw-r--r--   0 root         (0) root         (0)      353 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/openImage.pug
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/saveAnnotation.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.866526 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/layout/
+-rw-r--r--   0 root         (0) root         (0)      925 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/layout/header.pug
+-rw-r--r--   0 root         (0) root         (0)      865 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/layout/headerAnalyses.pug
+-rw-r--r--   0 root         (0) root         (0)     1467 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/layout/headerImage.pug
+-rw-r--r--   0 root         (0) root         (0)      641 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/layout/headerUser.pug
+-rw-r--r--   0 root         (0) root         (0)      157 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/layout/layout.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.866526 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/
+-rw-r--r--   0 root         (0) root         (0)     3961 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/annotationSelector.pug
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/drawWidget.pug
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/drawWidgetElement.pug
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/frameSelectorWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/metadataPlot.pug
+-rw-r--r--   0 root         (0) root         (0)      815 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/metadataWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/overviewWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/panel.pug
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/regionSelector.pug
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/zoomWidget.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.866526 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/popover/
+-rw-r--r--   0 root         (0) root         (0)      576 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/popover/annotationContextMenu.pug
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/popover/annotationPopover.pug
+-rw-r--r--   0 root         (0) root         (0)      204 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/templates/popover/pixelmapContextMenu.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.866526 histomicsui-1.4.4.dev2/histomicsui/web_client/views/
+-rw-r--r--   0 root         (0) root         (0)      525 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/HierarchyWidget.js
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/View.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.866526 histomicsui-1.4.4.dev2/histomicsui/web_client/views/body/
+-rw-r--r--   0 root         (0) root         (0)     7205 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/body/ConfigView.js
+-rw-r--r--   0 root         (0) root         (0)    68637 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/body/ImageView.js
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/body/index.js
+-rw-r--r--   0 root         (0) root         (0)      190 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/index.js
+-rw-r--r--   0 root         (0) root         (0)     3436 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/itemList.js
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/itemPage.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.870526 histomicsui-1.4.4.dev2/histomicsui/web_client/views/layout/
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/layout/HeaderAnalysesView.js
+-rw-r--r--   0 root         (0) root         (0)     2861 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/layout/HeaderImageView.js
+-rw-r--r--   0 root         (0) root         (0)      421 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/layout/HeaderUserView.js
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/layout/HeaderView.js
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/layout/index.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.870526 histomicsui-1.4.4.dev2/histomicsui/web_client/views/popover/
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/popover/AnnotationContextMenu.js
+-rw-r--r--   0 root         (0) root         (0)    10799 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/popover/AnnotationPopover.js
+-rw-r--r--   0 root         (0) root         (0)     1231 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/popover/PixelmapContextMenu.js
+-rw-r--r--   0 root         (0) root         (0)      176 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/popover/index.js
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/views/utils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.830526 histomicsui-1.4.4.dev2/histomicsui/web_client/vue/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.870526 histomicsui-1.4.4.dev2/histomicsui/web_client/vue/components/
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/vue/components/ColorPickerInput.vue
+-rw-r--r--   0 root         (0) root         (0)    12531 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue
+-rw-r--r--   0 root         (0) root         (0)      745 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue
+-rw-r--r--   0 root         (0) root         (0)      906 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/web_client/webpack.helper.js
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/histomicsui/webroot.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.842526 histomicsui-1.4.4.dev2/histomicsui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6974 2023-06-09 19:20:39.000000 histomicsui-1.4.4.dev2/histomicsui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7360 2023-06-09 19:20:39.000000 histomicsui-1.4.4.dev2/histomicsui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 19:20:39.000000 histomicsui-1.4.4.dev2/histomicsui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-09 19:20:39.000000 histomicsui-1.4.4.dev2/histomicsui.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 19:19:42.000000 histomicsui-1.4.4.dev2/histomicsui.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-09 19:20:39.000000 histomicsui-1.4.4.dev2/histomicsui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-09 19:20:39.000000 histomicsui-1.4.4.dev2/histomicsui.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-09 19:20:39.874526 histomicsui-1.4.4.dev2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2289 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.870526 histomicsui-1.4.4.dev2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/datastore.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/girder_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.870526 histomicsui-1.4.4.dev2/tests/test_files/
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/test_files/.histomicsui_config.yaml
+-rw-r--r--   0 root         (0) root         (0)      424 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/test_files/sample.anot
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/test_files/sample.meta
+-rw-r--r--   0 root         (0) root         (0)      493 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/test_files/sample_girder_id.anot
+-rw-r--r--   0 root         (0) root         (0)     8928 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/test_files/test_analysis_detection.xml
+-rw-r--r--   0 root         (0) root         (0)    12017 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/test_files/test_analysis_features.xml
+-rw-r--r--   0 root         (0) root         (0)     5257 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/test_handlers.py
+-rw-r--r--   0 root         (0) root         (0)    19443 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/test_hui_rest.py
+-rw-r--r--   0 root         (0) root         (0)     4365 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/test_image_browse_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/test_load.py
+-rw-r--r--   0 root         (0) root         (0)    32496 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/test_tcga.py
+-rw-r--r--   0 root         (0) root         (0)     5993 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/test_web_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:20:39.874526 histomicsui-1.4.4.dev2/tests/web_client_specs/
+-rw-r--r--   0 root         (0) root         (0)      238 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/web_client_specs/.eslintrc
+-rw-r--r--   0 root         (0) root         (0)     6643 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/web_client_specs/analysisSpec.js
+-rw-r--r--   0 root         (0) root         (0)    81737 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/web_client_specs/annotationSpec.js
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/web_client_specs/girderUISpec.js
+-rw-r--r--   0 root         (0) root         (0)     4036 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/web_client_specs/huiSpec.js
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/web_client_specs/huiTest.js
+-rw-r--r--   0 root         (0) root         (0)     4393 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/web_client_specs/itemSpec.js
+-rw-r--r--   0 root         (0) root         (0)     4436 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/web_client_specs/metadataPanelSpec.js
+-rw-r--r--   0 root         (0) root         (0)     6855 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/web_client_specs/metadataPlotSpec.js
+-rw-r--r--   0 root         (0) root         (0)     6131 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/web_client_specs/overviewPanelSpec.js
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/web_client_specs/panelLayoutSpec.js
+-rw-r--r--   0 root         (0) root         (0)    13991 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tests/web_client_specs/pixelmapCategorySpec.js
+-rw-r--r--   0 root         (0) root         (0)     2944 2023-06-09 19:19:25.000000 histomicsui-1.4.4.dev2/tox.ini
```

### Comparing `histomicsui-1.4.3.dev8/.circleci/config.yml` & `histomicsui-1.4.4.dev2/.circleci/config.yml`

 * *Files 6% similar despite different names*

```diff
@@ -24,28 +24,23 @@
           # consume the exit code
           command: PYTEST_NUMPROCESSES=2 tox -e << parameters.env >> | cat; test ${PIPESTATUS[0]} -eq 0
   coverage:
     description: "Upload coverage"
     steps:
       - run:
           name: Install Codecov client
-          command: pip install codecov
+          command: |
+              curl -Os https://uploader.codecov.io/latest/linux/codecov
+              chmod +x codecov
       - run:
           name: Upload coverage
           # Retry as codecov can be flaky
-          command: for i in $(seq 1 10); do [ $i -gt 1 ] && echo "retrying $i" && sleep 5; codecov --disable search pycov gcov --file .tox/coverage/py_coverage.xml .tox/coverage/cobertura-coverage.xml && s=0 && break || s=$?; done; (exit $s)
+          command: for i in $(seq 1 10); do [ $i -gt 1 ] && echo "retrying $i" && sleep 5; ./codecov --disable search pycov gcov --file .tox/coverage/py_coverage.xml .tox/coverage/cobertura-coverage.xml && s=0 && break || s=$?; done; (exit $s)
 
 jobs:
-  py36:
-    executor: toxandnode
-    steps:
-      - checkout
-      - tox:
-          env: py36
-      - coverage
   py37:
     executor: toxandnode
     steps:
       - checkout
       - tox:
           env: py37
       - coverage
@@ -66,14 +61,21 @@
   py310:
     executor: toxandnode
     steps:
       - checkout
       - tox:
           env: py310
       - coverage
+  py311:
+    executor: toxandnode
+    steps:
+      - checkout
+      - tox:
+          env: py311
+      - coverage
   noanalysis:
     executor: toxandnode
     steps:
       - checkout
       - tox:
           env: noanalysis
       - coverage
@@ -94,43 +96,43 @@
           # consume the exit code
           command: tox -e release | cat; test ${PIPESTATUS[0]} -eq 0
 
 workflows:
   version: 2
   ci:
     jobs:
-      - py36:
+      - py37:
           filters:
             tags:
               only: /^v.*/
             branches:
               ignore:
                 - gh-pages
-      - py37:
+      - py38:
           filters:
             tags:
               only: /^v.*/
             branches:
               ignore:
                 - gh-pages
-      - py38:
+      - py39:
           filters:
             tags:
               only: /^v.*/
             branches:
               ignore:
                 - gh-pages
-      - py39:
+      - py310:
           filters:
             tags:
               only: /^v.*/
             branches:
               ignore:
                 - gh-pages
-      - py310:
+      - py311:
           filters:
             tags:
               only: /^v.*/
             branches:
               ignore:
                 - gh-pages
       - noanalysis:
@@ -145,18 +147,18 @@
             tags:
               only: /^v.*/
             branches:
               ignore:
                 - gh-pages
       - release:
           requires:
-            - py36
             - py37
             - py38
             - py39
             - py310
+            - py311
             - lint_and_docs
           filters:
             tags:
               only: /^v.*/
             branches:
               only: master
```

### Comparing `histomicsui-1.4.3.dev8/.gitignore` & `histomicsui-1.4.4.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/.travis.yml` & `histomicsui-1.4.4.dev2/.travis.yml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/LICENSE` & `histomicsui-1.4.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/NOTICE` & `histomicsui-1.4.4.dev2/NOTICE`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/PKG-INFO` & `histomicsui-1.4.4.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histomicsui
-Version: 1.4.3.dev8
+Version: 1.4.4.dev2
 Summary: Organize, visualize, and analyze histology images.
 Home-page: https://github.com/DigitalSlideArchive/histomicsui
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,histomicsui
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `histomicsui-1.4.3.dev8/README.rst` & `histomicsui-1.4.4.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/docs/config_options.rst` & `histomicsui-1.4.4.dev2/docs/config_options.rst`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/docs/controls.rst` & `histomicsui-1.4.4.dev2/docs/controls.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 --------------------
 
 - **Pan**:
 
   - **Left-drag**: Hold down the left mouse button and drag the image to change
     the area that is in view.
 
+  - **Middle-drag**: Hold down the middle mouse button and drag the image to
+    change the area that is in view.  This works even when editing annotations.
+
   - **Single touch drag**
 
   - **Arrow keys**: The arrow keys (up, down, left, right) to nudge the area in
     view one screen pixel.  If you hold down shift, arrow keys will move the
     view area half a screen size.  Shift+ctrl and arrow keys will move an
     intermediate amount.
```

### Comparing `histomicsui-1.4.3.dev8/docs/images/difference.gif` & `histomicsui-1.4.4.dev2/docs/images/difference.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/docs/images/intersect.gif` & `histomicsui-1.4.4.dev2/docs/images/intersect.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/docs/images/union.gif` & `histomicsui-1.4.4.dev2/docs/images/union.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/docs/images/xor.gif` & `histomicsui-1.4.4.dev2/docs/images/xor.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/__init__.py` & `histomicsui-1.4.4.dev2/histomicsui/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/constants.py` & `histomicsui-1.4.4.dev2/histomicsui/constants.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/handlers.py` & `histomicsui-1.4.4.dev2/histomicsui/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,21 +120,18 @@
     """Add annotations to an image on a ``data.process`` event"""
     results = _itemFromEvent(event, 'AnnotationFile')
     if not results:
         return
     item = results['item']
     user = results['user']
 
-    startTime = time.time()
     file = File().load(
         event.info.get('file', {}).get('_id'),
         level=AccessType.READ, user=user
     )
-    if time.time() - startTime > 10:
-        logger.info('Loaded annotation file in %5.3fs', time.time() - startTime)
     startTime = time.time()
 
     if not file:
         logger.error('Could not load models from the database')
         return
     try:
         if file['size'] > 1 * 1024 ** 3:
```

### Comparing `histomicsui-1.4.3.dev8/histomicsui/models/aperio.py` & `histomicsui-1.4.4.dev2/histomicsui/models/aperio.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/models/case.py` & `histomicsui-1.4.4.dev2/histomicsui/models/case.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/models/cohort.py` & `histomicsui-1.4.4.dev2/histomicsui/models/cohort.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/models/image.py` & `histomicsui-1.4.4.dev2/histomicsui/models/image.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/models/meta.py` & `histomicsui-1.4.4.dev2/histomicsui/models/meta.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/models/pathology.py` & `histomicsui-1.4.4.dev2/histomicsui/models/pathology.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/models/slide.py` & `histomicsui-1.4.4.dev2/histomicsui/models/slide.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/rest/__init__.py` & `histomicsui-1.4.4.dev2/histomicsui/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/rest/aperio.py` & `histomicsui-1.4.4.dev2/histomicsui/rest/aperio.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/rest/hui_resource.py` & `histomicsui-1.4.4.dev2/histomicsui/rest/hui_resource.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/rest/image_browse_resource.py` & `histomicsui-1.4.4.dev2/histomicsui/rest/image_browse_resource.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/rest/system.py` & `histomicsui-1.4.4.dev2/histomicsui/rest/system.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/rest/tcga.py` & `histomicsui-1.4.4.dev2/histomicsui/rest/tcga.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/app.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/app.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/confirmDialog.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/confirmDialog.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/editElement.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/editElement.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/editRegionOfInterest.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/editRegionOfInterest.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/editStyleGroups.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/editStyleGroups.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/metadataPlot.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/metadataPlot.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/openAnnotatedImage.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/openAnnotatedImage.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/openImage.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/openImage.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/saveAnnotation.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/dialogs/saveAnnotation.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/main.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/main.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/panels/AnnotationSelector.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/panels/AnnotationSelector.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/panels/DrawWidget.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/panels/DrawWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/panels/MetadataPlot.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/panels/MetadataPlot.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/panels/MetadataWidget.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/panels/MetadataWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/panels/OverviewWidget.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/panels/OverviewWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/panels/RegionSelector.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/panels/RegionSelector.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/panels/ZoomWidget.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/panels/ZoomWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/router.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/router.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/static/favicon.png` & `histomicsui-1.4.4.dev2/histomicsui/web_client/static/favicon.png`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl` & `histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 #g-dialog-container
   .h-access
     float left
+
 .hui-info-list-entry
   user-select text
+
 .hui-annotation-metadata.hui-annotation-metadata-dialog
   .s-panel-title-container
     background-color #f0f0f0
     padding 5px 6px
     color #555
     font-size 16px
     font-weight bold
     margin-top 8px
     position relative
+
     i.icon-up-open, i.icon-down-open
       display none
+
     .g-widget-metadata-add-button
       margin-top 0
-@media (min-width: 768px)
+
+@media (min-width 768px)
   .modal-dialog.hui-save-annotation-dialog
     width inherit
-@media (min-width: 900px)
+
+@media (min-width 900px)
   .modal-dialog.hui-save-annotation-dialog
     width 70%
     max-width 900px
+
 label.unstyled
   margin-bottom unset
   font-weight normal
   margin-left 4px
+
 .h-functional-value
   input[type="number"]
     width 100px
     margin-left 5px
```

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/layout/header.styl` & `histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/layout/header.styl`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,57 @@
 .hui-body
   #g-app-header-container
     #h-navbar-brand
       font-size 25px
       font-weight 700
+
     .g-header-wrapper
       .h-image-menu-wrapper
         display inline
         float right
+
     .h-help-button
       padding 15px 7px
+
     z-index 1000
-  @media (min-width: 768px)
+
+  @media (min-width 768px)
     .navbar-right
       float none
       margin-right 0
       position absolute
       right 0
       white-space nowrap
       z-index 10
+
     .navbar-nav > li
       float none
       display inline-block
+
     .navbar > .container-fluid .navbar-brand
       margin-left 0
+
     .navbar-text
       float none
+
   .navbar-header
     z-index 20
     float none
     position absolute
     left 0
+
   .navbar-header a#h-navbar-brand.navbar-brand
-      background-color transparent
+    background-color transparent
+
   .navbar-default .navbar-nav
     &> .open > a
       color inherit
       background-color rgba(217, 217, 217, 0.5)
+
     &> .open > a:hover
       color inherit
+
     &> .open > a:focus
       color inherit
+
     &> li > a
       color inherit
```

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/layout/layout.styl` & `histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/layout/layout.styl`

 * *Files 7% similar despite different names*

```diff
@@ -72,9 +72,10 @@
   display flex
   flex-direction column
   flex-wrap nowrap
 
   .s-panel-content
     overflow-y auto
     flex-grow 1
+
   i.icon-up-open
     display none
```

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/annotationSelector.styl` & `histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/panels/annotationSelector.styl`

 * *Files 8% similar despite different names*

```diff
@@ -5,43 +5,46 @@
   display flex
 
   button.btn
     padding 2px 5px
     margin 0
     background none
 
-  .h-annotation-opacity-container,
-  .h-annotation-fill-opacity-container
-    flex 1 1 0
+  .h-annotation-opacity-container, .h-annotation-fill-opacity-container
+    flex 1 1 0%
     position relative
     margin 2px 5px
 
 .h-annotation
   padding 2px
   line-height 1.1
   font-weight initial
   margin-left 5px
   border-radius 3px
+
   span
     cursor pointer
+
   .h-float-left
     float left
     margin-right 0.5em
 
   .h-annotation-right
     float right
 
   a
     color #333
+
   .h-annotation-name
     width 170px
     display inline-block
     text-overflow ellipsis
     white-space nowrap
     overflow hidden
+
   span.partial
     -webkit-mask-image linear-gradient(225deg, #000, rgba(0, 0, 0, 0))
     mask-image linear-gradient(225deg, #000, rgba(0, 0, 0, 0))
 
 .h-annotation-group-name
   font-weight bold
   text-align left
@@ -82,13 +85,15 @@
 .h-annotation:hover
   background-color #eee
 
 .h-annotation-selector
   .s-panel-title
     .save-mark
       display none
+
 .h-annotation-selector.saving
   .s-panel-title
     .icon-tags
       display none
+
     .save-mark
       display inherit
```

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/drawWidget.styl` & `histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/panels/drawWidget.styl`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 .h-elements-container
-    width 100%
-    max-height 300px
-    overflow-y auto
-    margin-top 5px
-    padding 3px 5px
-
-    .h-element
-        border-radius 3px
-        span
-            cursor pointer
-
-        .h-element-label
-            margin-left 5px
-            white-space nowrap
-            overflow hidden
-            display inline-block
-            vertical-align top
-            max-width calc(100% - 75px)
-            text-overflow ellipsis
-
-        .h-view-element
-            margin-left 3px
-            display none
+  width 100%
+  max-height 300px
+  overflow-y auto
+  margin-top 5px
+  padding 3px 5px
+
+  .h-element
+    border-radius 3px
+
+    span
+      cursor pointer
+
+    .h-element-label
+      margin-left 5px
+      white-space nowrap
+      overflow hidden
+      display inline-block
+      vertical-align top
+      max-width calc(100% - 75px)
+      text-overflow ellipsis
 
-        .h-delete-element
-            float right
+    .h-view-element
+      margin-left 3px
+      display none
 
-    .h-element.h-highlight-element
-        background-color #ccc
+    .h-delete-element
+      float right
 
-    .h-element:hover
-        background-color #eee
+  .h-element.h-highlight-element
+    background-color #ccc
+
+  .h-element:hover
+    background-color #eee
 
 .h-save-annotation
-    float right
+  float right
 
 .h-draw-widget
   .h-draw-tools
     .btn-group-sm>.btn
       padding-left 3px
       padding-right 7px
+
     .btn-group-sm>.btn.h-brush-dropdown
       padding-left 0
       padding-right 0
 
   .h-style-group-row
     margin 10px 0
 
@@ -65,19 +67,21 @@
       padding-left 5px
       max-width 200px
 
       .h-group-count-option
         white-space nowrap
         overflow hidden
         text-overflow ellipsis
+
     .h-group-count-select
       padding-left 10px
 
   .btn-default.active
     background-color #5790ff
+
     &:focus, &:hover
       background-color #4672cc
 
   .h-panel-name:before
     content " - "
 
   .h-panel-name
@@ -86,52 +90,65 @@
     white-space nowrap
     text-overflow ellipsis
     font-weight normal
 
   button[data-type="brush"]
     span.shape
       display none
+
   button[data-type="brush"][shape="square"]
     span.shape
       &.square
         display inline
+
   button[data-type="brush"][shape="circle"]
     span.shape
       &.circle
         display inline
 
   .h-dropdown-title i
     pointer-events none
+
   .h-dropdown-content
     position absolute
     background white
     border 2px solid black
     border-radius 5px
     right 0
     top 30px
     padding 5px 10px
+
     .form-group
       margin-bottom 0
       padding 0
+
       input[type="radio"]
         margin-top 2px
+
       input[type="number"]
         margin-left 5px
+
       input[type="checkbox"]
         margin-right 5px
+
   .h-brush-controls
     width 165px
+
   .h-brush-size
     width 60px
+
   .h-fixed-shape-controls
     @extend .h-brush-controls
     z-index 10
     padding 0 25%
+
   .h-fixed-shape-form-group
     height 100%
+
   .h-fixed-width
     width 50%
+
   .h-fixed-height
     width 50%
 
 .flattenicon:before
-  transform: scale(1, 0.67)
+  transform scale(1, 0.67)
```

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/metadataWidget.styl` & `histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/panels/metadataWidget.styl`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     width 100%
     margin 0
     overflow hidden
 
     .jsoneditor-menu
       height initial
       min-height 35px
+
     table.jsoneditor-search
       position initial
 
   .g-widget-metadata-value
     width 59%
 
   button.g-widget-metadata-add-button
```

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/zoomWidget.styl` & `histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/panels/zoomWidget.styl`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
   .h-zoom-range-controls
     line-height 0
     display table-cell
     float left
     width 12px
     padding-left 4px
+
     button
       padding 0
       display inline-block
       font-size 8px
 
 #h-download-submit
   margin-right 8px
```

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/popover/annotationPopover.styl` & `histomicsui-1.4.4.dev2/histomicsui/web_client/stylesheets/popover/annotationPopover.styl`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 #h-annotation-popover-container
-    position absolute
-    pointer-events none
-    margin-left 15px
+  position absolute
+  pointer-events none
+  margin-left 15px
 
-    .h-annotation-popover
-        position absolute
-        width max-content
-        max-width 400px
-        background-color #fff
-        z-index 1100
-        padding 5px 5px 10px
-        border-radius 3px
-        border 1px solid #000
-        box-shadow 0 5px 10px rgba(0, 0, 0, 0.5)
-
-        &:before
-            content ""
-            border-color transparent #000 transparent transparent
-            border-style solid
-            border-width 13px
-            height 0
-            width 0
-            position absolute
-            left -26px
-            top calc(50% - 13px)
-
-        &:after
-            content ""
-            border-color transparent #fff transparent transparent
-            border-style solid
-            border-width 13px
-            height 0
-            width 0
-            position absolute
-            left -25px
-            top calc(50% - 13px)
-
-        > :not(.h-annotation-name)
-            padding 0 20px
-
-        > :not(.h-annotation-description)
-            white-space nowrap
-
-        .h-annotation-description
-            padding-top 10px
-            width 400px
-
-        .h-annotation-name
-            white-space normal
-            font-weight bold
-
-        .h-annotation-creator, .h-annotation-created
-            font-family italic
-
-        .h-annotation-elements
-            font-size 90%
-
-            > table
-                padding-left 10px
-                display inline-block
-
-                td:first-child
-                    font-family monospace
-                    padding-right 10px
-
-                td:nth-child(2)
-                    text-overflow ellipsis
-                    overflow hidden
-                    max-width 300px
+  .h-annotation-popover
+    position absolute
+    width max-content
+    max-width 400px
+    background-color #fff
+    z-index 1100
+    padding 5px 5px 10px
+    border-radius 3px
+    border 1px solid #000
+    box-shadow 0 5px 10px rgba(0, 0, 0, 0.5)
+
+    &:before
+      content ""
+      border-color transparent #000 transparent transparent
+      border-style solid
+      border-width 13px
+      height 0
+      width 0
+      position absolute
+      left -26px
+      top calc(50% - 13px)
+
+    &:after
+      content ""
+      border-color transparent #fff transparent transparent
+      border-style solid
+      border-width 13px
+      height 0
+      width 0
+      position absolute
+      left -25px
+      top calc(50% - 13px)
+
+    > :not(.h-annotation-name)
+      padding 0 20px
+
+    > :not(.h-annotation-description)
+      white-space nowrap
+
+    .h-annotation-description
+      padding-top 10px
+      width 400px
+
+    .h-annotation-name
+      white-space normal
+      font-weight bold
+
+    .h-annotation-creator, .h-annotation-created
+      font-family italic
+
+    .h-annotation-elements
+      font-size 90%
+
+      > table
+        padding-left 10px
+        display inline-block
+
+        td:first-child
+          font-family monospace
+          padding-right 10px
+
+        td:nth-child(2)
+          text-overflow ellipsis
+          overflow hidden
+          max-width 300px
 
-            .h-element-type
-                font-weight bold
+      .h-element-type
+        font-weight bold
```

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/body/configView.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/body/configView.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/body/image.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/body/image.pug`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     .h-image-coordinates-container.hidden
       span.icon-location
       span.h-image-coordinates 0, 0
   .h-control-panel-container.s-panel-group.h-panel-group-left
     #h-analysis-panel
   #h-annotation-selector-container.s-panel-group.h-panel-group-right
     #h-overview-panel.h-overview-widget.s-panel
+    #h-frame-selector-panel.h-frame-selector-widget.s-panel
     #h-zoom-panel.h-zoom-widget.s-panel
     #h-metadata-panel.h-metadata-widget.s-panel
     #h-metadataplot-panel.h-metadata-plot.s-panel
     #h-annotation-panel.h-annotation-selector.s-panel
     #h-draw-panel.h-draw-widget.s-panel.hidden
   #h-annotation-popover-container
   #h-annotation-context-menu.hidden
```

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/editElement.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/editElement.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/editStyleGroups.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/editStyleGroups.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/metadataPlot.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/metadataPlot.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/saveAnnotation.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/dialogs/saveAnnotation.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/header.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/layout/header.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/headerAnalyses.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/layout/headerAnalyses.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/headerImage.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/layout/headerImage.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/headerUser.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/layout/headerUser.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/annotationSelector.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/annotationSelector.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/drawWidget.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/drawWidget.pug`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 extends ./panel.pug
 
 block title
-  | #[span.icon-pencil] #{title} #[span.h-panel-name #{name}]
+  | #[span.icon-pencil] #{title} #[span.h-panel-name(title=name) #{name}]
 
 block content
   .input-group.input-group-sm.h-style-group-row
     select.form-control.h-style-group
       each group in groups.sortBy('id')
         option(value=group.id, selected=group.id === style)
           = group.id
```

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/drawWidgetElement.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/drawWidgetElement.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/metadataWidget.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/metadataWidget.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/zoomWidget.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/panels/zoomWidget.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/popover/annotationContextMenu.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/popover/annotationContextMenu.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/popover/annotationPopover.pug` & `histomicsui-1.4.4.dev2/histomicsui/web_client/templates/popover/annotationPopover.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/views/HierarchyWidget.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/views/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/views/View.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/views/View.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/views/body/ConfigView.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/views/body/ConfigView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/views/body/ImageView.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/views/body/ImageView.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -34,14 +34,15 @@
 
 import AnnotationContextMenu from '../popover/AnnotationContextMenu';
 import AnnotationPopover from '../popover/AnnotationPopover';
 import PixelmapContextMenu from '../popover/PixelmapContextMenu';
 import AnnotationSelector from '../../panels/AnnotationSelector';
 import OverviewWidget from '../../panels/OverviewWidget';
 import ZoomWidget from '../../panels/ZoomWidget';
+import FrameSelectorWidget from '../../panels/FrameSelectorWidget';
 import MetadataWidget from '../../panels/MetadataWidget';
 import MetadataPlot from '../../panels/MetadataPlot';
 import DrawWidget from '../../panels/DrawWidget';
 import editElement from '../../dialogs/editElement';
 import router from '../../router';
 import events from '../../events';
 import {
@@ -100,14 +101,17 @@
         });
         this.overviewWidget = new OverviewWidget({
             parentView: this
         });
         this.zoomWidget = new ZoomWidget({
             parentView: this
         });
+        this.frameSelectorWidget = new FrameSelectorWidget({
+            parentView: this
+        });
         this.metadataWidget = new MetadataWidget({
             parentView: this
         });
         this.metadataPlot = new MetadataPlot({
             parentView: this
         });
         this.annotationSelector = new AnnotationSelector({
@@ -241,14 +245,15 @@
             this.listenTo(this.viewerWidget, 'g:mouseOffAnnotation', this.mouseOffAnnotation);
             this.listenTo(this.viewerWidget, 'g:mouseClickAnnotation', this.mouseClickAnnotation);
             this.listenTo(this.viewerWidget, 'g:mouseResetAnnotation', this.mouseResetAnnotation);
 
             // handle overlay events
             this.listenTo(this.viewerWidget, 'g:mouseClickAnnotationOverlay', this.mouseClickOverlay);
             this.listenTo(this.viewerWidget, 'g:mouseOverAnnotationOverlay', this.mouseOverOverlay);
+            this.listenTo(this.viewerWidget, 'g:mouseDownAnnotationOverlay', this.mouseOverOverlay);
             this.listenTo(this.viewerWidget, 'g:drawOverlayAnnotation', this.overlayLayerDrawn);
             this.listenTo(this.viewerWidget, 'g:removeOverlayAnnotation', this.overlayLayerRemoved);
 
             this.viewerWidget.on('g:imageRendered', () => {
                 events.trigger('h:imageOpened', this.model);
                 // store a reference to the underlying viewer
                 this.viewer = this.viewerWidget.viewer;
@@ -301,14 +306,18 @@
                     .setViewer(this.viewerWidget)
                     .setElement('.h-overview-widget').render();
 
                 this.zoomWidget
                     .setViewer(this.viewerWidget)
                     .setElement('.h-zoom-widget').render();
 
+                this.frameSelectorWidget
+                    .setViewer(this.viewerWidget)
+                    .setElement('.h-frame-selector-widget').render();
+
                 this.metadataWidget
                     .setItem(this.model)
                     .setElement('.h-metadata-widget').render();
 
                 this.metadataPlot
                     .setItem(this.model)
                     .setElement('.h-metadata-plot').render();
@@ -417,14 +426,15 @@
         var getTilesDef = (itemId) => {
             return restRequest({
                 url: 'item/' + itemId + '/tiles'
             }).then((tiles) => {
                 this.zoomWidget.setMaxMagnification(tiles.magnification || 20, this._increaseZoom2x, this._increaseZoom2xRange);
                 this.zoomWidget.render();
                 this.overviewWidget.setImage(tiles);
+                this.frameSelectorWidget.setImage(itemId, tiles);
                 return null;
             });
         };
 
         var getFileModel = (fileId) => {
             return restRequest({
                 url: 'file/' + fileId
@@ -983,15 +993,15 @@
 
     mouseClickOverlay(overlayElement, overlayLayer, event) {
         if (overlayElement.get('type') !== 'pixelmap') {
             return;
         }
         const overlayAnnotationIsSelected = this.activeAnnotation && this.activeAnnotation.elements().get(overlayElement.id);
         const index = overlayElement.get('boundaries') ? (event.index - event.index % 2) : event.index;
-        if (event.mouse.buttonsDown.left && this.drawWidget && overlayAnnotationIsSelected) {
+        if (event.mouse.buttonsDown.left && !event.mouse.modifiers.shift && this.drawWidget && overlayAnnotationIsSelected) {
             // left click. check what the active style is and if it applies
             const style = this.drawWidget.getStyleGroup();
             const newIndex = this._getCategoryIndexFromStyleGroup(overlayElement, style);
 
             const offset = overlayElement.get('boundaries') ? 1 : 0;
             const data = overlayLayer.data();
             const categories = overlayElement.get('categories');
```

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/views/itemList.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/views/itemList.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/views/itemPage.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/views/itemPage.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/HeaderAnalysesView.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/views/layout/HeaderAnalysesView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/HeaderImageView.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/views/layout/HeaderImageView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/HeaderView.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/views/layout/HeaderView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/AnnotationContextMenu.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/views/popover/AnnotationContextMenu.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -61,15 +61,15 @@
     },
     _setStyleDefinition(group) {
         const style = this.styles.get({
             id: group
         }) || this.styles.get({
             id: this.parentView._defaultGroup
         });
-        const styleAttrs = Object.assign({}, style.toJSON());
+        const styleAttrs = Object.assign({}, style ? style.toJSON() : {});
         delete styleAttrs.id;
         let refresh = false;
         this.collection.each((element) => {
             /* eslint-disable backbone/no-silent */
             if (this.parentView.drawWidget && this.parentView.activeAnnotation.id === element.originalAnnotation.id &&
                 element.attributes.group !== group && ['point', 'polyline', 'rectangle', 'ellipse', 'circle'].includes(element.attributes.type)) {
                 this.parentView.drawWidget.updateCount(element.attributes.group || this.parentView._defaultGroup, -1);
```

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/AnnotationPopover.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/views/popover/AnnotationPopover.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/PixelmapContextMenu.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/views/popover/PixelmapContextMenu.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/views/utils.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/views/utils.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/vue/components/ColorPickerInput.vue` & `histomicsui-1.4.4.dev2/histomicsui/web_client/vue/components/ColorPickerInput.vue`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue` & `histomicsui-1.4.4.dev2/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue` & `histomicsui-1.4.4.dev2/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui/web_client/webpack.helper.js` & `histomicsui-1.4.4.dev2/histomicsui/web_client/webpack.helper.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
 module.exports = function(config) {
     config.plugins.push(
         new CopyWebpackPlugin([{
             from: path.join(path.resolve(__dirname), 'static'),
             to: config.output.path,
             toType: 'dir'
         }, {
-            from: path.join(path.resolve(__dirname), 'node_modules', 'sinon', 'pkg', 'sinon.js'),
+            from: require.resolve('sinon/pkg/sinon.js'),
             to: path.join(config.output.path, 'extra', 'sinon.js')
         }])
     );
     config.module.rules.push({
         resource: {
             test: /\.vue$/
         },
```

### Comparing `histomicsui-1.4.3.dev8/histomicsui/webroot.mako` & `histomicsui-1.4.4.dev2/histomicsui/webroot.mako`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/histomicsui.egg-info/PKG-INFO` & `histomicsui-1.4.4.dev2/histomicsui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histomicsui
-Version: 1.4.3.dev8
+Version: 1.4.4.dev2
 Summary: Organize, visualize, and analyze histology images.
 Home-page: https://github.com/DigitalSlideArchive/histomicsui
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,histomicsui
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `histomicsui-1.4.3.dev8/histomicsui.egg-info/SOURCES.txt` & `histomicsui-1.4.4.dev2/histomicsui.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,57 +48,58 @@
 histomicsui/web_client/index.js
 histomicsui/web_client/main.js
 histomicsui/web_client/package.json
 histomicsui/web_client/router.js
 histomicsui/web_client/routes.js
 histomicsui/web_client/webpack.helper.js
 histomicsui/web_client/collections/StyleCollection.js
+histomicsui/web_client/collections/UserCollection.js
 histomicsui/web_client/collections/index.js
 histomicsui/web_client/dialogs/confirmDialog.js
 histomicsui/web_client/dialogs/editElement.js
 histomicsui/web_client/dialogs/editRegionOfInterest.js
 histomicsui/web_client/dialogs/editStyleGroups.js
 histomicsui/web_client/dialogs/index.js
 histomicsui/web_client/dialogs/metadataPlot.js
 histomicsui/web_client/dialogs/openAnnotatedImage.js
 histomicsui/web_client/dialogs/openImage.js
 histomicsui/web_client/dialogs/saveAnnotation.js
 histomicsui/web_client/models/StyleModel.js
 histomicsui/web_client/models/index.js
 histomicsui/web_client/panels/AnnotationSelector.js
 histomicsui/web_client/panels/DrawWidget.js
+histomicsui/web_client/panels/FrameSelectorWidget.js
 histomicsui/web_client/panels/MetadataPlot.js
 histomicsui/web_client/panels/MetadataWidget.js
 histomicsui/web_client/panels/OverviewWidget.js
 histomicsui/web_client/panels/RegionSelector.js
 histomicsui/web_client/panels/ZoomWidget.js
 histomicsui/web_client/panels/index.js
 histomicsui/web_client/static/favicon.png
 histomicsui/web_client/stylesheets/body/configView.styl
-histomicsui/web_client/stylesheets/body/frontPage.styl
 histomicsui/web_client/stylesheets/body/image.styl
 histomicsui/web_client/stylesheets/dialogs/editStyleGroups.styl
 histomicsui/web_client/stylesheets/dialogs/openAnnotatedImage.styl
 histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl
 histomicsui/web_client/stylesheets/layout/header.styl
 histomicsui/web_client/stylesheets/layout/headerAnalyses.styl
 histomicsui/web_client/stylesheets/layout/headerImage.styl
 histomicsui/web_client/stylesheets/layout/layout.styl
 histomicsui/web_client/stylesheets/panels/annotationSelector.styl
 histomicsui/web_client/stylesheets/panels/drawWidget.styl
+histomicsui/web_client/stylesheets/panels/frameSelectorWidget.styl
 histomicsui/web_client/stylesheets/panels/metadataPlot.styl
 histomicsui/web_client/stylesheets/panels/metadataWidget.styl
 histomicsui/web_client/stylesheets/panels/overviewWidget.styl
 histomicsui/web_client/stylesheets/panels/regionSelector.styl
 histomicsui/web_client/stylesheets/panels/zoomWidget.styl
 histomicsui/web_client/stylesheets/popover/annotationContextMenu.styl
 histomicsui/web_client/stylesheets/popover/annotationPopover.styl
 histomicsui/web_client/stylesheets/views/itemList.styl
 histomicsui/web_client/templates/body/configView.pug
-histomicsui/web_client/templates/body/frontPage.pug
 histomicsui/web_client/templates/body/image.pug
 histomicsui/web_client/templates/dialogs/annotatedImageList.pug
 histomicsui/web_client/templates/dialogs/confirmDialog.pug
 histomicsui/web_client/templates/dialogs/editElement.pug
 histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug
 histomicsui/web_client/templates/dialogs/editStyleGroups.pug
 histomicsui/web_client/templates/dialogs/metadataPlot.pug
@@ -109,14 +110,15 @@
 histomicsui/web_client/templates/layout/headerAnalyses.pug
 histomicsui/web_client/templates/layout/headerImage.pug
 histomicsui/web_client/templates/layout/headerUser.pug
 histomicsui/web_client/templates/layout/layout.pug
 histomicsui/web_client/templates/panels/annotationSelector.pug
 histomicsui/web_client/templates/panels/drawWidget.pug
 histomicsui/web_client/templates/panels/drawWidgetElement.pug
+histomicsui/web_client/templates/panels/frameSelectorWidget.pug
 histomicsui/web_client/templates/panels/metadataPlot.pug
 histomicsui/web_client/templates/panels/metadataWidget.pug
 histomicsui/web_client/templates/panels/overviewWidget.pug
 histomicsui/web_client/templates/panels/panel.pug
 histomicsui/web_client/templates/panels/regionSelector.pug
 histomicsui/web_client/templates/panels/zoomWidget.pug
 histomicsui/web_client/templates/popover/annotationContextMenu.pug
@@ -125,15 +127,14 @@
 histomicsui/web_client/views/HierarchyWidget.js
 histomicsui/web_client/views/View.js
 histomicsui/web_client/views/index.js
 histomicsui/web_client/views/itemList.js
 histomicsui/web_client/views/itemPage.js
 histomicsui/web_client/views/utils.js
 histomicsui/web_client/views/body/ConfigView.js
-histomicsui/web_client/views/body/FrontPageView.js
 histomicsui/web_client/views/body/ImageView.js
 histomicsui/web_client/views/body/index.js
 histomicsui/web_client/views/layout/HeaderAnalysesView.js
 histomicsui/web_client/views/layout/HeaderImageView.js
 histomicsui/web_client/views/layout/HeaderUserView.js
 histomicsui/web_client/views/layout/HeaderView.js
 histomicsui/web_client/views/layout/index.js
```

### Comparing `histomicsui-1.4.3.dev8/setup.py` & `histomicsui-1.4.4.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/tests/datastore.py` & `histomicsui-1.4.4.dev2/tests/datastore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 
 import pooch
 
 registry = {
     #
     # Source: Easy1.png
-'Easy1.png': 'sha512:feaf2b24c4ab3123caf1aa35f51acb1d8b83b34941b28d130f878702fd3be4ae9bf46176209f7511d1213da511d414c2b4b7738ad567b089224de9d6c189e664',  # noqa
+    'Easy1.png': 'sha512:feaf2b24c4ab3123caf1aa35f51acb1d8b83b34941b28d130f878702fd3be4ae9bf46176209f7511d1213da511d414c2b4b7738ad567b089224de9d6c189e664',  # noqa
     #
     # Source: sample_svs_image.TCGA-DU-6399-01A-01-TS1.e8eb65de-d63e-42db-af6f-14fefbbdf7bd.svs
-'sample_svs_image.TCGA-DU-6399-01A-01-TS1.e8eb65de-d63e-42db-af6f-14fefbbdf7bd.svs': 'sha512:5580c2b5a5360d279d102f1eb5b0e646a4943e362ec1d47f2db01f8e9e52b302e51692171198d0d35c7fa9ec9f5b8e445ef91fa7ea0bdb05ead31ab49e0118f9',  # noqa
+    'sample_svs_image.TCGA-DU-6399-01A-01-TS1.e8eb65de-d63e-42db-af6f-14fefbbdf7bd.svs': 'sha512:5580c2b5a5360d279d102f1eb5b0e646a4943e362ec1d47f2db01f8e9e52b302e51692171198d0d35c7fa9ec9f5b8e445ef91fa7ea0bdb05ead31ab49e0118f9',  # noqa
 }
 
 
 class DKCPooch(pooch.Pooch):
     def get_url(self, fname):
         self._assert_file_in_registry(fname)
         algo, hashvalue = self.registry[fname].split(':')
```

### Comparing `histomicsui-1.4.3.dev8/tests/girder_utilities.py` & `histomicsui-1.4.4.dev2/tests/girder_utilities.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/tests/test_files/.histomicsui_config.yaml` & `histomicsui-1.4.4.dev2/tests/test_files/.histomicsui_config.yaml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/tests/test_files/test_analysis_detection.xml` & `histomicsui-1.4.4.dev2/tests/test_files/test_analysis_detection.xml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/tests/test_files/test_analysis_features.xml` & `histomicsui-1.4.4.dev2/tests/test_files/test_analysis_features.xml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/tests/test_handlers.py` & `histomicsui-1.4.4.dev2/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/tests/test_hui_rest.py` & `histomicsui-1.4.4.dev2/tests/test_hui_rest.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/tests/test_image_browse_endpoints.py` & `histomicsui-1.4.4.dev2/tests/test_image_browse_endpoints.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/tests/test_tcga.py` & `histomicsui-1.4.4.dev2/tests/test_tcga.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/tests/test_web_client.py` & `histomicsui-1.4.4.dev2/tests/test_web_client.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev8/tests/web_client_specs/analysisSpec.js` & `histomicsui-1.4.4.dev2/tests/web_client_specs/analysisSpec.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,8 @@
-/* global huiTest */
-
-/* global huiTest */
+/* global huiTest girderTest beforeEach girder describe it waitsFor runs $ afterEach expect */
 
 girderTest.importPlugin('jobs', 'large_image', 'large_image_annotation', 'slicer_cli_web', 'histomicsui');
 girderTest.addScript('/static/built/plugins/histomicsui/huiTest.js');
 
 girderTest.promise.done(function() {
     huiTest.startApp();
```

### Comparing `histomicsui-1.4.3.dev8/tests/web_client_specs/annotationSpec.js` & `histomicsui-1.4.4.dev2/tests/web_client_specs/annotationSpec.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/* global huiTest */
+/* global huiTest girderTest beforeEach girder describe it waitsFor runs $ afterEach expect waits _ */
 
 girderTest.importPlugin('jobs', 'large_image', 'large_image_annotation', 'slicer_cli_web', 'histomicsui');
 girderTest.addScript('/static/built/plugins/histomicsui/huiTest.js');
 
 function asciiToUint8Array(text) {
     var l = text.length,
         arr = new Uint8Array(l),
@@ -1357,26 +1357,26 @@
             });
 
             it('show new annotations during job events', function() {
                 var uploaded = false;
 
                 runs(function() {
                     var rect = {
-                        'name': 'rectangle',
-                        'description': 'the description',
-                        'elements': [{
-                            'center': [
+                        name: 'rectangle',
+                        description: 'the description',
+                        elements: [{
+                            center: [
                                 2000,
                                 2000,
                                 0
                             ],
-                            'height': 4000,
-                            'rotation': 0,
-                            'type': 'rectangle',
-                            'width': 4000
+                            height: 4000,
+                            rotation: 0,
+                            type: 'rectangle',
+                            width: 4000
                         }]
                     };
 
                     girder.rest.restRequest({
                         url: 'annotation?itemId=' + huiTest.imageId(),
                         contentType: 'application/json',
                         processData: false,
```

### Comparing `histomicsui-1.4.3.dev8/tests/web_client_specs/girderUISpec.js` & `histomicsui-1.4.4.dev2/tests/web_client_specs/girderUISpec.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,7 +1,9 @@
+/* global girderTest describe it waitsFor runs $ expect _ */
+
 girderTest.importPlugin('jobs', 'large_image', 'large_image_annotation', 'slicer_cli_web', 'histomicsui');
 
 girderTest.startApp();
 
 describe('itemList', function() {
     it('mock Webgl', function() {
         var GeojsViewer = window.girder.plugins.large_image.views.imageViewerWidget.geojs;
```

### Comparing `histomicsui-1.4.3.dev8/tests/web_client_specs/huiSpec.js` & `histomicsui-1.4.4.dev2/tests/web_client_specs/huiSpec.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
-/* globals girder, girderTest, describe, it, expect, waitsFor, runs */
+/* globals girder, girderTest, describe, it, expect, waitsFor, runs, $ */
 
 girderTest.importPlugin('jobs', 'large_image', 'large_image_annotation', 'slicer_cli_web', 'histomicsui');
 
 girderTest.startApp();
 
 describe('Test the HistomicsUI plugin', function() {
     it('change the HistomicsUI settings', function() {
         var styles = [{
-            'lineWidth': 8,
-            'id': 'Sample Group'
+            lineWidth: 8,
+            id: 'Sample Group'
         }];
         var styleJSON = JSON.stringify(styles);
 
         girderTest.login('admin', 'Admin', 'Admin', 'password')();
         waitsFor(function() {
             return $('a.g-nav-link[g-target="admin"]').length > 0;
         }, 'admin console link to load');
```

### Comparing `histomicsui-1.4.3.dev8/tests/web_client_specs/huiTest.js` & `histomicsui-1.4.4.dev2/tests/web_client_specs/huiTest.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,7 +1,9 @@
+/* global waitsFor girderTest $ girder runs expect */
+
 (function(global) {
     global.huiTest = {};
 
     var app;
     var currentImageId;
 
     function waitsForPromise(promise, description) {
```

### Comparing `histomicsui-1.4.3.dev8/tests/web_client_specs/itemSpec.js` & `histomicsui-1.4.4.dev2/tests/web_client_specs/itemSpec.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/* globals girder, girderTest, describe, it, expect, waitsFor, runs */
+/* globals girder, girderTest, describe, it, expect, waitsFor, runs, _, $ */
 
 girderTest.importPlugin('jobs', 'large_image', 'large_image_annotation', 'slicer_cli_web', 'histomicsui');
 
 girderTest.startApp();
 
 describe('Test the HistomicsUI itemUI screen', function() {
     var brandName = 'TestBrandName';
```

### Comparing `histomicsui-1.4.3.dev8/tests/web_client_specs/metadataPanelSpec.js` & `histomicsui-1.4.4.dev2/tests/web_client_specs/metadataPanelSpec.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/* global huiTest */
+/* global huiTest girderTest describe it runs $ expect waitsFor */
 
 girderTest.importPlugin('jobs', 'large_image', 'large_image_annotation', 'slicer_cli_web', 'histomicsui');
 girderTest.addScript('/static/built/plugins/histomicsui/huiTest.js');
 
 girderTest.promise.done(function() {
     huiTest.startApp();
```

### Comparing `histomicsui-1.4.3.dev8/tests/web_client_specs/metadataPlotSpec.js` & `histomicsui-1.4.4.dev2/tests/web_client_specs/metadataPlotSpec.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/* global huiTest */
+/* global huiTest girderTest describe it runs $ expect girder waitsFor */
 
 girderTest.importPlugin('jobs', 'large_image', 'large_image_annotation', 'slicer_cli_web', 'histomicsui');
 girderTest.addScript('/static/built/plugins/histomicsui/huiTest.js');
 
 girderTest.promise.done(function() {
     huiTest.startApp();
```

### Comparing `histomicsui-1.4.3.dev8/tests/web_client_specs/overviewPanelSpec.js` & `histomicsui-1.4.4.dev2/tests/web_client_specs/overviewPanelSpec.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/* global huiTest */
+/* global huiTest girderTest describe it runs expect waitsFor */
 
 girderTest.importPlugin('jobs', 'large_image', 'large_image_annotation', 'slicer_cli_web', 'histomicsui');
 girderTest.addScript('/static/built/plugins/histomicsui/huiTest.js');
 
 girderTest.promise.done(function() {
     huiTest.startApp();
```

### Comparing `histomicsui-1.4.3.dev8/tests/web_client_specs/panelLayoutSpec.js` & `histomicsui-1.4.4.dev2/tests/web_client_specs/panelLayoutSpec.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/* global huiTest */
+/* global huiTest girderTest describe it runs $ expect girder waitsFor */
 
 girderTest.importPlugin('jobs', 'large_image', 'large_image_annotation', 'slicer_cli_web', 'histomicsui');
 girderTest.addScript('/static/built/plugins/histomicsui/huiTest.js');
 
 girderTest.promise.done(function() {
     huiTest.startApp();
 
@@ -51,15 +51,15 @@
                     });
                     expect(leftIds.toArray()).toEqual(['h-zoom-panel', 'h-analysis-panel']);
 
                     var right = $('.h-panel-group-right [id^=h-][id$=-panel]');
                     var rightIds = right.map(function(idx, panel) {
                         return $(panel).attr('id');
                     });
-                    expect(rightIds.toArray()).toEqual(['h-annotation-panel', 'h-metadata-panel', 'h-overview-panel', 'h-metadataplot-panel', 'h-draw-panel']);
+                    expect(rightIds.toArray()).toEqual(['h-annotation-panel', 'h-metadata-panel', 'h-overview-panel', 'h-frame-selector-panel', 'h-metadataplot-panel', 'h-draw-panel']);
                 });
                 waitsFor(function() {
                     return !$('#h-annotation-panel .s-panel-content').hasClass('in');
                 }, 'panel to close');
                 runs(function() {
                     expect($('#h-annotation-panel .s-panel-content').hasClass('in')).toBe(false);
                 });
```

### Comparing `histomicsui-1.4.3.dev8/tests/web_client_specs/pixelmapCategorySpec.js` & `histomicsui-1.4.4.dev2/tests/web_client_specs/pixelmapCategorySpec.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/* globals beforeEach, afterEach, describe, it, expect, girder, backbone, waitsFor, runs, _, huiTest */
+/* globals beforeEach, describe, it, expect, waitsFor, runs, huiTest, $, girderTest, sinon */
 
 girderTest.importPlugin('jobs', 'large_image', 'large_image_annotation', 'slicer_cli_web', 'histomicsui');
 girderTest.addScripts([
     '/static/built/plugins/histomicsui/huiTest.js',
     '/static/built/plugins/histomicsui/extra/sinon.js'
 ]);
 
@@ -46,15 +46,15 @@
                                     strokeColor: 'rgb(0, 0, 0)',
                                     fillColor: 'rgb(0, 0, 0)'
                                 }, {
                                     label: 'category1',
                                     strokeColor: 'rgb(0, 0, 0)',
                                     fillColor: 'rgb(0, 0, 0)'
                                 }],
-                                boundaries: true,
+                                boundaries: true
                             }]
                         })
                     }).then(function(resp) {
                         pixelmapId = resp._id;
                         return null;
                     });
                 });
@@ -64,41 +64,41 @@
                 girderTest.waitForLoad();
                 runs(function() {
                     pixelmapAnnotation = new largeImageAnnotation.models.AnnotationModel({
                         _id: pixelmapId
                     });
                     pixelmapAnnotation.fetch().then(function() {
                         fetched = true;
+                        return null;
                     });
                 });
                 waitsFor(function() {
                     return fetched;
                 });
             });
 
             it('initializes the draw widget', function() {
                 huiTest.app.bodyView.annotations.add(pixelmapAnnotation);
                 huiTest.app.bodyView._editAnnotation(pixelmapAnnotation);
                 runs(function() {
                     expect($('.h-draw-widget').hasClass('hidden')).toBe(false);
                 });
-
             });
 
             it('creates a new style group for categories', function() {
                 pixelmapElement = pixelmapAnnotation.elements().first();
                 var groups = huiTest.app.bodyView.drawWidget._groups;
                 expect(groups.get('category1')).toBeUndefined();
                 huiTest.app.bodyView._reconcilePixelmapCategories(pixelmapElement, groups, pixelmapAnnotation);
                 newCategory = groups.get('category1');
                 expect(newCategory).toBeDefined();
             });
 
             it('creates a new category for style groups', function() {
-                pixelampElement = pixelmapAnnotation.elements().first();
+                pixelmapElement = pixelmapAnnotation.elements().first();
                 var groups = huiTest.app.bodyView.drawWidget._groups;
                 newGroup = new histomicsUI.models.StyleModel({
                     id: 'category2',
                     fillColor: 'rgb(255, 0, 0)',
                     lineColor: 'rgb(255, 0, 0)'
                 });
                 groups.push(newGroup);
@@ -137,48 +137,49 @@
                 var values = pixelmapElement.get('values');
                 expect(categories[0].label).toEqual('default');
                 expect(values[0]).toEqual(1);
                 expect(values[1]).toEqual(0);
                 expect(values[values.length - 1]).toEqual(2);
             });
 
-            it('updates layer data on  left click', function() {
+            it('updates layer data on left click', function() {
                 pixelmapElement.set('values', [1, 1, 1, 1, 1, 1, 1, 1]);
                 var layerData = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1];
                 var clickEvent = {
                     index: 0,
                     mouse: {
                         buttonsDown: {
                             left: true
-                        }
+                        },
+                        modifiers: {}
                     }
                 };
                 var mockLayer = {
                     data: function(newData) {
                         if (newData) {
                             layerData = newData;
                         }
                         return layerData;
                     },
                     indexModified: function(min, max) {
                         return null;
                     },
                     draw: function() {
-                        return null
-                    },
+                        return null;
+                    }
                 };
                 var stubIndexModified = sinon.stub(mockLayer, 'indexModified');
                 stubIndexModified.returns(mockLayer);
                 var stubDraw = sinon.stub(mockLayer, 'draw');
                 stubDebounce = sinon.stub(huiTest.app.bodyView, '_debounceUpdatePixelmapValues');
                 huiTest.app.bodyView.mouseClickOverlay(pixelmapElement, mockLayer, clickEvent);
                 expect(layerData[0]).toEqual(0);
                 expect(layerData[1]).toEqual(0);
                 sinon.assert.called(stubDraw);
-                sinon.assert.called(stubDebounce)
+                sinon.assert.called(stubDebounce);
             });
 
             it('allows click shift and drag', function() {
                 pixelmapElement.set('values', [1, 1, 1, 1, 1, 1, 1, 1]);
                 var layerData = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1];
                 var clickEvent = {
                     index: 1,
@@ -197,15 +198,15 @@
                     },
                     indexModified: function(min, max) {
                         return null;
                     },
                     draw: function() {
                         return null;
                     }
-                }
+                };
                 var stubIndexModified = sinon.stub(mockLayer, 'indexModified');
                 stubIndexModified.returns(mockLayer);
                 var stubDraw = sinon.stub(mockLayer, 'draw');
                 huiTest.app.bodyView.mouseOverOverlay(pixelmapElement, mockLayer, clickEvent);
                 expect(layerData[0]).toEqual(0);
                 expect(layerData[1]).toEqual(0);
                 sinon.assert.called(stubDraw);
@@ -217,40 +218,40 @@
                 pixelmapElement.set('values', [1, 1, 1, 1, 1, 1, 1, 1]);
                 var layerData = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1];
                 var clickEvent = {
                     index: 0,
                     mouse: {
                         buttonsDown: {
                             left: true
-                        }
+                        },
+                        modifiers: {}
                     }
                 };
                 var mockLayer = {
                     data: function(newData) {
                         if (newData) {
                             layerData = newData;
                         }
                         return layerData;
                     },
                     indexModified: function(min, max) {
                         return null;
                     },
                     draw: function() {
-                        return null
-                    },
+                        return null;
+                    }
                 };
                 var stubIndexModified = sinon.stub(mockLayer, 'indexModified');
                 stubIndexModified.returns(mockLayer);
                 var stubDraw = sinon.stub(mockLayer, 'draw');
                 huiTest.app.bodyView.mouseClickOverlay(pixelmapElement, mockLayer, clickEvent);
                 expect(layerData[0]).toEqual(1);
                 expect(layerData[1]).toEqual(1);
                 sinon.assert.notCalled(stubDraw);
                 sinon.assert.calledTwice(stubDebounce);
-
             });
 
             it('does nothing on click and drag if no draw widget', function() {
                 pixelmapElement.set('values', [1, 1, 1, 1, 1, 1, 1, 1]);
                 var layerData = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1];
                 var clickEvent = {
                     index: 1,
@@ -269,24 +270,23 @@
                     },
                     indexModified: function(min, max) {
                         return null;
                     },
                     draw: function() {
                         return null;
                     }
-                }
+                };
                 var stubIndexModified = sinon.stub(mockLayer, 'indexModified');
                 stubIndexModified.returns(mockLayer);
                 var stubDraw = sinon.stub(mockLayer, 'draw');
                 huiTest.app.bodyView.mouseOverOverlay(pixelmapElement, mockLayer, clickEvent);
                 expect(layerData[0]).toEqual(1);
                 expect(layerData[1]).toEqual(1);
                 sinon.assert.notCalled(stubDraw);
                 sinon.assert.calledTwice(stubDebounce);
-
             });
 
             it('opens context menu for right click', function() {
                 pixelmapElement.set('values', [1, 1, 1, 1, 1, 1, 1, 1]);
                 var layerData = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1];
                 var clickEvent = {
                     index: 0,
@@ -307,21 +307,21 @@
                         }
                         return layerData;
                     },
                     indexModified: function(min, max) {
                         return null;
                     },
                     draw: function() {
-                        return null
-                    },
+                        return null;
+                    }
                 };
                 var spyQueueMouse = sinon.spy(huiTest.app.bodyView, '_queueMouseClickAction');
                 huiTest.app.bodyView.mouseClickOverlay(pixelmapElement, mockLayer, clickEvent);
                 sinon.assert.called(spyQueueMouse);
 
                 waitsFor(function() {
                     return huiTest.app.bodyView._pixelmapContextMenuActive === true;
                 });
             });
         });
     });
-})
+});
```

### Comparing `histomicsui-1.4.3.dev8/tox.ini` & `histomicsui-1.4.4.dev2/tox.ini`

 * *Files identical despite different names*

