# Comparing `tmp/photobooth_app-0.1.0b3.tar.gz` & `tmp/photobooth_app-0.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photobooth_app-0.1.0b3.tar", max compression
+gzip compressed data, was "photobooth_app-0.1.0b4.tar", max compression
```

## Comparing `photobooth_app-0.1.0b3.tar` & `photobooth_app-0.1.0b4.tar`

### file list

```diff
@@ -1,102 +1,135 @@
--rw-r--r--   0        0        0     1084 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/LICENSE.md
--rw-r--r--   0        0        0     6586 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/README.md
--rw-r--r--   0        0        0       33 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/__init__.py
--rw-r--r--   0        0        0     3726 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/__main__.py
--rw-r--r--   0        0        0    17065 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/appconfig.py
--rw-r--r--   0        0        0     3322 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/application.py
--rw-r--r--   0        0        0     1427 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/containers.py
--rw-r--r--   0        0        0       36 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/__init__.py
--rw-r--r--   0        0        0     3379 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/aquisition.py
--rw-r--r--   0        0        0     2326 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/config.py
--rw-r--r--   0        0        0      593 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/home.py
--rw-r--r--   0        0        0      770 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/log.py
--rw-r--r--   0        0        0     2133 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/mediacollection.py
--rw-r--r--   0        0        0     3390 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/mediaprocessing.py
--rw-r--r--   0        0        0     1135 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/processing.py
--rw-r--r--   0        0        0     3908 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/sse.py
--rw-r--r--   0        0        0     1942 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/system.py
--rw-r--r--   0        0        0       36 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/services/__init__.py
--rw-r--r--   0        0        0     3121 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/services/aquisitionservice.py
--rw-r--r--   0        0        0      463 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/services/assets/systemservice/boothupload.service
--rw-r--r--   0        0        0      368 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/services/assets/systemservice/boothupload.sh
--rw-r--r--   0        0        0      699 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/services/assets/systemservice/photobooth-app.service
--rw-r--r--   0        0        0       36 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/services/backends/__init__.py
--rw-r--r--   0        0        0     7195 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/services/backends/abstractbackend.py
--rw-r--r--   0        0        0    11560 2023-06-07 20:03:38.741789 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
--rw-r--r--   0        0        0   167336 2023-06-07 20:03:38.741789 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
--rw-r--r--   0        0        0   710982 2023-06-07 20:03:38.745789 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
--rw-r--r--   0        0        0   585221 2023-06-07 20:03:38.749790 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
--rw-r--r--   0        0        0   865667 2023-06-07 20:03:38.753790 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
--rw-r--r--   0        0        0  2314332 2023-06-07 20:03:38.765790 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
--rw-r--r--   0        0        0  2126411 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
--rw-r--r--   0        0        0    43739 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
--rw-r--r--   0        0        0     2618 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/containers.py
--rw-r--r--   0        0        0    10517 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/gphoto2.py
--rw-r--r--   0        0        0    16264 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/picamera2.py
--rw-r--r--   0        0        0     3001 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/picamera2_libcamafcontinuous.py
--rw-r--r--   0        0        0     4473 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/picamera2_libcamafinterval.py
--rw-r--r--   0        0        0     6965 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/simulated.py
--rw-r--r--   0        0        0    10084 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/webcamcv2.py
--rw-r--r--   0        0        0     7597 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/webcamv4l.py
--rw-r--r--   0        0        0      506 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/baseservice.py
--rw-r--r--   0        0        0     3263 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/containers.py
--rw-r--r--   0        0        0     4202 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/informationservice.py
--rw-r--r--   0        0        0     2011 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/keyboardservice.py
--rw-r--r--   0        0        0     6280 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/loggingservice.py
--rw-r--r--   0        0        0       36 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/mediacollection/__init__.py
--rw-r--r--   0        0        0     6853 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/mediacollection/mediaitem.py
--rw-r--r--   0        0        0     6010 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/mediacollectionservice.py
--rw-r--r--   0        0        0     1934 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/mediaprocessing/image_pipelinestages.py
--rw-r--r--   0        0        0    10102 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/mediaprocessingservice.py
--rw-r--r--   0        0        0     8753 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/processingservice.py
--rw-r--r--   0        0        0     4068 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/systemservice.py
--rw-r--r--   0        0        0     5647 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/wledservice.py
--rw-r--r--   0        0        0       93 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/utils/exceptions.py
--rw-r--r--   0        0        0      430 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/utils/fastapi_get_openapi.py
--rw-r--r--   0        0        0      454 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/utils/helper.py
--rw-r--r--   0        0        0      883 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/utils/repeatedtimer.py
--rw-r--r--   0        0        0      621 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/utils/stoppablethread.py
--rw-r--r--   0        0        0    11358 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   168060 2023-06-07 20:03:38.777790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0        0        0   174108 2023-06-07 20:03:38.777790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0        0        0   167336 2023-06-07 20:03:38.777790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2023-06-07 20:03:38.781790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2023-06-07 20:03:38.781790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   167000 2023-06-07 20:03:38.781790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0        0        0   173172 2023-06-07 20:03:38.781790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0        0        0   168644 2023-06-07 20:03:38.785790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0        0        0   173416 2023-06-07 20:03:38.785790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0        0        0   168260 2023-06-07 20:03:38.785790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0   168488 2023-06-07 20:03:38.785790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0        0        0   172860 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0        0        0      144 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/css/31.363e41a9.css
--rw-r--r--   0        0        0       88 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/css/706.42cb67d0.css
--rw-r--r--   0        0        0      163 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/css/71.0be6c807.css
--rw-r--r--   0        0        0      359 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/css/app.f5a22106.css
--rw-r--r--   0        0        0   208939 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/css/vendor.46e03c42.css
--rw-r--r--   0        0        0    64483 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/favicon.ico-todo
--rw-r--r--   0        0        0    20436 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0        0        0    20544 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0        0        0    20416 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0        0        0    20408 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0        0        0    20424 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0        0        0    20344 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0        0        0   164912 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0        0        0   128616 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-r--r--   0        0        0     5336 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/icons/favicon-128x128.png
--rw-r--r--   0        0        0      905 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/index.html
--rw-r--r--   0        0        0     9915 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/js/31.51d7e662.js
--rw-r--r--   0        0        0     2918 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/js/391.70a80bd8.js
--rw-r--r--   0        0        0     1217 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/js/546.92b02def.js
--rw-r--r--   0        0        0     3034 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/js/645.2ddc3ded.js
--rw-r--r--   0        0        0     5660 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/js/692.cf3b55d3.js
--rw-r--r--   0        0        0     3924 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/js/705.fc48b137.js
--rw-r--r--   0        0        0     9305 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/js/706.f32434a0.js
--rw-r--r--   0        0        0     5357 2023-06-07 20:03:38.793790 photobooth_app-0.1.0b3/photobooth/web_spa/js/71.3aaf5d7d.js
--rw-r--r--   0        0        0     1581 2023-06-07 20:03:38.793790 photobooth_app-0.1.0b3/photobooth/web_spa/js/770.b7df615e.js
--rw-r--r--   0        0        0      778 2023-06-07 20:03:38.793790 photobooth_app-0.1.0b3/photobooth/web_spa/js/862.525f2f13.js
--rw-r--r--   0        0        0     1520 2023-06-07 20:03:38.793790 photobooth_app-0.1.0b3/photobooth/web_spa/js/863.e0c5ac02.js
--rw-r--r--   0        0        0    12590 2023-06-07 20:03:38.793790 photobooth_app-0.1.0b3/photobooth/web_spa/js/app.ed0492eb.js
--rw-r--r--   0        0        0  1417500 2023-06-07 20:03:38.797790 photobooth_app-0.1.0b3/photobooth/web_spa/js/vendor.c9e02ba9.js
--rw-r--r--   0        0        0     3966 2023-06-07 20:03:38.797790 photobooth_app-0.1.0b3/pyproject.toml
--rw-r--r--   0        0        0     8075 1970-01-01 00:00:00.000000 photobooth_app-0.1.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/LICENSE.md
+-rw-r--r--   0        0        0     6552 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/README.md
+-rw-r--r--   0        0        0       33 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/__init__.py
+-rw-r--r--   0        0        0     3726 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/__main__.py
+-rw-r--r--   0        0        0    17065 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/appconfig.py
+-rw-r--r--   0        0        0     3322 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/application.py
+-rw-r--r--   0        0        0     1427 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/containers.py
+-rw-r--r--   0        0        0       36 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/__init__.py
+-rw-r--r--   0        0        0     3379 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/aquisition.py
+-rw-r--r--   0        0        0     2326 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/config.py
+-rw-r--r--   0        0        0      593 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/home.py
+-rw-r--r--   0        0        0      770 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/log.py
+-rw-r--r--   0        0        0     2133 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/mediacollection.py
+-rw-r--r--   0        0        0     3390 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/mediaprocessing.py
+-rw-r--r--   0        0        0     1135 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/processing.py
+-rw-r--r--   0        0        0     3908 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/sse.py
+-rw-r--r--   0        0        0     1942 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/system.py
+-rw-r--r--   0        0        0       36 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/__init__.py
+-rw-r--r--   0        0        0     3121 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/aquisitionservice.py
+-rw-r--r--   0        0        0      463 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/assets/systemservice/boothupload.service
+-rw-r--r--   0        0        0      368 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/assets/systemservice/boothupload.sh
+-rw-r--r--   0        0        0      699 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/assets/systemservice/photobooth-app.service
+-rw-r--r--   0        0        0       36 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/backends/__init__.py
+-rw-r--r--   0        0        0     7195 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/backends/abstractbackend.py
+-rw-r--r--   0        0        0    11560 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
+-rw-r--r--   0        0        0   167336 2023-06-09 05:57:53.637930 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   710982 2023-06-09 05:57:53.637930 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
+-rw-r--r--   0        0        0   585221 2023-06-09 05:57:53.641930 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
+-rw-r--r--   0        0        0   865667 2023-06-09 05:57:53.645930 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
+-rw-r--r--   0        0        0  2314332 2023-06-09 05:57:53.661931 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
+-rw-r--r--   0        0        0  2126411 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
+-rw-r--r--   0        0        0    43739 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
+-rw-r--r--   0        0        0     2618 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/containers.py
+-rw-r--r--   0        0        0    10517 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/gphoto2.py
+-rw-r--r--   0        0        0    16264 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/picamera2.py
+-rw-r--r--   0        0        0     3001 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/picamera2_libcamafcontinuous.py
+-rw-r--r--   0        0        0     4473 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/picamera2_libcamafinterval.py
+-rw-r--r--   0        0        0     6965 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/simulated.py
+-rw-r--r--   0        0        0    10084 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/webcamcv2.py
+-rw-r--r--   0        0        0     7597 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/webcamv4l.py
+-rw-r--r--   0        0        0      506 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/baseservice.py
+-rw-r--r--   0        0        0     3207 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/containers.py
+-rw-r--r--   0        0        0     4202 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/informationservice.py
+-rw-r--r--   0        0        0     2022 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/keyboardservice.py
+-rw-r--r--   0        0        0     6280 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/loggingservice.py
+-rw-r--r--   0        0        0       36 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/mediacollection/__init__.py
+-rw-r--r--   0        0        0     6853 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/mediacollection/mediaitem.py
+-rw-r--r--   0        0        0     6010 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/mediacollectionservice.py
+-rw-r--r--   0        0        0     1934 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/mediaprocessing/image_pipelinestages.py
+-rw-r--r--   0        0        0    10102 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/mediaprocessingservice.py
+-rw-r--r--   0        0        0     8753 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/processingservice.py
+-rw-r--r--   0        0        0     4068 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/systemservice.py
+-rw-r--r--   0        0        0     5647 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/wledservice.py
+-rw-r--r--   0        0        0       93 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/utils/exceptions.py
+-rw-r--r--   0        0        0      430 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/utils/fastapi_get_openapi.py
+-rw-r--r--   0        0        0      454 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/utils/helper.py
+-rw-r--r--   0        0        0      883 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/utils/repeatedtimer.py
+-rw-r--r--   0        0        0      621 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/utils/stoppablethread.py
+-rw-r--r--   0        0        0    11358 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   168060 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0        0        0   174108 2023-06-09 05:57:53.673931 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0        0        0   167336 2023-06-09 05:57:53.673931 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2023-06-09 05:57:53.673931 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2023-06-09 05:57:53.677932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   167000 2023-06-09 05:57:53.677932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0        0        0   173172 2023-06-09 05:57:53.677932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0        0        0   168644 2023-06-09 05:57:53.677932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0        0        0   173416 2023-06-09 05:57:53.681932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0        0        0   168260 2023-06-09 05:57:53.681932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0   168488 2023-06-09 05:57:53.681932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0        0        0   172860 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0        0        0      483 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/.gitattributes
+-rw-r--r--   0        0        0     2014 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/.gitignore
+-rw-r--r--   0        0        0     6155 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/CHANGES.md
+-rw-r--r--   0        0        0     1064 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/LICENSE.txt
+-rw-r--r--   0        0        0       56 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/MANIFEST.in
+-rw-r--r--   0        0        0      710 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/Makefile
+-rw-r--r--   0        0        0    29447 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/README.md
+-rw-r--r--   0        0        0      131 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/10_second_macro.py
+-rw-r--r--   0        0        0      276 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/customizable_hotkey.py
+-rw-r--r--   0        0        0      453 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/pressed_keys.py
+-rw-r--r--   0        0        0      660 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py
+-rw-r--r--   0        0        0     1601 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/segmented_macro.py
+-rw-r--r--   0        0        0      210 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/simulate_held_down.py
+-rw-r--r--   0        0        0      857 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py
+-rw-r--r--   0        0        0      237 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/write.py
+-rw-r--r--   0        0        0    46771 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/__init__.py
+-rw-r--r--   0        0        0      364 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/__main__.py
+-rw-r--r--   0        0        0    29387 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py
+-rw-r--r--   0        0        0    19352 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py
+-rw-r--r--   0        0        0     6457 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py
+-rw-r--r--   0        0        0     2110 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_generic.py
+-rw-r--r--   0        0        0     1551 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py
+-rw-r--r--   0        0        0    36792 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py
+-rw-r--r--   0        0        0      398 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_mouse_event.py
+-rw-r--r--   0        0        0     9984 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py
+-rw-r--r--   0        0        0     5947 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py
+-rw-r--r--   0        0        0     6254 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py
+-rw-r--r--   0        0        0     3384 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py
+-rw-r--r--   0        0        0    20549 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py
+-rw-r--r--   0        0        0     5804 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py
+-rw-r--r--   0        0        0     7608 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/mouse.py
+-rw-r--r--   0        0        0     3794 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/make_release.py
+-rw-r--r--   0        0        0     1333 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/setup.py
+-rw-r--r--   0        0        0      144 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/css/31.363e41a9.css
+-rw-r--r--   0        0        0       88 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/css/706.42cb67d0.css
+-rw-r--r--   0        0        0      163 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/css/71.0be6c807.css
+-rw-r--r--   0        0        0      359 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/css/app.f5a22106.css
+-rw-r--r--   0        0        0   208939 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/css/vendor.46e03c42.css
+-rw-r--r--   0        0        0    64483 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/favicon.ico-todo
+-rw-r--r--   0        0        0    20436 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0        0        0    20544 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0        0        0    20416 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0        0        0    20408 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0        0        0    20424 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0        0        0    20344 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0        0        0   164912 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0        0        0   128616 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-r--r--   0        0        0     5336 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/icons/favicon-128x128.png
+-rw-r--r--   0        0        0      905 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/index.html
+-rw-r--r--   0        0        0     9915 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/31.51d7e662.js
+-rw-r--r--   0        0        0     2918 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/391.70a80bd8.js
+-rw-r--r--   0        0        0     1217 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/546.92b02def.js
+-rw-r--r--   0        0        0     3034 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/645.2ddc3ded.js
+-rw-r--r--   0        0        0     5660 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/692.cf3b55d3.js
+-rw-r--r--   0        0        0     3924 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/705.fc48b137.js
+-rw-r--r--   0        0        0     9305 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/706.f32434a0.js
+-rw-r--r--   0        0        0     5357 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/71.3aaf5d7d.js
+-rw-r--r--   0        0        0     1581 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/770.b7df615e.js
+-rw-r--r--   0        0        0      778 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/862.525f2f13.js
+-rw-r--r--   0        0        0     1520 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/863.e0c5ac02.js
+-rw-r--r--   0        0        0    12590 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/app.ed0492eb.js
+-rw-r--r--   0        0        0  1417500 2023-06-09 05:57:53.697933 photobooth_app-0.1.0b4/photobooth/web_spa/js/vendor.c9e02ba9.js
+-rw-r--r--   0        0        0     3959 2023-06-09 05:57:53.697933 photobooth_app-0.1.0b4/pyproject.toml
+-rw-r--r--   0        0        0     8041 1970-01-01 00:00:00.000000 photobooth_app-0.1.0b4/PKG-INFO
```

### Comparing `photobooth_app-0.1.0b3/LICENSE.md` & `photobooth_app-0.1.0b4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/README.md` & `photobooth_app-0.1.0b4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,29 +33,29 @@
 
 The booth is made from 3d printed parts, [see the documentation ✍ over here](https://github.com/mgrl/photobooth-3d).
 The camera support is mostly ready to use, the frontend is not production ready yet.
 Use [photobooth project](https://photoboothproject.github.io/) as frontend.
 
 ## 💅 Screenshots
 
-![frontpage](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/frontpage.png)
-![gallery list](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/gallery_list.png)
-![gallery detail](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/gallery_detail.png)
-![admin center page dashboard](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_dashboard.png)
-![admin center page config tab backends](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_config_backends.png)
-![admin center page config tab userinterface](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_config_ui.png)
-![admin center page status](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_status.png)
+![frontpage](https://raw.githubusercontent.com/mgrl/photobooth-app/main/screenshots/frontpage.png)
+![gallery list](https://raw.githubusercontent.com/mgrl/photobooth-app/main/screenshots/gallery_list.png)
+![gallery detail](https://raw.githubusercontent.com/mgrl/photobooth-app/main/screenshots/gallery_detail.png)
+![admin center page dashboard](https://raw.githubusercontent.com/mgrl/photobooth-app/main/screenshots/admin_dashboard.png)
+![admin center page config tab backends](https://raw.githubusercontent.com/mgrl/photobooth-app/main/screenshots/admin_config_backends.png)
+![admin center page config tab userinterface](https://raw.githubusercontent.com/mgrl/photobooth-app/main/screenshots/admin_config_ui.png)
+![admin center page status](https://raw.githubusercontent.com/mgrl/photobooth-app/main/screenshots/admin_status.png)
 
 ## 🔧 Installation
 
 ### Prerequisites
 
 - Python 3.9 or later
 - Camera, can be one or two (first camera for stills, second camera for live view)
-  - DSLR: [gphoto2](https://github.com/gonzalo/gphoto2-updater) on linx
+  - DSLR: [gphoto2](https://github.com/gonzalo/gphoto2-updater) on Linux
   - Picamera2: installed and working (test with `libcamera-hello`)
   - Webcamera: no additional prerequisites, ensure camera is working using native system apps
 - Raspberry Pi Bullseye for Picamera2 or any other linux/windows system
 - Turbojpeg (via apt on linux, manually install on windows)
 - [works probably best with 3d printed photobooth and parts listed in the BOM](https://github.com/mgrl/photobooth-3d)
 
 The photobooth app can be used standalone but is not feature complete yet.
```

### Comparing `photobooth_app-0.1.0b3/photobooth/__main__.py` & `photobooth_app-0.1.0b4/photobooth/__main__.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/appconfig.py` & `photobooth_app-0.1.0b4/photobooth/appconfig.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/application.py` & `photobooth_app-0.1.0b4/photobooth/application.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/containers.py` & `photobooth_app-0.1.0b4/photobooth/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/routers/aquisition.py` & `photobooth_app-0.1.0b4/photobooth/routers/aquisition.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/routers/config.py` & `photobooth_app-0.1.0b4/photobooth/routers/config.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/routers/home.py` & `photobooth_app-0.1.0b4/photobooth/routers/home.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/routers/log.py` & `photobooth_app-0.1.0b4/photobooth/routers/log.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/routers/mediacollection.py` & `photobooth_app-0.1.0b4/photobooth/routers/mediacollection.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/routers/mediaprocessing.py` & `photobooth_app-0.1.0b4/photobooth/routers/mediaprocessing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/routers/processing.py` & `photobooth_app-0.1.0b4/photobooth/routers/processing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/routers/sse.py` & `photobooth_app-0.1.0b4/photobooth/routers/sse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/routers/system.py` & `photobooth_app-0.1.0b4/photobooth/routers/system.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/aquisitionservice.py` & `photobooth_app-0.1.0b4/photobooth/services/aquisitionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/assets/systemservice/photobooth-app.service` & `photobooth_app-0.1.0b4/photobooth/services/assets/systemservice/photobooth-app.service`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/abstractbackend.py` & `photobooth_app-0.1.0b4/photobooth/services/backends/abstractbackend.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt` & `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf` & `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg` & `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg` & `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg` & `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg` & `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg` & `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg` & `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/containers.py` & `photobooth_app-0.1.0b4/photobooth/services/backends/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/gphoto2.py` & `photobooth_app-0.1.0b4/photobooth/services/backends/gphoto2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/picamera2.py` & `photobooth_app-0.1.0b4/photobooth/services/backends/picamera2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/picamera2_libcamafcontinuous.py` & `photobooth_app-0.1.0b4/photobooth/services/backends/picamera2_libcamafcontinuous.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/picamera2_libcamafinterval.py` & `photobooth_app-0.1.0b4/photobooth/services/backends/picamera2_libcamafinterval.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/simulated.py` & `photobooth_app-0.1.0b4/photobooth/services/backends/simulated.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/webcamcv2.py` & `photobooth_app-0.1.0b4/photobooth/services/backends/webcamcv2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/backends/webcamv4l.py` & `photobooth_app-0.1.0b4/photobooth/services/backends/webcamv4l.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/containers.py` & `photobooth_app-0.1.0b4/photobooth/services/containers.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from dependency_injector import containers, providers
 from pymitter import EventEmitter
 
 from ..appconfig import AppConfig
 from .aquisitionservice import AquisitionService
 from .informationservice import InformationService
+from .keyboardservice import KeyboardService
 from .mediacollectionservice import MediacollectionService
 from .mediaprocessingservice import MediaprocessingService
 from .processingservice import ProcessingService
 from .systemservice import SystemService
 from .wledservice import WledService
 
 logger = logging.getLogger(__name__)
@@ -92,21 +93,20 @@
         evtbus=evtbus,
         config=config,
         aquisition_service=aquisition_service,
         mediacollection_service=mediacollection_service,
         mediaprocessing_service=mediaprocessing_service,
     )
 
-    # disable for now as lib used is unmaintained. switch to browser based keycode listeners
-    # keyboard_service = providers.Resource(
-    #    KeyboardService,
-    #    evtbus=evtbus,
-    #    config=config,
-    #    processing_service=processing_service,
-    # )
+    keyboard_service = providers.Resource(
+        KeyboardService,
+        evtbus=evtbus,
+        config=config,
+        processing_service=processing_service,
+    )
     system_service = providers.Factory(SystemService, evtbus=evtbus, config=config)
 
     wled_service = providers.Resource(
         init_wled_resource,
         evtbus=evtbus,
         config=config,
     )
```

### Comparing `photobooth_app-0.1.0b3/photobooth/services/informationservice.py` & `photobooth_app-0.1.0b4/photobooth/services/informationservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/keyboardservice.py` & `photobooth_app-0.1.0b4/photobooth/services/keyboardservice.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 hid: untested, needs additional libraries on win/linux to be installed
 evdev: linux only
 sshkeyboard: ?
 """
 import json
 
 from pymitter import EventEmitter
-from vendor.keyboard import keyboard
 
 from ..appconfig import AppConfig
+from ..vendor.packages.keyboard import keyboard
 from .baseservice import BaseService
 from .processingservice import ProcessingService
 
 
 class KeyboardService(BaseService):
     """_summary_"""
```

### Comparing `photobooth_app-0.1.0b3/photobooth/services/loggingservice.py` & `photobooth_app-0.1.0b4/photobooth/services/loggingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/mediacollection/mediaitem.py` & `photobooth_app-0.1.0b4/photobooth/services/mediacollection/mediaitem.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/mediacollectionservice.py` & `photobooth_app-0.1.0b4/photobooth/services/mediacollectionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/mediaprocessing/image_pipelinestages.py` & `photobooth_app-0.1.0b4/photobooth/services/mediaprocessing/image_pipelinestages.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/mediaprocessingservice.py` & `photobooth_app-0.1.0b4/photobooth/services/mediaprocessingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/processingservice.py` & `photobooth_app-0.1.0b4/photobooth/services/processingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/systemservice.py` & `photobooth_app-0.1.0b4/photobooth/services/systemservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/services/wledservice.py` & `photobooth_app-0.1.0b4/photobooth/services/wledservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/utils/repeatedtimer.py` & `photobooth_app-0.1.0b4/photobooth/utils/repeatedtimer.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/utils/stoppablethread.py` & `photobooth_app-0.1.0b4/photobooth/utils/stoppablethread.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/LICENSE.txt` & `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf` & `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf` & `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf` & `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf` & `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf` & `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf` & `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf` & `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf` & `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf` & `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf` & `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf` & `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf` & `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/css/vendor.46e03c42.css` & `photobooth_app-0.1.0b4/photobooth/web_spa/css/vendor.46e03c42.css`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/favicon.ico-todo` & `photobooth_app-0.1.0b4/photobooth/web_spa/favicon.ico-todo`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/icons/favicon-128x128.png` & `photobooth_app-0.1.0b4/photobooth/web_spa/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/index.html` & `photobooth_app-0.1.0b4/photobooth/web_spa/index.html`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/js/31.51d7e662.js` & `photobooth_app-0.1.0b4/photobooth/web_spa/js/31.51d7e662.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/js/391.70a80bd8.js` & `photobooth_app-0.1.0b4/photobooth/web_spa/js/391.70a80bd8.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/js/546.92b02def.js` & `photobooth_app-0.1.0b4/photobooth/web_spa/js/546.92b02def.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/js/645.2ddc3ded.js` & `photobooth_app-0.1.0b4/photobooth/web_spa/js/645.2ddc3ded.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/js/692.cf3b55d3.js` & `photobooth_app-0.1.0b4/photobooth/web_spa/js/692.cf3b55d3.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/js/705.fc48b137.js` & `photobooth_app-0.1.0b4/photobooth/web_spa/js/705.fc48b137.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/js/706.f32434a0.js` & `photobooth_app-0.1.0b4/photobooth/web_spa/js/706.f32434a0.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/js/71.3aaf5d7d.js` & `photobooth_app-0.1.0b4/photobooth/web_spa/js/71.3aaf5d7d.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/js/770.b7df615e.js` & `photobooth_app-0.1.0b4/photobooth/web_spa/js/770.b7df615e.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/js/862.525f2f13.js` & `photobooth_app-0.1.0b4/photobooth/web_spa/js/862.525f2f13.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/js/863.e0c5ac02.js` & `photobooth_app-0.1.0b4/photobooth/web_spa/js/863.e0c5ac02.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/js/app.ed0492eb.js` & `photobooth_app-0.1.0b4/photobooth/web_spa/js/app.ed0492eb.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/photobooth/web_spa/js/vendor.c9e02ba9.js` & `photobooth_app-0.1.0b4/photobooth/web_spa/js/vendor.c9e02ba9.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b3/pyproject.toml` & `photobooth_app-0.1.0b4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2270 686f 746f 626f 6f74 682d 6170  = "photobooth-ap
 00000020: 7022 0d0a 7265 7175 6972 6573 2d70 7974  p"..requires-pyt
 00000030: 686f 6e20 3d20 223e 3d33 2e39 2c3c 332e  hon = ">=3.9,<3.
 00000040: 3132 220d 0a76 6572 7369 6f6e 203d 2022  12"..version = "
-00000050: 302e 312e 3062 3322 0d0a 6465 7363 7269  0.1.0b3"..descri
+00000050: 302e 312e 3062 3422 0d0a 6465 7363 7269  0.1.0b4"..descri
 00000060: 7074 696f 6e20 3d20 2250 686f 746f 626f  ption = "Photobo
 00000070: 6f74 6820 6170 7020 7772 6974 7465 6e20  oth app written 
 00000080: 696e 2050 7974 686f 6e20 7375 7070 6f72  in Python suppor
 00000090: 7469 6e67 2044 534c 522c 2070 6963 616d  ting DSLR, picam
 000000a0: 6572 6132 2c20 7765 6263 616d 6572 6173  era2, webcameras
 000000b0: 220d 0a61 7574 686f 7273 203d 205b 7b20  "..authors = [{ 
 000000c0: 6e61 6d65 203d 2022 4d69 6368 6165 6c20  name = "Michael 
@@ -68,15 +68,15 @@
 00000430: 656e 7461 7469 6f6e 203d 2022 6874 7470  entation = "http
 00000440: 733a 2f2f 6d67 726c 2e67 6974 6875 622e  s://mgrl.github.
 00000450: 696f 2f70 686f 746f 626f 6f74 682d 646f  io/photobooth-do
 00000460: 6373 220d 0a0d 0a0d 0a5b 746f 6f6c 2e70  cs"......[tool.p
 00000470: 6f65 7472 795d 0d0a 6e61 6d65 203d 2022  oetry]..name = "
 00000480: 7068 6f74 6f62 6f6f 7468 2d61 7070 220d  photobooth-app".
 00000490: 0a76 6572 7369 6f6e 203d 2022 302e 312e  .version = "0.1.
-000004a0: 3062 3322 0d0a 6465 7363 7269 7074 696f  0b3"..descriptio
+000004a0: 3062 3422 0d0a 6465 7363 7269 7074 696f  0b4"..descriptio
 000004b0: 6e20 3d20 2250 686f 746f 626f 6f74 6820  n = "Photobooth 
 000004c0: 6170 7020 7772 6974 7465 6e20 696e 2050  app written in P
 000004d0: 7974 686f 6e20 7375 7070 6f72 7469 6e67  ython supporting
 000004e0: 2044 534c 522c 2070 6963 616d 6572 6132   DSLR, picamera2
 000004f0: 2c20 7765 6263 616d 6572 6173 220d 0a61  , webcameras"..a
 00000500: 7574 686f 7273 203d 205b 224d 6963 6861  uthors = ["Micha
 00000510: 656c 2047 203c 6d65 406d 6772 6c2e 6465  el G <me@mgrl.de
@@ -170,79 +170,79 @@
 00000a90: 2e70 6f65 7472 792e 6772 6f75 702e 6465  .poetry.group.de
 00000aa0: 762e 6465 7065 6e64 656e 6369 6573 5d0d  v.dependencies].
 00000ab0: 0a70 7974 6573 7420 3d20 225e 372e 322e  .pytest = "^7.2.
 00000ac0: 3022 0d0a 7079 7465 7374 2d62 656e 6368  0"..pytest-bench
 00000ad0: 6d61 726b 203d 2022 5e34 2e30 2e30 220d  mark = "^4.0.0".
 00000ae0: 0a70 7974 6573 742d 636f 7620 3d20 225e  .pytest-cov = "^
 00000af0: 342e 302e 3022 0d0a 7275 6666 203d 2022  4.0.0"..ruff = "
-00000b00: 5e30 2e30 2e32 3730 220d 0a68 7474 7078  ^0.0.270"..httpx
-00000b10: 2d73 7365 203d 2022 5e30 2e33 2e31 220d  -sse = "^0.3.1".
-00000b20: 0a68 7474 7078 203d 2022 5e30 2e32 342e  .httpx = "^0.24.
-00000b30: 3122 0d0a 7369 6d70 6c65 6a70 6567 203d  1"..simplejpeg =
-00000b40: 2022 5e31 2e36 2e36 220d 0a63 6f76 6572   "^1.6.6"..cover
-00000b50: 6167 6520 3d20 7b65 7874 7261 7320 3d20  age = {extras = 
-00000b60: 5b22 746f 6d6c 225d 2c20 7665 7273 696f  ["toml"], versio
-00000b70: 6e20 3d20 225e 372e 322e 3722 7d0d 0a0d  n = "^7.2.7"}...
-00000b80: 0a5b 6275 696c 642d 7379 7374 656d 5d0d  .[build-system].
-00000b90: 0a72 6571 7569 7265 7320 3d20 5b22 706f  .requires = ["po
-00000ba0: 6574 7279 2d63 6f72 6522 5d0d 0a62 7569  etry-core"]..bui
-00000bb0: 6c64 2d62 6163 6b65 6e64 203d 2022 706f  ld-backend = "po
-00000bc0: 6574 7279 2e63 6f72 652e 6d61 736f 6e72  etry.core.masonr
-00000bd0: 792e 6170 6922 0d0a 0d0a 0d0a 5b74 6f6f  y.api"......[too
-00000be0: 6c2e 7079 7465 7374 2e69 6e69 5f6f 7074  l.pytest.ini_opt
-00000bf0: 696f 6e73 5d0d 0a6c 6f67 5f63 6c69 203d  ions]..log_cli =
-00000c00: 2074 7275 650d 0a6c 6f67 5f63 6c69 5f6c   true..log_cli_l
-00000c10: 6576 656c 203d 2022 4445 4255 4722 0d0a  evel = "DEBUG"..
-00000c20: 6c6f 675f 636c 695f 666f 726d 6174 203d  log_cli_format =
-00000c30: 2022 2528 6173 6374 696d 6529 7320 5b25   "%(asctime)s [%
-00000c40: 286c 6576 656c 6e61 6d65 2938 735d 2025  (levelname)8s] %
-00000c50: 286d 6573 7361 6765 2973 2028 2528 6669  (message)s (%(fi
-00000c60: 6c65 6e61 6d65 2973 3a25 286c 696e 656e  lename)s:%(linen
-00000c70: 6f29 7329 220d 0a6c 6f67 5f63 6c69 5f64  o)s)"..log_cli_d
-00000c80: 6174 655f 666f 726d 6174 203d 2022 2559  ate_format = "%Y
-00000c90: 2d25 6d2d 2564 2025 483a 254d 3a25 5322  -%m-%d %H:%M:%S"
-00000ca0: 0d0a 0d0a 5b74 6f6f 6c2e 636f 7665 7261  ....[tool.covera
-00000cb0: 6765 2e72 756e 5d0d 0a23 2064 6973 6162  ge.run]..# disab
-00000cc0: 6c65 2063 6f75 6c64 6e74 2d70 6172 7365  le couldnt-parse
-00000cd0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-00000ce0: 2e63 6f6d 2f6e 6564 6261 742f 636f 7665  .com/nedbat/cove
-00000cf0: 7261 6765 7079 2f69 7373 7565 732f 3133  ragepy/issues/13
-00000d00: 3932 0d0a 6469 7361 626c 655f 7761 726e  92..disable_warn
-00000d10: 696e 6773 203d 205b 2263 6f75 6c64 6e74  ings = ["couldnt
-00000d20: 2d70 6172 7365 225d 0d0a 6f6d 6974 203d  -parse"]..omit =
-00000d30: 205b 0d0a 2020 2020 2269 6e73 7461 6c6c   [..    "install
-00000d40: 2e70 7922 2c0d 0a20 2020 2022 7465 7374  .py",..    "test
-00000d50: 5f2a 2e70 7922 2c0d 0a20 2020 2022 2e2f  _*.py",..    "./
-00000d60: 7465 7374 732f 2a22 0d0a 2020 2020 5d0d  tests/*"..    ].
-00000d70: 0a70 6172 616c 6c65 6c20 3d20 7472 7565  .parallel = true
-00000d80: 0d0a 636f 6e63 7572 7265 6e63 7920 3d20  ..concurrency = 
-00000d90: 5b22 7468 7265 6164 222c 226d 756c 7469  ["thread","multi
-00000da0: 7072 6f63 6573 7369 6e67 225d 0d0a 0d0a  processing"]....
-00000db0: 5b74 6f6f 6c2e 626c 6163 6b5d 0d0a 6c69  [tool.black]..li
-00000dc0: 6e65 2d6c 656e 6774 6820 3d20 3132 300d  ne-length = 120.
-00000dd0: 0a0d 0a5b 746f 6f6c 2e72 7566 665d 0d0a  ...[tool.ruff]..
-00000de0: 6c69 6e65 2d6c 656e 6774 6820 3d20 3132  line-length = 12
-00000df0: 300d 0a73 656c 6563 7420 3d20 5b0d 0a20  0..select = [.. 
-00000e00: 2022 4522 2c20 2020 2320 7079 636f 6465   "E",   # pycode
-00000e10: 7374 796c 650d 0a20 2022 5722 2c20 2020  style..  "W",   
-00000e20: 2320 7079 636f 6465 7374 796c 650d 0a20  # pycodestyle.. 
-00000e30: 2022 4622 2c20 2020 2320 7079 666c 616b   "F",   # pyflak
-00000e40: 6573 0d0a 2020 2242 222c 2020 2023 2062  es..  "B",   # b
-00000e50: 7567 6265 6172 0d0a 2020 2255 5022 2c20  ugbear..  "UP", 
-00000e60: 2023 2070 7975 7067 7261 6465 0d0a 2020   # pyupgrade..  
-00000e70: 2249 222c 2020 2023 2069 736f 7274 0d0a  "I",   # isort..
-00000e80: 2020 2322 4422 2c20 2020 2320 7079 646f    #"D",   # pydo
-00000e90: 6373 7479 6c65 2020 2023 2061 6464 206c  cstyle   # add l
-00000ea0: 6174 6572 0d0a 5d0d 0a69 676e 6f72 6520  ater..]..ignore 
-00000eb0: 3d20 5b0d 0a20 2022 4230 3038 2220 2375  = [..  "B008" #u
-00000ec0: 7365 6420 666f 7220 4449 2069 6e6a 6563  sed for DI injec
-00000ed0: 7469 6f6e 0d0a 2020 5d0d 0a65 7874 656e  tion..  ]..exten
-00000ee0: 642d 6578 636c 7564 6520 3d20 5b22 2e2f  d-exclude = ["./
-00000ef0: 7363 7269 7074 7322 2c20 2269 6e73 7461  scripts", "insta
-00000f00: 6c6c 2e70 7922 5d0d 0a0d 0a5b 746f 6f6c  ll.py"]....[tool
-00000f10: 2e72 7566 662e 7065 722d 6669 6c65 2d69  .ruff.per-file-i
-00000f20: 676e 6f72 6573 5d0d 0a22 7068 6f74 6f62  gnores].."photob
-00000f30: 6f6f 7468 2f61 7070 636f 6e66 6967 2e70  ooth/appconfig.p
-00000f40: 7922 203d 205b 2245 3530 3122 5d0d 0a0d  y" = ["E501"]...
-00000f50: 0a5b 746f 6f6c 2e72 7566 662e 7079 646f  .[tool.ruff.pydo
-00000f60: 6373 7479 6c65 5d0d 0a63 6f6e 7665 6e74  cstyle]..convent
-00000f70: 696f 6e20 3d20 2267 6f6f 676c 6522       ion = "google"
+00000b00: 3e3d 302e 302e 3237 302c 3c30 2e30 2e32  >=0.0.270,<0.0.2
+00000b10: 3733 220d 0a68 7474 7078 2d73 7365 203d  73"..httpx-sse =
+00000b20: 2022 5e30 2e33 2e31 220d 0a68 7474 7078   "^0.3.1"..httpx
+00000b30: 203d 2022 5e30 2e32 342e 3122 0d0a 7369   = "^0.24.1"..si
+00000b40: 6d70 6c65 6a70 6567 203d 2022 5e31 2e36  mplejpeg = "^1.6
+00000b50: 2e36 220d 0a63 6f76 6572 6167 6520 3d20  .6"..coverage = 
+00000b60: 7b65 7874 7261 7320 3d20 5b22 746f 6d6c  {extras = ["toml
+00000b70: 225d 2c20 7665 7273 696f 6e20 3d20 225e  "], version = "^
+00000b80: 372e 322e 3722 7d0d 0a0d 0a5b 6275 696c  7.2.7"}....[buil
+00000b90: 642d 7379 7374 656d 5d0d 0a72 6571 7569  d-system]..requi
+00000ba0: 7265 7320 3d20 5b22 706f 6574 7279 2d63  res = ["poetry-c
+00000bb0: 6f72 6522 5d0d 0a62 7569 6c64 2d62 6163  ore"]..build-bac
+00000bc0: 6b65 6e64 203d 2022 706f 6574 7279 2e63  kend = "poetry.c
+00000bd0: 6f72 652e 6d61 736f 6e72 792e 6170 6922  ore.masonry.api"
+00000be0: 0d0a 0d0a 0d0a 5b74 6f6f 6c2e 7079 7465  ......[tool.pyte
+00000bf0: 7374 2e69 6e69 5f6f 7074 696f 6e73 5d0d  st.ini_options].
+00000c00: 0a6c 6f67 5f63 6c69 203d 2074 7275 650d  .log_cli = true.
+00000c10: 0a6c 6f67 5f63 6c69 5f6c 6576 656c 203d  .log_cli_level =
+00000c20: 2022 4445 4255 4722 0d0a 6c6f 675f 636c   "DEBUG"..log_cl
+00000c30: 695f 666f 726d 6174 203d 2022 2528 6173  i_format = "%(as
+00000c40: 6374 696d 6529 7320 5b25 286c 6576 656c  ctime)s [%(level
+00000c50: 6e61 6d65 2938 735d 2025 286d 6573 7361  name)8s] %(messa
+00000c60: 6765 2973 2028 2528 6669 6c65 6e61 6d65  ge)s (%(filename
+00000c70: 2973 3a25 286c 696e 656e 6f29 7329 220d  )s:%(lineno)s)".
+00000c80: 0a6c 6f67 5f63 6c69 5f64 6174 655f 666f  .log_cli_date_fo
+00000c90: 726d 6174 203d 2022 2559 2d25 6d2d 2564  rmat = "%Y-%m-%d
+00000ca0: 2025 483a 254d 3a25 5322 0d0a 0d0a 5b74   %H:%M:%S"....[t
+00000cb0: 6f6f 6c2e 636f 7665 7261 6765 2e72 756e  ool.coverage.run
+00000cc0: 5d0d 0a23 2064 6973 6162 6c65 2063 6f75  ]..# disable cou
+00000cd0: 6c64 6e74 2d70 6172 7365 3a20 6874 7470  ldnt-parse: http
+00000ce0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
+00000cf0: 6564 6261 742f 636f 7665 7261 6765 7079  edbat/coveragepy
+00000d00: 2f69 7373 7565 732f 3133 3932 0d0a 6469  /issues/1392..di
+00000d10: 7361 626c 655f 7761 726e 696e 6773 203d  sable_warnings =
+00000d20: 205b 2263 6f75 6c64 6e74 2d70 6172 7365   ["couldnt-parse
+00000d30: 225d 0d0a 6f6d 6974 203d 205b 0d0a 2020  "]..omit = [..  
+00000d40: 2020 2269 6e73 7461 6c6c 2e70 7922 2c0d    "install.py",.
+00000d50: 0a20 2020 2022 7465 7374 5f2a 2e70 7922  .    "test_*.py"
+00000d60: 2c0d 0a20 2020 2022 2e2f 7465 7374 732f  ,..    "./tests/
+00000d70: 2a22 0d0a 2020 2020 5d0d 0a70 6172 616c  *"..    ]..paral
+00000d80: 6c65 6c20 3d20 7472 7565 0d0a 636f 6e63  lel = true..conc
+00000d90: 7572 7265 6e63 7920 3d20 5b22 7468 7265  urrency = ["thre
+00000da0: 6164 222c 226d 756c 7469 7072 6f63 6573  ad","multiproces
+00000db0: 7369 6e67 225d 0d0a 0d0a 5b74 6f6f 6c2e  sing"]....[tool.
+00000dc0: 626c 6163 6b5d 0d0a 6c69 6e65 2d6c 656e  black]..line-len
+00000dd0: 6774 6820 3d20 3132 300d 0a0d 0a5b 746f  gth = 120....[to
+00000de0: 6f6c 2e72 7566 665d 0d0a 6c69 6e65 2d6c  ol.ruff]..line-l
+00000df0: 656e 6774 6820 3d20 3132 300d 0a73 656c  ength = 120..sel
+00000e00: 6563 7420 3d20 5b0d 0a20 2022 4522 2c20  ect = [..  "E", 
+00000e10: 2020 2320 7079 636f 6465 7374 796c 650d    # pycodestyle.
+00000e20: 0a20 2022 5722 2c20 2020 2320 7079 636f  .  "W",   # pyco
+00000e30: 6465 7374 796c 650d 0a20 2022 4622 2c20  destyle..  "F", 
+00000e40: 2020 2320 7079 666c 616b 6573 0d0a 2020    # pyflakes..  
+00000e50: 2242 222c 2020 2023 2062 7567 6265 6172  "B",   # bugbear
+00000e60: 0d0a 2020 2255 5022 2c20 2023 2070 7975  ..  "UP",  # pyu
+00000e70: 7067 7261 6465 0d0a 2020 2249 222c 2020  pgrade..  "I",  
+00000e80: 2023 2069 736f 7274 0d0a 2020 2322 4422   # isort..  #"D"
+00000e90: 2c20 2020 2320 7079 646f 6373 7479 6c65  ,   # pydocstyle
+00000ea0: 2020 2023 2061 6464 206c 6174 6572 0d0a     # add later..
+00000eb0: 5d0d 0a69 676e 6f72 6520 3d20 5b0d 0a20  ]..ignore = [.. 
+00000ec0: 2022 4230 3038 2220 2375 7365 6420 666f   "B008" #used fo
+00000ed0: 7220 4449 2069 6e6a 6563 7469 6f6e 0d0a  r DI injection..
+00000ee0: 2020 5d0d 0a65 7874 656e 642d 6578 636c    ]..extend-excl
+00000ef0: 7564 6520 3d20 5b22 7665 6e64 6f72 225d  ude = ["vendor"]
+00000f00: 0d0a 0d0a 5b74 6f6f 6c2e 7275 6666 2e70  ....[tool.ruff.p
+00000f10: 6572 2d66 696c 652d 6967 6e6f 7265 735d  er-file-ignores]
+00000f20: 0d0a 2270 686f 746f 626f 6f74 682f 6170  .."photobooth/ap
+00000f30: 7063 6f6e 6669 672e 7079 2220 3d20 5b22  pconfig.py" = ["
+00000f40: 4535 3031 225d 0d0a 0d0a 5b74 6f6f 6c2e  E501"]....[tool.
+00000f50: 7275 6666 2e70 7964 6f63 7374 796c 655d  ruff.pydocstyle]
+00000f60: 0d0a 636f 6e76 656e 7469 6f6e 203d 2022  ..convention = "
+00000f70: 676f 6f67 6c65 22                        google"
```

### Comparing `photobooth_app-0.1.0b3/PKG-INFO` & `photobooth_app-0.1.0b4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photobooth-app
-Version: 0.1.0b3
+Version: 0.1.0b4
 Summary: Photobooth app written in Python supporting DSLR, picamera2, webcameras
 Home-page: https://github.com/mgrl/photobooth-app
 License: MIT
 Author: Michael G
 Author-email: me@mgrl.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -71,29 +71,29 @@
 
 The booth is made from 3d printed parts, [see the documentation ✍ over here](https://github.com/mgrl/photobooth-3d).
 The camera support is mostly ready to use, the frontend is not production ready yet.
 Use [photobooth project](https://photoboothproject.github.io/) as frontend.
 
 ## 💅 Screenshots
 
-![frontpage](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/frontpage.png)
-![gallery list](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/gallery_list.png)
-![gallery detail](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/gallery_detail.png)
-![admin center page dashboard](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_dashboard.png)
-![admin center page config tab backends](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_config_backends.png)
-![admin center page config tab userinterface](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_config_ui.png)
-![admin center page status](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_status.png)
+![frontpage](https://raw.githubusercontent.com/mgrl/photobooth-app/main/screenshots/frontpage.png)
+![gallery list](https://raw.githubusercontent.com/mgrl/photobooth-app/main/screenshots/gallery_list.png)
+![gallery detail](https://raw.githubusercontent.com/mgrl/photobooth-app/main/screenshots/gallery_detail.png)
+![admin center page dashboard](https://raw.githubusercontent.com/mgrl/photobooth-app/main/screenshots/admin_dashboard.png)
+![admin center page config tab backends](https://raw.githubusercontent.com/mgrl/photobooth-app/main/screenshots/admin_config_backends.png)
+![admin center page config tab userinterface](https://raw.githubusercontent.com/mgrl/photobooth-app/main/screenshots/admin_config_ui.png)
+![admin center page status](https://raw.githubusercontent.com/mgrl/photobooth-app/main/screenshots/admin_status.png)
 
 ## 🔧 Installation
 
 ### Prerequisites
 
 - Python 3.9 or later
 - Camera, can be one or two (first camera for stills, second camera for live view)
-  - DSLR: [gphoto2](https://github.com/gonzalo/gphoto2-updater) on linx
+  - DSLR: [gphoto2](https://github.com/gonzalo/gphoto2-updater) on Linux
   - Picamera2: installed and working (test with `libcamera-hello`)
   - Webcamera: no additional prerequisites, ensure camera is working using native system apps
 - Raspberry Pi Bullseye for Picamera2 or any other linux/windows system
 - Turbojpeg (via apt on linux, manually install on windows)
 - [works probably best with 3d printed photobooth and parts listed in the BOM](https://github.com/mgrl/photobooth-3d)
 
 The photobooth app can be used standalone but is not feature complete yet.
```

