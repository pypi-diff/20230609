# Comparing `tmp/ionicons_python-1.0.0.tar.gz` & `tmp/ionicons_python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ionicons_python-1.0.0.tar", last modified: Fri Jun  9 04:33:08 2023, max compression
+gzip compressed data, was "ionicons_python-1.0.1.tar", last modified: Fri Jun  9 04:45:10 2023, max compression
```

## Comparing `ionicons_python-1.0.0.tar` & `ionicons_python-1.0.1.tar`

### file list

```diff
@@ -1,1372 +1,1372 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 04:33:08.889942 ionicons_python-1.0.0/
--rw-rw-rw-   0        0        0       66 2023-06-09 03:18:29.000000 ionicons_python-1.0.0/AUTHORS.md
--rw-rw-rw-   0        0        0      315 2023-06-09 03:15:09.000000 ionicons_python-1.0.0/CONTACT.md
--rw-rw-rw-   0        0        0     1096 2023-06-08 06:22:28.000000 ionicons_python-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      176 2023-06-09 03:54:03.000000 ionicons_python-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3879 2023-06-09 04:33:08.889942 ionicons_python-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2359 2023-06-09 04:07:40.000000 ionicons_python-1.0.0/README.md
--rw-rw-rw-   0        0        0      697 2023-06-09 04:29:39.000000 ionicons_python-1.0.0/RELEASE.md
-drwxrwxrwx   0        0        0        0 2023-06-09 04:33:08.086248 ionicons_python-1.0.0/ionicons_python/
--rw-rw-rw-   0        0        0       29 2023-06-08 03:58:02.000000 ionicons_python-1.0.0/ionicons_python/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 04:33:08.112083 ionicons_python-1.0.0/ionicons_python/extra_icons/
--rw-rw-rw-   0        0        0        0 2023-06-09 01:31:09.000000 ionicons_python-1.0.0/ionicons_python/extra_icons/__init__.py
--rw-rw-rw-   0        0        0     2259 2023-05-22 03:07:13.000000 ionicons_python-1.0.0/ionicons_python/extra_icons/chatgpt.svg
--rw-rw-rw-   0        0        0      613 2023-06-09 01:35:37.000000 ionicons_python-1.0.0/ionicons_python/extra_icons/gmail.svg
--rw-rw-rw-   0        0        0      396 2023-06-09 01:40:51.000000 ionicons_python-1.0.0/ionicons_python/extra_icons/google-docs.svg
--rw-rw-rw-   0        0        0     1121 2023-06-09 03:00:43.000000 ionicons_python-1.0.0/ionicons_python/extra_icons/google-drive.svg
--rw-rw-rw-   0        0        0      497 2023-06-09 01:39:57.000000 ionicons_python-1.0.0/ionicons_python/extra_icons/google-sheets.svg
--rw-rw-rw-   0        0        0      438 2023-06-09 01:42:39.000000 ionicons_python-1.0.0/ionicons_python/extra_icons/google-slides.svg
--rw-rw-rw-   0        0        0      990 2023-06-09 01:38:19.000000 ionicons_python-1.0.0/ionicons_python/extra_icons/google_color.svg
--rw-rw-rw-   0        0        0     1595 2023-06-09 02:34:08.000000 ionicons_python-1.0.0/ionicons_python/extra_icons/python_color.svg
--rw-rw-rw-   0        0        0      552 2023-05-24 07:21:17.000000 ionicons_python-1.0.0/ionicons_python/extra_icons/streamlit.svg
--rw-rw-rw-   0        0        0      733 2023-06-09 03:57:28.000000 ionicons_python-1.0.0/ionicons_python/extra_icons.py
-drwxrwxrwx   0        0        0        0 2023-06-09 04:33:08.888942 ionicons_python-1.0.0/ionicons_python/icons/
--rw-rw-rw-   0        0        0        0 2023-06-08 05:29:45.000000 ionicons_python-1.0.0/ionicons_python/icons/__init__.py
--rw-rw-rw-   0        0        0      744 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/accessibility-outline.svg
--rw-rw-rw-   0        0        0      333 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/accessibility-sharp.svg
--rw-rw-rw-   0        0        0      846 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/accessibility.svg
--rw-rw-rw-   0        0        0      517 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/add-circle-outline.svg
--rw-rw-rw-   0        0        0      240 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/add-circle-sharp.svg
--rw-rw-rw-   0        0        0      297 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/add-circle.svg
--rw-rw-rw-   0        0        0      361 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/add-outline.svg
--rw-rw-rw-   0        0        0      363 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/add-sharp.svg
--rw-rw-rw-   0        0        0      361 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/add.svg
--rw-rw-rw-   0        0        0      742 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/airplane-outline.svg
--rw-rw-rw-   0        0        0      494 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/airplane-sharp.svg
--rw-rw-rw-   0        0        0      741 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/airplane.svg
--rw-rw-rw-   0        0        0     1273 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/alarm-outline.svg
--rw-rw-rw-   0        0        0      882 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/alarm-sharp.svg
--rw-rw-rw-   0        0        0      912 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/alarm.svg
--rw-rw-rw-   0        0        0      476 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/albums-outline.svg
--rw-rw-rw-   0        0        0      217 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/albums-sharp.svg
--rw-rw-rw-   0        0        0      383 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/albums.svg
--rw-rw-rw-   0        0        0      507 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/alert-circle-outline.svg
--rw-rw-rw-   0        0        0      315 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/alert-circle-sharp.svg
--rw-rw-rw-   0        0        0      328 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/alert-circle.svg
--rw-rw-rw-   0        0        0      426 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/alert-outline.svg
--rw-rw-rw-   0        0        0      377 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/alert-sharp.svg
--rw-rw-rw-   0        0        0      426 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/alert.svg
--rw-rw-rw-   0        0        0     1145 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/american-football-outline.svg
--rw-rw-rw-   0        0        0      969 2023-05-22 03:19:27.000000 ionicons_python-1.0.0/ionicons_python/icons/american-football-sharp.svg
--rw-rw-rw-   0        0        0     1118 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/american-football.svg
--rw-rw-rw-   0        0        0      993 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/analytics-outline.svg
--rw-rw-rw-   0        0        0      341 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/analytics-sharp.svg
--rw-rw-rw-   0        0        0      346 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/analytics.svg
--rw-rw-rw-   0        0        0     1362 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/aperture-outline.svg
--rw-rw-rw-   0        0        0      641 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/aperture-sharp.svg
--rw-rw-rw-   0        0        0     1130 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/aperture.svg
--rw-rw-rw-   0        0        0     1266 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/apps-outline.svg
--rw-rw-rw-   0        0        0      645 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/apps-sharp.svg
--rw-rw-rw-   0        0        0      678 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/apps.svg
--rw-rw-rw-   0        0        0      666 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/archive-outline.svg
--rw-rw-rw-   0        0        0      305 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/archive-sharp.svg
--rw-rw-rw-   0        0        0      507 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/archive.svg
--rw-rw-rw-   0        0        0      527 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-back-circle-outline.svg
--rw-rw-rw-   0        0        0      276 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-back-circle-sharp.svg
--rw-rw-rw-   0        0        0      367 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-back-circle.svg
--rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-back-outline.svg
--rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-back-sharp.svg
--rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-back.svg
--rw-rw-rw-   0        0        0      525 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-down-circle-outline.svg
--rw-rw-rw-   0        0        0      278 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-down-circle-sharp.svg
--rw-rw-rw-   0        0        0      371 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-down-circle.svg
--rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-down-outline.svg
--rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-down-sharp.svg
--rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-down.svg
--rw-rw-rw-   0        0        0      526 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-forward-circle-outline.svg
--rw-rw-rw-   0        0        0      280 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-forward-circle-sharp.svg
--rw-rw-rw-   0        0        0      372 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-forward-circle.svg
--rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-forward-outline.svg
--rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-forward-sharp.svg
--rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-forward.svg
--rw-rw-rw-   0        0        0      482 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-redo-circle-outline.svg
--rw-rw-rw-   0        0        0      300 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-redo-circle-sharp.svg
--rw-rw-rw-   0        0        0      413 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-redo-circle.svg
--rw-rw-rw-   0        0        0      252 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-redo-outline.svg
--rw-rw-rw-   0        0        0      289 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-redo-sharp.svg
--rw-rw-rw-   0        0        0      379 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-redo.svg
--rw-rw-rw-   0        0        0      485 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-undo-circle-outline.svg
--rw-rw-rw-   0        0        0      308 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-undo-circle-sharp.svg
--rw-rw-rw-   0        0        0      424 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-undo-circle.svg
--rw-rw-rw-   0        0        0      253 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-undo-outline.svg
--rw-rw-rw-   0        0        0      292 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-undo-sharp.svg
--rw-rw-rw-   0        0        0      380 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-undo.svg
--rw-rw-rw-   0        0        0      527 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-up-circle-outline.svg
--rw-rw-rw-   0        0        0      278 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-up-circle-sharp.svg
--rw-rw-rw-   0        0        0      367 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-up-circle.svg
--rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-up-outline.svg
--rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-up-sharp.svg
--rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/arrow-up.svg
--rw-rw-rw-   0        0        0      696 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/at-circle-outline.svg
--rw-rw-rw-   0        0        0     1224 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/at-circle-sharp.svg
--rw-rw-rw-   0        0        0     1221 2023-05-22 03:19:28.000000 ionicons_python-1.0.0/ionicons_python/icons/at-circle.svg
--rw-rw-rw-   0        0        0      606 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/at-outline.svg
--rw-rw-rw-   0        0        0     1221 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/at-sharp.svg
--rw-rw-rw-   0        0        0      606 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/at.svg
--rw-rw-rw-   0        0        0      315 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/attach-outline.svg
--rw-rw-rw-   0        0        0      316 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/attach-sharp.svg
--rw-rw-rw-   0        0        0      315 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/attach.svg
--rw-rw-rw-   0        0        0      924 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/backspace-outline.svg
--rw-rw-rw-   0        0        0      238 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/backspace-sharp.svg
--rw-rw-rw-   0        0        0      523 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/backspace.svg
--rw-rw-rw-   0        0        0      751 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bag-add-outline.svg
--rw-rw-rw-   0        0        0      394 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bag-add-sharp.svg
--rw-rw-rw-   0        0        0      430 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bag-add.svg
--rw-rw-rw-   0        0        0      612 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bag-check-outline.svg
--rw-rw-rw-   0        0        0      413 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bag-check-sharp.svg
--rw-rw-rw-   0        0        0      470 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bag-check.svg
--rw-rw-rw-   0        0        0      599 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bag-handle-outline.svg
--rw-rw-rw-   0        0        0      409 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bag-handle-sharp.svg
--rw-rw-rw-   0        0        0      416 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bag-handle.svg
--rw-rw-rw-   0        0        0      472 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bag-outline.svg
--rw-rw-rw-   0        0        0      606 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bag-remove-outline.svg
--rw-rw-rw-   0        0        0      367 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bag-remove-sharp.svg
--rw-rw-rw-   0        0        0      376 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bag-remove.svg
--rw-rw-rw-   0        0        0      337 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bag-sharp.svg
--rw-rw-rw-   0        0        0      325 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bag.svg
--rw-rw-rw-   0        0        0      745 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/balloon-outline.svg
--rw-rw-rw-   0        0        0      630 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/balloon-sharp.svg
--rw-rw-rw-   0        0        0      825 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/balloon.svg
--rw-rw-rw-   0        0        0      303 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/ban-outline.svg
--rw-rw-rw-   0        0        0      361 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/ban-sharp.svg
--rw-rw-rw-   0        0        0      280 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/ban.svg
--rw-rw-rw-   0        0        0      659 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bandage-outline.svg
--rw-rw-rw-   0        0        0      618 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bandage-sharp.svg
--rw-rw-rw-   0        0        0     1481 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bandage.svg
--rw-rw-rw-   0        0        0      692 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bar-chart-outline.svg
--rw-rw-rw-   0        0        0      263 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bar-chart-sharp.svg
--rw-rw-rw-   0        0        0      516 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/bar-chart.svg
--rw-rw-rw-   0        0        0      836 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/barbell-outline.svg
--rw-rw-rw-   0        0        0      274 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/barbell-sharp.svg
--rw-rw-rw-   0        0        0      744 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/barbell.svg
--rw-rw-rw-   0        0        0     1144 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/barcode-outline.svg
--rw-rw-rw-   0        0        0     1066 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/barcode-sharp.svg
--rw-rw-rw-   0        0        0      547 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/barcode.svg
--rw-rw-rw-   0        0        0     1670 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/baseball-outline.svg
--rw-rw-rw-   0        0        0     1795 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/baseball-sharp.svg
--rw-rw-rw-   0        0        0     2180 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/baseball.svg
--rw-rw-rw-   0        0        0      545 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/basket-outline.svg
--rw-rw-rw-   0        0        0      363 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/basket-sharp.svg
--rw-rw-rw-   0        0        0      485 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/basket.svg
--rw-rw-rw-   0        0        0      796 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/basketball-outline.svg
--rw-rw-rw-   0        0        0     1061 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/basketball-sharp.svg
--rw-rw-rw-   0        0        0     1061 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/basketball.svg
--rw-rw-rw-   0        0        0     2111 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/battery-charging-outline.svg
--rw-rw-rw-   0        0        0     1204 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/battery-charging-sharp.svg
--rw-rw-rw-   0        0        0     2111 2023-05-22 03:19:29.000000 ionicons_python-1.0.0/ionicons_python/icons/battery-charging.svg
--rw-rw-rw-   0        0        0      390 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/battery-dead-outline.svg
--rw-rw-rw-   0        0        0      371 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/battery-dead-sharp.svg
--rw-rw-rw-   0        0        0      390 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/battery-dead.svg
--rw-rw-rw-   0        0        0      544 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/battery-full-outline.svg
--rw-rw-rw-   0        0        0      255 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/battery-full-sharp.svg
--rw-rw-rw-   0        0        0      544 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/battery-full.svg
--rw-rw-rw-   0        0        0      544 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/battery-half-outline.svg
--rw-rw-rw-   0        0        0      255 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/battery-half-sharp.svg
--rw-rw-rw-   0        0        0      544 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/battery-half.svg
--rw-rw-rw-   0        0        0      517 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/beaker-outline.svg
--rw-rw-rw-   0        0        0      407 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/beaker-sharp.svg
--rw-rw-rw-   0        0        0      516 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/beaker.svg
--rw-rw-rw-   0        0        0      943 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bed-outline.svg
--rw-rw-rw-   0        0        0      331 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bed-sharp.svg
--rw-rw-rw-   0        0        0      647 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bed.svg
--rw-rw-rw-   0        0        0     1394 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/beer-outline.svg
--rw-rw-rw-   0        0        0     1157 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/beer-sharp.svg
--rw-rw-rw-   0        0        0     1176 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/beer.svg
--rw-rw-rw-   0        0        0      608 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bicycle-outline.svg
--rw-rw-rw-   0        0        0      649 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bicycle-sharp.svg
--rw-rw-rw-   0        0        0      847 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bicycle.svg
--rw-rw-rw-   0        0        0      251 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bluetooth-outline.svg
--rw-rw-rw-   0        0        0      298 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bluetooth-sharp.svg
--rw-rw-rw-   0        0        0      425 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bluetooth.svg
--rw-rw-rw-   0        0        0     1499 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/boat-outline.svg
--rw-rw-rw-   0        0        0      798 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/boat-sharp.svg
--rw-rw-rw-   0        0        0     1180 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/boat.svg
--rw-rw-rw-   0        0        0      599 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/body-outline.svg
--rw-rw-rw-   0        0        0      259 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/body-sharp.svg
--rw-rw-rw-   0        0        0      560 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/body.svg
--rw-rw-rw-   0        0        0     1804 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bonfire-outline.svg
--rw-rw-rw-   0        0        0     1610 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bonfire-sharp.svg
--rw-rw-rw-   0        0        0     2042 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bonfire.svg
--rw-rw-rw-   0        0        0      544 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/book-outline.svg
--rw-rw-rw-   0        0        0      335 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/book-sharp.svg
--rw-rw-rw-   0        0        0      598 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/book.svg
--rw-rw-rw-   0        0        0      268 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bookmark-outline.svg
--rw-rw-rw-   0        0        0      139 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bookmark-sharp.svg
--rw-rw-rw-   0        0        0      252 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bookmark.svg
--rw-rw-rw-   0        0        0      415 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bookmarks-outline.svg
--rw-rw-rw-   0        0        0      221 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bookmarks-sharp.svg
--rw-rw-rw-   0        0        0      440 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bookmarks.svg
--rw-rw-rw-   0        0        0      283 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bowling-ball-outline.svg
--rw-rw-rw-   0        0        0      295 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bowling-ball-sharp.svg
--rw-rw-rw-   0        0        0      295 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/bowling-ball.svg
--rw-rw-rw-   0        0        0      666 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/briefcase-outline.svg
--rw-rw-rw-   0        0        0      307 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/briefcase-sharp.svg
--rw-rw-rw-   0        0        0      526 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/briefcase.svg
--rw-rw-rw-   0        0        0      366 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/browsers-outline.svg
--rw-rw-rw-   0        0        0      282 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/browsers-sharp.svg
--rw-rw-rw-   0        0        0      302 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/browsers.svg
--rw-rw-rw-   0        0        0      581 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/brush-outline.svg
--rw-rw-rw-   0        0        0      295 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/brush-sharp.svg
--rw-rw-rw-   0        0        0      541 2023-05-22 03:19:30.000000 ionicons_python-1.0.0/ionicons_python/icons/brush.svg
--rw-rw-rw-   0        0        0     1509 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/bug-outline.svg
--rw-rw-rw-   0        0        0      775 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/bug-sharp.svg
--rw-rw-rw-   0        0        0     1292 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/bug.svg
--rw-rw-rw-   0        0        0      588 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/build-outline.svg
--rw-rw-rw-   0        0        0      331 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/build-sharp.svg
--rw-rw-rw-   0        0        0      596 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/build.svg
--rw-rw-rw-   0        0        0      905 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/bulb-outline.svg
--rw-rw-rw-   0        0        0      533 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/bulb-sharp.svg
--rw-rw-rw-   0        0        0      762 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/bulb.svg
--rw-rw-rw-   0        0        0     1547 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/bus-outline.svg
--rw-rw-rw-   0        0        0      523 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/bus-sharp.svg
--rw-rw-rw-   0        0        0      740 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/bus.svg
--rw-rw-rw-   0        0        0     2041 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/business-outline.svg
--rw-rw-rw-   0        0        0      593 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/business-sharp.svg
--rw-rw-rw-   0        0        0     1511 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/business.svg
--rw-rw-rw-   0        0        0      573 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/cafe-outline.svg
--rw-rw-rw-   0        0        0      426 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/cafe-sharp.svg
--rw-rw-rw-   0        0        0      339 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/cafe.svg
--rw-rw-rw-   0        0        0      692 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/calculator-outline.svg
--rw-rw-rw-   0        0        0      358 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/calculator-sharp.svg
--rw-rw-rw-   0        0        0      712 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/calculator.svg
--rw-rw-rw-   0        0        0      587 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/calendar-clear-outline.svg
--rw-rw-rw-   0        0        0      251 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/calendar-clear-sharp.svg
--rw-rw-rw-   0        0        0      376 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/calendar-clear.svg
--rw-rw-rw-   0        0        0     1224 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/calendar-number-outline.svg
--rw-rw-rw-   0        0        0      955 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/calendar-number-sharp.svg
--rw-rw-rw-   0        0        0     1144 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/calendar-number.svg
--rw-rw-rw-   0        0        0      870 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/calendar-outline.svg
--rw-rw-rw-   0        0        0      911 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/calendar-sharp.svg
--rw-rw-rw-   0        0        0      781 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/calendar.svg
--rw-rw-rw-   0        0        0      678 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/call-outline.svg
--rw-rw-rw-   0        0        0      819 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/call-sharp.svg
--rw-rw-rw-   0        0        0      938 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/call.svg
--rw-rw-rw-   0        0        0      712 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/camera-outline.svg
--rw-rw-rw-   0        0        0     1065 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/camera-reverse-outline.svg
--rw-rw-rw-   0        0        0      641 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/camera-reverse-sharp.svg
--rw-rw-rw-   0        0        0      817 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/camera-reverse.svg
--rw-rw-rw-   0        0        0      466 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/camera-sharp.svg
--rw-rw-rw-   0        0        0      549 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/camera.svg
--rw-rw-rw-   0        0        0      966 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/car-outline.svg
--rw-rw-rw-   0        0        0      495 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/car-sharp.svg
--rw-rw-rw-   0        0        0     1901 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/car-sport-outline.svg
--rw-rw-rw-   0        0        0     1356 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/car-sport-sharp.svg
--rw-rw-rw-   0        0        0     2023 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/car-sport.svg
--rw-rw-rw-   0        0        0      579 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/car.svg
--rw-rw-rw-   0        0        0      474 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/card-outline.svg
--rw-rw-rw-   0        0        0      304 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/card-sharp.svg
--rw-rw-rw-   0        0        0      320 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/card.svg
--rw-rw-rw-   0        0        0      376 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-back-circle-outline.svg
--rw-rw-rw-   0        0        0      226 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-back-circle-sharp.svg
--rw-rw-rw-   0        0        0      301 2023-05-22 03:19:31.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-back-circle.svg
--rw-rw-rw-   0        0        0      239 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-back-outline.svg
--rw-rw-rw-   0        0        0      142 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-back-sharp.svg
--rw-rw-rw-   0        0        0      239 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-back.svg
--rw-rw-rw-   0        0        0      377 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-down-circle-outline.svg
--rw-rw-rw-   0        0        0      228 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-down-circle-sharp.svg
--rw-rw-rw-   0        0        0      311 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-down-circle.svg
--rw-rw-rw-   0        0        0      239 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-down-outline.svg
--rw-rw-rw-   0        0        0      142 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-down-sharp.svg
--rw-rw-rw-   0        0        0      239 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-down.svg
--rw-rw-rw-   0        0        0      376 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-forward-circle-outline.svg
--rw-rw-rw-   0        0        0      229 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-forward-circle-sharp.svg
--rw-rw-rw-   0        0        0      305 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-forward-circle.svg
--rw-rw-rw-   0        0        0      243 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-forward-outline.svg
--rw-rw-rw-   0        0        0      143 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-forward-sharp.svg
--rw-rw-rw-   0        0        0      243 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-forward.svg
--rw-rw-rw-   0        0        0      377 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-up-circle-outline.svg
--rw-rw-rw-   0        0        0      227 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-up-circle-sharp.svg
--rw-rw-rw-   0        0        0      301 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-up-circle.svg
--rw-rw-rw-   0        0        0      243 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-up-outline.svg
--rw-rw-rw-   0        0        0      143 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-up-sharp.svg
--rw-rw-rw-   0        0        0      243 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/caret-up.svg
--rw-rw-rw-   0        0        0      654 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/cart-outline.svg
--rw-rw-rw-   0        0        0      304 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/cart-sharp.svg
--rw-rw-rw-   0        0        0      420 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/cart.svg
--rw-rw-rw-   0        0        0     1173 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/cash-outline.svg
--rw-rw-rw-   0        0        0      660 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/cash-sharp.svg
--rw-rw-rw-   0        0        0      784 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/cash.svg
--rw-rw-rw-   0        0        0      615 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/cellular-outline.svg
--rw-rw-rw-   0        0        0      219 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/cellular-sharp.svg
--rw-rw-rw-   0        0        0      529 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/cellular.svg
--rw-rw-rw-   0        0        0      436 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/chatbox-ellipses-outline.svg
--rw-rw-rw-   0        0        0      361 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/chatbox-ellipses-sharp.svg
--rw-rw-rw-   0        0        0      402 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/chatbox-ellipses.svg
--rw-rw-rw-   0        0        0      334 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/chatbox-outline.svg
--rw-rw-rw-   0        0        0      221 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/chatbox-sharp.svg
--rw-rw-rw-   0        0        0      294 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/chatbox.svg
--rw-rw-rw-   0        0        0      720 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/chatbubble-ellipses-outline.svg
--rw-rw-rw-   0        0        0      612 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/chatbubble-ellipses-sharp.svg
--rw-rw-rw-   0        0        0      820 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/chatbubble-ellipses.svg
--rw-rw-rw-   0        0        0      614 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/chatbubble-outline.svg
--rw-rw-rw-   0        0        0      477 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/chatbubble-sharp.svg
--rw-rw-rw-   0        0        0      697 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/chatbubble.svg
--rw-rw-rw-   0        0        0      906 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/chatbubbles-outline.svg
--rw-rw-rw-   0        0        0      888 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/chatbubbles-sharp.svg
--rw-rw-rw-   0        0        0     1270 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/chatbubbles.svg
--rw-rw-rw-   0        0        0      362 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/checkbox-outline.svg
--rw-rw-rw-   0        0        0      191 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/checkbox-sharp.svg
--rw-rw-rw-   0        0        0      380 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/checkbox.svg
--rw-rw-rw-   0        0        0      386 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/checkmark-circle-outline.svg
--rw-rw-rw-   0        0        0      261 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/checkmark-circle-sharp.svg
--rw-rw-rw-   0        0        0      347 2023-05-22 03:19:32.000000 ionicons_python-1.0.0/ionicons_python/icons/checkmark-circle.svg
--rw-rw-rw-   0        0        0      667 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/checkmark-done-circle-outline.svg
--rw-rw-rw-   0        0        0      356 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/checkmark-done-circle-sharp.svg
--rw-rw-rw-   0        0        0      611 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/checkmark-done-circle.svg
--rw-rw-rw-   0        0        0      495 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/checkmark-done-outline.svg
--rw-rw-rw-   0        0        0      495 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/checkmark-done-sharp.svg
--rw-rw-rw-   0        0        0      495 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/checkmark-done.svg
--rw-rw-rw-   0        0        0      227 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/checkmark-outline.svg
--rw-rw-rw-   0        0        0      227 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/checkmark-sharp.svg
--rw-rw-rw-   0        0        0      227 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/checkmark.svg
--rw-rw-rw-   0        0        0      382 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-back-circle-outline.svg
--rw-rw-rw-   0        0        0      255 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-back-circle-sharp.svg
--rw-rw-rw-   0        0        0      299 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-back-circle.svg
--rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-back-outline.svg
--rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-back-sharp.svg
--rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-back.svg
--rw-rw-rw-   0        0        0      338 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-collapse-outline.svg
--rw-rw-rw-   0        0        0      297 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-collapse-sharp.svg
--rw-rw-rw-   0        0        0      552 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-collapse.svg
--rw-rw-rw-   0        0        0      382 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-down-circle-outline.svg
--rw-rw-rw-   0        0        0      251 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-down-circle-sharp.svg
--rw-rw-rw-   0        0        0      315 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-down-circle.svg
--rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-down-outline.svg
--rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-down-sharp.svg
--rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-down.svg
--rw-rw-rw-   0        0        0      339 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-expand-outline.svg
--rw-rw-rw-   0        0        0      293 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-expand-sharp.svg
--rw-rw-rw-   0        0        0      339 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-expand.svg
--rw-rw-rw-   0        0        0      381 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-forward-circle-outline.svg
--rw-rw-rw-   0        0        0      250 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-forward-circle-sharp.svg
--rw-rw-rw-   0        0        0      295 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-forward-circle.svg
--rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-forward-outline.svg
--rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-forward-sharp.svg
--rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-forward.svg
--rw-rw-rw-   0        0        0      382 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-up-circle-outline.svg
--rw-rw-rw-   0        0        0      249 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-up-circle-sharp.svg
--rw-rw-rw-   0        0        0      334 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-up-circle.svg
--rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-up-outline.svg
--rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-up-sharp.svg
--rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/chevron-up.svg
--rw-rw-rw-   0        0        0      410 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/clipboard-outline.svg
--rw-rw-rw-   0        0        0      278 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/clipboard-sharp.svg
--rw-rw-rw-   0        0        0      373 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/clipboard.svg
--rw-rw-rw-   0        0        0      517 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/close-circle-outline.svg
--rw-rw-rw-   0        0        0      292 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/close-circle-sharp.svg
--rw-rw-rw-   0        0        0      385 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/close-circle.svg
--rw-rw-rw-   0        0        0      361 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/close-outline.svg
--rw-rw-rw-   0        0        0      255 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/close-sharp.svg
--rw-rw-rw-   0        0        0      240 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/close.svg
--rw-rw-rw-   0        0        0      513 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-circle-outline.svg
--rw-rw-rw-   0        0        0      347 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-circle-sharp.svg
--rw-rw-rw-   0        0        0      450 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-circle.svg
--rw-rw-rw-   0        0        0      474 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-done-outline.svg
--rw-rw-rw-   0        0        0      550 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-done-sharp.svg
--rw-rw-rw-   0        0        0      683 2023-05-22 03:19:33.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-done.svg
--rw-rw-rw-   0        0        0      624 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-download-outline.svg
--rw-rw-rw-   0        0        0      559 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-download-sharp.svg
--rw-rw-rw-   0        0        0      684 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-download.svg
--rw-rw-rw-   0        0        0      624 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-offline-outline.svg
--rw-rw-rw-   0        0        0      602 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-offline-sharp.svg
--rw-rw-rw-   0        0        0      690 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-offline.svg
--rw-rw-rw-   0        0        0      335 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-outline.svg
--rw-rw-rw-   0        0        0      472 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-sharp.svg
--rw-rw-rw-   0        0        0      643 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-upload-outline.svg
--rw-rw-rw-   0        0        0      644 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-upload-sharp.svg
--rw-rw-rw-   0        0        0      800 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud-upload.svg
--rw-rw-rw-   0        0        0      508 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloud.svg
--rw-rw-rw-   0        0        0      740 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloudy-night-outline.svg
--rw-rw-rw-   0        0        0      796 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloudy-night-sharp.svg
--rw-rw-rw-   0        0        0     1015 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloudy-night.svg
--rw-rw-rw-   0        0        0      428 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloudy-outline.svg
--rw-rw-rw-   0        0        0      462 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloudy-sharp.svg
--rw-rw-rw-   0        0        0      500 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cloudy.svg
--rw-rw-rw-   0        0        0      638 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/code-download-outline.svg
--rw-rw-rw-   0        0        0      638 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/code-download-sharp.svg
--rw-rw-rw-   0        0        0      638 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/code-download.svg
--rw-rw-rw-   0        0        0      362 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/code-outline.svg
--rw-rw-rw-   0        0        0      300 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/code-sharp.svg
--rw-rw-rw-   0        0        0      495 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/code-slash-outline.svg
--rw-rw-rw-   0        0        0      372 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/code-slash-sharp.svg
--rw-rw-rw-   0        0        0      501 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/code-slash.svg
--rw-rw-rw-   0        0        0      464 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/code-working-outline.svg
--rw-rw-rw-   0        0        0      707 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/code-working-sharp.svg
--rw-rw-rw-   0        0        0      641 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/code-working.svg
--rw-rw-rw-   0        0        0      401 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/code.svg
--rw-rw-rw-   0        0        0     3072 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cog-outline.svg
--rw-rw-rw-   0        0        0     3333 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cog-sharp.svg
--rw-rw-rw-   0        0        0     3567 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/cog.svg
--rw-rw-rw-   0        0        0      645 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/color-fill-outline.svg
--rw-rw-rw-   0        0        0      302 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/color-fill-sharp.svg
--rw-rw-rw-   0        0        0      748 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/color-fill.svg
--rw-rw-rw-   0        0        0      408 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/color-filter-outline.svg
--rw-rw-rw-   0        0        0     1006 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/color-filter-sharp.svg
--rw-rw-rw-   0        0        0     1577 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/color-filter.svg
--rw-rw-rw-   0        0        0      650 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/color-palette-outline.svg
--rw-rw-rw-   0        0        0      648 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/color-palette-sharp.svg
--rw-rw-rw-   0        0        0      838 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/color-palette.svg
--rw-rw-rw-   0        0        0     1005 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/color-wand-outline.svg
--rw-rw-rw-   0        0        0      665 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/color-wand-sharp.svg
--rw-rw-rw-   0        0        0     1447 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/color-wand.svg
--rw-rw-rw-   0        0        0      465 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/compass-outline.svg
--rw-rw-rw-   0        0        0      257 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/compass-sharp.svg
--rw-rw-rw-   0        0        0      384 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/compass.svg
--rw-rw-rw-   0        0        0     1992 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/construct-outline.svg
--rw-rw-rw-   0        0        0     1275 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/construct-sharp.svg
--rw-rw-rw-   0        0        0     1638 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/construct.svg
--rw-rw-rw-   0        0        0     1181 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/contract-outline.svg
--rw-rw-rw-   0        0        0     1181 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/contract-sharp.svg
--rw-rw-rw-   0        0        0     1181 2023-05-22 03:19:34.000000 ionicons_python-1.0.0/ionicons_python/icons/contract.svg
--rw-rw-rw-   0        0        0      264 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/contrast-outline.svg
--rw-rw-rw-   0        0        0      269 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/contrast-sharp.svg
--rw-rw-rw-   0        0        0      261 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/contrast.svg
--rw-rw-rw-   0        0        0      429 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/copy-outline.svg
--rw-rw-rw-   0        0        0      318 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/copy-sharp.svg
--rw-rw-rw-   0        0        0      332 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/copy.svg
--rw-rw-rw-   0        0        0      620 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/create-outline.svg
--rw-rw-rw-   0        0        0      549 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/create-sharp.svg
--rw-rw-rw-   0        0        0      719 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/create.svg
--rw-rw-rw-   0        0        0      633 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/crop-outline.svg
--rw-rw-rw-   0        0        0      303 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/crop-sharp.svg
--rw-rw-rw-   0        0        0      371 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/crop.svg
--rw-rw-rw-   0        0        0      682 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/cube-outline.svg
--rw-rw-rw-   0        0        0      267 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/cube-sharp.svg
--rw-rw-rw-   0        0        0      480 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/cube.svg
--rw-rw-rw-   0        0        0     1017 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/cut-outline.svg
--rw-rw-rw-   0        0        0      481 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/cut-sharp.svg
--rw-rw-rw-   0        0        0      804 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/cut.svg
--rw-rw-rw-   0        0        0      624 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/desktop-outline.svg
--rw-rw-rw-   0        0        0      313 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/desktop-sharp.svg
--rw-rw-rw-   0        0        0      365 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/desktop.svg
--rw-rw-rw-   0        0        0     1066 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/diamond-outline.svg
--rw-rw-rw-   0        0        0      578 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/diamond-sharp.svg
--rw-rw-rw-   0        0        0     1064 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/diamond.svg
--rw-rw-rw-   0        0        0      965 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/dice-outline.svg
--rw-rw-rw-   0        0        0      751 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/dice-sharp.svg
--rw-rw-rw-   0        0        0     1048 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/dice.svg
--rw-rw-rw-   0        0        0      334 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/disc-outline.svg
--rw-rw-rw-   0        0        0      260 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/disc-sharp.svg
--rw-rw-rw-   0        0        0      342 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/disc.svg
--rw-rw-rw-   0        0        0      708 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/document-attach-outline.svg
--rw-rw-rw-   0        0        0      681 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/document-attach-sharp.svg
--rw-rw-rw-   0        0        0      750 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/document-attach.svg
--rw-rw-rw-   0        0        0      710 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/document-lock-outline.svg
--rw-rw-rw-   0        0        0      526 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/document-lock-sharp.svg
--rw-rw-rw-   0        0        0      538 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/document-lock.svg
--rw-rw-rw-   0        0        0      454 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/document-outline.svg
--rw-rw-rw-   0        0        0      309 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/document-sharp.svg
--rw-rw-rw-   0        0        0      722 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/document-text-outline.svg
--rw-rw-rw-   0        0        0      340 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/document-text-sharp.svg
--rw-rw-rw-   0        0        0      453 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/document-text.svg
--rw-rw-rw-   0        0        0      354 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/document.svg
--rw-rw-rw-   0        0        0      851 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/documents-outline.svg
--rw-rw-rw-   0        0        0      493 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/documents-sharp.svg
--rw-rw-rw-   0        0        0      644 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/documents.svg
--rw-rw-rw-   0        0        0      562 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/download-outline.svg
--rw-rw-rw-   0        0        0      314 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/download-sharp.svg
--rw-rw-rw-   0        0        0      392 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/download.svg
--rw-rw-rw-   0        0        0      697 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/duplicate-outline.svg
--rw-rw-rw-   0        0        0      366 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/duplicate-sharp.svg
--rw-rw-rw-   0        0        0      575 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/duplicate.svg
--rw-rw-rw-   0        0        0      714 2023-05-22 03:19:35.000000 ionicons_python-1.0.0/ionicons_python/icons/ear-outline.svg
--rw-rw-rw-   0        0        0      716 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ear-sharp.svg
--rw-rw-rw-   0        0        0      758 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ear.svg
--rw-rw-rw-   0        0        0     3614 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/earth-outline.svg
--rw-rw-rw-   0        0        0     2560 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/earth-sharp.svg
--rw-rw-rw-   0        0        0     2249 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/earth.svg
--rw-rw-rw-   0        0        0      759 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/easel-outline.svg
--rw-rw-rw-   0        0        0      373 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/easel-sharp.svg
--rw-rw-rw-   0        0        0      536 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/easel.svg
--rw-rw-rw-   0        0        0      260 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/egg-outline.svg
--rw-rw-rw-   0        0        0      548 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/egg-sharp.svg
--rw-rw-rw-   0        0        0      351 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/egg.svg
--rw-rw-rw-   0        0        0      219 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ellipse-outline.svg
--rw-rw-rw-   0        0        0      196 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ellipse-sharp.svg
--rw-rw-rw-   0        0        0      196 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ellipse.svg
--rw-rw-rw-   0        0        0      351 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ellipsis-horizontal-circle-outline.svg
--rw-rw-rw-   0        0        0      328 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ellipsis-horizontal-circle-sharp.svg
--rw-rw-rw-   0        0        0      351 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ellipsis-horizontal-circle.svg
--rw-rw-rw-   0        0        0      401 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ellipsis-horizontal-outline.svg
--rw-rw-rw-   0        0        0      194 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ellipsis-horizontal-sharp.svg
--rw-rw-rw-   0        0        0      194 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ellipsis-horizontal.svg
--rw-rw-rw-   0        0        0      351 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ellipsis-vertical-circle-outline.svg
--rw-rw-rw-   0        0        0      330 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ellipsis-vertical-circle-sharp.svg
--rw-rw-rw-   0        0        0      351 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ellipsis-vertical-circle.svg
--rw-rw-rw-   0        0        0      401 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ellipsis-vertical-outline.svg
--rw-rw-rw-   0        0        0      194 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ellipsis-vertical-sharp.svg
--rw-rw-rw-   0        0        0      194 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/ellipsis-vertical.svg
--rw-rw-rw-   0        0        0      564 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/enter-outline.svg
--rw-rw-rw-   0        0        0      315 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/enter-sharp.svg
--rw-rw-rw-   0        0        0      393 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/enter.svg
--rw-rw-rw-   0        0        0      564 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/exit-outline.svg
--rw-rw-rw-   0        0        0      353 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/exit-sharp.svg
--rw-rw-rw-   0        0        0      392 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/exit.svg
--rw-rw-rw-   0        0        0     1177 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/expand-outline.svg
--rw-rw-rw-   0        0        0     1177 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/expand-sharp.svg
--rw-rw-rw-   0        0        0     1177 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/expand.svg
--rw-rw-rw-   0        0        0      730 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/extension-puzzle-outline.svg
--rw-rw-rw-   0        0        0      656 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/extension-puzzle-sharp.svg
--rw-rw-rw-   0        0        0      716 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/extension-puzzle.svg
--rw-rw-rw-   0        0        0     1239 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/eye-off-outline.svg
--rw-rw-rw-   0        0        0      797 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/eye-off-sharp.svg
--rw-rw-rw-   0        0        0     1047 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/eye-off.svg
--rw-rw-rw-   0        0        0      498 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/eye-outline.svg
--rw-rw-rw-   0        0        0      473 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/eye-sharp.svg
--rw-rw-rw-   0        0        0      536 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/eye.svg
--rw-rw-rw-   0        0        0      919 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/eyedrop-outline.svg
--rw-rw-rw-   0        0        0      449 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/eyedrop-sharp.svg
--rw-rw-rw-   0        0        0      800 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/eyedrop.svg
--rw-rw-rw-   0        0        0     1469 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/fast-food-outline.svg
--rw-rw-rw-   0        0        0      942 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/fast-food-sharp.svg
--rw-rw-rw-   0        0        0     1511 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/fast-food.svg
--rw-rw-rw-   0        0        0      487 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/female-outline.svg
--rw-rw-rw-   0        0        0      351 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/female-sharp.svg
--rw-rw-rw-   0        0        0      392 2023-05-22 03:19:36.000000 ionicons_python-1.0.0/ionicons_python/icons/female.svg
--rw-rw-rw-   0        0        0      965 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/file-tray-full-outline.svg
--rw-rw-rw-   0        0        0      274 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/file-tray-full-sharp.svg
--rw-rw-rw-   0        0        0      701 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/file-tray-full.svg
--rw-rw-rw-   0        0        0      697 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/file-tray-outline.svg
--rw-rw-rw-   0        0        0      180 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/file-tray-sharp.svg
--rw-rw-rw-   0        0        0     1239 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/file-tray-stacked-outline.svg
--rw-rw-rw-   0        0        0      233 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/file-tray-stacked-sharp.svg
--rw-rw-rw-   0        0        0      732 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/file-tray-stacked.svg
--rw-rw-rw-   0        0        0      575 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/file-tray.svg
--rw-rw-rw-   0        0        0     1542 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/film-outline.svg
--rw-rw-rw-   0        0        0      281 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/film-sharp.svg
--rw-rw-rw-   0        0        0      999 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/film.svg
--rw-rw-rw-   0        0        0      624 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/filter-circle-outline.svg
--rw-rw-rw-   0        0        0      225 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/filter-circle-sharp.svg
--rw-rw-rw-   0        0        0      315 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/filter-circle.svg
--rw-rw-rw-   0        0        0      494 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/filter-outline.svg
--rw-rw-rw-   0        0        0      232 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/filter-sharp.svg
--rw-rw-rw-   0        0        0      280 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/filter.svg
--rw-rw-rw-   0        0        0     2114 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/finger-print-outline.svg
--rw-rw-rw-   0        0        0     2251 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/finger-print-sharp.svg
--rw-rw-rw-   0        0        0     2486 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/finger-print.svg
--rw-rw-rw-   0        0        0      703 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/fish-outline.svg
--rw-rw-rw-   0        0        0      902 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/fish-sharp.svg
--rw-rw-rw-   0        0        0     1146 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/fish.svg
--rw-rw-rw-   0        0        0      569 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/fitness-outline.svg
--rw-rw-rw-   0        0        0      673 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/fitness-sharp.svg
--rw-rw-rw-   0        0        0      876 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/fitness.svg
--rw-rw-rw-   0        0        0      416 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flag-outline.svg
--rw-rw-rw-   0        0        0      402 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flag-sharp.svg
--rw-rw-rw-   0        0        0      473 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flag.svg
--rw-rw-rw-   0        0        0      453 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flame-outline.svg
--rw-rw-rw-   0        0        0      565 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flame-sharp.svg
--rw-rw-rw-   0        0        0      600 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flame.svg
--rw-rw-rw-   0        0        0      886 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flash-off-outline.svg
--rw-rw-rw-   0        0        0      352 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flash-off-sharp.svg
--rw-rw-rw-   0        0        0      618 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flash-off.svg
--rw-rw-rw-   0        0        0      364 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flash-outline.svg
--rw-rw-rw-   0        0        0      144 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flash-sharp.svg
--rw-rw-rw-   0        0        0      327 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flash.svg
--rw-rw-rw-   0        0        0      711 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flashlight-outline.svg
--rw-rw-rw-   0        0        0      364 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flashlight-sharp.svg
--rw-rw-rw-   0        0        0      720 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flashlight.svg
--rw-rw-rw-   0        0        0      632 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flask-outline.svg
--rw-rw-rw-   0        0        0      374 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flask-sharp.svg
--rw-rw-rw-   0        0        0      607 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flask.svg
--rw-rw-rw-   0        0        0     2153 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flower-outline.svg
--rw-rw-rw-   0        0        0     1028 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flower-sharp.svg
--rw-rw-rw-   0        0        0      997 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/flower.svg
--rw-rw-rw-   0        0        0      552 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/folder-open-outline.svg
--rw-rw-rw-   0        0        0      322 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/folder-open-sharp.svg
--rw-rw-rw-   0        0        0      427 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/folder-open.svg
--rw-rw-rw-   0        0        0      491 2023-05-22 03:19:37.000000 ionicons_python-1.0.0/ionicons_python/icons/folder-outline.svg
--rw-rw-rw-   0        0        0      241 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/folder-sharp.svg
--rw-rw-rw-   0        0        0      354 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/folder.svg
--rw-rw-rw-   0        0        0     1824 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/football-outline.svg
--rw-rw-rw-   0        0        0      648 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/football-sharp.svg
--rw-rw-rw-   0        0        0     1238 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/football.svg
--rw-rw-rw-   0        0        0      968 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/footsteps-outline.svg
--rw-rw-rw-   0        0        0     1063 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/footsteps-sharp.svg
--rw-rw-rw-   0        0        0     1394 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/footsteps.svg
--rw-rw-rw-   0        0        0      410 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/funnel-outline.svg
--rw-rw-rw-   0        0        0      161 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/funnel-sharp.svg
--rw-rw-rw-   0        0        0      332 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/funnel.svg
--rw-rw-rw-   0        0        0      970 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/game-controller-outline.svg
--rw-rw-rw-   0        0        0      600 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/game-controller-sharp.svg
--rw-rw-rw-   0        0        0      947 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/game-controller.svg
--rw-rw-rw-   0        0        0      826 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/gift-outline.svg
--rw-rw-rw-   0        0        0      592 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/gift-sharp.svg
--rw-rw-rw-   0        0        0      832 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/gift.svg
--rw-rw-rw-   0        0        0      733 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-branch-outline.svg
--rw-rw-rw-   0        0        0      392 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-branch-sharp.svg
--rw-rw-rw-   0        0        0      508 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-branch.svg
--rw-rw-rw-   0        0        0      485 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-commit-outline.svg
--rw-rw-rw-   0        0        0      232 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-commit-sharp.svg
--rw-rw-rw-   0        0        0      262 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-commit.svg
--rw-rw-rw-   0        0        0      882 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-compare-outline.svg
--rw-rw-rw-   0        0        0      438 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-compare-sharp.svg
--rw-rw-rw-   0        0        0      546 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-compare.svg
--rw-rw-rw-   0        0        0      733 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-merge-outline.svg
--rw-rw-rw-   0        0        0      375 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-merge-sharp.svg
--rw-rw-rw-   0        0        0      451 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-merge.svg
--rw-rw-rw-   0        0        0      874 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-network-outline.svg
--rw-rw-rw-   0        0        0      434 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-network-sharp.svg
--rw-rw-rw-   0        0        0      599 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-network.svg
--rw-rw-rw-   0        0        0      869 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-pull-request-outline.svg
--rw-rw-rw-   0        0        0      453 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-pull-request-sharp.svg
--rw-rw-rw-   0        0        0      504 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/git-pull-request.svg
--rw-rw-rw-   0        0        0      837 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/glasses-outline.svg
--rw-rw-rw-   0        0        0      212 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/glasses-sharp.svg
--rw-rw-rw-   0        0        0      780 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/glasses.svg
--rw-rw-rw-   0        0        0     1028 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/globe-outline.svg
--rw-rw-rw-   0        0        0     1028 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/globe-sharp.svg
--rw-rw-rw-   0        0        0     3175 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/globe.svg
--rw-rw-rw-   0        0        0      449 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/golf-outline.svg
--rw-rw-rw-   0        0        0      416 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/golf-sharp.svg
--rw-rw-rw-   0        0        0      547 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/golf.svg
--rw-rw-rw-   0        0        0      709 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/grid-outline.svg
--rw-rw-rw-   0        0        0      221 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/grid-sharp.svg
--rw-rw-rw-   0        0        0      533 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/grid.svg
--rw-rw-rw-   0        0        0     1407 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/hammer-outline.svg
--rw-rw-rw-   0        0        0      989 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/hammer-sharp.svg
--rw-rw-rw-   0        0        0     1195 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/hammer.svg
--rw-rw-rw-   0        0        0      957 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/hand-left-outline.svg
--rw-rw-rw-   0        0        0      609 2023-05-22 03:19:38.000000 ionicons_python-1.0.0/ionicons_python/icons/hand-left-sharp.svg
--rw-rw-rw-   0        0        0      661 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/hand-left.svg
--rw-rw-rw-   0        0        0      960 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/hand-right-outline.svg
--rw-rw-rw-   0        0        0      604 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/hand-right-sharp.svg
--rw-rw-rw-   0        0        0      654 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/hand-right.svg
--rw-rw-rw-   0        0        0      407 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/happy-outline.svg
--rw-rw-rw-   0        0        0      414 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/happy-sharp.svg
--rw-rw-rw-   0        0        0      403 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/happy.svg
--rw-rw-rw-   0        0        0     1955 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/hardware-chip-outline.svg
--rw-rw-rw-   0        0        0      426 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/hardware-chip-sharp.svg
--rw-rw-rw-   0        0        0      904 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/hardware-chip.svg
--rw-rw-rw-   0        0        0      784 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/headset-outline.svg
--rw-rw-rw-   0        0        0      547 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/headset-sharp.svg
--rw-rw-rw-   0        0        0      879 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/headset.svg
--rw-rw-rw-   0        0        0      574 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/heart-circle-outline.svg
--rw-rw-rw-   0        0        0      491 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/heart-circle-sharp.svg
--rw-rw-rw-   0        0        0      509 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/heart-circle.svg
--rw-rw-rw-   0        0        0      804 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/heart-dislike-circle-outline.svg
--rw-rw-rw-   0        0        0      605 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/heart-dislike-circle-sharp.svg
--rw-rw-rw-   0        0        0      721 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/heart-dislike-circle.svg
--rw-rw-rw-   0        0        0      919 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/heart-dislike-outline.svg
--rw-rw-rw-   0        0        0      597 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/heart-dislike-sharp.svg
--rw-rw-rw-   0        0        0      624 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/heart-dislike.svg
--rw-rw-rw-   0        0        0      592 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/heart-half-outline.svg
--rw-rw-rw-   0        0        0      581 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/heart-half-sharp.svg
--rw-rw-rw-   0        0        0      592 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/heart-half.svg
--rw-rw-rw-   0        0        0      403 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/heart-outline.svg
--rw-rw-rw-   0        0        0      372 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/heart-sharp.svg
--rw-rw-rw-   0        0        0      441 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/heart.svg
--rw-rw-rw-   0        0        0     1412 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/help-buoy-outline.svg
--rw-rw-rw-   0        0        0      697 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/help-buoy-sharp.svg
--rw-rw-rw-   0        0        0      973 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/help-buoy.svg
--rw-rw-rw-   0        0        0      534 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/help-circle-outline.svg
--rw-rw-rw-   0        0        0     1363 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/help-circle-sharp.svg
--rw-rw-rw-   0        0        0      650 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/help-circle.svg
--rw-rw-rw-   0        0        0      406 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/help-outline.svg
--rw-rw-rw-   0        0        0      439 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/help-sharp.svg
--rw-rw-rw-   0        0        0      406 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/help.svg
--rw-rw-rw-   0        0        0      596 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/home-outline.svg
--rw-rw-rw-   0        0        0      242 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/home-sharp.svg
--rw-rw-rw-   0        0        0      668 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/home.svg
--rw-rw-rw-   0        0        0      726 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/hourglass-outline.svg
--rw-rw-rw-   0        0        0      207 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/hourglass-sharp.svg
--rw-rw-rw-   0        0        0      885 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/hourglass.svg
--rw-rw-rw-   0        0        0      607 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/ice-cream-outline.svg
--rw-rw-rw-   0        0        0      550 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/ice-cream-sharp.svg
--rw-rw-rw-   0        0        0      725 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/ice-cream.svg
--rw-rw-rw-   0        0        0      794 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/id-card-outline.svg
--rw-rw-rw-   0        0        0      335 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/id-card-sharp.svg
--rw-rw-rw-   0        0        0      711 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/id-card.svg
--rw-rw-rw-   0        0        0      638 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/image-outline.svg
--rw-rw-rw-   0        0        0      388 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/image-sharp.svg
--rw-rw-rw-   0        0        0      457 2023-05-22 03:19:39.000000 ionicons_python-1.0.0/ionicons_python/icons/image.svg
--rw-rw-rw-   0        0        0      861 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/images-outline.svg
--rw-rw-rw-   0        0        0      540 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/images-sharp.svg
--rw-rw-rw-   0        0        0      638 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/images.svg
--rw-rw-rw-   0        0        0      459 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/infinite-outline.svg
--rw-rw-rw-   0        0        0      614 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/infinite-sharp.svg
--rw-rw-rw-   0        0        0      462 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/infinite.svg
--rw-rw-rw-   0        0        0      589 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/information-circle-outline.svg
--rw-rw-rw-   0        0        0      278 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/information-circle-sharp.svg
--rw-rw-rw-   0        0        0      339 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/information-circle.svg
--rw-rw-rw-   0        0        0      420 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/information-outline.svg
--rw-rw-rw-   0        0        0      421 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/information-sharp.svg
--rw-rw-rw-   0        0        0      420 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/information.svg
--rw-rw-rw-   0        0        0      303 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/invert-mode-outline.svg
--rw-rw-rw-   0        0        0      290 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/invert-mode-sharp.svg
--rw-rw-rw-   0        0        0      304 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/invert-mode.svg
--rw-rw-rw-   0        0        0      337 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/journal-outline.svg
--rw-rw-rw-   0        0        0      232 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/journal-sharp.svg
--rw-rw-rw-   0        0        0      256 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/journal.svg
--rw-rw-rw-   0        0        0      723 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/key-outline.svg
--rw-rw-rw-   0        0        0      456 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/key-sharp.svg
--rw-rw-rw-   0        0        0      653 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/key.svg
--rw-rw-rw-   0        0        0     1145 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/keypad-outline.svg
--rw-rw-rw-   0        0        0      687 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/keypad-sharp.svg
--rw-rw-rw-   0        0        0      660 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/keypad.svg
--rw-rw-rw-   0        0        0      911 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/language-outline.svg
--rw-rw-rw-   0        0        0      601 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/language-sharp.svg
--rw-rw-rw-   0        0        0      779 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/language.svg
--rw-rw-rw-   0        0        0      353 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/laptop-outline.svg
--rw-rw-rw-   0        0        0      229 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/laptop-sharp.svg
--rw-rw-rw-   0        0        0      291 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/laptop.svg
--rw-rw-rw-   0        0        0      846 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/layers-outline.svg
--rw-rw-rw-   0        0        0      345 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/layers-sharp.svg
--rw-rw-rw-   0        0        0     1038 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/layers.svg
--rw-rw-rw-   0        0        0      462 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/leaf-outline.svg
--rw-rw-rw-   0        0        0      738 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/leaf-sharp.svg
--rw-rw-rw-   0        0        0      768 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/leaf.svg
--rw-rw-rw-   0        0        0     1037 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/library-outline.svg
--rw-rw-rw-   0        0        0      647 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/library-sharp.svg
--rw-rw-rw-   0        0        0      770 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/library.svg
--rw-rw-rw-   0        0        0      505 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/link-outline.svg
--rw-rw-rw-   0        0        0      521 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/link-sharp.svg
--rw-rw-rw-   0        0        0      518 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/link.svg
--rw-rw-rw-   0        0        0     1023 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/list-circle-outline.svg
--rw-rw-rw-   0        0        0      531 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/list-circle-sharp.svg
--rw-rw-rw-   0        0        0      475 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/list-circle.svg
--rw-rw-rw-   0        0        0      867 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/list-outline.svg
--rw-rw-rw-   0        0        0      843 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/list-sharp.svg
--rw-rw-rw-   0        0        0      867 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/list.svg
--rw-rw-rw-   0        0        0      759 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/locate-outline.svg
--rw-rw-rw-   0        0        0      786 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/locate-sharp.svg
--rw-rw-rw-   0        0        0      781 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/locate.svg
--rw-rw-rw-   0        0        0      466 2023-05-22 03:19:40.000000 ionicons_python-1.0.0/ionicons_python/icons/location-outline.svg
--rw-rw-rw-   0        0        0      255 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/location-sharp.svg
--rw-rw-rw-   0        0        0      407 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/location.svg
--rw-rw-rw-   0        0        0      383 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/lock-closed-outline.svg
--rw-rw-rw-   0        0        0      269 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/lock-closed-sharp.svg
--rw-rw-rw-   0        0        0      290 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/lock-closed.svg
--rw-rw-rw-   0        0        0      379 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/lock-open-outline.svg
--rw-rw-rw-   0        0        0      292 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/lock-open-sharp.svg
--rw-rw-rw-   0        0        0      292 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/lock-open.svg
--rw-rw-rw-   0        0        0      570 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/log-in-outline.svg
--rw-rw-rw-   0        0        0      340 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/log-in-sharp.svg
--rw-rw-rw-   0        0        0      389 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/log-in.svg
--rw-rw-rw-   0        0        0      568 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/log-out-outline.svg
--rw-rw-rw-   0        0        0      330 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/log-out-sharp.svg
--rw-rw-rw-   0        0        0      417 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/log-out.svg
--rw-rw-rw-   0        0        0      788 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-alipay.svg
--rw-rw-rw-   0        0        0     1456 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-amazon.svg
--rw-rw-rw-   0        0        0      267 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-amplify.svg
--rw-rw-rw-   0        0        0      506 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-android.svg
--rw-rw-rw-   0        0        0      273 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-angular.svg
--rw-rw-rw-   0        0        0     1044 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-apple-appstore.svg
--rw-rw-rw-   0        0        0     2007 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-apple-ar.svg
--rw-rw-rw-   0        0        0      637 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-apple.svg
--rw-rw-rw-   0        0        0      813 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-behance.svg
--rw-rw-rw-   0        0        0      417 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-bitbucket.svg
--rw-rw-rw-   0        0        0      979 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-bitcoin.svg
--rw-rw-rw-   0        0        0     1051 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-buffer.svg
--rw-rw-rw-   0        0        0      309 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-capacitor.svg
--rw-rw-rw-   0        0        0      948 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-chrome.svg
--rw-rw-rw-   0        0        0     1510 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-closed-captioning.svg
--rw-rw-rw-   0        0        0     1439 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-codepen.svg
--rw-rw-rw-   0        0        0      302 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-css3.svg
--rw-rw-rw-   0        0        0      476 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-designernews.svg
--rw-rw-rw-   0        0        0      347 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-deviantart.svg
--rw-rw-rw-   0        0        0     1230 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-discord.svg
--rw-rw-rw-   0        0        0     1707 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-docker.svg
--rw-rw-rw-   0        0        0     1164 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-dribbble.svg
--rw-rw-rw-   0        0        0      349 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-dropbox.svg
--rw-rw-rw-   0        0        0      557 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-edge.svg
--rw-rw-rw-   0        0        0     2227 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-electron.svg
--rw-rw-rw-   0        0        0      466 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-euro.svg
--rw-rw-rw-   0        0        0      421 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-facebook.svg
--rw-rw-rw-   0        0        0      203 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-figma.svg
--rw-rw-rw-   0        0        0      327 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-firebase.svg
--rw-rw-rw-   0        0        0      883 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-firefox.svg
--rw-rw-rw-   0        0        0      335 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-flickr.svg
--rw-rw-rw-   0        0        0      773 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-foursquare.svg
--rw-rw-rw-   0        0        0      898 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-github.svg
--rw-rw-rw-   0        0        0      820 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-gitlab.svg
--rw-rw-rw-   0        0        0      468 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-google-playstore.svg
--rw-rw-rw-   0        0        0      607 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-google.svg
--rw-rw-rw-   0        0        0      191 2023-05-22 03:19:41.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-hackernews.svg
--rw-rw-rw-   0        0        0      297 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-html5.svg
--rw-rw-rw-   0        0        0      628 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-instagram.svg
--rw-rw-rw-   0        0        0      616 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-ionic.svg
--rw-rw-rw-   0        0        0     2056 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-ionitron.svg
--rw-rw-rw-   0        0        0      713 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-javascript.svg
--rw-rw-rw-   0        0        0     1818 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-laravel.svg
--rw-rw-rw-   0        0        0      647 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-linkedin.svg
--rw-rw-rw-   0        0        0      336 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-markdown.svg
--rw-rw-rw-   0        0        0      962 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-mastodon.svg
--rw-rw-rw-   0        0        0      870 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-medium.svg
--rw-rw-rw-   0        0        0      259 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-microsoft.svg
--rw-rw-rw-   0        0        0     1772 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-no-smoking.svg
--rw-rw-rw-   0        0        0     1470 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-nodejs.svg
--rw-rw-rw-   0        0        0      375 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-npm.svg
--rw-rw-rw-   0        0        0     1684 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-octocat.svg
--rw-rw-rw-   0        0        0      824 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-paypal.svg
--rw-rw-rw-   0        0        0      800 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-pinterest.svg
--rw-rw-rw-   0        0        0     1398 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-playstation.svg
--rw-rw-rw-   0        0        0      566 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-pwa.svg
--rw-rw-rw-   0        0        0     1016 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-python.svg
--rw-rw-rw-   0        0        0     3100 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-react.svg
--rw-rw-rw-   0        0        0     1860 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-reddit.svg
--rw-rw-rw-   0        0        0      398 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-rss.svg
--rw-rw-rw-   0        0        0     3393 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-sass.svg
--rw-rw-rw-   0        0        0     1776 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-skype.svg
--rw-rw-rw-   0        0        0      675 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-slack.svg
--rw-rw-rw-   0        0        0     1478 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-snapchat.svg
--rw-rw-rw-   0        0        0     2146 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-soundcloud.svg
--rw-rw-rw-   0        0        0      357 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-stackoverflow.svg
--rw-rw-rw-   0        0        0      731 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-steam.svg
--rw-rw-rw-   0        0        0      232 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-stencil.svg
--rw-rw-rw-   0        0        0      892 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-tableau.svg
--rw-rw-rw-   0        0        0      959 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-tiktok.svg
--rw-rw-rw-   0        0        0      366 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-tumblr.svg
--rw-rw-rw-   0        0        0     5509 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-tux.svg
--rw-rw-rw-   0        0        0      288 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-twitch.svg
--rw-rw-rw-   0        0        0      688 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-twitter.svg
--rw-rw-rw-   0        0        0      583 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-usd.svg
--rw-rw-rw-   0        0        0      456 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-venmo.svg
--rw-rw-rw-   0        0        0      119 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-vercel.svg
--rw-rw-rw-   0        0        0      934 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-vimeo.svg
--rw-rw-rw-   0        0        0      884 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-vk.svg
--rw-rw-rw-   0        0        0      299 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-vue.svg
--rw-rw-rw-   0        0        0      608 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-web-component.svg
--rw-rw-rw-   0        0        0     1278 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-wechat.svg
--rw-rw-rw-   0        0        0     1156 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-whatsapp.svg
--rw-rw-rw-   0        0        0      255 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-windows.svg
--rw-rw-rw-   0        0        0     1419 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-wordpress.svg
--rw-rw-rw-   0        0        0      753 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-xbox.svg
--rw-rw-rw-   0        0        0      389 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-xing.svg
--rw-rw-rw-   0        0        0      340 2023-05-22 03:19:42.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-yahoo.svg
--rw-rw-rw-   0        0        0      232 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-yen.svg
--rw-rw-rw-   0        0        0      452 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/logo-youtube.svg
--rw-rw-rw-   0        0        0     1309 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/magnet-outline.svg
--rw-rw-rw-   0        0        0      915 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/magnet-sharp.svg
--rw-rw-rw-   0        0        0     1092 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/magnet.svg
--rw-rw-rw-   0        0        0      816 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mail-open-outline.svg
--rw-rw-rw-   0        0        0      331 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mail-open-sharp.svg
--rw-rw-rw-   0        0        0      391 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mail-open.svg
--rw-rw-rw-   0        0        0      381 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mail-outline.svg
--rw-rw-rw-   0        0        0      297 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mail-sharp.svg
--rw-rw-rw-   0        0        0      577 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mail-unread-outline.svg
--rw-rw-rw-   0        0        0     1670 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mail-unread-sharp.svg
--rw-rw-rw-   0        0        0     1823 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mail-unread.svg
--rw-rw-rw-   0        0        0      349 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mail.svg
--rw-rw-rw-   0        0        0      759 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/male-female-outline.svg
--rw-rw-rw-   0        0        0      398 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/male-female-sharp.svg
--rw-rw-rw-   0        0        0      490 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/male-female.svg
--rw-rw-rw-   0        0        0      485 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/male-outline.svg
--rw-rw-rw-   0        0        0      418 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/male-sharp.svg
--rw-rw-rw-   0        0        0      470 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/male.svg
--rw-rw-rw-   0        0        0      811 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/man-outline.svg
--rw-rw-rw-   0        0        0      239 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/man-sharp.svg
--rw-rw-rw-   0        0        0      560 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/man.svg
--rw-rw-rw-   0        0        0      743 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/map-outline.svg
--rw-rw-rw-   0        0        0      197 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/map-sharp.svg
--rw-rw-rw-   0        0        0      580 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/map.svg
--rw-rw-rw-   0        0        0      992 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/medal-outline.svg
--rw-rw-rw-   0        0        0      347 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/medal-sharp.svg
--rw-rw-rw-   0        0        0      566 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/medal.svg
--rw-rw-rw-   0        0        0      790 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/medical-outline.svg
--rw-rw-rw-   0        0        0      290 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/medical-sharp.svg
--rw-rw-rw-   0        0        0      813 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/medical.svg
--rw-rw-rw-   0        0        0      651 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/medkit-outline.svg
--rw-rw-rw-   0        0        0      374 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/medkit-sharp.svg
--rw-rw-rw-   0        0        0      524 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/medkit.svg
--rw-rw-rw-   0        0        0     1149 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/megaphone-outline.svg
--rw-rw-rw-   0        0        0      544 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/megaphone-sharp.svg
--rw-rw-rw-   0        0        0     1010 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/megaphone.svg
--rw-rw-rw-   0        0        0      489 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/menu-outline.svg
--rw-rw-rw-   0        0        0      173 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/menu-sharp.svg
--rw-rw-rw-   0        0        0      489 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/menu.svg
--rw-rw-rw-   0        0        0      763 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mic-circle-outline.svg
--rw-rw-rw-   0        0        0      550 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mic-circle-sharp.svg
--rw-rw-rw-   0        0        0      605 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mic-circle.svg
--rw-rw-rw-   0        0        0     1268 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mic-off-circle-outline.svg
--rw-rw-rw-   0        0        0      695 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mic-off-circle-sharp.svg
--rw-rw-rw-   0        0        0     1119 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mic-off-circle.svg
--rw-rw-rw-   0        0        0     1254 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mic-off-outline.svg
--rw-rw-rw-   0        0        0      641 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mic-off-sharp.svg
--rw-rw-rw-   0        0        0     1028 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mic-off.svg
--rw-rw-rw-   0        0        0      725 2023-05-22 03:19:43.000000 ionicons_python-1.0.0/ionicons_python/icons/mic-outline.svg
--rw-rw-rw-   0        0        0      691 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/mic-sharp.svg
--rw-rw-rw-   0        0        0      691 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/mic.svg
--rw-rw-rw-   0        0        0      372 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/moon-outline.svg
--rw-rw-rw-   0        0        0      324 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/moon-sharp.svg
--rw-rw-rw-   0        0        0      329 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/moon.svg
--rw-rw-rw-   0        0        0      900 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/move-outline.svg
--rw-rw-rw-   0        0        0      768 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/move-sharp.svg
--rw-rw-rw-   0        0        0      900 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/move.svg
--rw-rw-rw-   0        0        0      506 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/musical-note-outline.svg
--rw-rw-rw-   0        0        0      431 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/musical-note-sharp.svg
--rw-rw-rw-   0        0        0      451 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/musical-note.svg
--rw-rw-rw-   0        0        0      688 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/musical-notes-outline.svg
--rw-rw-rw-   0        0        0      641 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/musical-notes-sharp.svg
--rw-rw-rw-   0        0        0      695 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/musical-notes.svg
--rw-rw-rw-   0        0        0      409 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/navigate-circle-outline.svg
--rw-rw-rw-   0        0        0      259 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/navigate-circle-sharp.svg
--rw-rw-rw-   0        0        0      407 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/navigate-circle.svg
--rw-rw-rw-   0        0        0      236 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/navigate-outline.svg
--rw-rw-rw-   0        0        0      149 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/navigate-sharp.svg
--rw-rw-rw-   0        0        0      279 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/navigate.svg
--rw-rw-rw-   0        0        0     1211 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/newspaper-outline.svg
--rw-rw-rw-   0        0        0      517 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/newspaper-sharp.svg
--rw-rw-rw-   0        0        0     1058 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/newspaper.svg
--rw-rw-rw-   0        0        0      687 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/notifications-circle-outline.svg
--rw-rw-rw-   0        0        0      613 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/notifications-circle-sharp.svg
--rw-rw-rw-   0        0        0      600 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/notifications-circle.svg
--rw-rw-rw-   0        0        0      951 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/notifications-off-circle-outline.svg
--rw-rw-rw-   0        0        0      500 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/notifications-off-circle-sharp.svg
--rw-rw-rw-   0        0        0      845 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/notifications-off-circle.svg
--rw-rw-rw-   0        0        0      883 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/notifications-off-outline.svg
--rw-rw-rw-   0        0        0      481 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/notifications-off-sharp.svg
--rw-rw-rw-   0        0        0      906 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/notifications-off.svg
--rw-rw-rw-   0        0        0      665 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/notifications-outline.svg
--rw-rw-rw-   0        0        0      298 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/notifications-sharp.svg
--rw-rw-rw-   0        0        0      674 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/notifications.svg
--rw-rw-rw-   0        0        0     1164 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/nuclear-outline.svg
--rw-rw-rw-   0        0        0      571 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/nuclear-sharp.svg
--rw-rw-rw-   0        0        0      830 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/nuclear.svg
--rw-rw-rw-   0        0        0      599 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/nutrition-outline.svg
--rw-rw-rw-   0        0        0      882 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/nutrition-sharp.svg
--rw-rw-rw-   0        0        0      935 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/nutrition.svg
--rw-rw-rw-   0        0        0      543 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/open-outline.svg
--rw-rw-rw-   0        0        0      295 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/open-sharp.svg
--rw-rw-rw-   0        0        0      475 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/open.svg
--rw-rw-rw-   0        0        0     1269 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/options-outline.svg
--rw-rw-rw-   0        0        0      417 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/options-sharp.svg
--rw-rw-rw-   0        0        0      433 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/options.svg
--rw-rw-rw-   0        0        0      476 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/paper-plane-outline.svg
--rw-rw-rw-   0        0        0      167 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/paper-plane-sharp.svg
--rw-rw-rw-   0        0        0      423 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/paper-plane.svg
--rw-rw-rw-   0        0        0     1125 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/partly-sunny-outline.svg
--rw-rw-rw-   0        0        0      988 2023-05-22 03:19:44.000000 ionicons_python-1.0.0/ionicons_python/icons/partly-sunny-sharp.svg
--rw-rw-rw-   0        0        0     1223 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/partly-sunny.svg
--rw-rw-rw-   0        0        0      515 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pause-circle-outline.svg
--rw-rw-rw-   0        0        0      230 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pause-circle-sharp.svg
--rw-rw-rw-   0        0        0      284 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pause-circle.svg
--rw-rw-rw-   0        0        0      367 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pause-outline.svg
--rw-rw-rw-   0        0        0      155 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pause-sharp.svg
--rw-rw-rw-   0        0        0      311 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pause.svg
--rw-rw-rw-   0        0        0     1579 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/paw-outline.svg
--rw-rw-rw-   0        0        0      644 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/paw-sharp.svg
--rw-rw-rw-   0        0        0     1687 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/paw.svg
--rw-rw-rw-   0        0        0      471 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pencil-outline.svg
--rw-rw-rw-   0        0        0      345 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pencil-sharp.svg
--rw-rw-rw-   0        0        0      497 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pencil.svg
--rw-rw-rw-   0        0        0     1201 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/people-circle-outline.svg
--rw-rw-rw-   0        0        0      641 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/people-circle-sharp.svg
--rw-rw-rw-   0        0        0     3874 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/people-circle.svg
--rw-rw-rw-   0        0        0      956 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/people-outline.svg
--rw-rw-rw-   0        0        0      394 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/people-sharp.svg
--rw-rw-rw-   0        0        0     1154 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/people.svg
--rw-rw-rw-   0        0        0      754 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/person-add-outline.svg
--rw-rw-rw-   0        0        0      334 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/person-add-sharp.svg
--rw-rw-rw-   0        0        0      699 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/person-add.svg
--rw-rw-rw-   0        0        0      729 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/person-circle-outline.svg
--rw-rw-rw-   0        0        0      363 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/person-circle-sharp.svg
--rw-rw-rw-   0        0        0      571 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/person-circle.svg
--rw-rw-rw-   0        0        0      490 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/person-outline.svg
--rw-rw-rw-   0        0        0      622 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/person-remove-outline.svg
--rw-rw-rw-   0        0        0      263 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/person-remove-sharp.svg
--rw-rw-rw-   0        0        0      645 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/person-remove.svg
--rw-rw-rw-   0        0        0      232 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/person-sharp.svg
--rw-rw-rw-   0        0        0      563 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/person.svg
--rw-rw-rw-   0        0        0      478 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/phone-landscape-outline.svg
--rw-rw-rw-   0        0        0      219 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/phone-landscape-sharp.svg
--rw-rw-rw-   0        0        0      902 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/phone-landscape.svg
--rw-rw-rw-   0        0        0      434 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/phone-portrait-outline.svg
--rw-rw-rw-   0        0        0      219 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/phone-portrait-sharp.svg
--rw-rw-rw-   0        0        0      899 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/phone-portrait.svg
--rw-rw-rw-   0        0        0      470 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pie-chart-outline.svg
--rw-rw-rw-   0        0        0      290 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pie-chart-sharp.svg
--rw-rw-rw-   0        0        0      475 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pie-chart.svg
--rw-rw-rw-   0        0        0      409 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pin-outline.svg
--rw-rw-rw-   0        0        0      225 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pin-sharp.svg
--rw-rw-rw-   0        0        0      316 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pin.svg
--rw-rw-rw-   0        0        0      601 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pint-outline.svg
--rw-rw-rw-   0        0        0      386 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pint-sharp.svg
--rw-rw-rw-   0        0        0      601 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pint.svg
--rw-rw-rw-   0        0        0      882 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pizza-outline.svg
--rw-rw-rw-   0        0        0     1063 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pizza-sharp.svg
--rw-rw-rw-   0        0        0      969 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/pizza.svg
--rw-rw-rw-   0        0        0      420 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/planet-outline.svg
--rw-rw-rw-   0        0        0     1320 2023-05-22 03:19:45.000000 ionicons_python-1.0.0/ionicons_python/icons/planet-sharp.svg
--rw-rw-rw-   0        0        0     1443 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/planet.svg
--rw-rw-rw-   0        0        0      490 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-back-circle-outline.svg
--rw-rw-rw-   0        0        0      249 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-back-circle-sharp.svg
--rw-rw-rw-   0        0        0      419 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-back-circle.svg
--rw-rw-rw-   0        0        0      525 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-back-outline.svg
--rw-rw-rw-   0        0        0      194 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-back-sharp.svg
--rw-rw-rw-   0        0        0      437 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-back.svg
--rw-rw-rw-   0        0        0      396 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-circle-outline.svg
--rw-rw-rw-   0        0        0      213 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-circle-sharp.svg
--rw-rw-rw-   0        0        0      329 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-circle.svg
--rw-rw-rw-   0        0        0      493 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-forward-circle-outline.svg
--rw-rw-rw-   0        0        0      252 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-forward-circle-sharp.svg
--rw-rw-rw-   0        0        0      427 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-forward-circle.svg
--rw-rw-rw-   0        0        0      519 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-forward-outline.svg
--rw-rw-rw-   0        0        0      192 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-forward-sharp.svg
--rw-rw-rw-   0        0        0      435 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-forward.svg
--rw-rw-rw-   0        0        0      295 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-outline.svg
--rw-rw-rw-   0        0        0      140 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-sharp.svg
--rw-rw-rw-   0        0        0      420 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-skip-back-circle-outline.svg
--rw-rw-rw-   0        0        0      238 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-skip-back-circle-sharp.svg
--rw-rw-rw-   0        0        0      326 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-skip-back-circle.svg
--rw-rw-rw-   0        0        0      429 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-skip-back-outline.svg
--rw-rw-rw-   0        0        0      199 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-skip-back-sharp.svg
--rw-rw-rw-   0        0        0      324 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-skip-back.svg
--rw-rw-rw-   0        0        0      422 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-skip-forward-circle-outline.svg
--rw-rw-rw-   0        0        0      242 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-skip-forward-circle-sharp.svg
--rw-rw-rw-   0        0        0      330 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-skip-forward-circle.svg
--rw-rw-rw-   0        0        0      427 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-skip-forward-outline.svg
--rw-rw-rw-   0        0        0      199 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-skip-forward-sharp.svg
--rw-rw-rw-   0        0        0      325 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play-skip-forward.svg
--rw-rw-rw-   0        0        0      302 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/play.svg
--rw-rw-rw-   0        0        0      613 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/podium-outline.svg
--rw-rw-rw-   0        0        0      235 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/podium-sharp.svg
--rw-rw-rw-   0        0        0      390 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/podium.svg
--rw-rw-rw-   0        0        0      420 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/power-outline.svg
--rw-rw-rw-   0        0        0      451 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/power-sharp.svg
--rw-rw-rw-   0        0        0      471 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/power.svg
--rw-rw-rw-   0        0        0      441 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/pricetag-outline.svg
--rw-rw-rw-   0        0        0      185 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/pricetag-sharp.svg
--rw-rw-rw-   0        0        0      370 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/pricetag.svg
--rw-rw-rw-   0        0        0      585 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/pricetags-outline.svg
--rw-rw-rw-   0        0        0      260 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/pricetags-sharp.svg
--rw-rw-rw-   0        0        0      484 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/pricetags.svg
--rw-rw-rw-   0        0        0      620 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/print-outline.svg
--rw-rw-rw-   0        0        0      584 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/print-sharp.svg
--rw-rw-rw-   0        0        0      552 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/print.svg
--rw-rw-rw-   0        0        0      488 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/prism-outline.svg
--rw-rw-rw-   0        0        0      150 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/prism-sharp.svg
--rw-rw-rw-   0        0        0      398 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/prism.svg
--rw-rw-rw-   0        0        0      383 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/pulse-outline.svg
--rw-rw-rw-   0        0        0      417 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/pulse-sharp.svg
--rw-rw-rw-   0        0        0      443 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/pulse.svg
--rw-rw-rw-   0        0        0      562 2023-05-22 03:19:46.000000 ionicons_python-1.0.0/ionicons_python/icons/push-outline.svg
--rw-rw-rw-   0        0        0      314 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/push-sharp.svg
--rw-rw-rw-   0        0        0      392 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/push.svg
--rw-rw-rw-   0        0        0     1030 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/qr-code-outline.svg
--rw-rw-rw-   0        0        0      609 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/qr-code-sharp.svg
--rw-rw-rw-   0        0        0      946 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/qr-code.svg
--rw-rw-rw-   0        0        0      249 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/radio-button-off-outline.svg
--rw-rw-rw-   0        0        0      249 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/radio-button-off-sharp.svg
--rw-rw-rw-   0        0        0      249 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/radio-button-off.svg
--rw-rw-rw-   0        0        0      284 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/radio-button-on-outline.svg
--rw-rw-rw-   0        0        0      284 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/radio-button-on-sharp.svg
--rw-rw-rw-   0        0        0      284 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/radio-button-on.svg
--rw-rw-rw-   0        0        0      958 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/radio-outline.svg
--rw-rw-rw-   0        0        0      964 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/radio-sharp.svg
--rw-rw-rw-   0        0        0     1003 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/radio.svg
--rw-rw-rw-   0        0        0      967 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/rainy-outline.svg
--rw-rw-rw-   0        0        0      947 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/rainy-sharp.svg
--rw-rw-rw-   0        0        0      960 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/rainy.svg
--rw-rw-rw-   0        0        0      627 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reader-outline.svg
--rw-rw-rw-   0        0        0      256 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reader-sharp.svg
--rw-rw-rw-   0        0        0      372 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reader.svg
--rw-rw-rw-   0        0        0      747 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/receipt-outline.svg
--rw-rw-rw-   0        0        0      420 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/receipt-sharp.svg
--rw-rw-rw-   0        0        0      953 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/receipt.svg
--rw-rw-rw-   0        0        0      477 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/recording-outline.svg
--rw-rw-rw-   0        0        0      300 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/recording-sharp.svg
--rw-rw-rw-   0        0        0      436 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/recording.svg
--rw-rw-rw-   0        0        0      523 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/refresh-circle-outline.svg
--rw-rw-rw-   0        0        0      364 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/refresh-circle-sharp.svg
--rw-rw-rw-   0        0        0      434 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/refresh-circle.svg
--rw-rw-rw-   0        0        0      374 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/refresh-outline.svg
--rw-rw-rw-   0        0        0      375 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/refresh-sharp.svg
--rw-rw-rw-   0        0        0      374 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/refresh.svg
--rw-rw-rw-   0        0        0      563 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reload-circle-outline.svg
--rw-rw-rw-   0        0        0      410 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reload-circle-sharp.svg
--rw-rw-rw-   0        0        0      505 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reload-circle.svg
--rw-rw-rw-   0        0        0      436 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reload-outline.svg
--rw-rw-rw-   0        0        0      412 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reload-sharp.svg
--rw-rw-rw-   0        0        0      436 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reload.svg
--rw-rw-rw-   0        0        0      383 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/remove-circle-outline.svg
--rw-rw-rw-   0        0        0      213 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/remove-circle-sharp.svg
--rw-rw-rw-   0        0        0      243 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/remove-circle.svg
--rw-rw-rw-   0        0        0      227 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/remove-outline.svg
--rw-rw-rw-   0        0        0      228 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/remove-sharp.svg
--rw-rw-rw-   0        0        0      227 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/remove.svg
--rw-rw-rw-   0        0        0      625 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reorder-four-outline.svg
--rw-rw-rw-   0        0        0      633 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reorder-four-sharp.svg
--rw-rw-rw-   0        0        0      629 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reorder-four.svg
--rw-rw-rw-   0        0        0      492 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reorder-three-outline.svg
--rw-rw-rw-   0        0        0      498 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reorder-three-sharp.svg
--rw-rw-rw-   0        0        0      495 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reorder-three.svg
--rw-rw-rw-   0        0        0      361 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reorder-two-outline.svg
--rw-rw-rw-   0        0        0      363 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reorder-two-sharp.svg
--rw-rw-rw-   0        0        0      361 2023-05-22 03:19:47.000000 ionicons_python-1.0.0/ionicons_python/icons/reorder-two.svg
--rw-rw-rw-   0        0        0      648 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/repeat-outline.svg
--rw-rw-rw-   0        0        0      631 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/repeat-sharp.svg
--rw-rw-rw-   0        0        0      648 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/repeat.svg
--rw-rw-rw-   0        0        0      504 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/resize-outline.svg
--rw-rw-rw-   0        0        0      504 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/resize-sharp.svg
--rw-rw-rw-   0        0        0      504 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/resize.svg
--rw-rw-rw-   0        0        0     1110 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/restaurant-outline.svg
--rw-rw-rw-   0        0        0      660 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/restaurant-sharp.svg
--rw-rw-rw-   0        0        0     1331 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/restaurant.svg
--rw-rw-rw-   0        0        0      371 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/return-down-back-outline.svg
--rw-rw-rw-   0        0        0      361 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/return-down-back-sharp.svg
--rw-rw-rw-   0        0        0      371 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/return-down-back.svg
--rw-rw-rw-   0        0        0      374 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/return-down-forward-outline.svg
--rw-rw-rw-   0        0        0      361 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/return-down-forward-sharp.svg
--rw-rw-rw-   0        0        0      374 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/return-down-forward.svg
--rw-rw-rw-   0        0        0      370 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/return-up-back-outline.svg
--rw-rw-rw-   0        0        0      361 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/return-up-back-sharp.svg
--rw-rw-rw-   0        0        0      370 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/return-up-back.svg
--rw-rw-rw-   0        0        0      373 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/return-up-forward-outline.svg
--rw-rw-rw-   0        0        0      361 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/return-up-forward-sharp.svg
--rw-rw-rw-   0        0        0      373 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/return-up-forward.svg
--rw-rw-rw-   0        0        0      694 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/ribbon-outline.svg
--rw-rw-rw-   0        0        0      499 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/ribbon-sharp.svg
--rw-rw-rw-   0        0        0      945 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/ribbon.svg
--rw-rw-rw-   0        0        0      968 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/rocket-outline.svg
--rw-rw-rw-   0        0        0      966 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/rocket-sharp.svg
--rw-rw-rw-   0        0        0     1229 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/rocket.svg
--rw-rw-rw-   0        0        0      963 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/rose-outline.svg
--rw-rw-rw-   0        0        0     1126 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/rose-sharp.svg
--rw-rw-rw-   0        0        0     1382 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/rose.svg
--rw-rw-rw-   0        0        0      400 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/sad-outline.svg
--rw-rw-rw-   0        0        0      406 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/sad-sharp.svg
--rw-rw-rw-   0        0        0      401 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/sad.svg
--rw-rw-rw-   0        0        0      514 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/save-outline.svg
--rw-rw-rw-   0        0        0      285 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/save-sharp.svg
--rw-rw-rw-   0        0        0      452 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/save.svg
--rw-rw-rw-   0        0        0      555 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/scale-outline.svg
--rw-rw-rw-   0        0        0      480 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/scale-sharp.svg
--rw-rw-rw-   0        0        0      526 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/scale.svg
--rw-rw-rw-   0        0        0      795 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/scan-circle-outline.svg
--rw-rw-rw-   0        0        0      464 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/scan-circle-sharp.svg
--rw-rw-rw-   0        0        0      579 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/scan-circle.svg
--rw-rw-rw-   0        0        0      638 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/scan-outline.svg
--rw-rw-rw-   0        0        0      419 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/scan-sharp.svg
--rw-rw-rw-   0        0        0      638 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/scan.svg
--rw-rw-rw-   0        0        0      659 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/school-outline.svg
--rw-rw-rw-   0        0        0      290 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/school-sharp.svg
--rw-rw-rw-   0        0        0      563 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/school.svg
--rw-rw-rw-   0        0        0      492 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/search-circle-outline.svg
--rw-rw-rw-   0        0        0      291 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/search-circle-sharp.svg
--rw-rw-rw-   0        0        0      342 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/search-circle.svg
--rw-rw-rw-   0        0        0      386 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/search-outline.svg
--rw-rw-rw-   0        0        0      361 2023-05-22 03:19:48.000000 ionicons_python-1.0.0/ionicons_python/icons/search-sharp.svg
--rw-rw-rw-   0        0        0      389 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/search.svg
--rw-rw-rw-   0        0        0      412 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/send-outline.svg
--rw-rw-rw-   0        0        0      145 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/send-sharp.svg
--rw-rw-rw-   0        0        0      417 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/send.svg
--rw-rw-rw-   0        0        0      696 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/server-outline.svg
--rw-rw-rw-   0        0        0     1435 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/server-sharp.svg
--rw-rw-rw-   0        0        0     1538 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/server.svg
--rw-rw-rw-   0        0        0     1333 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/settings-outline.svg
--rw-rw-rw-   0        0        0      941 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/settings-sharp.svg
--rw-rw-rw-   0        0        0     1367 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/settings.svg
--rw-rw-rw-   0        0        0      330 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shapes-outline.svg
--rw-rw-rw-   0        0        0      286 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shapes-sharp.svg
--rw-rw-rw-   0        0        0      308 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shapes.svg
--rw-rw-rw-   0        0        0      561 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/share-outline.svg
--rw-rw-rw-   0        0        0      332 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/share-sharp.svg
--rw-rw-rw-   0        0        0      760 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/share-social-outline.svg
--rw-rw-rw-   0        0        0      287 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/share-social-sharp.svg
--rw-rw-rw-   0        0        0      278 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/share-social.svg
--rw-rw-rw-   0        0        0      391 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/share.svg
--rw-rw-rw-   0        0        0      494 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shield-checkmark-outline.svg
--rw-rw-rw-   0        0        0      553 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shield-checkmark-sharp.svg
--rw-rw-rw-   0        0        0      643 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shield-checkmark.svg
--rw-rw-rw-   0        0        0      433 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shield-half-outline.svg
--rw-rw-rw-   0        0        0      550 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shield-half-sharp.svg
--rw-rw-rw-   0        0        0      430 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shield-half.svg
--rw-rw-rw-   0        0        0      355 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shield-outline.svg
--rw-rw-rw-   0        0        0      375 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shield-sharp.svg
--rw-rw-rw-   0        0        0      493 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shield.svg
--rw-rw-rw-   0        0        0      563 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shirt-outline.svg
--rw-rw-rw-   0        0        0      351 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shirt-sharp.svg
--rw-rw-rw-   0        0        0      701 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shirt.svg
--rw-rw-rw-   0        0        0      840 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shuffle-outline.svg
--rw-rw-rw-   0        0        0      774 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shuffle-sharp.svg
--rw-rw-rw-   0        0        0      840 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/shuffle.svg
--rw-rw-rw-   0        0        0     1251 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/skull-outline.svg
--rw-rw-rw-   0        0        0      411 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/skull-sharp.svg
--rw-rw-rw-   0        0        0     1012 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/skull.svg
--rw-rw-rw-   0        0        0     1390 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/snow-outline.svg
--rw-rw-rw-   0        0        0     1465 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/snow-sharp.svg
--rw-rw-rw-   0        0        0     1518 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/snow.svg
--rw-rw-rw-   0        0        0      836 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/sparkles-outline.svg
--rw-rw-rw-   0        0        0      358 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/sparkles-sharp.svg
--rw-rw-rw-   0        0        0     1176 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/sparkles.svg
--rw-rw-rw-   0        0        0     1258 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/speedometer-outline.svg
--rw-rw-rw-   0        0        0      654 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/speedometer-sharp.svg
--rw-rw-rw-   0        0        0      787 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/speedometer.svg
--rw-rw-rw-   0        0        0      317 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/square-outline.svg
--rw-rw-rw-   0        0        0      139 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/square-sharp.svg
--rw-rw-rw-   0        0        0      226 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/square.svg
--rw-rw-rw-   0        0        0      317 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/star-half-outline.svg
--rw-rw-rw-   0        0        0      309 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/star-half-sharp.svg
--rw-rw-rw-   0        0        0      317 2023-05-22 03:19:49.000000 ionicons_python-1.0.0/ionicons_python/icons/star-half.svg
--rw-rw-rw-   0        0        0      245 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/star-outline.svg
--rw-rw-rw-   0        0        0      205 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/star-sharp.svg
--rw-rw-rw-   0        0        0      336 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/star.svg
--rw-rw-rw-   0        0        0      699 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/stats-chart-outline.svg
--rw-rw-rw-   0        0        0      218 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/stats-chart-sharp.svg
--rw-rw-rw-   0        0        0      531 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/stats-chart.svg
--rw-rw-rw-   0        0        0      408 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/stop-circle-outline.svg
--rw-rw-rw-   0        0        0      213 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/stop-circle-sharp.svg
--rw-rw-rw-   0        0        0      333 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/stop-circle.svg
--rw-rw-rw-   0        0        0      225 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/stop-outline.svg
--rw-rw-rw-   0        0        0      139 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/stop-sharp.svg
--rw-rw-rw-   0        0        0      204 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/stop.svg
--rw-rw-rw-   0        0        0      728 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/stopwatch-outline.svg
--rw-rw-rw-   0        0        0      347 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/stopwatch-sharp.svg
--rw-rw-rw-   0        0        0      417 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/stopwatch.svg
--rw-rw-rw-   0        0        0     1270 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/storefront-outline.svg
--rw-rw-rw-   0        0        0     1165 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/storefront-sharp.svg
--rw-rw-rw-   0        0        0     1492 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/storefront.svg
--rw-rw-rw-   0        0        0     1121 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/subway-outline.svg
--rw-rw-rw-   0        0        0      603 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/subway-sharp.svg
--rw-rw-rw-   0        0        0      645 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/subway.svg
--rw-rw-rw-   0        0        0     1325 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/sunny-outline.svg
--rw-rw-rw-   0        0        0      748 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/sunny-sharp.svg
--rw-rw-rw-   0        0        0      973 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/sunny.svg
--rw-rw-rw-   0        0        0      631 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/swap-horizontal-outline.svg
--rw-rw-rw-   0        0        0      631 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/swap-horizontal-sharp.svg
--rw-rw-rw-   0        0        0      631 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/swap-horizontal.svg
--rw-rw-rw-   0        0        0      631 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/swap-vertical-outline.svg
--rw-rw-rw-   0        0        0      631 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/swap-vertical-sharp.svg
--rw-rw-rw-   0        0        0      631 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/swap-vertical.svg
--rw-rw-rw-   0        0        0      735 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/sync-circle-outline.svg
--rw-rw-rw-   0        0        0      501 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/sync-circle-sharp.svg
--rw-rw-rw-   0        0        0      567 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/sync-circle.svg
--rw-rw-rw-   0        0        0      615 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/sync-outline.svg
--rw-rw-rw-   0        0        0      615 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/sync-sharp.svg
--rw-rw-rw-   0        0        0      615 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/sync.svg
--rw-rw-rw-   0        0        0      287 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/tablet-landscape-outline.svg
--rw-rw-rw-   0        0        0      216 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/tablet-landscape-sharp.svg
--rw-rw-rw-   0        0        0      636 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/tablet-landscape.svg
--rw-rw-rw-   0        0        0      246 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/tablet-portrait-outline.svg
--rw-rw-rw-   0        0        0      218 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/tablet-portrait-sharp.svg
--rw-rw-rw-   0        0        0      631 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/tablet-portrait.svg
--rw-rw-rw-   0        0        0     1145 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/telescope-outline.svg
--rw-rw-rw-   0        0        0      403 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/telescope-sharp.svg
--rw-rw-rw-   0        0        0     1015 2023-05-22 03:19:50.000000 ionicons_python-1.0.0/ionicons_python/icons/telescope.svg
--rw-rw-rw-   0        0        0      589 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/tennisball-outline.svg
--rw-rw-rw-   0        0        0      774 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/tennisball-sharp.svg
--rw-rw-rw-   0        0        0      706 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/tennisball.svg
--rw-rw-rw-   0        0        0      492 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/terminal-outline.svg
--rw-rw-rw-   0        0        0      283 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/terminal-sharp.svg
--rw-rw-rw-   0        0        0      389 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/terminal.svg
--rw-rw-rw-   0        0        0      737 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/text-outline.svg
--rw-rw-rw-   0        0        0      731 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/text-sharp.svg
--rw-rw-rw-   0        0        0      955 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/text.svg
--rw-rw-rw-   0        0        0      547 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/thermometer-outline.svg
--rw-rw-rw-   0        0        0      287 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/thermometer-sharp.svg
--rw-rw-rw-   0        0        0      467 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/thermometer.svg
--rw-rw-rw-   0        0        0     1210 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/thumbs-down-outline.svg
--rw-rw-rw-   0        0        0      710 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/thumbs-down-sharp.svg
--rw-rw-rw-   0        0        0     1874 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/thumbs-down.svg
--rw-rw-rw-   0        0        0     1226 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/thumbs-up-outline.svg
--rw-rw-rw-   0        0        0      370 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/thumbs-up-sharp.svg
--rw-rw-rw-   0        0        0     1902 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/thumbs-up.svg
--rw-rw-rw-   0        0        0     1121 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/thunderstorm-outline.svg
--rw-rw-rw-   0        0        0      731 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/thunderstorm-sharp.svg
--rw-rw-rw-   0        0        0      779 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/thunderstorm.svg
--rw-rw-rw-   0        0        0     1279 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/ticket-outline.svg
--rw-rw-rw-   0        0        0      467 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/ticket-sharp.svg
--rw-rw-rw-   0        0        0     1017 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/ticket.svg
--rw-rw-rw-   0        0        0      382 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/time-outline.svg
--rw-rw-rw-   0        0        0      326 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/time-sharp.svg
--rw-rw-rw-   0        0        0      268 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/time.svg
--rw-rw-rw-   0        0        0      485 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/timer-outline.svg
--rw-rw-rw-   0        0        0      477 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/timer-sharp.svg
--rw-rw-rw-   0        0        0      620 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/timer.svg
--rw-rw-rw-   0        0        0      732 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/today-outline.svg
--rw-rw-rw-   0        0        0      390 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/today-sharp.svg
--rw-rw-rw-   0        0        0      536 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/today.svg
--rw-rw-rw-   0        0        0      333 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/toggle-outline.svg
--rw-rw-rw-   0        0        0      213 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/toggle-sharp.svg
--rw-rw-rw-   0        0        0      261 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/toggle.svg
--rw-rw-rw-   0        0        0      949 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/trail-sign-outline.svg
--rw-rw-rw-   0        0        0      207 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/trail-sign-sharp.svg
--rw-rw-rw-   0        0        0      487 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/trail-sign.svg
--rw-rw-rw-   0        0        0      881 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/train-outline.svg
--rw-rw-rw-   0        0        0      522 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/train-sharp.svg
--rw-rw-rw-   0        0        0      893 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/train.svg
--rw-rw-rw-   0        0        0     1170 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/transgender-outline.svg
--rw-rw-rw-   0        0        0      598 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/transgender-sharp.svg
--rw-rw-rw-   0        0        0      780 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/transgender.svg
--rw-rw-rw-   0        0        0      699 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/trash-bin-outline.svg
--rw-rw-rw-   0        0        0      704 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/trash-bin-sharp.svg
--rw-rw-rw-   0        0        0      510 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/trash-bin.svg
--rw-rw-rw-   0        0        0      968 2023-05-22 03:19:51.000000 ionicons_python-1.0.0/ionicons_python/icons/trash-outline.svg
--rw-rw-rw-   0        0        0      536 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/trash-sharp.svg
--rw-rw-rw-   0        0        0      660 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/trash.svg
--rw-rw-rw-   0        0        0      412 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/trending-down-outline.svg
--rw-rw-rw-   0        0        0      370 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/trending-down-sharp.svg
--rw-rw-rw-   0        0        0      412 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/trending-down.svg
--rw-rw-rw-   0        0        0      412 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/trending-up-outline.svg
--rw-rw-rw-   0        0        0      370 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/trending-up-sharp.svg
--rw-rw-rw-   0        0        0      412 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/trending-up.svg
--rw-rw-rw-   0        0        0      232 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/triangle-outline.svg
--rw-rw-rw-   0        0        0      141 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/triangle-sharp.svg
--rw-rw-rw-   0        0        0      197 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/triangle.svg
--rw-rw-rw-   0        0        0      904 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/trophy-outline.svg
--rw-rw-rw-   0        0        0      631 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/trophy-sharp.svg
--rw-rw-rw-   0        0        0     1066 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/trophy.svg
--rw-rw-rw-   0        0        0      354 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/tv-outline.svg
--rw-rw-rw-   0        0        0      249 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/tv-sharp.svg
--rw-rw-rw-   0        0        0      372 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/tv.svg
--rw-rw-rw-   0        0        0      660 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/umbrella-outline.svg
--rw-rw-rw-   0        0        0      718 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/umbrella-sharp.svg
--rw-rw-rw-   0        0        0      773 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/umbrella.svg
--rw-rw-rw-   0        0        0      351 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/unlink-outline.svg
--rw-rw-rw-   0        0        0      366 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/unlink-sharp.svg
--rw-rw-rw-   0        0        0      364 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/unlink.svg
--rw-rw-rw-   0        0        0      789 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/videocam-off-outline.svg
--rw-rw-rw-   0        0        0      341 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/videocam-off-sharp.svg
--rw-rw-rw-   0        0        0      677 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/videocam-off.svg
--rw-rw-rw-   0        0        0      550 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/videocam-outline.svg
--rw-rw-rw-   0        0        0      216 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/videocam-sharp.svg
--rw-rw-rw-   0        0        0      458 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/videocam.svg
--rw-rw-rw-   0        0        0      826 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/volume-high-outline.svg
--rw-rw-rw-   0        0        0      647 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/volume-high-sharp.svg
--rw-rw-rw-   0        0        0      971 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/volume-high.svg
--rw-rw-rw-   0        0        0      522 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/volume-low-outline.svg
--rw-rw-rw-   0        0        0      385 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/volume-low-sharp.svg
--rw-rw-rw-   0        0        0      486 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/volume-low.svg
--rw-rw-rw-   0        0        0      670 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/volume-medium-outline.svg
--rw-rw-rw-   0        0        0      493 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/volume-medium-sharp.svg
--rw-rw-rw-   0        0        0      696 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/volume-medium.svg
--rw-rw-rw-   0        0        0     1412 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/volume-mute-outline.svg
--rw-rw-rw-   0        0        0      940 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/volume-mute-sharp.svg
--rw-rw-rw-   0        0        0     1235 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/volume-mute.svg
--rw-rw-rw-   0        0        0      364 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/volume-off-outline.svg
--rw-rw-rw-   0        0        0      186 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/volume-off-sharp.svg
--rw-rw-rw-   0        0        0      308 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/volume-off.svg
--rw-rw-rw-   0        0        0      871 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/walk-outline.svg
--rw-rw-rw-   0        0        0      752 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/walk-sharp.svg
--rw-rw-rw-   0        0        0      963 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/walk.svg
--rw-rw-rw-   0        0        0      438 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/wallet-outline.svg
--rw-rw-rw-   0        0        0      521 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/wallet-sharp.svg
--rw-rw-rw-   0        0        0      554 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/wallet.svg
--rw-rw-rw-   0        0        0      583 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/warning-outline.svg
--rw-rw-rw-   0        0        0      257 2023-05-22 03:19:52.000000 ionicons_python-1.0.0/ionicons_python/icons/warning-sharp.svg
--rw-rw-rw-   0        0        0      409 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/warning.svg
--rw-rw-rw-   0        0        0      484 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/watch-outline.svg
--rw-rw-rw-   0        0        0      382 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/watch-sharp.svg
--rw-rw-rw-   0        0        0      491 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/watch.svg
--rw-rw-rw-   0        0        0      445 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/water-outline.svg
--rw-rw-rw-   0        0        0      282 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/water-sharp.svg
--rw-rw-rw-   0        0        0      409 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/water.svg
--rw-rw-rw-   0        0        0      577 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/wifi-outline.svg
--rw-rw-rw-   0        0        0      580 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/wifi-sharp.svg
--rw-rw-rw-   0        0        0      530 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/wifi.svg
--rw-rw-rw-   0        0        0      594 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/wine-outline.svg
--rw-rw-rw-   0        0        0      209 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/wine-sharp.svg
--rw-rw-rw-   0        0        0      513 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/wine.svg
--rw-rw-rw-   0        0        0      999 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/woman-outline.svg
--rw-rw-rw-   0        0        0      484 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/woman-sharp.svg
--rw-rw-rw-   0        0        0      783 2023-05-22 03:19:53.000000 ionicons_python-1.0.0/ionicons_python/icons/woman.svg
--rw-rw-rw-   0        0        0    72254 2023-06-09 03:57:28.000000 ionicons_python-1.0.0/ionicons_python/ionicons_icons.py
--rw-rw-rw-   0        0        0      246 2023-06-08 13:23:49.000000 ionicons_python-1.0.0/ionicons_python/load_icon.py
-drwxrwxrwx   0        0        0        0 2023-06-09 04:33:08.101626 ionicons_python-1.0.0/ionicons_python.egg-info/
--rw-rw-rw-   0        0        0     3879 2023-06-09 04:33:07.000000 ionicons_python-1.0.0/ionicons_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    55107 2023-06-09 04:33:08.000000 ionicons_python-1.0.0/ionicons_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 04:33:07.000000 ionicons_python-1.0.0/ionicons_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-08 13:44:15.000000 ionicons_python-1.0.0/ionicons_python.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-06-09 04:33:07.000000 ionicons_python-1.0.0/ionicons_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 04:33:08.889942 ionicons_python-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1238 2023-06-09 04:29:39.000000 ionicons_python-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 04:45:10.333529 ionicons_python-1.0.1/
+-rw-rw-rw-   0        0        0       66 2023-06-09 03:18:29.000000 ionicons_python-1.0.1/AUTHORS.md
+-rw-rw-rw-   0        0        0      315 2023-06-09 03:15:09.000000 ionicons_python-1.0.1/CONTACT.md
+-rw-rw-rw-   0        0        0     1096 2023-06-08 06:22:28.000000 ionicons_python-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      176 2023-06-09 03:54:03.000000 ionicons_python-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3929 2023-06-09 04:45:10.333529 ionicons_python-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2359 2023-06-09 04:07:40.000000 ionicons_python-1.0.1/README.md
+-rw-rw-rw-   0        0        0      747 2023-06-09 04:40:37.000000 ionicons_python-1.0.1/RELEASE.md
+drwxrwxrwx   0        0        0        0 2023-06-09 04:45:09.516819 ionicons_python-1.0.1/ionicons_python/
+-rw-rw-rw-   0        0        0       57 2023-06-09 04:40:37.000000 ionicons_python-1.0.1/ionicons_python/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 04:45:09.551433 ionicons_python-1.0.1/ionicons_python/extra_icons/
+-rw-rw-rw-   0        0        0        0 2023-06-09 01:31:09.000000 ionicons_python-1.0.1/ionicons_python/extra_icons/__init__.py
+-rw-rw-rw-   0        0        0     2259 2023-05-22 03:07:13.000000 ionicons_python-1.0.1/ionicons_python/extra_icons/chatgpt.svg
+-rw-rw-rw-   0        0        0      613 2023-06-09 01:35:37.000000 ionicons_python-1.0.1/ionicons_python/extra_icons/gmail.svg
+-rw-rw-rw-   0        0        0      396 2023-06-09 01:40:51.000000 ionicons_python-1.0.1/ionicons_python/extra_icons/google-docs.svg
+-rw-rw-rw-   0        0        0     1121 2023-06-09 03:00:43.000000 ionicons_python-1.0.1/ionicons_python/extra_icons/google-drive.svg
+-rw-rw-rw-   0        0        0      497 2023-06-09 01:39:57.000000 ionicons_python-1.0.1/ionicons_python/extra_icons/google-sheets.svg
+-rw-rw-rw-   0        0        0      438 2023-06-09 01:42:39.000000 ionicons_python-1.0.1/ionicons_python/extra_icons/google-slides.svg
+-rw-rw-rw-   0        0        0      990 2023-06-09 01:38:19.000000 ionicons_python-1.0.1/ionicons_python/extra_icons/google_color.svg
+-rw-rw-rw-   0        0        0     1595 2023-06-09 02:34:08.000000 ionicons_python-1.0.1/ionicons_python/extra_icons/python_color.svg
+-rw-rw-rw-   0        0        0      552 2023-05-24 07:21:17.000000 ionicons_python-1.0.1/ionicons_python/extra_icons/streamlit.svg
+-rw-rw-rw-   0        0        0      733 2023-06-09 03:57:28.000000 ionicons_python-1.0.1/ionicons_python/extra_icons.py
+drwxrwxrwx   0        0        0        0 2023-06-09 04:45:10.332532 ionicons_python-1.0.1/ionicons_python/icons/
+-rw-rw-rw-   0        0        0        0 2023-06-08 05:29:45.000000 ionicons_python-1.0.1/ionicons_python/icons/__init__.py
+-rw-rw-rw-   0        0        0      744 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/accessibility-outline.svg
+-rw-rw-rw-   0        0        0      333 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/accessibility-sharp.svg
+-rw-rw-rw-   0        0        0      846 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/accessibility.svg
+-rw-rw-rw-   0        0        0      517 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/add-circle-outline.svg
+-rw-rw-rw-   0        0        0      240 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/add-circle-sharp.svg
+-rw-rw-rw-   0        0        0      297 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/add-circle.svg
+-rw-rw-rw-   0        0        0      361 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/add-outline.svg
+-rw-rw-rw-   0        0        0      363 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/add-sharp.svg
+-rw-rw-rw-   0        0        0      361 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/add.svg
+-rw-rw-rw-   0        0        0      742 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/airplane-outline.svg
+-rw-rw-rw-   0        0        0      494 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/airplane-sharp.svg
+-rw-rw-rw-   0        0        0      741 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/airplane.svg
+-rw-rw-rw-   0        0        0     1273 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/alarm-outline.svg
+-rw-rw-rw-   0        0        0      882 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/alarm-sharp.svg
+-rw-rw-rw-   0        0        0      912 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/alarm.svg
+-rw-rw-rw-   0        0        0      476 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/albums-outline.svg
+-rw-rw-rw-   0        0        0      217 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/albums-sharp.svg
+-rw-rw-rw-   0        0        0      383 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/albums.svg
+-rw-rw-rw-   0        0        0      507 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/alert-circle-outline.svg
+-rw-rw-rw-   0        0        0      315 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/alert-circle-sharp.svg
+-rw-rw-rw-   0        0        0      328 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/alert-circle.svg
+-rw-rw-rw-   0        0        0      426 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/alert-outline.svg
+-rw-rw-rw-   0        0        0      377 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/alert-sharp.svg
+-rw-rw-rw-   0        0        0      426 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/alert.svg
+-rw-rw-rw-   0        0        0     1145 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/american-football-outline.svg
+-rw-rw-rw-   0        0        0      969 2023-05-22 03:19:27.000000 ionicons_python-1.0.1/ionicons_python/icons/american-football-sharp.svg
+-rw-rw-rw-   0        0        0     1118 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/american-football.svg
+-rw-rw-rw-   0        0        0      993 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/analytics-outline.svg
+-rw-rw-rw-   0        0        0      341 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/analytics-sharp.svg
+-rw-rw-rw-   0        0        0      346 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/analytics.svg
+-rw-rw-rw-   0        0        0     1362 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/aperture-outline.svg
+-rw-rw-rw-   0        0        0      641 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/aperture-sharp.svg
+-rw-rw-rw-   0        0        0     1130 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/aperture.svg
+-rw-rw-rw-   0        0        0     1266 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/apps-outline.svg
+-rw-rw-rw-   0        0        0      645 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/apps-sharp.svg
+-rw-rw-rw-   0        0        0      678 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/apps.svg
+-rw-rw-rw-   0        0        0      666 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/archive-outline.svg
+-rw-rw-rw-   0        0        0      305 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/archive-sharp.svg
+-rw-rw-rw-   0        0        0      507 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/archive.svg
+-rw-rw-rw-   0        0        0      527 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-back-circle-outline.svg
+-rw-rw-rw-   0        0        0      276 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-back-circle-sharp.svg
+-rw-rw-rw-   0        0        0      367 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-back-circle.svg
+-rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-back-outline.svg
+-rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-back-sharp.svg
+-rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-back.svg
+-rw-rw-rw-   0        0        0      525 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-down-circle-outline.svg
+-rw-rw-rw-   0        0        0      278 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-down-circle-sharp.svg
+-rw-rw-rw-   0        0        0      371 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-down-circle.svg
+-rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-down-outline.svg
+-rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-down-sharp.svg
+-rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-down.svg
+-rw-rw-rw-   0        0        0      526 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-forward-circle-outline.svg
+-rw-rw-rw-   0        0        0      280 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-forward-circle-sharp.svg
+-rw-rw-rw-   0        0        0      372 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-forward-circle.svg
+-rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-forward-outline.svg
+-rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-forward-sharp.svg
+-rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-forward.svg
+-rw-rw-rw-   0        0        0      482 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-redo-circle-outline.svg
+-rw-rw-rw-   0        0        0      300 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-redo-circle-sharp.svg
+-rw-rw-rw-   0        0        0      413 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-redo-circle.svg
+-rw-rw-rw-   0        0        0      252 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-redo-outline.svg
+-rw-rw-rw-   0        0        0      289 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-redo-sharp.svg
+-rw-rw-rw-   0        0        0      379 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-redo.svg
+-rw-rw-rw-   0        0        0      485 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-undo-circle-outline.svg
+-rw-rw-rw-   0        0        0      308 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-undo-circle-sharp.svg
+-rw-rw-rw-   0        0        0      424 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-undo-circle.svg
+-rw-rw-rw-   0        0        0      253 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-undo-outline.svg
+-rw-rw-rw-   0        0        0      292 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-undo-sharp.svg
+-rw-rw-rw-   0        0        0      380 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-undo.svg
+-rw-rw-rw-   0        0        0      527 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-up-circle-outline.svg
+-rw-rw-rw-   0        0        0      278 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-up-circle-sharp.svg
+-rw-rw-rw-   0        0        0      367 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-up-circle.svg
+-rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-up-outline.svg
+-rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-up-sharp.svg
+-rw-rw-rw-   0        0        0      362 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/arrow-up.svg
+-rw-rw-rw-   0        0        0      696 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/at-circle-outline.svg
+-rw-rw-rw-   0        0        0     1224 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/at-circle-sharp.svg
+-rw-rw-rw-   0        0        0     1221 2023-05-22 03:19:28.000000 ionicons_python-1.0.1/ionicons_python/icons/at-circle.svg
+-rw-rw-rw-   0        0        0      606 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/at-outline.svg
+-rw-rw-rw-   0        0        0     1221 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/at-sharp.svg
+-rw-rw-rw-   0        0        0      606 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/at.svg
+-rw-rw-rw-   0        0        0      315 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/attach-outline.svg
+-rw-rw-rw-   0        0        0      316 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/attach-sharp.svg
+-rw-rw-rw-   0        0        0      315 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/attach.svg
+-rw-rw-rw-   0        0        0      924 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/backspace-outline.svg
+-rw-rw-rw-   0        0        0      238 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/backspace-sharp.svg
+-rw-rw-rw-   0        0        0      523 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/backspace.svg
+-rw-rw-rw-   0        0        0      751 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bag-add-outline.svg
+-rw-rw-rw-   0        0        0      394 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bag-add-sharp.svg
+-rw-rw-rw-   0        0        0      430 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bag-add.svg
+-rw-rw-rw-   0        0        0      612 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bag-check-outline.svg
+-rw-rw-rw-   0        0        0      413 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bag-check-sharp.svg
+-rw-rw-rw-   0        0        0      470 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bag-check.svg
+-rw-rw-rw-   0        0        0      599 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bag-handle-outline.svg
+-rw-rw-rw-   0        0        0      409 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bag-handle-sharp.svg
+-rw-rw-rw-   0        0        0      416 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bag-handle.svg
+-rw-rw-rw-   0        0        0      472 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bag-outline.svg
+-rw-rw-rw-   0        0        0      606 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bag-remove-outline.svg
+-rw-rw-rw-   0        0        0      367 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bag-remove-sharp.svg
+-rw-rw-rw-   0        0        0      376 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bag-remove.svg
+-rw-rw-rw-   0        0        0      337 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bag-sharp.svg
+-rw-rw-rw-   0        0        0      325 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bag.svg
+-rw-rw-rw-   0        0        0      745 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/balloon-outline.svg
+-rw-rw-rw-   0        0        0      630 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/balloon-sharp.svg
+-rw-rw-rw-   0        0        0      825 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/balloon.svg
+-rw-rw-rw-   0        0        0      303 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/ban-outline.svg
+-rw-rw-rw-   0        0        0      361 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/ban-sharp.svg
+-rw-rw-rw-   0        0        0      280 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/ban.svg
+-rw-rw-rw-   0        0        0      659 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bandage-outline.svg
+-rw-rw-rw-   0        0        0      618 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bandage-sharp.svg
+-rw-rw-rw-   0        0        0     1481 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bandage.svg
+-rw-rw-rw-   0        0        0      692 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bar-chart-outline.svg
+-rw-rw-rw-   0        0        0      263 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bar-chart-sharp.svg
+-rw-rw-rw-   0        0        0      516 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/bar-chart.svg
+-rw-rw-rw-   0        0        0      836 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/barbell-outline.svg
+-rw-rw-rw-   0        0        0      274 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/barbell-sharp.svg
+-rw-rw-rw-   0        0        0      744 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/barbell.svg
+-rw-rw-rw-   0        0        0     1144 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/barcode-outline.svg
+-rw-rw-rw-   0        0        0     1066 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/barcode-sharp.svg
+-rw-rw-rw-   0        0        0      547 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/barcode.svg
+-rw-rw-rw-   0        0        0     1670 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/baseball-outline.svg
+-rw-rw-rw-   0        0        0     1795 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/baseball-sharp.svg
+-rw-rw-rw-   0        0        0     2180 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/baseball.svg
+-rw-rw-rw-   0        0        0      545 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/basket-outline.svg
+-rw-rw-rw-   0        0        0      363 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/basket-sharp.svg
+-rw-rw-rw-   0        0        0      485 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/basket.svg
+-rw-rw-rw-   0        0        0      796 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/basketball-outline.svg
+-rw-rw-rw-   0        0        0     1061 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/basketball-sharp.svg
+-rw-rw-rw-   0        0        0     1061 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/basketball.svg
+-rw-rw-rw-   0        0        0     2111 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/battery-charging-outline.svg
+-rw-rw-rw-   0        0        0     1204 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/battery-charging-sharp.svg
+-rw-rw-rw-   0        0        0     2111 2023-05-22 03:19:29.000000 ionicons_python-1.0.1/ionicons_python/icons/battery-charging.svg
+-rw-rw-rw-   0        0        0      390 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/battery-dead-outline.svg
+-rw-rw-rw-   0        0        0      371 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/battery-dead-sharp.svg
+-rw-rw-rw-   0        0        0      390 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/battery-dead.svg
+-rw-rw-rw-   0        0        0      544 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/battery-full-outline.svg
+-rw-rw-rw-   0        0        0      255 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/battery-full-sharp.svg
+-rw-rw-rw-   0        0        0      544 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/battery-full.svg
+-rw-rw-rw-   0        0        0      544 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/battery-half-outline.svg
+-rw-rw-rw-   0        0        0      255 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/battery-half-sharp.svg
+-rw-rw-rw-   0        0        0      544 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/battery-half.svg
+-rw-rw-rw-   0        0        0      517 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/beaker-outline.svg
+-rw-rw-rw-   0        0        0      407 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/beaker-sharp.svg
+-rw-rw-rw-   0        0        0      516 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/beaker.svg
+-rw-rw-rw-   0        0        0      943 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bed-outline.svg
+-rw-rw-rw-   0        0        0      331 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bed-sharp.svg
+-rw-rw-rw-   0        0        0      647 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bed.svg
+-rw-rw-rw-   0        0        0     1394 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/beer-outline.svg
+-rw-rw-rw-   0        0        0     1157 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/beer-sharp.svg
+-rw-rw-rw-   0        0        0     1176 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/beer.svg
+-rw-rw-rw-   0        0        0      608 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bicycle-outline.svg
+-rw-rw-rw-   0        0        0      649 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bicycle-sharp.svg
+-rw-rw-rw-   0        0        0      847 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bicycle.svg
+-rw-rw-rw-   0        0        0      251 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bluetooth-outline.svg
+-rw-rw-rw-   0        0        0      298 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bluetooth-sharp.svg
+-rw-rw-rw-   0        0        0      425 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bluetooth.svg
+-rw-rw-rw-   0        0        0     1499 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/boat-outline.svg
+-rw-rw-rw-   0        0        0      798 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/boat-sharp.svg
+-rw-rw-rw-   0        0        0     1180 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/boat.svg
+-rw-rw-rw-   0        0        0      599 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/body-outline.svg
+-rw-rw-rw-   0        0        0      259 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/body-sharp.svg
+-rw-rw-rw-   0        0        0      560 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/body.svg
+-rw-rw-rw-   0        0        0     1804 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bonfire-outline.svg
+-rw-rw-rw-   0        0        0     1610 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bonfire-sharp.svg
+-rw-rw-rw-   0        0        0     2042 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bonfire.svg
+-rw-rw-rw-   0        0        0      544 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/book-outline.svg
+-rw-rw-rw-   0        0        0      335 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/book-sharp.svg
+-rw-rw-rw-   0        0        0      598 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/book.svg
+-rw-rw-rw-   0        0        0      268 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bookmark-outline.svg
+-rw-rw-rw-   0        0        0      139 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bookmark-sharp.svg
+-rw-rw-rw-   0        0        0      252 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bookmark.svg
+-rw-rw-rw-   0        0        0      415 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bookmarks-outline.svg
+-rw-rw-rw-   0        0        0      221 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bookmarks-sharp.svg
+-rw-rw-rw-   0        0        0      440 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bookmarks.svg
+-rw-rw-rw-   0        0        0      283 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bowling-ball-outline.svg
+-rw-rw-rw-   0        0        0      295 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bowling-ball-sharp.svg
+-rw-rw-rw-   0        0        0      295 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/bowling-ball.svg
+-rw-rw-rw-   0        0        0      666 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/briefcase-outline.svg
+-rw-rw-rw-   0        0        0      307 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/briefcase-sharp.svg
+-rw-rw-rw-   0        0        0      526 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/briefcase.svg
+-rw-rw-rw-   0        0        0      366 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/browsers-outline.svg
+-rw-rw-rw-   0        0        0      282 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/browsers-sharp.svg
+-rw-rw-rw-   0        0        0      302 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/browsers.svg
+-rw-rw-rw-   0        0        0      581 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/brush-outline.svg
+-rw-rw-rw-   0        0        0      295 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/brush-sharp.svg
+-rw-rw-rw-   0        0        0      541 2023-05-22 03:19:30.000000 ionicons_python-1.0.1/ionicons_python/icons/brush.svg
+-rw-rw-rw-   0        0        0     1509 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/bug-outline.svg
+-rw-rw-rw-   0        0        0      775 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/bug-sharp.svg
+-rw-rw-rw-   0        0        0     1292 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/bug.svg
+-rw-rw-rw-   0        0        0      588 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/build-outline.svg
+-rw-rw-rw-   0        0        0      331 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/build-sharp.svg
+-rw-rw-rw-   0        0        0      596 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/build.svg
+-rw-rw-rw-   0        0        0      905 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/bulb-outline.svg
+-rw-rw-rw-   0        0        0      533 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/bulb-sharp.svg
+-rw-rw-rw-   0        0        0      762 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/bulb.svg
+-rw-rw-rw-   0        0        0     1547 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/bus-outline.svg
+-rw-rw-rw-   0        0        0      523 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/bus-sharp.svg
+-rw-rw-rw-   0        0        0      740 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/bus.svg
+-rw-rw-rw-   0        0        0     2041 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/business-outline.svg
+-rw-rw-rw-   0        0        0      593 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/business-sharp.svg
+-rw-rw-rw-   0        0        0     1511 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/business.svg
+-rw-rw-rw-   0        0        0      573 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/cafe-outline.svg
+-rw-rw-rw-   0        0        0      426 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/cafe-sharp.svg
+-rw-rw-rw-   0        0        0      339 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/cafe.svg
+-rw-rw-rw-   0        0        0      692 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/calculator-outline.svg
+-rw-rw-rw-   0        0        0      358 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/calculator-sharp.svg
+-rw-rw-rw-   0        0        0      712 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/calculator.svg
+-rw-rw-rw-   0        0        0      587 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/calendar-clear-outline.svg
+-rw-rw-rw-   0        0        0      251 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/calendar-clear-sharp.svg
+-rw-rw-rw-   0        0        0      376 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/calendar-clear.svg
+-rw-rw-rw-   0        0        0     1224 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/calendar-number-outline.svg
+-rw-rw-rw-   0        0        0      955 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/calendar-number-sharp.svg
+-rw-rw-rw-   0        0        0     1144 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/calendar-number.svg
+-rw-rw-rw-   0        0        0      870 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/calendar-outline.svg
+-rw-rw-rw-   0        0        0      911 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/calendar-sharp.svg
+-rw-rw-rw-   0        0        0      781 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/calendar.svg
+-rw-rw-rw-   0        0        0      678 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/call-outline.svg
+-rw-rw-rw-   0        0        0      819 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/call-sharp.svg
+-rw-rw-rw-   0        0        0      938 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/call.svg
+-rw-rw-rw-   0        0        0      712 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/camera-outline.svg
+-rw-rw-rw-   0        0        0     1065 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/camera-reverse-outline.svg
+-rw-rw-rw-   0        0        0      641 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/camera-reverse-sharp.svg
+-rw-rw-rw-   0        0        0      817 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/camera-reverse.svg
+-rw-rw-rw-   0        0        0      466 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/camera-sharp.svg
+-rw-rw-rw-   0        0        0      549 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/camera.svg
+-rw-rw-rw-   0        0        0      966 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/car-outline.svg
+-rw-rw-rw-   0        0        0      495 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/car-sharp.svg
+-rw-rw-rw-   0        0        0     1901 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/car-sport-outline.svg
+-rw-rw-rw-   0        0        0     1356 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/car-sport-sharp.svg
+-rw-rw-rw-   0        0        0     2023 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/car-sport.svg
+-rw-rw-rw-   0        0        0      579 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/car.svg
+-rw-rw-rw-   0        0        0      474 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/card-outline.svg
+-rw-rw-rw-   0        0        0      304 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/card-sharp.svg
+-rw-rw-rw-   0        0        0      320 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/card.svg
+-rw-rw-rw-   0        0        0      376 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-back-circle-outline.svg
+-rw-rw-rw-   0        0        0      226 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-back-circle-sharp.svg
+-rw-rw-rw-   0        0        0      301 2023-05-22 03:19:31.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-back-circle.svg
+-rw-rw-rw-   0        0        0      239 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-back-outline.svg
+-rw-rw-rw-   0        0        0      142 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-back-sharp.svg
+-rw-rw-rw-   0        0        0      239 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-back.svg
+-rw-rw-rw-   0        0        0      377 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-down-circle-outline.svg
+-rw-rw-rw-   0        0        0      228 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-down-circle-sharp.svg
+-rw-rw-rw-   0        0        0      311 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-down-circle.svg
+-rw-rw-rw-   0        0        0      239 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-down-outline.svg
+-rw-rw-rw-   0        0        0      142 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-down-sharp.svg
+-rw-rw-rw-   0        0        0      239 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-down.svg
+-rw-rw-rw-   0        0        0      376 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-forward-circle-outline.svg
+-rw-rw-rw-   0        0        0      229 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-forward-circle-sharp.svg
+-rw-rw-rw-   0        0        0      305 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-forward-circle.svg
+-rw-rw-rw-   0        0        0      243 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-forward-outline.svg
+-rw-rw-rw-   0        0        0      143 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-forward-sharp.svg
+-rw-rw-rw-   0        0        0      243 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-forward.svg
+-rw-rw-rw-   0        0        0      377 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-up-circle-outline.svg
+-rw-rw-rw-   0        0        0      227 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-up-circle-sharp.svg
+-rw-rw-rw-   0        0        0      301 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-up-circle.svg
+-rw-rw-rw-   0        0        0      243 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-up-outline.svg
+-rw-rw-rw-   0        0        0      143 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-up-sharp.svg
+-rw-rw-rw-   0        0        0      243 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/caret-up.svg
+-rw-rw-rw-   0        0        0      654 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/cart-outline.svg
+-rw-rw-rw-   0        0        0      304 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/cart-sharp.svg
+-rw-rw-rw-   0        0        0      420 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/cart.svg
+-rw-rw-rw-   0        0        0     1173 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/cash-outline.svg
+-rw-rw-rw-   0        0        0      660 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/cash-sharp.svg
+-rw-rw-rw-   0        0        0      784 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/cash.svg
+-rw-rw-rw-   0        0        0      615 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/cellular-outline.svg
+-rw-rw-rw-   0        0        0      219 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/cellular-sharp.svg
+-rw-rw-rw-   0        0        0      529 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/cellular.svg
+-rw-rw-rw-   0        0        0      436 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/chatbox-ellipses-outline.svg
+-rw-rw-rw-   0        0        0      361 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/chatbox-ellipses-sharp.svg
+-rw-rw-rw-   0        0        0      402 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/chatbox-ellipses.svg
+-rw-rw-rw-   0        0        0      334 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/chatbox-outline.svg
+-rw-rw-rw-   0        0        0      221 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/chatbox-sharp.svg
+-rw-rw-rw-   0        0        0      294 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/chatbox.svg
+-rw-rw-rw-   0        0        0      720 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/chatbubble-ellipses-outline.svg
+-rw-rw-rw-   0        0        0      612 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/chatbubble-ellipses-sharp.svg
+-rw-rw-rw-   0        0        0      820 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/chatbubble-ellipses.svg
+-rw-rw-rw-   0        0        0      614 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/chatbubble-outline.svg
+-rw-rw-rw-   0        0        0      477 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/chatbubble-sharp.svg
+-rw-rw-rw-   0        0        0      697 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/chatbubble.svg
+-rw-rw-rw-   0        0        0      906 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/chatbubbles-outline.svg
+-rw-rw-rw-   0        0        0      888 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/chatbubbles-sharp.svg
+-rw-rw-rw-   0        0        0     1270 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/chatbubbles.svg
+-rw-rw-rw-   0        0        0      362 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/checkbox-outline.svg
+-rw-rw-rw-   0        0        0      191 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/checkbox-sharp.svg
+-rw-rw-rw-   0        0        0      380 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/checkbox.svg
+-rw-rw-rw-   0        0        0      386 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/checkmark-circle-outline.svg
+-rw-rw-rw-   0        0        0      261 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/checkmark-circle-sharp.svg
+-rw-rw-rw-   0        0        0      347 2023-05-22 03:19:32.000000 ionicons_python-1.0.1/ionicons_python/icons/checkmark-circle.svg
+-rw-rw-rw-   0        0        0      667 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/checkmark-done-circle-outline.svg
+-rw-rw-rw-   0        0        0      356 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/checkmark-done-circle-sharp.svg
+-rw-rw-rw-   0        0        0      611 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/checkmark-done-circle.svg
+-rw-rw-rw-   0        0        0      495 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/checkmark-done-outline.svg
+-rw-rw-rw-   0        0        0      495 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/checkmark-done-sharp.svg
+-rw-rw-rw-   0        0        0      495 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/checkmark-done.svg
+-rw-rw-rw-   0        0        0      227 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/checkmark-outline.svg
+-rw-rw-rw-   0        0        0      227 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/checkmark-sharp.svg
+-rw-rw-rw-   0        0        0      227 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/checkmark.svg
+-rw-rw-rw-   0        0        0      382 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-back-circle-outline.svg
+-rw-rw-rw-   0        0        0      255 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-back-circle-sharp.svg
+-rw-rw-rw-   0        0        0      299 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-back-circle.svg
+-rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-back-outline.svg
+-rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-back-sharp.svg
+-rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-back.svg
+-rw-rw-rw-   0        0        0      338 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-collapse-outline.svg
+-rw-rw-rw-   0        0        0      297 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-collapse-sharp.svg
+-rw-rw-rw-   0        0        0      552 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-collapse.svg
+-rw-rw-rw-   0        0        0      382 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-down-circle-outline.svg
+-rw-rw-rw-   0        0        0      251 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-down-circle-sharp.svg
+-rw-rw-rw-   0        0        0      315 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-down-circle.svg
+-rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-down-outline.svg
+-rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-down-sharp.svg
+-rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-down.svg
+-rw-rw-rw-   0        0        0      339 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-expand-outline.svg
+-rw-rw-rw-   0        0        0      293 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-expand-sharp.svg
+-rw-rw-rw-   0        0        0      339 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-expand.svg
+-rw-rw-rw-   0        0        0      381 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-forward-circle-outline.svg
+-rw-rw-rw-   0        0        0      250 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-forward-circle-sharp.svg
+-rw-rw-rw-   0        0        0      295 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-forward-circle.svg
+-rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-forward-outline.svg
+-rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-forward-sharp.svg
+-rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-forward.svg
+-rw-rw-rw-   0        0        0      382 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-up-circle-outline.svg
+-rw-rw-rw-   0        0        0      249 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-up-circle-sharp.svg
+-rw-rw-rw-   0        0        0      334 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-up-circle.svg
+-rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-up-outline.svg
+-rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-up-sharp.svg
+-rw-rw-rw-   0        0        0      228 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/chevron-up.svg
+-rw-rw-rw-   0        0        0      410 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/clipboard-outline.svg
+-rw-rw-rw-   0        0        0      278 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/clipboard-sharp.svg
+-rw-rw-rw-   0        0        0      373 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/clipboard.svg
+-rw-rw-rw-   0        0        0      517 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/close-circle-outline.svg
+-rw-rw-rw-   0        0        0      292 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/close-circle-sharp.svg
+-rw-rw-rw-   0        0        0      385 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/close-circle.svg
+-rw-rw-rw-   0        0        0      361 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/close-outline.svg
+-rw-rw-rw-   0        0        0      255 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/close-sharp.svg
+-rw-rw-rw-   0        0        0      240 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/close.svg
+-rw-rw-rw-   0        0        0      513 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-circle-outline.svg
+-rw-rw-rw-   0        0        0      347 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-circle-sharp.svg
+-rw-rw-rw-   0        0        0      450 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-circle.svg
+-rw-rw-rw-   0        0        0      474 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-done-outline.svg
+-rw-rw-rw-   0        0        0      550 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-done-sharp.svg
+-rw-rw-rw-   0        0        0      683 2023-05-22 03:19:33.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-done.svg
+-rw-rw-rw-   0        0        0      624 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-download-outline.svg
+-rw-rw-rw-   0        0        0      559 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-download-sharp.svg
+-rw-rw-rw-   0        0        0      684 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-download.svg
+-rw-rw-rw-   0        0        0      624 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-offline-outline.svg
+-rw-rw-rw-   0        0        0      602 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-offline-sharp.svg
+-rw-rw-rw-   0        0        0      690 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-offline.svg
+-rw-rw-rw-   0        0        0      335 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-outline.svg
+-rw-rw-rw-   0        0        0      472 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-sharp.svg
+-rw-rw-rw-   0        0        0      643 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-upload-outline.svg
+-rw-rw-rw-   0        0        0      644 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-upload-sharp.svg
+-rw-rw-rw-   0        0        0      800 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud-upload.svg
+-rw-rw-rw-   0        0        0      508 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloud.svg
+-rw-rw-rw-   0        0        0      740 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloudy-night-outline.svg
+-rw-rw-rw-   0        0        0      796 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloudy-night-sharp.svg
+-rw-rw-rw-   0        0        0     1015 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloudy-night.svg
+-rw-rw-rw-   0        0        0      428 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloudy-outline.svg
+-rw-rw-rw-   0        0        0      462 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloudy-sharp.svg
+-rw-rw-rw-   0        0        0      500 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cloudy.svg
+-rw-rw-rw-   0        0        0      638 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/code-download-outline.svg
+-rw-rw-rw-   0        0        0      638 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/code-download-sharp.svg
+-rw-rw-rw-   0        0        0      638 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/code-download.svg
+-rw-rw-rw-   0        0        0      362 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/code-outline.svg
+-rw-rw-rw-   0        0        0      300 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/code-sharp.svg
+-rw-rw-rw-   0        0        0      495 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/code-slash-outline.svg
+-rw-rw-rw-   0        0        0      372 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/code-slash-sharp.svg
+-rw-rw-rw-   0        0        0      501 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/code-slash.svg
+-rw-rw-rw-   0        0        0      464 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/code-working-outline.svg
+-rw-rw-rw-   0        0        0      707 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/code-working-sharp.svg
+-rw-rw-rw-   0        0        0      641 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/code-working.svg
+-rw-rw-rw-   0        0        0      401 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/code.svg
+-rw-rw-rw-   0        0        0     3072 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cog-outline.svg
+-rw-rw-rw-   0        0        0     3333 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cog-sharp.svg
+-rw-rw-rw-   0        0        0     3567 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/cog.svg
+-rw-rw-rw-   0        0        0      645 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/color-fill-outline.svg
+-rw-rw-rw-   0        0        0      302 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/color-fill-sharp.svg
+-rw-rw-rw-   0        0        0      748 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/color-fill.svg
+-rw-rw-rw-   0        0        0      408 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/color-filter-outline.svg
+-rw-rw-rw-   0        0        0     1006 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/color-filter-sharp.svg
+-rw-rw-rw-   0        0        0     1577 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/color-filter.svg
+-rw-rw-rw-   0        0        0      650 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/color-palette-outline.svg
+-rw-rw-rw-   0        0        0      648 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/color-palette-sharp.svg
+-rw-rw-rw-   0        0        0      838 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/color-palette.svg
+-rw-rw-rw-   0        0        0     1005 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/color-wand-outline.svg
+-rw-rw-rw-   0        0        0      665 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/color-wand-sharp.svg
+-rw-rw-rw-   0        0        0     1447 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/color-wand.svg
+-rw-rw-rw-   0        0        0      465 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/compass-outline.svg
+-rw-rw-rw-   0        0        0      257 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/compass-sharp.svg
+-rw-rw-rw-   0        0        0      384 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/compass.svg
+-rw-rw-rw-   0        0        0     1992 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/construct-outline.svg
+-rw-rw-rw-   0        0        0     1275 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/construct-sharp.svg
+-rw-rw-rw-   0        0        0     1638 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/construct.svg
+-rw-rw-rw-   0        0        0     1181 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/contract-outline.svg
+-rw-rw-rw-   0        0        0     1181 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/contract-sharp.svg
+-rw-rw-rw-   0        0        0     1181 2023-05-22 03:19:34.000000 ionicons_python-1.0.1/ionicons_python/icons/contract.svg
+-rw-rw-rw-   0        0        0      264 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/contrast-outline.svg
+-rw-rw-rw-   0        0        0      269 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/contrast-sharp.svg
+-rw-rw-rw-   0        0        0      261 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/contrast.svg
+-rw-rw-rw-   0        0        0      429 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/copy-outline.svg
+-rw-rw-rw-   0        0        0      318 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/copy-sharp.svg
+-rw-rw-rw-   0        0        0      332 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/copy.svg
+-rw-rw-rw-   0        0        0      620 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/create-outline.svg
+-rw-rw-rw-   0        0        0      549 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/create-sharp.svg
+-rw-rw-rw-   0        0        0      719 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/create.svg
+-rw-rw-rw-   0        0        0      633 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/crop-outline.svg
+-rw-rw-rw-   0        0        0      303 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/crop-sharp.svg
+-rw-rw-rw-   0        0        0      371 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/crop.svg
+-rw-rw-rw-   0        0        0      682 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/cube-outline.svg
+-rw-rw-rw-   0        0        0      267 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/cube-sharp.svg
+-rw-rw-rw-   0        0        0      480 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/cube.svg
+-rw-rw-rw-   0        0        0     1017 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/cut-outline.svg
+-rw-rw-rw-   0        0        0      481 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/cut-sharp.svg
+-rw-rw-rw-   0        0        0      804 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/cut.svg
+-rw-rw-rw-   0        0        0      624 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/desktop-outline.svg
+-rw-rw-rw-   0        0        0      313 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/desktop-sharp.svg
+-rw-rw-rw-   0        0        0      365 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/desktop.svg
+-rw-rw-rw-   0        0        0     1066 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/diamond-outline.svg
+-rw-rw-rw-   0        0        0      578 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/diamond-sharp.svg
+-rw-rw-rw-   0        0        0     1064 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/diamond.svg
+-rw-rw-rw-   0        0        0      965 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/dice-outline.svg
+-rw-rw-rw-   0        0        0      751 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/dice-sharp.svg
+-rw-rw-rw-   0        0        0     1048 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/dice.svg
+-rw-rw-rw-   0        0        0      334 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/disc-outline.svg
+-rw-rw-rw-   0        0        0      260 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/disc-sharp.svg
+-rw-rw-rw-   0        0        0      342 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/disc.svg
+-rw-rw-rw-   0        0        0      708 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/document-attach-outline.svg
+-rw-rw-rw-   0        0        0      681 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/document-attach-sharp.svg
+-rw-rw-rw-   0        0        0      750 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/document-attach.svg
+-rw-rw-rw-   0        0        0      710 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/document-lock-outline.svg
+-rw-rw-rw-   0        0        0      526 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/document-lock-sharp.svg
+-rw-rw-rw-   0        0        0      538 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/document-lock.svg
+-rw-rw-rw-   0        0        0      454 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/document-outline.svg
+-rw-rw-rw-   0        0        0      309 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/document-sharp.svg
+-rw-rw-rw-   0        0        0      722 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/document-text-outline.svg
+-rw-rw-rw-   0        0        0      340 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/document-text-sharp.svg
+-rw-rw-rw-   0        0        0      453 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/document-text.svg
+-rw-rw-rw-   0        0        0      354 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/document.svg
+-rw-rw-rw-   0        0        0      851 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/documents-outline.svg
+-rw-rw-rw-   0        0        0      493 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/documents-sharp.svg
+-rw-rw-rw-   0        0        0      644 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/documents.svg
+-rw-rw-rw-   0        0        0      562 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/download-outline.svg
+-rw-rw-rw-   0        0        0      314 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/download-sharp.svg
+-rw-rw-rw-   0        0        0      392 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/download.svg
+-rw-rw-rw-   0        0        0      697 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/duplicate-outline.svg
+-rw-rw-rw-   0        0        0      366 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/duplicate-sharp.svg
+-rw-rw-rw-   0        0        0      575 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/duplicate.svg
+-rw-rw-rw-   0        0        0      714 2023-05-22 03:19:35.000000 ionicons_python-1.0.1/ionicons_python/icons/ear-outline.svg
+-rw-rw-rw-   0        0        0      716 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ear-sharp.svg
+-rw-rw-rw-   0        0        0      758 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ear.svg
+-rw-rw-rw-   0        0        0     3614 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/earth-outline.svg
+-rw-rw-rw-   0        0        0     2560 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/earth-sharp.svg
+-rw-rw-rw-   0        0        0     2249 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/earth.svg
+-rw-rw-rw-   0        0        0      759 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/easel-outline.svg
+-rw-rw-rw-   0        0        0      373 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/easel-sharp.svg
+-rw-rw-rw-   0        0        0      536 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/easel.svg
+-rw-rw-rw-   0        0        0      260 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/egg-outline.svg
+-rw-rw-rw-   0        0        0      548 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/egg-sharp.svg
+-rw-rw-rw-   0        0        0      351 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/egg.svg
+-rw-rw-rw-   0        0        0      219 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ellipse-outline.svg
+-rw-rw-rw-   0        0        0      196 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ellipse-sharp.svg
+-rw-rw-rw-   0        0        0      196 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ellipse.svg
+-rw-rw-rw-   0        0        0      351 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ellipsis-horizontal-circle-outline.svg
+-rw-rw-rw-   0        0        0      328 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ellipsis-horizontal-circle-sharp.svg
+-rw-rw-rw-   0        0        0      351 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ellipsis-horizontal-circle.svg
+-rw-rw-rw-   0        0        0      401 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ellipsis-horizontal-outline.svg
+-rw-rw-rw-   0        0        0      194 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ellipsis-horizontal-sharp.svg
+-rw-rw-rw-   0        0        0      194 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ellipsis-horizontal.svg
+-rw-rw-rw-   0        0        0      351 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ellipsis-vertical-circle-outline.svg
+-rw-rw-rw-   0        0        0      330 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ellipsis-vertical-circle-sharp.svg
+-rw-rw-rw-   0        0        0      351 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ellipsis-vertical-circle.svg
+-rw-rw-rw-   0        0        0      401 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ellipsis-vertical-outline.svg
+-rw-rw-rw-   0        0        0      194 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ellipsis-vertical-sharp.svg
+-rw-rw-rw-   0        0        0      194 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/ellipsis-vertical.svg
+-rw-rw-rw-   0        0        0      564 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/enter-outline.svg
+-rw-rw-rw-   0        0        0      315 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/enter-sharp.svg
+-rw-rw-rw-   0        0        0      393 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/enter.svg
+-rw-rw-rw-   0        0        0      564 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/exit-outline.svg
+-rw-rw-rw-   0        0        0      353 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/exit-sharp.svg
+-rw-rw-rw-   0        0        0      392 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/exit.svg
+-rw-rw-rw-   0        0        0     1177 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/expand-outline.svg
+-rw-rw-rw-   0        0        0     1177 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/expand-sharp.svg
+-rw-rw-rw-   0        0        0     1177 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/expand.svg
+-rw-rw-rw-   0        0        0      730 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/extension-puzzle-outline.svg
+-rw-rw-rw-   0        0        0      656 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/extension-puzzle-sharp.svg
+-rw-rw-rw-   0        0        0      716 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/extension-puzzle.svg
+-rw-rw-rw-   0        0        0     1239 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/eye-off-outline.svg
+-rw-rw-rw-   0        0        0      797 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/eye-off-sharp.svg
+-rw-rw-rw-   0        0        0     1047 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/eye-off.svg
+-rw-rw-rw-   0        0        0      498 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/eye-outline.svg
+-rw-rw-rw-   0        0        0      473 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/eye-sharp.svg
+-rw-rw-rw-   0        0        0      536 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/eye.svg
+-rw-rw-rw-   0        0        0      919 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/eyedrop-outline.svg
+-rw-rw-rw-   0        0        0      449 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/eyedrop-sharp.svg
+-rw-rw-rw-   0        0        0      800 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/eyedrop.svg
+-rw-rw-rw-   0        0        0     1469 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/fast-food-outline.svg
+-rw-rw-rw-   0        0        0      942 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/fast-food-sharp.svg
+-rw-rw-rw-   0        0        0     1511 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/fast-food.svg
+-rw-rw-rw-   0        0        0      487 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/female-outline.svg
+-rw-rw-rw-   0        0        0      351 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/female-sharp.svg
+-rw-rw-rw-   0        0        0      392 2023-05-22 03:19:36.000000 ionicons_python-1.0.1/ionicons_python/icons/female.svg
+-rw-rw-rw-   0        0        0      965 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/file-tray-full-outline.svg
+-rw-rw-rw-   0        0        0      274 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/file-tray-full-sharp.svg
+-rw-rw-rw-   0        0        0      701 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/file-tray-full.svg
+-rw-rw-rw-   0        0        0      697 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/file-tray-outline.svg
+-rw-rw-rw-   0        0        0      180 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/file-tray-sharp.svg
+-rw-rw-rw-   0        0        0     1239 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/file-tray-stacked-outline.svg
+-rw-rw-rw-   0        0        0      233 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/file-tray-stacked-sharp.svg
+-rw-rw-rw-   0        0        0      732 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/file-tray-stacked.svg
+-rw-rw-rw-   0        0        0      575 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/file-tray.svg
+-rw-rw-rw-   0        0        0     1542 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/film-outline.svg
+-rw-rw-rw-   0        0        0      281 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/film-sharp.svg
+-rw-rw-rw-   0        0        0      999 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/film.svg
+-rw-rw-rw-   0        0        0      624 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/filter-circle-outline.svg
+-rw-rw-rw-   0        0        0      225 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/filter-circle-sharp.svg
+-rw-rw-rw-   0        0        0      315 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/filter-circle.svg
+-rw-rw-rw-   0        0        0      494 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/filter-outline.svg
+-rw-rw-rw-   0        0        0      232 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/filter-sharp.svg
+-rw-rw-rw-   0        0        0      280 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/filter.svg
+-rw-rw-rw-   0        0        0     2114 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/finger-print-outline.svg
+-rw-rw-rw-   0        0        0     2251 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/finger-print-sharp.svg
+-rw-rw-rw-   0        0        0     2486 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/finger-print.svg
+-rw-rw-rw-   0        0        0      703 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/fish-outline.svg
+-rw-rw-rw-   0        0        0      902 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/fish-sharp.svg
+-rw-rw-rw-   0        0        0     1146 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/fish.svg
+-rw-rw-rw-   0        0        0      569 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/fitness-outline.svg
+-rw-rw-rw-   0        0        0      673 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/fitness-sharp.svg
+-rw-rw-rw-   0        0        0      876 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/fitness.svg
+-rw-rw-rw-   0        0        0      416 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flag-outline.svg
+-rw-rw-rw-   0        0        0      402 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flag-sharp.svg
+-rw-rw-rw-   0        0        0      473 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flag.svg
+-rw-rw-rw-   0        0        0      453 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flame-outline.svg
+-rw-rw-rw-   0        0        0      565 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flame-sharp.svg
+-rw-rw-rw-   0        0        0      600 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flame.svg
+-rw-rw-rw-   0        0        0      886 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flash-off-outline.svg
+-rw-rw-rw-   0        0        0      352 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flash-off-sharp.svg
+-rw-rw-rw-   0        0        0      618 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flash-off.svg
+-rw-rw-rw-   0        0        0      364 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flash-outline.svg
+-rw-rw-rw-   0        0        0      144 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flash-sharp.svg
+-rw-rw-rw-   0        0        0      327 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flash.svg
+-rw-rw-rw-   0        0        0      711 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flashlight-outline.svg
+-rw-rw-rw-   0        0        0      364 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flashlight-sharp.svg
+-rw-rw-rw-   0        0        0      720 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flashlight.svg
+-rw-rw-rw-   0        0        0      632 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flask-outline.svg
+-rw-rw-rw-   0        0        0      374 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flask-sharp.svg
+-rw-rw-rw-   0        0        0      607 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flask.svg
+-rw-rw-rw-   0        0        0     2153 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flower-outline.svg
+-rw-rw-rw-   0        0        0     1028 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flower-sharp.svg
+-rw-rw-rw-   0        0        0      997 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/flower.svg
+-rw-rw-rw-   0        0        0      552 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/folder-open-outline.svg
+-rw-rw-rw-   0        0        0      322 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/folder-open-sharp.svg
+-rw-rw-rw-   0        0        0      427 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/folder-open.svg
+-rw-rw-rw-   0        0        0      491 2023-05-22 03:19:37.000000 ionicons_python-1.0.1/ionicons_python/icons/folder-outline.svg
+-rw-rw-rw-   0        0        0      241 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/folder-sharp.svg
+-rw-rw-rw-   0        0        0      354 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/folder.svg
+-rw-rw-rw-   0        0        0     1824 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/football-outline.svg
+-rw-rw-rw-   0        0        0      648 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/football-sharp.svg
+-rw-rw-rw-   0        0        0     1238 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/football.svg
+-rw-rw-rw-   0        0        0      968 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/footsteps-outline.svg
+-rw-rw-rw-   0        0        0     1063 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/footsteps-sharp.svg
+-rw-rw-rw-   0        0        0     1394 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/footsteps.svg
+-rw-rw-rw-   0        0        0      410 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/funnel-outline.svg
+-rw-rw-rw-   0        0        0      161 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/funnel-sharp.svg
+-rw-rw-rw-   0        0        0      332 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/funnel.svg
+-rw-rw-rw-   0        0        0      970 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/game-controller-outline.svg
+-rw-rw-rw-   0        0        0      600 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/game-controller-sharp.svg
+-rw-rw-rw-   0        0        0      947 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/game-controller.svg
+-rw-rw-rw-   0        0        0      826 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/gift-outline.svg
+-rw-rw-rw-   0        0        0      592 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/gift-sharp.svg
+-rw-rw-rw-   0        0        0      832 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/gift.svg
+-rw-rw-rw-   0        0        0      733 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-branch-outline.svg
+-rw-rw-rw-   0        0        0      392 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-branch-sharp.svg
+-rw-rw-rw-   0        0        0      508 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-branch.svg
+-rw-rw-rw-   0        0        0      485 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-commit-outline.svg
+-rw-rw-rw-   0        0        0      232 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-commit-sharp.svg
+-rw-rw-rw-   0        0        0      262 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-commit.svg
+-rw-rw-rw-   0        0        0      882 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-compare-outline.svg
+-rw-rw-rw-   0        0        0      438 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-compare-sharp.svg
+-rw-rw-rw-   0        0        0      546 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-compare.svg
+-rw-rw-rw-   0        0        0      733 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-merge-outline.svg
+-rw-rw-rw-   0        0        0      375 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-merge-sharp.svg
+-rw-rw-rw-   0        0        0      451 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-merge.svg
+-rw-rw-rw-   0        0        0      874 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-network-outline.svg
+-rw-rw-rw-   0        0        0      434 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-network-sharp.svg
+-rw-rw-rw-   0        0        0      599 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-network.svg
+-rw-rw-rw-   0        0        0      869 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-pull-request-outline.svg
+-rw-rw-rw-   0        0        0      453 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-pull-request-sharp.svg
+-rw-rw-rw-   0        0        0      504 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/git-pull-request.svg
+-rw-rw-rw-   0        0        0      837 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/glasses-outline.svg
+-rw-rw-rw-   0        0        0      212 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/glasses-sharp.svg
+-rw-rw-rw-   0        0        0      780 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/glasses.svg
+-rw-rw-rw-   0        0        0     1028 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/globe-outline.svg
+-rw-rw-rw-   0        0        0     1028 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/globe-sharp.svg
+-rw-rw-rw-   0        0        0     3175 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/globe.svg
+-rw-rw-rw-   0        0        0      449 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/golf-outline.svg
+-rw-rw-rw-   0        0        0      416 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/golf-sharp.svg
+-rw-rw-rw-   0        0        0      547 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/golf.svg
+-rw-rw-rw-   0        0        0      709 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/grid-outline.svg
+-rw-rw-rw-   0        0        0      221 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/grid-sharp.svg
+-rw-rw-rw-   0        0        0      533 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/grid.svg
+-rw-rw-rw-   0        0        0     1407 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/hammer-outline.svg
+-rw-rw-rw-   0        0        0      989 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/hammer-sharp.svg
+-rw-rw-rw-   0        0        0     1195 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/hammer.svg
+-rw-rw-rw-   0        0        0      957 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/hand-left-outline.svg
+-rw-rw-rw-   0        0        0      609 2023-05-22 03:19:38.000000 ionicons_python-1.0.1/ionicons_python/icons/hand-left-sharp.svg
+-rw-rw-rw-   0        0        0      661 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/hand-left.svg
+-rw-rw-rw-   0        0        0      960 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/hand-right-outline.svg
+-rw-rw-rw-   0        0        0      604 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/hand-right-sharp.svg
+-rw-rw-rw-   0        0        0      654 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/hand-right.svg
+-rw-rw-rw-   0        0        0      407 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/happy-outline.svg
+-rw-rw-rw-   0        0        0      414 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/happy-sharp.svg
+-rw-rw-rw-   0        0        0      403 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/happy.svg
+-rw-rw-rw-   0        0        0     1955 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/hardware-chip-outline.svg
+-rw-rw-rw-   0        0        0      426 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/hardware-chip-sharp.svg
+-rw-rw-rw-   0        0        0      904 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/hardware-chip.svg
+-rw-rw-rw-   0        0        0      784 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/headset-outline.svg
+-rw-rw-rw-   0        0        0      547 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/headset-sharp.svg
+-rw-rw-rw-   0        0        0      879 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/headset.svg
+-rw-rw-rw-   0        0        0      574 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/heart-circle-outline.svg
+-rw-rw-rw-   0        0        0      491 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/heart-circle-sharp.svg
+-rw-rw-rw-   0        0        0      509 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/heart-circle.svg
+-rw-rw-rw-   0        0        0      804 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/heart-dislike-circle-outline.svg
+-rw-rw-rw-   0        0        0      605 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/heart-dislike-circle-sharp.svg
+-rw-rw-rw-   0        0        0      721 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/heart-dislike-circle.svg
+-rw-rw-rw-   0        0        0      919 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/heart-dislike-outline.svg
+-rw-rw-rw-   0        0        0      597 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/heart-dislike-sharp.svg
+-rw-rw-rw-   0        0        0      624 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/heart-dislike.svg
+-rw-rw-rw-   0        0        0      592 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/heart-half-outline.svg
+-rw-rw-rw-   0        0        0      581 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/heart-half-sharp.svg
+-rw-rw-rw-   0        0        0      592 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/heart-half.svg
+-rw-rw-rw-   0        0        0      403 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/heart-outline.svg
+-rw-rw-rw-   0        0        0      372 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/heart-sharp.svg
+-rw-rw-rw-   0        0        0      441 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/heart.svg
+-rw-rw-rw-   0        0        0     1412 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/help-buoy-outline.svg
+-rw-rw-rw-   0        0        0      697 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/help-buoy-sharp.svg
+-rw-rw-rw-   0        0        0      973 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/help-buoy.svg
+-rw-rw-rw-   0        0        0      534 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/help-circle-outline.svg
+-rw-rw-rw-   0        0        0     1363 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/help-circle-sharp.svg
+-rw-rw-rw-   0        0        0      650 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/help-circle.svg
+-rw-rw-rw-   0        0        0      406 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/help-outline.svg
+-rw-rw-rw-   0        0        0      439 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/help-sharp.svg
+-rw-rw-rw-   0        0        0      406 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/help.svg
+-rw-rw-rw-   0        0        0      596 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/home-outline.svg
+-rw-rw-rw-   0        0        0      242 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/home-sharp.svg
+-rw-rw-rw-   0        0        0      668 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/home.svg
+-rw-rw-rw-   0        0        0      726 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/hourglass-outline.svg
+-rw-rw-rw-   0        0        0      207 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/hourglass-sharp.svg
+-rw-rw-rw-   0        0        0      885 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/hourglass.svg
+-rw-rw-rw-   0        0        0      607 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/ice-cream-outline.svg
+-rw-rw-rw-   0        0        0      550 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/ice-cream-sharp.svg
+-rw-rw-rw-   0        0        0      725 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/ice-cream.svg
+-rw-rw-rw-   0        0        0      794 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/id-card-outline.svg
+-rw-rw-rw-   0        0        0      335 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/id-card-sharp.svg
+-rw-rw-rw-   0        0        0      711 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/id-card.svg
+-rw-rw-rw-   0        0        0      638 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/image-outline.svg
+-rw-rw-rw-   0        0        0      388 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/image-sharp.svg
+-rw-rw-rw-   0        0        0      457 2023-05-22 03:19:39.000000 ionicons_python-1.0.1/ionicons_python/icons/image.svg
+-rw-rw-rw-   0        0        0      861 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/images-outline.svg
+-rw-rw-rw-   0        0        0      540 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/images-sharp.svg
+-rw-rw-rw-   0        0        0      638 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/images.svg
+-rw-rw-rw-   0        0        0      459 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/infinite-outline.svg
+-rw-rw-rw-   0        0        0      614 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/infinite-sharp.svg
+-rw-rw-rw-   0        0        0      462 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/infinite.svg
+-rw-rw-rw-   0        0        0      589 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/information-circle-outline.svg
+-rw-rw-rw-   0        0        0      278 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/information-circle-sharp.svg
+-rw-rw-rw-   0        0        0      339 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/information-circle.svg
+-rw-rw-rw-   0        0        0      420 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/information-outline.svg
+-rw-rw-rw-   0        0        0      421 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/information-sharp.svg
+-rw-rw-rw-   0        0        0      420 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/information.svg
+-rw-rw-rw-   0        0        0      303 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/invert-mode-outline.svg
+-rw-rw-rw-   0        0        0      290 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/invert-mode-sharp.svg
+-rw-rw-rw-   0        0        0      304 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/invert-mode.svg
+-rw-rw-rw-   0        0        0      337 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/journal-outline.svg
+-rw-rw-rw-   0        0        0      232 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/journal-sharp.svg
+-rw-rw-rw-   0        0        0      256 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/journal.svg
+-rw-rw-rw-   0        0        0      723 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/key-outline.svg
+-rw-rw-rw-   0        0        0      456 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/key-sharp.svg
+-rw-rw-rw-   0        0        0      653 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/key.svg
+-rw-rw-rw-   0        0        0     1145 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/keypad-outline.svg
+-rw-rw-rw-   0        0        0      687 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/keypad-sharp.svg
+-rw-rw-rw-   0        0        0      660 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/keypad.svg
+-rw-rw-rw-   0        0        0      911 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/language-outline.svg
+-rw-rw-rw-   0        0        0      601 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/language-sharp.svg
+-rw-rw-rw-   0        0        0      779 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/language.svg
+-rw-rw-rw-   0        0        0      353 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/laptop-outline.svg
+-rw-rw-rw-   0        0        0      229 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/laptop-sharp.svg
+-rw-rw-rw-   0        0        0      291 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/laptop.svg
+-rw-rw-rw-   0        0        0      846 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/layers-outline.svg
+-rw-rw-rw-   0        0        0      345 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/layers-sharp.svg
+-rw-rw-rw-   0        0        0     1038 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/layers.svg
+-rw-rw-rw-   0        0        0      462 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/leaf-outline.svg
+-rw-rw-rw-   0        0        0      738 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/leaf-sharp.svg
+-rw-rw-rw-   0        0        0      768 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/leaf.svg
+-rw-rw-rw-   0        0        0     1037 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/library-outline.svg
+-rw-rw-rw-   0        0        0      647 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/library-sharp.svg
+-rw-rw-rw-   0        0        0      770 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/library.svg
+-rw-rw-rw-   0        0        0      505 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/link-outline.svg
+-rw-rw-rw-   0        0        0      521 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/link-sharp.svg
+-rw-rw-rw-   0        0        0      518 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/link.svg
+-rw-rw-rw-   0        0        0     1023 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/list-circle-outline.svg
+-rw-rw-rw-   0        0        0      531 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/list-circle-sharp.svg
+-rw-rw-rw-   0        0        0      475 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/list-circle.svg
+-rw-rw-rw-   0        0        0      867 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/list-outline.svg
+-rw-rw-rw-   0        0        0      843 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/list-sharp.svg
+-rw-rw-rw-   0        0        0      867 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/list.svg
+-rw-rw-rw-   0        0        0      759 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/locate-outline.svg
+-rw-rw-rw-   0        0        0      786 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/locate-sharp.svg
+-rw-rw-rw-   0        0        0      781 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/locate.svg
+-rw-rw-rw-   0        0        0      466 2023-05-22 03:19:40.000000 ionicons_python-1.0.1/ionicons_python/icons/location-outline.svg
+-rw-rw-rw-   0        0        0      255 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/location-sharp.svg
+-rw-rw-rw-   0        0        0      407 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/location.svg
+-rw-rw-rw-   0        0        0      383 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/lock-closed-outline.svg
+-rw-rw-rw-   0        0        0      269 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/lock-closed-sharp.svg
+-rw-rw-rw-   0        0        0      290 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/lock-closed.svg
+-rw-rw-rw-   0        0        0      379 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/lock-open-outline.svg
+-rw-rw-rw-   0        0        0      292 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/lock-open-sharp.svg
+-rw-rw-rw-   0        0        0      292 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/lock-open.svg
+-rw-rw-rw-   0        0        0      570 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/log-in-outline.svg
+-rw-rw-rw-   0        0        0      340 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/log-in-sharp.svg
+-rw-rw-rw-   0        0        0      389 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/log-in.svg
+-rw-rw-rw-   0        0        0      568 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/log-out-outline.svg
+-rw-rw-rw-   0        0        0      330 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/log-out-sharp.svg
+-rw-rw-rw-   0        0        0      417 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/log-out.svg
+-rw-rw-rw-   0        0        0      788 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-alipay.svg
+-rw-rw-rw-   0        0        0     1456 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-amazon.svg
+-rw-rw-rw-   0        0        0      267 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-amplify.svg
+-rw-rw-rw-   0        0        0      506 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-android.svg
+-rw-rw-rw-   0        0        0      273 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-angular.svg
+-rw-rw-rw-   0        0        0     1044 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-apple-appstore.svg
+-rw-rw-rw-   0        0        0     2007 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-apple-ar.svg
+-rw-rw-rw-   0        0        0      637 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-apple.svg
+-rw-rw-rw-   0        0        0      813 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-behance.svg
+-rw-rw-rw-   0        0        0      417 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-bitbucket.svg
+-rw-rw-rw-   0        0        0      979 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-bitcoin.svg
+-rw-rw-rw-   0        0        0     1051 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-buffer.svg
+-rw-rw-rw-   0        0        0      309 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-capacitor.svg
+-rw-rw-rw-   0        0        0      948 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-chrome.svg
+-rw-rw-rw-   0        0        0     1510 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-closed-captioning.svg
+-rw-rw-rw-   0        0        0     1439 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-codepen.svg
+-rw-rw-rw-   0        0        0      302 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-css3.svg
+-rw-rw-rw-   0        0        0      476 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-designernews.svg
+-rw-rw-rw-   0        0        0      347 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-deviantart.svg
+-rw-rw-rw-   0        0        0     1230 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-discord.svg
+-rw-rw-rw-   0        0        0     1707 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-docker.svg
+-rw-rw-rw-   0        0        0     1164 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-dribbble.svg
+-rw-rw-rw-   0        0        0      349 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-dropbox.svg
+-rw-rw-rw-   0        0        0      557 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-edge.svg
+-rw-rw-rw-   0        0        0     2227 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-electron.svg
+-rw-rw-rw-   0        0        0      466 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-euro.svg
+-rw-rw-rw-   0        0        0      421 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-facebook.svg
+-rw-rw-rw-   0        0        0      203 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-figma.svg
+-rw-rw-rw-   0        0        0      327 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-firebase.svg
+-rw-rw-rw-   0        0        0      883 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-firefox.svg
+-rw-rw-rw-   0        0        0      335 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-flickr.svg
+-rw-rw-rw-   0        0        0      773 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-foursquare.svg
+-rw-rw-rw-   0        0        0      898 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-github.svg
+-rw-rw-rw-   0        0        0      820 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-gitlab.svg
+-rw-rw-rw-   0        0        0      468 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-google-playstore.svg
+-rw-rw-rw-   0        0        0      607 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-google.svg
+-rw-rw-rw-   0        0        0      191 2023-05-22 03:19:41.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-hackernews.svg
+-rw-rw-rw-   0        0        0      297 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-html5.svg
+-rw-rw-rw-   0        0        0      628 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-instagram.svg
+-rw-rw-rw-   0        0        0      616 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-ionic.svg
+-rw-rw-rw-   0        0        0     2056 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-ionitron.svg
+-rw-rw-rw-   0        0        0      713 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-javascript.svg
+-rw-rw-rw-   0        0        0     1818 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-laravel.svg
+-rw-rw-rw-   0        0        0      647 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-linkedin.svg
+-rw-rw-rw-   0        0        0      336 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-markdown.svg
+-rw-rw-rw-   0        0        0      962 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-mastodon.svg
+-rw-rw-rw-   0        0        0      870 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-medium.svg
+-rw-rw-rw-   0        0        0      259 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-microsoft.svg
+-rw-rw-rw-   0        0        0     1772 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-no-smoking.svg
+-rw-rw-rw-   0        0        0     1470 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-nodejs.svg
+-rw-rw-rw-   0        0        0      375 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-npm.svg
+-rw-rw-rw-   0        0        0     1684 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-octocat.svg
+-rw-rw-rw-   0        0        0      824 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-paypal.svg
+-rw-rw-rw-   0        0        0      800 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-pinterest.svg
+-rw-rw-rw-   0        0        0     1398 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-playstation.svg
+-rw-rw-rw-   0        0        0      566 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-pwa.svg
+-rw-rw-rw-   0        0        0     1016 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-python.svg
+-rw-rw-rw-   0        0        0     3100 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-react.svg
+-rw-rw-rw-   0        0        0     1860 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-reddit.svg
+-rw-rw-rw-   0        0        0      398 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-rss.svg
+-rw-rw-rw-   0        0        0     3393 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-sass.svg
+-rw-rw-rw-   0        0        0     1776 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-skype.svg
+-rw-rw-rw-   0        0        0      675 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-slack.svg
+-rw-rw-rw-   0        0        0     1478 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-snapchat.svg
+-rw-rw-rw-   0        0        0     2146 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-soundcloud.svg
+-rw-rw-rw-   0        0        0      357 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-stackoverflow.svg
+-rw-rw-rw-   0        0        0      731 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-steam.svg
+-rw-rw-rw-   0        0        0      232 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-stencil.svg
+-rw-rw-rw-   0        0        0      892 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-tableau.svg
+-rw-rw-rw-   0        0        0      959 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-tiktok.svg
+-rw-rw-rw-   0        0        0      366 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-tumblr.svg
+-rw-rw-rw-   0        0        0     5509 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-tux.svg
+-rw-rw-rw-   0        0        0      288 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-twitch.svg
+-rw-rw-rw-   0        0        0      688 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-twitter.svg
+-rw-rw-rw-   0        0        0      583 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-usd.svg
+-rw-rw-rw-   0        0        0      456 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-venmo.svg
+-rw-rw-rw-   0        0        0      119 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-vercel.svg
+-rw-rw-rw-   0        0        0      934 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-vimeo.svg
+-rw-rw-rw-   0        0        0      884 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-vk.svg
+-rw-rw-rw-   0        0        0      299 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-vue.svg
+-rw-rw-rw-   0        0        0      608 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-web-component.svg
+-rw-rw-rw-   0        0        0     1278 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-wechat.svg
+-rw-rw-rw-   0        0        0     1156 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-whatsapp.svg
+-rw-rw-rw-   0        0        0      255 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-windows.svg
+-rw-rw-rw-   0        0        0     1419 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-wordpress.svg
+-rw-rw-rw-   0        0        0      753 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-xbox.svg
+-rw-rw-rw-   0        0        0      389 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-xing.svg
+-rw-rw-rw-   0        0        0      340 2023-05-22 03:19:42.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-yahoo.svg
+-rw-rw-rw-   0        0        0      232 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-yen.svg
+-rw-rw-rw-   0        0        0      452 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/logo-youtube.svg
+-rw-rw-rw-   0        0        0     1309 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/magnet-outline.svg
+-rw-rw-rw-   0        0        0      915 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/magnet-sharp.svg
+-rw-rw-rw-   0        0        0     1092 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/magnet.svg
+-rw-rw-rw-   0        0        0      816 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mail-open-outline.svg
+-rw-rw-rw-   0        0        0      331 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mail-open-sharp.svg
+-rw-rw-rw-   0        0        0      391 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mail-open.svg
+-rw-rw-rw-   0        0        0      381 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mail-outline.svg
+-rw-rw-rw-   0        0        0      297 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mail-sharp.svg
+-rw-rw-rw-   0        0        0      577 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mail-unread-outline.svg
+-rw-rw-rw-   0        0        0     1670 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mail-unread-sharp.svg
+-rw-rw-rw-   0        0        0     1823 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mail-unread.svg
+-rw-rw-rw-   0        0        0      349 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mail.svg
+-rw-rw-rw-   0        0        0      759 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/male-female-outline.svg
+-rw-rw-rw-   0        0        0      398 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/male-female-sharp.svg
+-rw-rw-rw-   0        0        0      490 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/male-female.svg
+-rw-rw-rw-   0        0        0      485 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/male-outline.svg
+-rw-rw-rw-   0        0        0      418 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/male-sharp.svg
+-rw-rw-rw-   0        0        0      470 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/male.svg
+-rw-rw-rw-   0        0        0      811 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/man-outline.svg
+-rw-rw-rw-   0        0        0      239 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/man-sharp.svg
+-rw-rw-rw-   0        0        0      560 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/man.svg
+-rw-rw-rw-   0        0        0      743 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/map-outline.svg
+-rw-rw-rw-   0        0        0      197 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/map-sharp.svg
+-rw-rw-rw-   0        0        0      580 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/map.svg
+-rw-rw-rw-   0        0        0      992 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/medal-outline.svg
+-rw-rw-rw-   0        0        0      347 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/medal-sharp.svg
+-rw-rw-rw-   0        0        0      566 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/medal.svg
+-rw-rw-rw-   0        0        0      790 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/medical-outline.svg
+-rw-rw-rw-   0        0        0      290 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/medical-sharp.svg
+-rw-rw-rw-   0        0        0      813 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/medical.svg
+-rw-rw-rw-   0        0        0      651 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/medkit-outline.svg
+-rw-rw-rw-   0        0        0      374 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/medkit-sharp.svg
+-rw-rw-rw-   0        0        0      524 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/medkit.svg
+-rw-rw-rw-   0        0        0     1149 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/megaphone-outline.svg
+-rw-rw-rw-   0        0        0      544 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/megaphone-sharp.svg
+-rw-rw-rw-   0        0        0     1010 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/megaphone.svg
+-rw-rw-rw-   0        0        0      489 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/menu-outline.svg
+-rw-rw-rw-   0        0        0      173 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/menu-sharp.svg
+-rw-rw-rw-   0        0        0      489 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/menu.svg
+-rw-rw-rw-   0        0        0      763 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mic-circle-outline.svg
+-rw-rw-rw-   0        0        0      550 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mic-circle-sharp.svg
+-rw-rw-rw-   0        0        0      605 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mic-circle.svg
+-rw-rw-rw-   0        0        0     1268 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mic-off-circle-outline.svg
+-rw-rw-rw-   0        0        0      695 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mic-off-circle-sharp.svg
+-rw-rw-rw-   0        0        0     1119 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mic-off-circle.svg
+-rw-rw-rw-   0        0        0     1254 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mic-off-outline.svg
+-rw-rw-rw-   0        0        0      641 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mic-off-sharp.svg
+-rw-rw-rw-   0        0        0     1028 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mic-off.svg
+-rw-rw-rw-   0        0        0      725 2023-05-22 03:19:43.000000 ionicons_python-1.0.1/ionicons_python/icons/mic-outline.svg
+-rw-rw-rw-   0        0        0      691 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/mic-sharp.svg
+-rw-rw-rw-   0        0        0      691 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/mic.svg
+-rw-rw-rw-   0        0        0      372 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/moon-outline.svg
+-rw-rw-rw-   0        0        0      324 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/moon-sharp.svg
+-rw-rw-rw-   0        0        0      329 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/moon.svg
+-rw-rw-rw-   0        0        0      900 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/move-outline.svg
+-rw-rw-rw-   0        0        0      768 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/move-sharp.svg
+-rw-rw-rw-   0        0        0      900 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/move.svg
+-rw-rw-rw-   0        0        0      506 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/musical-note-outline.svg
+-rw-rw-rw-   0        0        0      431 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/musical-note-sharp.svg
+-rw-rw-rw-   0        0        0      451 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/musical-note.svg
+-rw-rw-rw-   0        0        0      688 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/musical-notes-outline.svg
+-rw-rw-rw-   0        0        0      641 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/musical-notes-sharp.svg
+-rw-rw-rw-   0        0        0      695 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/musical-notes.svg
+-rw-rw-rw-   0        0        0      409 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/navigate-circle-outline.svg
+-rw-rw-rw-   0        0        0      259 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/navigate-circle-sharp.svg
+-rw-rw-rw-   0        0        0      407 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/navigate-circle.svg
+-rw-rw-rw-   0        0        0      236 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/navigate-outline.svg
+-rw-rw-rw-   0        0        0      149 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/navigate-sharp.svg
+-rw-rw-rw-   0        0        0      279 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/navigate.svg
+-rw-rw-rw-   0        0        0     1211 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/newspaper-outline.svg
+-rw-rw-rw-   0        0        0      517 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/newspaper-sharp.svg
+-rw-rw-rw-   0        0        0     1058 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/newspaper.svg
+-rw-rw-rw-   0        0        0      687 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/notifications-circle-outline.svg
+-rw-rw-rw-   0        0        0      613 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/notifications-circle-sharp.svg
+-rw-rw-rw-   0        0        0      600 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/notifications-circle.svg
+-rw-rw-rw-   0        0        0      951 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/notifications-off-circle-outline.svg
+-rw-rw-rw-   0        0        0      500 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/notifications-off-circle-sharp.svg
+-rw-rw-rw-   0        0        0      845 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/notifications-off-circle.svg
+-rw-rw-rw-   0        0        0      883 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/notifications-off-outline.svg
+-rw-rw-rw-   0        0        0      481 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/notifications-off-sharp.svg
+-rw-rw-rw-   0        0        0      906 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/notifications-off.svg
+-rw-rw-rw-   0        0        0      665 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/notifications-outline.svg
+-rw-rw-rw-   0        0        0      298 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/notifications-sharp.svg
+-rw-rw-rw-   0        0        0      674 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/notifications.svg
+-rw-rw-rw-   0        0        0     1164 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/nuclear-outline.svg
+-rw-rw-rw-   0        0        0      571 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/nuclear-sharp.svg
+-rw-rw-rw-   0        0        0      830 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/nuclear.svg
+-rw-rw-rw-   0        0        0      599 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/nutrition-outline.svg
+-rw-rw-rw-   0        0        0      882 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/nutrition-sharp.svg
+-rw-rw-rw-   0        0        0      935 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/nutrition.svg
+-rw-rw-rw-   0        0        0      543 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/open-outline.svg
+-rw-rw-rw-   0        0        0      295 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/open-sharp.svg
+-rw-rw-rw-   0        0        0      475 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/open.svg
+-rw-rw-rw-   0        0        0     1269 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/options-outline.svg
+-rw-rw-rw-   0        0        0      417 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/options-sharp.svg
+-rw-rw-rw-   0        0        0      433 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/options.svg
+-rw-rw-rw-   0        0        0      476 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/paper-plane-outline.svg
+-rw-rw-rw-   0        0        0      167 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/paper-plane-sharp.svg
+-rw-rw-rw-   0        0        0      423 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/paper-plane.svg
+-rw-rw-rw-   0        0        0     1125 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/partly-sunny-outline.svg
+-rw-rw-rw-   0        0        0      988 2023-05-22 03:19:44.000000 ionicons_python-1.0.1/ionicons_python/icons/partly-sunny-sharp.svg
+-rw-rw-rw-   0        0        0     1223 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/partly-sunny.svg
+-rw-rw-rw-   0        0        0      515 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pause-circle-outline.svg
+-rw-rw-rw-   0        0        0      230 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pause-circle-sharp.svg
+-rw-rw-rw-   0        0        0      284 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pause-circle.svg
+-rw-rw-rw-   0        0        0      367 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pause-outline.svg
+-rw-rw-rw-   0        0        0      155 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pause-sharp.svg
+-rw-rw-rw-   0        0        0      311 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pause.svg
+-rw-rw-rw-   0        0        0     1579 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/paw-outline.svg
+-rw-rw-rw-   0        0        0      644 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/paw-sharp.svg
+-rw-rw-rw-   0        0        0     1687 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/paw.svg
+-rw-rw-rw-   0        0        0      471 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pencil-outline.svg
+-rw-rw-rw-   0        0        0      345 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pencil-sharp.svg
+-rw-rw-rw-   0        0        0      497 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pencil.svg
+-rw-rw-rw-   0        0        0     1201 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/people-circle-outline.svg
+-rw-rw-rw-   0        0        0      641 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/people-circle-sharp.svg
+-rw-rw-rw-   0        0        0     3874 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/people-circle.svg
+-rw-rw-rw-   0        0        0      956 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/people-outline.svg
+-rw-rw-rw-   0        0        0      394 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/people-sharp.svg
+-rw-rw-rw-   0        0        0     1154 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/people.svg
+-rw-rw-rw-   0        0        0      754 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/person-add-outline.svg
+-rw-rw-rw-   0        0        0      334 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/person-add-sharp.svg
+-rw-rw-rw-   0        0        0      699 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/person-add.svg
+-rw-rw-rw-   0        0        0      729 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/person-circle-outline.svg
+-rw-rw-rw-   0        0        0      363 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/person-circle-sharp.svg
+-rw-rw-rw-   0        0        0      571 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/person-circle.svg
+-rw-rw-rw-   0        0        0      490 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/person-outline.svg
+-rw-rw-rw-   0        0        0      622 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/person-remove-outline.svg
+-rw-rw-rw-   0        0        0      263 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/person-remove-sharp.svg
+-rw-rw-rw-   0        0        0      645 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/person-remove.svg
+-rw-rw-rw-   0        0        0      232 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/person-sharp.svg
+-rw-rw-rw-   0        0        0      563 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/person.svg
+-rw-rw-rw-   0        0        0      478 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/phone-landscape-outline.svg
+-rw-rw-rw-   0        0        0      219 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/phone-landscape-sharp.svg
+-rw-rw-rw-   0        0        0      902 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/phone-landscape.svg
+-rw-rw-rw-   0        0        0      434 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/phone-portrait-outline.svg
+-rw-rw-rw-   0        0        0      219 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/phone-portrait-sharp.svg
+-rw-rw-rw-   0        0        0      899 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/phone-portrait.svg
+-rw-rw-rw-   0        0        0      470 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pie-chart-outline.svg
+-rw-rw-rw-   0        0        0      290 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pie-chart-sharp.svg
+-rw-rw-rw-   0        0        0      475 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pie-chart.svg
+-rw-rw-rw-   0        0        0      409 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pin-outline.svg
+-rw-rw-rw-   0        0        0      225 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pin-sharp.svg
+-rw-rw-rw-   0        0        0      316 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pin.svg
+-rw-rw-rw-   0        0        0      601 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pint-outline.svg
+-rw-rw-rw-   0        0        0      386 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pint-sharp.svg
+-rw-rw-rw-   0        0        0      601 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pint.svg
+-rw-rw-rw-   0        0        0      882 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pizza-outline.svg
+-rw-rw-rw-   0        0        0     1063 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pizza-sharp.svg
+-rw-rw-rw-   0        0        0      969 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/pizza.svg
+-rw-rw-rw-   0        0        0      420 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/planet-outline.svg
+-rw-rw-rw-   0        0        0     1320 2023-05-22 03:19:45.000000 ionicons_python-1.0.1/ionicons_python/icons/planet-sharp.svg
+-rw-rw-rw-   0        0        0     1443 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/planet.svg
+-rw-rw-rw-   0        0        0      490 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-back-circle-outline.svg
+-rw-rw-rw-   0        0        0      249 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-back-circle-sharp.svg
+-rw-rw-rw-   0        0        0      419 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-back-circle.svg
+-rw-rw-rw-   0        0        0      525 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-back-outline.svg
+-rw-rw-rw-   0        0        0      194 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-back-sharp.svg
+-rw-rw-rw-   0        0        0      437 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-back.svg
+-rw-rw-rw-   0        0        0      396 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-circle-outline.svg
+-rw-rw-rw-   0        0        0      213 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-circle-sharp.svg
+-rw-rw-rw-   0        0        0      329 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-circle.svg
+-rw-rw-rw-   0        0        0      493 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-forward-circle-outline.svg
+-rw-rw-rw-   0        0        0      252 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-forward-circle-sharp.svg
+-rw-rw-rw-   0        0        0      427 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-forward-circle.svg
+-rw-rw-rw-   0        0        0      519 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-forward-outline.svg
+-rw-rw-rw-   0        0        0      192 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-forward-sharp.svg
+-rw-rw-rw-   0        0        0      435 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-forward.svg
+-rw-rw-rw-   0        0        0      295 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-outline.svg
+-rw-rw-rw-   0        0        0      140 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-sharp.svg
+-rw-rw-rw-   0        0        0      420 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-skip-back-circle-outline.svg
+-rw-rw-rw-   0        0        0      238 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-skip-back-circle-sharp.svg
+-rw-rw-rw-   0        0        0      326 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-skip-back-circle.svg
+-rw-rw-rw-   0        0        0      429 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-skip-back-outline.svg
+-rw-rw-rw-   0        0        0      199 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-skip-back-sharp.svg
+-rw-rw-rw-   0        0        0      324 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-skip-back.svg
+-rw-rw-rw-   0        0        0      422 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-skip-forward-circle-outline.svg
+-rw-rw-rw-   0        0        0      242 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-skip-forward-circle-sharp.svg
+-rw-rw-rw-   0        0        0      330 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-skip-forward-circle.svg
+-rw-rw-rw-   0        0        0      427 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-skip-forward-outline.svg
+-rw-rw-rw-   0        0        0      199 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-skip-forward-sharp.svg
+-rw-rw-rw-   0        0        0      325 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play-skip-forward.svg
+-rw-rw-rw-   0        0        0      302 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/play.svg
+-rw-rw-rw-   0        0        0      613 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/podium-outline.svg
+-rw-rw-rw-   0        0        0      235 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/podium-sharp.svg
+-rw-rw-rw-   0        0        0      390 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/podium.svg
+-rw-rw-rw-   0        0        0      420 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/power-outline.svg
+-rw-rw-rw-   0        0        0      451 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/power-sharp.svg
+-rw-rw-rw-   0        0        0      471 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/power.svg
+-rw-rw-rw-   0        0        0      441 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/pricetag-outline.svg
+-rw-rw-rw-   0        0        0      185 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/pricetag-sharp.svg
+-rw-rw-rw-   0        0        0      370 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/pricetag.svg
+-rw-rw-rw-   0        0        0      585 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/pricetags-outline.svg
+-rw-rw-rw-   0        0        0      260 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/pricetags-sharp.svg
+-rw-rw-rw-   0        0        0      484 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/pricetags.svg
+-rw-rw-rw-   0        0        0      620 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/print-outline.svg
+-rw-rw-rw-   0        0        0      584 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/print-sharp.svg
+-rw-rw-rw-   0        0        0      552 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/print.svg
+-rw-rw-rw-   0        0        0      488 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/prism-outline.svg
+-rw-rw-rw-   0        0        0      150 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/prism-sharp.svg
+-rw-rw-rw-   0        0        0      398 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/prism.svg
+-rw-rw-rw-   0        0        0      383 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/pulse-outline.svg
+-rw-rw-rw-   0        0        0      417 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/pulse-sharp.svg
+-rw-rw-rw-   0        0        0      443 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/pulse.svg
+-rw-rw-rw-   0        0        0      562 2023-05-22 03:19:46.000000 ionicons_python-1.0.1/ionicons_python/icons/push-outline.svg
+-rw-rw-rw-   0        0        0      314 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/push-sharp.svg
+-rw-rw-rw-   0        0        0      392 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/push.svg
+-rw-rw-rw-   0        0        0     1030 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/qr-code-outline.svg
+-rw-rw-rw-   0        0        0      609 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/qr-code-sharp.svg
+-rw-rw-rw-   0        0        0      946 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/qr-code.svg
+-rw-rw-rw-   0        0        0      249 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/radio-button-off-outline.svg
+-rw-rw-rw-   0        0        0      249 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/radio-button-off-sharp.svg
+-rw-rw-rw-   0        0        0      249 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/radio-button-off.svg
+-rw-rw-rw-   0        0        0      284 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/radio-button-on-outline.svg
+-rw-rw-rw-   0        0        0      284 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/radio-button-on-sharp.svg
+-rw-rw-rw-   0        0        0      284 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/radio-button-on.svg
+-rw-rw-rw-   0        0        0      958 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/radio-outline.svg
+-rw-rw-rw-   0        0        0      964 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/radio-sharp.svg
+-rw-rw-rw-   0        0        0     1003 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/radio.svg
+-rw-rw-rw-   0        0        0      967 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/rainy-outline.svg
+-rw-rw-rw-   0        0        0      947 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/rainy-sharp.svg
+-rw-rw-rw-   0        0        0      960 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/rainy.svg
+-rw-rw-rw-   0        0        0      627 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reader-outline.svg
+-rw-rw-rw-   0        0        0      256 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reader-sharp.svg
+-rw-rw-rw-   0        0        0      372 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reader.svg
+-rw-rw-rw-   0        0        0      747 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/receipt-outline.svg
+-rw-rw-rw-   0        0        0      420 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/receipt-sharp.svg
+-rw-rw-rw-   0        0        0      953 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/receipt.svg
+-rw-rw-rw-   0        0        0      477 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/recording-outline.svg
+-rw-rw-rw-   0        0        0      300 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/recording-sharp.svg
+-rw-rw-rw-   0        0        0      436 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/recording.svg
+-rw-rw-rw-   0        0        0      523 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/refresh-circle-outline.svg
+-rw-rw-rw-   0        0        0      364 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/refresh-circle-sharp.svg
+-rw-rw-rw-   0        0        0      434 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/refresh-circle.svg
+-rw-rw-rw-   0        0        0      374 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/refresh-outline.svg
+-rw-rw-rw-   0        0        0      375 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/refresh-sharp.svg
+-rw-rw-rw-   0        0        0      374 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/refresh.svg
+-rw-rw-rw-   0        0        0      563 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reload-circle-outline.svg
+-rw-rw-rw-   0        0        0      410 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reload-circle-sharp.svg
+-rw-rw-rw-   0        0        0      505 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reload-circle.svg
+-rw-rw-rw-   0        0        0      436 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reload-outline.svg
+-rw-rw-rw-   0        0        0      412 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reload-sharp.svg
+-rw-rw-rw-   0        0        0      436 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reload.svg
+-rw-rw-rw-   0        0        0      383 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/remove-circle-outline.svg
+-rw-rw-rw-   0        0        0      213 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/remove-circle-sharp.svg
+-rw-rw-rw-   0        0        0      243 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/remove-circle.svg
+-rw-rw-rw-   0        0        0      227 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/remove-outline.svg
+-rw-rw-rw-   0        0        0      228 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/remove-sharp.svg
+-rw-rw-rw-   0        0        0      227 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/remove.svg
+-rw-rw-rw-   0        0        0      625 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reorder-four-outline.svg
+-rw-rw-rw-   0        0        0      633 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reorder-four-sharp.svg
+-rw-rw-rw-   0        0        0      629 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reorder-four.svg
+-rw-rw-rw-   0        0        0      492 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reorder-three-outline.svg
+-rw-rw-rw-   0        0        0      498 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reorder-three-sharp.svg
+-rw-rw-rw-   0        0        0      495 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reorder-three.svg
+-rw-rw-rw-   0        0        0      361 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reorder-two-outline.svg
+-rw-rw-rw-   0        0        0      363 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reorder-two-sharp.svg
+-rw-rw-rw-   0        0        0      361 2023-05-22 03:19:47.000000 ionicons_python-1.0.1/ionicons_python/icons/reorder-two.svg
+-rw-rw-rw-   0        0        0      648 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/repeat-outline.svg
+-rw-rw-rw-   0        0        0      631 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/repeat-sharp.svg
+-rw-rw-rw-   0        0        0      648 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/repeat.svg
+-rw-rw-rw-   0        0        0      504 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/resize-outline.svg
+-rw-rw-rw-   0        0        0      504 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/resize-sharp.svg
+-rw-rw-rw-   0        0        0      504 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/resize.svg
+-rw-rw-rw-   0        0        0     1110 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/restaurant-outline.svg
+-rw-rw-rw-   0        0        0      660 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/restaurant-sharp.svg
+-rw-rw-rw-   0        0        0     1331 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/restaurant.svg
+-rw-rw-rw-   0        0        0      371 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/return-down-back-outline.svg
+-rw-rw-rw-   0        0        0      361 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/return-down-back-sharp.svg
+-rw-rw-rw-   0        0        0      371 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/return-down-back.svg
+-rw-rw-rw-   0        0        0      374 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/return-down-forward-outline.svg
+-rw-rw-rw-   0        0        0      361 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/return-down-forward-sharp.svg
+-rw-rw-rw-   0        0        0      374 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/return-down-forward.svg
+-rw-rw-rw-   0        0        0      370 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/return-up-back-outline.svg
+-rw-rw-rw-   0        0        0      361 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/return-up-back-sharp.svg
+-rw-rw-rw-   0        0        0      370 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/return-up-back.svg
+-rw-rw-rw-   0        0        0      373 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/return-up-forward-outline.svg
+-rw-rw-rw-   0        0        0      361 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/return-up-forward-sharp.svg
+-rw-rw-rw-   0        0        0      373 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/return-up-forward.svg
+-rw-rw-rw-   0        0        0      694 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/ribbon-outline.svg
+-rw-rw-rw-   0        0        0      499 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/ribbon-sharp.svg
+-rw-rw-rw-   0        0        0      945 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/ribbon.svg
+-rw-rw-rw-   0        0        0      968 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/rocket-outline.svg
+-rw-rw-rw-   0        0        0      966 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/rocket-sharp.svg
+-rw-rw-rw-   0        0        0     1229 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/rocket.svg
+-rw-rw-rw-   0        0        0      963 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/rose-outline.svg
+-rw-rw-rw-   0        0        0     1126 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/rose-sharp.svg
+-rw-rw-rw-   0        0        0     1382 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/rose.svg
+-rw-rw-rw-   0        0        0      400 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/sad-outline.svg
+-rw-rw-rw-   0        0        0      406 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/sad-sharp.svg
+-rw-rw-rw-   0        0        0      401 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/sad.svg
+-rw-rw-rw-   0        0        0      514 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/save-outline.svg
+-rw-rw-rw-   0        0        0      285 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/save-sharp.svg
+-rw-rw-rw-   0        0        0      452 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/save.svg
+-rw-rw-rw-   0        0        0      555 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/scale-outline.svg
+-rw-rw-rw-   0        0        0      480 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/scale-sharp.svg
+-rw-rw-rw-   0        0        0      526 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/scale.svg
+-rw-rw-rw-   0        0        0      795 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/scan-circle-outline.svg
+-rw-rw-rw-   0        0        0      464 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/scan-circle-sharp.svg
+-rw-rw-rw-   0        0        0      579 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/scan-circle.svg
+-rw-rw-rw-   0        0        0      638 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/scan-outline.svg
+-rw-rw-rw-   0        0        0      419 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/scan-sharp.svg
+-rw-rw-rw-   0        0        0      638 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/scan.svg
+-rw-rw-rw-   0        0        0      659 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/school-outline.svg
+-rw-rw-rw-   0        0        0      290 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/school-sharp.svg
+-rw-rw-rw-   0        0        0      563 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/school.svg
+-rw-rw-rw-   0        0        0      492 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/search-circle-outline.svg
+-rw-rw-rw-   0        0        0      291 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/search-circle-sharp.svg
+-rw-rw-rw-   0        0        0      342 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/search-circle.svg
+-rw-rw-rw-   0        0        0      386 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/search-outline.svg
+-rw-rw-rw-   0        0        0      361 2023-05-22 03:19:48.000000 ionicons_python-1.0.1/ionicons_python/icons/search-sharp.svg
+-rw-rw-rw-   0        0        0      389 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/search.svg
+-rw-rw-rw-   0        0        0      412 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/send-outline.svg
+-rw-rw-rw-   0        0        0      145 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/send-sharp.svg
+-rw-rw-rw-   0        0        0      417 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/send.svg
+-rw-rw-rw-   0        0        0      696 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/server-outline.svg
+-rw-rw-rw-   0        0        0     1435 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/server-sharp.svg
+-rw-rw-rw-   0        0        0     1538 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/server.svg
+-rw-rw-rw-   0        0        0     1333 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/settings-outline.svg
+-rw-rw-rw-   0        0        0      941 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/settings-sharp.svg
+-rw-rw-rw-   0        0        0     1367 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/settings.svg
+-rw-rw-rw-   0        0        0      330 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shapes-outline.svg
+-rw-rw-rw-   0        0        0      286 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shapes-sharp.svg
+-rw-rw-rw-   0        0        0      308 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shapes.svg
+-rw-rw-rw-   0        0        0      561 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/share-outline.svg
+-rw-rw-rw-   0        0        0      332 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/share-sharp.svg
+-rw-rw-rw-   0        0        0      760 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/share-social-outline.svg
+-rw-rw-rw-   0        0        0      287 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/share-social-sharp.svg
+-rw-rw-rw-   0        0        0      278 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/share-social.svg
+-rw-rw-rw-   0        0        0      391 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/share.svg
+-rw-rw-rw-   0        0        0      494 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shield-checkmark-outline.svg
+-rw-rw-rw-   0        0        0      553 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shield-checkmark-sharp.svg
+-rw-rw-rw-   0        0        0      643 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shield-checkmark.svg
+-rw-rw-rw-   0        0        0      433 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shield-half-outline.svg
+-rw-rw-rw-   0        0        0      550 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shield-half-sharp.svg
+-rw-rw-rw-   0        0        0      430 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shield-half.svg
+-rw-rw-rw-   0        0        0      355 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shield-outline.svg
+-rw-rw-rw-   0        0        0      375 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shield-sharp.svg
+-rw-rw-rw-   0        0        0      493 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shield.svg
+-rw-rw-rw-   0        0        0      563 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shirt-outline.svg
+-rw-rw-rw-   0        0        0      351 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shirt-sharp.svg
+-rw-rw-rw-   0        0        0      701 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shirt.svg
+-rw-rw-rw-   0        0        0      840 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shuffle-outline.svg
+-rw-rw-rw-   0        0        0      774 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shuffle-sharp.svg
+-rw-rw-rw-   0        0        0      840 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/shuffle.svg
+-rw-rw-rw-   0        0        0     1251 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/skull-outline.svg
+-rw-rw-rw-   0        0        0      411 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/skull-sharp.svg
+-rw-rw-rw-   0        0        0     1012 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/skull.svg
+-rw-rw-rw-   0        0        0     1390 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/snow-outline.svg
+-rw-rw-rw-   0        0        0     1465 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/snow-sharp.svg
+-rw-rw-rw-   0        0        0     1518 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/snow.svg
+-rw-rw-rw-   0        0        0      836 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/sparkles-outline.svg
+-rw-rw-rw-   0        0        0      358 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/sparkles-sharp.svg
+-rw-rw-rw-   0        0        0     1176 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/sparkles.svg
+-rw-rw-rw-   0        0        0     1258 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/speedometer-outline.svg
+-rw-rw-rw-   0        0        0      654 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/speedometer-sharp.svg
+-rw-rw-rw-   0        0        0      787 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/speedometer.svg
+-rw-rw-rw-   0        0        0      317 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/square-outline.svg
+-rw-rw-rw-   0        0        0      139 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/square-sharp.svg
+-rw-rw-rw-   0        0        0      226 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/square.svg
+-rw-rw-rw-   0        0        0      317 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/star-half-outline.svg
+-rw-rw-rw-   0        0        0      309 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/star-half-sharp.svg
+-rw-rw-rw-   0        0        0      317 2023-05-22 03:19:49.000000 ionicons_python-1.0.1/ionicons_python/icons/star-half.svg
+-rw-rw-rw-   0        0        0      245 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/star-outline.svg
+-rw-rw-rw-   0        0        0      205 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/star-sharp.svg
+-rw-rw-rw-   0        0        0      336 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/star.svg
+-rw-rw-rw-   0        0        0      699 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/stats-chart-outline.svg
+-rw-rw-rw-   0        0        0      218 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/stats-chart-sharp.svg
+-rw-rw-rw-   0        0        0      531 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/stats-chart.svg
+-rw-rw-rw-   0        0        0      408 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/stop-circle-outline.svg
+-rw-rw-rw-   0        0        0      213 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/stop-circle-sharp.svg
+-rw-rw-rw-   0        0        0      333 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/stop-circle.svg
+-rw-rw-rw-   0        0        0      225 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/stop-outline.svg
+-rw-rw-rw-   0        0        0      139 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/stop-sharp.svg
+-rw-rw-rw-   0        0        0      204 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/stop.svg
+-rw-rw-rw-   0        0        0      728 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/stopwatch-outline.svg
+-rw-rw-rw-   0        0        0      347 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/stopwatch-sharp.svg
+-rw-rw-rw-   0        0        0      417 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/stopwatch.svg
+-rw-rw-rw-   0        0        0     1270 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/storefront-outline.svg
+-rw-rw-rw-   0        0        0     1165 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/storefront-sharp.svg
+-rw-rw-rw-   0        0        0     1492 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/storefront.svg
+-rw-rw-rw-   0        0        0     1121 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/subway-outline.svg
+-rw-rw-rw-   0        0        0      603 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/subway-sharp.svg
+-rw-rw-rw-   0        0        0      645 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/subway.svg
+-rw-rw-rw-   0        0        0     1325 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/sunny-outline.svg
+-rw-rw-rw-   0        0        0      748 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/sunny-sharp.svg
+-rw-rw-rw-   0        0        0      973 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/sunny.svg
+-rw-rw-rw-   0        0        0      631 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/swap-horizontal-outline.svg
+-rw-rw-rw-   0        0        0      631 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/swap-horizontal-sharp.svg
+-rw-rw-rw-   0        0        0      631 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/swap-horizontal.svg
+-rw-rw-rw-   0        0        0      631 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/swap-vertical-outline.svg
+-rw-rw-rw-   0        0        0      631 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/swap-vertical-sharp.svg
+-rw-rw-rw-   0        0        0      631 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/swap-vertical.svg
+-rw-rw-rw-   0        0        0      735 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/sync-circle-outline.svg
+-rw-rw-rw-   0        0        0      501 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/sync-circle-sharp.svg
+-rw-rw-rw-   0        0        0      567 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/sync-circle.svg
+-rw-rw-rw-   0        0        0      615 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/sync-outline.svg
+-rw-rw-rw-   0        0        0      615 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/sync-sharp.svg
+-rw-rw-rw-   0        0        0      615 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/sync.svg
+-rw-rw-rw-   0        0        0      287 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/tablet-landscape-outline.svg
+-rw-rw-rw-   0        0        0      216 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/tablet-landscape-sharp.svg
+-rw-rw-rw-   0        0        0      636 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/tablet-landscape.svg
+-rw-rw-rw-   0        0        0      246 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/tablet-portrait-outline.svg
+-rw-rw-rw-   0        0        0      218 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/tablet-portrait-sharp.svg
+-rw-rw-rw-   0        0        0      631 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/tablet-portrait.svg
+-rw-rw-rw-   0        0        0     1145 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/telescope-outline.svg
+-rw-rw-rw-   0        0        0      403 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/telescope-sharp.svg
+-rw-rw-rw-   0        0        0     1015 2023-05-22 03:19:50.000000 ionicons_python-1.0.1/ionicons_python/icons/telescope.svg
+-rw-rw-rw-   0        0        0      589 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/tennisball-outline.svg
+-rw-rw-rw-   0        0        0      774 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/tennisball-sharp.svg
+-rw-rw-rw-   0        0        0      706 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/tennisball.svg
+-rw-rw-rw-   0        0        0      492 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/terminal-outline.svg
+-rw-rw-rw-   0        0        0      283 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/terminal-sharp.svg
+-rw-rw-rw-   0        0        0      389 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/terminal.svg
+-rw-rw-rw-   0        0        0      737 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/text-outline.svg
+-rw-rw-rw-   0        0        0      731 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/text-sharp.svg
+-rw-rw-rw-   0        0        0      955 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/text.svg
+-rw-rw-rw-   0        0        0      547 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/thermometer-outline.svg
+-rw-rw-rw-   0        0        0      287 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/thermometer-sharp.svg
+-rw-rw-rw-   0        0        0      467 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/thermometer.svg
+-rw-rw-rw-   0        0        0     1210 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/thumbs-down-outline.svg
+-rw-rw-rw-   0        0        0      710 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/thumbs-down-sharp.svg
+-rw-rw-rw-   0        0        0     1874 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/thumbs-down.svg
+-rw-rw-rw-   0        0        0     1226 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/thumbs-up-outline.svg
+-rw-rw-rw-   0        0        0      370 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/thumbs-up-sharp.svg
+-rw-rw-rw-   0        0        0     1902 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/thumbs-up.svg
+-rw-rw-rw-   0        0        0     1121 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/thunderstorm-outline.svg
+-rw-rw-rw-   0        0        0      731 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/thunderstorm-sharp.svg
+-rw-rw-rw-   0        0        0      779 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/thunderstorm.svg
+-rw-rw-rw-   0        0        0     1279 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/ticket-outline.svg
+-rw-rw-rw-   0        0        0      467 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/ticket-sharp.svg
+-rw-rw-rw-   0        0        0     1017 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/ticket.svg
+-rw-rw-rw-   0        0        0      382 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/time-outline.svg
+-rw-rw-rw-   0        0        0      326 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/time-sharp.svg
+-rw-rw-rw-   0        0        0      268 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/time.svg
+-rw-rw-rw-   0        0        0      485 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/timer-outline.svg
+-rw-rw-rw-   0        0        0      477 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/timer-sharp.svg
+-rw-rw-rw-   0        0        0      620 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/timer.svg
+-rw-rw-rw-   0        0        0      732 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/today-outline.svg
+-rw-rw-rw-   0        0        0      390 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/today-sharp.svg
+-rw-rw-rw-   0        0        0      536 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/today.svg
+-rw-rw-rw-   0        0        0      333 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/toggle-outline.svg
+-rw-rw-rw-   0        0        0      213 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/toggle-sharp.svg
+-rw-rw-rw-   0        0        0      261 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/toggle.svg
+-rw-rw-rw-   0        0        0      949 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/trail-sign-outline.svg
+-rw-rw-rw-   0        0        0      207 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/trail-sign-sharp.svg
+-rw-rw-rw-   0        0        0      487 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/trail-sign.svg
+-rw-rw-rw-   0        0        0      881 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/train-outline.svg
+-rw-rw-rw-   0        0        0      522 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/train-sharp.svg
+-rw-rw-rw-   0        0        0      893 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/train.svg
+-rw-rw-rw-   0        0        0     1170 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/transgender-outline.svg
+-rw-rw-rw-   0        0        0      598 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/transgender-sharp.svg
+-rw-rw-rw-   0        0        0      780 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/transgender.svg
+-rw-rw-rw-   0        0        0      699 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/trash-bin-outline.svg
+-rw-rw-rw-   0        0        0      704 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/trash-bin-sharp.svg
+-rw-rw-rw-   0        0        0      510 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/trash-bin.svg
+-rw-rw-rw-   0        0        0      968 2023-05-22 03:19:51.000000 ionicons_python-1.0.1/ionicons_python/icons/trash-outline.svg
+-rw-rw-rw-   0        0        0      536 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/trash-sharp.svg
+-rw-rw-rw-   0        0        0      660 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/trash.svg
+-rw-rw-rw-   0        0        0      412 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/trending-down-outline.svg
+-rw-rw-rw-   0        0        0      370 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/trending-down-sharp.svg
+-rw-rw-rw-   0        0        0      412 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/trending-down.svg
+-rw-rw-rw-   0        0        0      412 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/trending-up-outline.svg
+-rw-rw-rw-   0        0        0      370 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/trending-up-sharp.svg
+-rw-rw-rw-   0        0        0      412 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/trending-up.svg
+-rw-rw-rw-   0        0        0      232 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/triangle-outline.svg
+-rw-rw-rw-   0        0        0      141 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/triangle-sharp.svg
+-rw-rw-rw-   0        0        0      197 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/triangle.svg
+-rw-rw-rw-   0        0        0      904 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/trophy-outline.svg
+-rw-rw-rw-   0        0        0      631 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/trophy-sharp.svg
+-rw-rw-rw-   0        0        0     1066 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/trophy.svg
+-rw-rw-rw-   0        0        0      354 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/tv-outline.svg
+-rw-rw-rw-   0        0        0      249 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/tv-sharp.svg
+-rw-rw-rw-   0        0        0      372 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/tv.svg
+-rw-rw-rw-   0        0        0      660 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/umbrella-outline.svg
+-rw-rw-rw-   0        0        0      718 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/umbrella-sharp.svg
+-rw-rw-rw-   0        0        0      773 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/umbrella.svg
+-rw-rw-rw-   0        0        0      351 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/unlink-outline.svg
+-rw-rw-rw-   0        0        0      366 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/unlink-sharp.svg
+-rw-rw-rw-   0        0        0      364 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/unlink.svg
+-rw-rw-rw-   0        0        0      789 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/videocam-off-outline.svg
+-rw-rw-rw-   0        0        0      341 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/videocam-off-sharp.svg
+-rw-rw-rw-   0        0        0      677 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/videocam-off.svg
+-rw-rw-rw-   0        0        0      550 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/videocam-outline.svg
+-rw-rw-rw-   0        0        0      216 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/videocam-sharp.svg
+-rw-rw-rw-   0        0        0      458 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/videocam.svg
+-rw-rw-rw-   0        0        0      826 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/volume-high-outline.svg
+-rw-rw-rw-   0        0        0      647 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/volume-high-sharp.svg
+-rw-rw-rw-   0        0        0      971 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/volume-high.svg
+-rw-rw-rw-   0        0        0      522 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/volume-low-outline.svg
+-rw-rw-rw-   0        0        0      385 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/volume-low-sharp.svg
+-rw-rw-rw-   0        0        0      486 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/volume-low.svg
+-rw-rw-rw-   0        0        0      670 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/volume-medium-outline.svg
+-rw-rw-rw-   0        0        0      493 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/volume-medium-sharp.svg
+-rw-rw-rw-   0        0        0      696 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/volume-medium.svg
+-rw-rw-rw-   0        0        0     1412 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/volume-mute-outline.svg
+-rw-rw-rw-   0        0        0      940 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/volume-mute-sharp.svg
+-rw-rw-rw-   0        0        0     1235 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/volume-mute.svg
+-rw-rw-rw-   0        0        0      364 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/volume-off-outline.svg
+-rw-rw-rw-   0        0        0      186 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/volume-off-sharp.svg
+-rw-rw-rw-   0        0        0      308 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/volume-off.svg
+-rw-rw-rw-   0        0        0      871 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/walk-outline.svg
+-rw-rw-rw-   0        0        0      752 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/walk-sharp.svg
+-rw-rw-rw-   0        0        0      963 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/walk.svg
+-rw-rw-rw-   0        0        0      438 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/wallet-outline.svg
+-rw-rw-rw-   0        0        0      521 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/wallet-sharp.svg
+-rw-rw-rw-   0        0        0      554 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/wallet.svg
+-rw-rw-rw-   0        0        0      583 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/warning-outline.svg
+-rw-rw-rw-   0        0        0      257 2023-05-22 03:19:52.000000 ionicons_python-1.0.1/ionicons_python/icons/warning-sharp.svg
+-rw-rw-rw-   0        0        0      409 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/warning.svg
+-rw-rw-rw-   0        0        0      484 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/watch-outline.svg
+-rw-rw-rw-   0        0        0      382 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/watch-sharp.svg
+-rw-rw-rw-   0        0        0      491 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/watch.svg
+-rw-rw-rw-   0        0        0      445 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/water-outline.svg
+-rw-rw-rw-   0        0        0      282 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/water-sharp.svg
+-rw-rw-rw-   0        0        0      409 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/water.svg
+-rw-rw-rw-   0        0        0      577 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/wifi-outline.svg
+-rw-rw-rw-   0        0        0      580 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/wifi-sharp.svg
+-rw-rw-rw-   0        0        0      530 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/wifi.svg
+-rw-rw-rw-   0        0        0      594 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/wine-outline.svg
+-rw-rw-rw-   0        0        0      209 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/wine-sharp.svg
+-rw-rw-rw-   0        0        0      513 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/wine.svg
+-rw-rw-rw-   0        0        0      999 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/woman-outline.svg
+-rw-rw-rw-   0        0        0      484 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/woman-sharp.svg
+-rw-rw-rw-   0        0        0      783 2023-05-22 03:19:53.000000 ionicons_python-1.0.1/ionicons_python/icons/woman.svg
+-rw-rw-rw-   0        0        0    72254 2023-06-09 03:57:28.000000 ionicons_python-1.0.1/ionicons_python/ionicons_icons.py
+-rw-rw-rw-   0        0        0      246 2023-06-08 13:23:49.000000 ionicons_python-1.0.1/ionicons_python/load_icon.py
+drwxrwxrwx   0        0        0        0 2023-06-09 04:45:09.536134 ionicons_python-1.0.1/ionicons_python.egg-info/
+-rw-rw-rw-   0        0        0     3929 2023-06-09 04:45:09.000000 ionicons_python-1.0.1/ionicons_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    55107 2023-06-09 04:45:09.000000 ionicons_python-1.0.1/ionicons_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 04:45:09.000000 ionicons_python-1.0.1/ionicons_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-08 13:44:15.000000 ionicons_python-1.0.1/ionicons_python.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-06-09 04:45:09.000000 ionicons_python-1.0.1/ionicons_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 04:45:10.334531 ionicons_python-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1238 2023-06-09 04:44:59.000000 ionicons_python-1.0.1/setup.py
```

### Comparing `ionicons_python-1.0.0/LICENSE` & `ionicons_python-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/PKG-INFO` & `ionicons_python-1.0.1/ionicons_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ionicons_python
-Version: 1.0.0
+Name: ionicons-python
+Version: 1.0.1
 Summary: Package containing icons taken from ionicons website.
 Home-page: https://github.com/srang992/ionicons_python
 Author: Subhradeep Rang
 Author-email: srang992@gmail.com
 License: MIT license
 Keywords: ionicons_python
 Classifier: Development Status :: 5 - Production/Stable
@@ -99,15 +99,16 @@
 ```
 if you want to know which colored icons are available, see the **Releases** section. All the icons provided here is in **.svg** format. So, if you change the size of the icon, it will still looks sharp.
 
 if you want to see all the ionicons icons available, visit [this](https://ionic.io/ionicons) website.
 
 🍃**Releases**
 ----------------
-###### **
+###### **1.0.1**
+- fixed minor bugs and done improvements.
 ###### **1.0.0**
 - This library is now Stable. You can also see some new colored icons which are taken from icons8, flaticons, etc. The icons are listed below.
 
    -  `chatgpt_icon`
    -  `gmail_icon`
    -  `google_color_icon`
    -  `google_docs_icon`
```

### Comparing `ionicons_python-1.0.0/README.md` & `ionicons_python-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/RELEASE.md` & `ionicons_python-1.0.1/RELEASE.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 🍃**Releases**
 ----------------
-###### **
+###### **1.0.1**
+- fixed minor bugs and done improvements.
 ###### **1.0.0**
 - This library is now Stable. You can also see some new colored icons which are taken from icons8, flaticons, etc. The icons are listed below.
 
    -  `chatgpt_icon`
    -  `gmail_icon`
    -  `google_color_icon`
    -  `google_docs_icon`
```

### Comparing `ionicons_python-1.0.0/ionicons_python/extra_icons/chatgpt.svg` & `ionicons_python-1.0.1/ionicons_python/extra_icons/chatgpt.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/extra_icons/gmail.svg` & `ionicons_python-1.0.1/ionicons_python/extra_icons/gmail.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/extra_icons/google-drive.svg` & `ionicons_python-1.0.1/ionicons_python/extra_icons/google-drive.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/extra_icons/google_color.svg` & `ionicons_python-1.0.1/ionicons_python/extra_icons/google_color.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/extra_icons/python_color.svg` & `ionicons_python-1.0.1/ionicons_python/extra_icons/python_color.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/extra_icons/streamlit.svg` & `ionicons_python-1.0.1/ionicons_python/extra_icons/streamlit.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/extra_icons.py` & `ionicons_python-1.0.1/ionicons_python/extra_icons.py`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/accessibility-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/accessibility-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/accessibility.svg` & `ionicons_python-1.0.1/ionicons_python/icons/accessibility.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/add-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/add-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/airplane-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/airplane-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/airplane.svg` & `ionicons_python-1.0.1/ionicons_python/icons/airplane.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/alarm-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/alarm-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/alarm-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/alarm-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/alarm.svg` & `ionicons_python-1.0.1/ionicons_python/icons/alarm.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/american-football-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/american-football-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/american-football-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/american-football-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/american-football.svg` & `ionicons_python-1.0.1/ionicons_python/icons/american-football.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/analytics-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/analytics-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/aperture-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/aperture-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/aperture-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/aperture-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/aperture.svg` & `ionicons_python-1.0.1/ionicons_python/icons/aperture.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/apps-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/apps-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/apps-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/apps-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/apps.svg` & `ionicons_python-1.0.1/ionicons_python/icons/apps.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/archive-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/archive-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/arrow-back-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/arrow-back-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/arrow-down-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/arrow-down-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/arrow-forward-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/arrow-forward-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/arrow-up-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/arrow-up-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/at-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/at-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/at-circle-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/at-circle-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/at-circle.svg` & `ionicons_python-1.0.1/ionicons_python/icons/at-circle.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/at-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/at-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/at-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/at-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/at.svg` & `ionicons_python-1.0.1/ionicons_python/icons/at.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/backspace-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/backspace-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/backspace.svg` & `ionicons_python-1.0.1/ionicons_python/icons/backspace.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bag-add-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bag-add-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bag-check-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bag-check-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bag-handle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bag-handle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bag-remove-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bag-remove-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/balloon-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/balloon-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/balloon-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/balloon-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/balloon.svg` & `ionicons_python-1.0.1/ionicons_python/icons/balloon.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bandage-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bandage-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bandage-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bandage-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bandage.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bandage.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bar-chart-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bar-chart-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bar-chart.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bar-chart.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/barbell-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/barbell-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/barbell.svg` & `ionicons_python-1.0.1/ionicons_python/icons/barbell.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/barcode-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/barcode-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/barcode-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/barcode-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/barcode.svg` & `ionicons_python-1.0.1/ionicons_python/icons/barcode.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/baseball-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/baseball-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/baseball-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/baseball-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/baseball.svg` & `ionicons_python-1.0.1/ionicons_python/icons/baseball.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/basket-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/basket-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/basketball-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/basketball-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/basketball-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/basketball-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/basketball.svg` & `ionicons_python-1.0.1/ionicons_python/icons/basketball.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/battery-charging-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/battery-charging-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/battery-charging-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/battery-charging-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/battery-charging.svg` & `ionicons_python-1.0.1/ionicons_python/icons/battery-charging.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/battery-full-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/battery-full-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/battery-full.svg` & `ionicons_python-1.0.1/ionicons_python/icons/battery-full.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/battery-half-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/battery-half-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/battery-half.svg` & `ionicons_python-1.0.1/ionicons_python/icons/battery-half.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/beaker-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/beaker-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/beaker.svg` & `ionicons_python-1.0.1/ionicons_python/icons/beaker.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bed-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bed-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bed.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bed.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/beer-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/beer-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/beer-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/beer-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/beer.svg` & `ionicons_python-1.0.1/ionicons_python/icons/beer.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bicycle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bicycle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bicycle-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bicycle-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bicycle.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bicycle.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/boat-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/boat-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/boat-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/boat-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/boat.svg` & `ionicons_python-1.0.1/ionicons_python/icons/boat.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/body-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/body-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/body.svg` & `ionicons_python-1.0.1/ionicons_python/icons/body.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bonfire-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bonfire-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bonfire-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bonfire-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bonfire.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bonfire.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/book-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/book-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/book.svg` & `ionicons_python-1.0.1/ionicons_python/icons/book.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/briefcase-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/briefcase-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/briefcase.svg` & `ionicons_python-1.0.1/ionicons_python/icons/briefcase.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/brush-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/brush-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/brush.svg` & `ionicons_python-1.0.1/ionicons_python/icons/brush.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bug-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bug-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bug-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bug-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bug.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bug.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/build-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/build-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/build.svg` & `ionicons_python-1.0.1/ionicons_python/icons/build.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bulb-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bulb-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bulb-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bulb-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bulb.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bulb.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bus-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bus-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bus-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bus-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/bus.svg` & `ionicons_python-1.0.1/ionicons_python/icons/bus.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/business-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/business-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/business-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/business-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/business.svg` & `ionicons_python-1.0.1/ionicons_python/icons/business.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cafe-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cafe-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/calculator-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/calculator-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/calculator.svg` & `ionicons_python-1.0.1/ionicons_python/icons/calculator.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/calendar-clear-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/calendar-clear-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/calendar-number-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/calendar-number-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/calendar-number-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/calendar-number-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/calendar-number.svg` & `ionicons_python-1.0.1/ionicons_python/icons/calendar-number.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/calendar-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/calendar-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/calendar-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/calendar-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/calendar.svg` & `ionicons_python-1.0.1/ionicons_python/icons/calendar.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/call-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/call-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/call-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/call-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/call.svg` & `ionicons_python-1.0.1/ionicons_python/icons/call.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/camera-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/camera-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/camera-reverse-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/camera-reverse-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/camera-reverse-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/camera-reverse-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/camera-reverse.svg` & `ionicons_python-1.0.1/ionicons_python/icons/camera-reverse.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/camera.svg` & `ionicons_python-1.0.1/ionicons_python/icons/camera.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/car-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/car-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/car-sport-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/car-sport-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/car-sport-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/car-sport-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/car-sport.svg` & `ionicons_python-1.0.1/ionicons_python/icons/car-sport.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/car.svg` & `ionicons_python-1.0.1/ionicons_python/icons/car.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cart-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cart-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cash-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cash-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cash-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cash-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cash.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cash.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cellular-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cellular-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cellular.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cellular.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/chatbubble-ellipses-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/chatbubble-ellipses-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/chatbubble-ellipses-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/chatbubble-ellipses-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/chatbubble-ellipses.svg` & `ionicons_python-1.0.1/ionicons_python/icons/chatbubble-ellipses.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/chatbubble-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/chatbubble-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/chatbubble.svg` & `ionicons_python-1.0.1/ionicons_python/icons/chatbubble.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/chatbubbles-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/chatbubbles-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/chatbubbles-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/chatbubbles-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/chatbubbles.svg` & `ionicons_python-1.0.1/ionicons_python/icons/chatbubbles.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/checkmark-done-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/checkmark-done-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/checkmark-done-circle.svg` & `ionicons_python-1.0.1/ionicons_python/icons/checkmark-done-circle.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/chevron-collapse.svg` & `ionicons_python-1.0.1/ionicons_python/icons/chevron-collapse.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/close-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/close-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cloud-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cloud-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cloud-done-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cloud-done-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cloud-done.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cloud-done.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cloud-download-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cloud-download-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cloud-download-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cloud-download-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cloud-download.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cloud-download.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cloud-offline-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cloud-offline-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cloud-offline-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cloud-offline-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cloud-offline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cloud-offline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cloud-upload-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cloud-upload-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cloud-upload-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cloud-upload-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cloud-upload.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cloud-upload.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cloudy-night-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cloudy-night-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cloudy-night-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cloudy-night-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cloudy-night.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cloudy-night.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/code-download-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/code-download-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/code-download-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/code-download-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/code-download.svg` & `ionicons_python-1.0.1/ionicons_python/icons/code-download.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/code-working-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/code-working-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/code-working.svg` & `ionicons_python-1.0.1/ionicons_python/icons/code-working.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cog-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cog-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cog-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cog-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cog.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cog.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/color-fill-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/color-fill-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/color-fill.svg` & `ionicons_python-1.0.1/ionicons_python/icons/color-fill.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/color-filter-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/color-filter-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/color-filter.svg` & `ionicons_python-1.0.1/ionicons_python/icons/color-filter.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/color-palette-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/color-palette-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/color-palette-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/color-palette-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/color-palette.svg` & `ionicons_python-1.0.1/ionicons_python/icons/color-palette.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/color-wand-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/color-wand-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/color-wand-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/color-wand-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/color-wand.svg` & `ionicons_python-1.0.1/ionicons_python/icons/color-wand.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/construct-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/construct-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/construct-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/construct-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/construct.svg` & `ionicons_python-1.0.1/ionicons_python/icons/construct.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/contract-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/contract-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/contract-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/contract-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/contract.svg` & `ionicons_python-1.0.1/ionicons_python/icons/contract.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/create-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/create-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/create-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/create-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/create.svg` & `ionicons_python-1.0.1/ionicons_python/icons/create.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/crop-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/crop-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cube-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cube-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cut-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cut-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/cut.svg` & `ionicons_python-1.0.1/ionicons_python/icons/cut.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/desktop-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/desktop-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/diamond-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/diamond-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/diamond-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/diamond-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/diamond.svg` & `ionicons_python-1.0.1/ionicons_python/icons/diamond.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/dice-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/dice-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/dice-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/dice-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/dice.svg` & `ionicons_python-1.0.1/ionicons_python/icons/dice.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/document-attach-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/document-attach-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/document-attach-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/document-attach-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/document-attach.svg` & `ionicons_python-1.0.1/ionicons_python/icons/document-attach.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/document-lock-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/document-lock-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/document-lock-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/document-lock-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/document-lock.svg` & `ionicons_python-1.0.1/ionicons_python/icons/document-lock.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/document-text-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/document-text-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/documents-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/documents-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/documents.svg` & `ionicons_python-1.0.1/ionicons_python/icons/documents.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/download-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/download-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/duplicate-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/duplicate-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/duplicate.svg` & `ionicons_python-1.0.1/ionicons_python/icons/duplicate.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/ear-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/ear-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/ear-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/ear-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/ear.svg` & `ionicons_python-1.0.1/ionicons_python/icons/ear.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/earth-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/earth-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/earth-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/earth-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/earth.svg` & `ionicons_python-1.0.1/ionicons_python/icons/earth.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/easel-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/easel-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/easel.svg` & `ionicons_python-1.0.1/ionicons_python/icons/easel.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/egg-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/egg-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/enter-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/enter-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/exit-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/exit-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/expand-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/expand-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/expand-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/expand-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/expand.svg` & `ionicons_python-1.0.1/ionicons_python/icons/expand.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/extension-puzzle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/extension-puzzle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/extension-puzzle-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/extension-puzzle-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/extension-puzzle.svg` & `ionicons_python-1.0.1/ionicons_python/icons/extension-puzzle.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/eye-off-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/eye-off-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/eye-off-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/eye-off-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/eye-off.svg` & `ionicons_python-1.0.1/ionicons_python/icons/eye-off.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/eye.svg` & `ionicons_python-1.0.1/ionicons_python/icons/eye.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/eyedrop-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/eyedrop-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/eyedrop.svg` & `ionicons_python-1.0.1/ionicons_python/icons/eyedrop.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/fast-food-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/fast-food-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/fast-food-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/fast-food-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/fast-food.svg` & `ionicons_python-1.0.1/ionicons_python/icons/fast-food.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/file-tray-full-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/file-tray-full-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/file-tray-full.svg` & `ionicons_python-1.0.1/ionicons_python/icons/file-tray-full.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/file-tray-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/file-tray-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/file-tray-stacked-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/file-tray-stacked-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/file-tray-stacked.svg` & `ionicons_python-1.0.1/ionicons_python/icons/file-tray-stacked.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/file-tray.svg` & `ionicons_python-1.0.1/ionicons_python/icons/file-tray.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/film-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/film-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/film.svg` & `ionicons_python-1.0.1/ionicons_python/icons/film.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/filter-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/filter-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/finger-print-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/finger-print-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/finger-print-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/finger-print-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/finger-print.svg` & `ionicons_python-1.0.1/ionicons_python/icons/finger-print.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/fish-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/fish-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/fish-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/fish-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/fish.svg` & `ionicons_python-1.0.1/ionicons_python/icons/fish.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/fitness-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/fitness-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/fitness-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/fitness-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/fitness.svg` & `ionicons_python-1.0.1/ionicons_python/icons/fitness.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/flame-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/flame-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/flame.svg` & `ionicons_python-1.0.1/ionicons_python/icons/flame.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/flash-off-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/flash-off-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/flash-off.svg` & `ionicons_python-1.0.1/ionicons_python/icons/flash-off.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/flashlight-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/flashlight-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/flashlight.svg` & `ionicons_python-1.0.1/ionicons_python/icons/flashlight.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/flask-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/flask-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/flask.svg` & `ionicons_python-1.0.1/ionicons_python/icons/flask.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/flower-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/flower-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/flower-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/flower-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/flower.svg` & `ionicons_python-1.0.1/ionicons_python/icons/flower.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/folder-open-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/folder-open-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/football-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/football-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/football-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/football-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/football.svg` & `ionicons_python-1.0.1/ionicons_python/icons/football.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/footsteps-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/footsteps-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/footsteps-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/footsteps-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/footsteps.svg` & `ionicons_python-1.0.1/ionicons_python/icons/footsteps.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/game-controller-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/game-controller-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/game-controller-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/game-controller-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/game-controller.svg` & `ionicons_python-1.0.1/ionicons_python/icons/game-controller.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/gift-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/gift-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/gift-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/gift-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/gift.svg` & `ionicons_python-1.0.1/ionicons_python/icons/gift.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/git-branch-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/git-branch-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/git-compare-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/git-compare-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/git-compare.svg` & `ionicons_python-1.0.1/ionicons_python/icons/git-compare.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/git-merge-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/git-merge-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/git-network-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/git-network-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/git-network.svg` & `ionicons_python-1.0.1/ionicons_python/icons/git-network.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/git-pull-request-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/git-pull-request-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/glasses-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/glasses-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/glasses.svg` & `ionicons_python-1.0.1/ionicons_python/icons/glasses.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/globe-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/globe-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/globe-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/globe-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/globe.svg` & `ionicons_python-1.0.1/ionicons_python/icons/globe.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/golf.svg` & `ionicons_python-1.0.1/ionicons_python/icons/golf.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/grid-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/grid-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/grid.svg` & `ionicons_python-1.0.1/ionicons_python/icons/grid.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/hammer-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/hammer-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/hammer-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/hammer-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/hammer.svg` & `ionicons_python-1.0.1/ionicons_python/icons/hammer.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/hand-left-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/hand-left-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/hand-left-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/hand-left-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/hand-left.svg` & `ionicons_python-1.0.1/ionicons_python/icons/hand-left.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/hand-right-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/hand-right-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/hand-right-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/hand-right-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/hand-right.svg` & `ionicons_python-1.0.1/ionicons_python/icons/hand-right.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/hardware-chip-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/hardware-chip-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/hardware-chip.svg` & `ionicons_python-1.0.1/ionicons_python/icons/hardware-chip.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/headset-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/headset-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/headset-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/headset-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/headset.svg` & `ionicons_python-1.0.1/ionicons_python/icons/headset.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/heart-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/heart-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/heart-dislike-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/heart-dislike-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/heart-dislike-circle-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/heart-dislike-circle-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/heart-dislike-circle.svg` & `ionicons_python-1.0.1/ionicons_python/icons/heart-dislike-circle.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/heart-dislike-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/heart-dislike-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/heart-dislike-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/heart-dislike-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/heart-dislike.svg` & `ionicons_python-1.0.1/ionicons_python/icons/heart-dislike.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/heart-half-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/heart-half-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/heart-half-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/heart-half-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/heart-half.svg` & `ionicons_python-1.0.1/ionicons_python/icons/heart-half.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/help-buoy-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/help-buoy-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/help-buoy-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/help-buoy-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/help-buoy.svg` & `ionicons_python-1.0.1/ionicons_python/icons/help-buoy.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/help-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/help-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/help-circle-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/help-circle-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/help-circle.svg` & `ionicons_python-1.0.1/ionicons_python/icons/help-circle.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/home-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/home-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/home.svg` & `ionicons_python-1.0.1/ionicons_python/icons/home.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/hourglass-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/hourglass-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/hourglass.svg` & `ionicons_python-1.0.1/ionicons_python/icons/hourglass.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/ice-cream-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/ice-cream-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/ice-cream-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/ice-cream-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/ice-cream.svg` & `ionicons_python-1.0.1/ionicons_python/icons/ice-cream.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/id-card-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/id-card-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/id-card.svg` & `ionicons_python-1.0.1/ionicons_python/icons/id-card.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/image-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/image-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/images-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/images-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/images-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/images-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/images.svg` & `ionicons_python-1.0.1/ionicons_python/icons/images.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/infinite-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/infinite-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/information-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/information-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/key-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/key-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/key.svg` & `ionicons_python-1.0.1/ionicons_python/icons/key.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/keypad-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/keypad-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/keypad-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/keypad-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/keypad.svg` & `ionicons_python-1.0.1/ionicons_python/icons/keypad.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/language-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/language-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/language-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/language-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/language.svg` & `ionicons_python-1.0.1/ionicons_python/icons/language.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/layers-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/layers-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/layers.svg` & `ionicons_python-1.0.1/ionicons_python/icons/layers.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/leaf-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/leaf-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/leaf.svg` & `ionicons_python-1.0.1/ionicons_python/icons/leaf.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/library-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/library-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/library-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/library-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/library.svg` & `ionicons_python-1.0.1/ionicons_python/icons/library.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/link-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/link-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/link.svg` & `ionicons_python-1.0.1/ionicons_python/icons/link.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/list-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/list-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/list-circle-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/list-circle-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/list-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/list-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/list-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/list-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/list.svg` & `ionicons_python-1.0.1/ionicons_python/icons/list.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/locate-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/locate-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/locate-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/locate-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/locate.svg` & `ionicons_python-1.0.1/ionicons_python/icons/locate.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/log-in-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/log-in-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/log-out-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/log-out-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-alipay.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-alipay.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-amazon.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-amazon.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-apple-appstore.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-apple-appstore.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-apple-ar.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-apple-ar.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-apple.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-apple.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-behance.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-behance.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-bitcoin.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-bitcoin.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-buffer.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-buffer.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-chrome.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-chrome.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-closed-captioning.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-closed-captioning.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-codepen.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-codepen.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-discord.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-discord.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-docker.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-docker.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-dribbble.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-dribbble.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-edge.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-edge.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-electron.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-electron.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-firefox.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-firefox.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-foursquare.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-foursquare.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-github.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-github.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-gitlab.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-gitlab.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-google.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-google.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-instagram.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-instagram.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-ionic.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-ionic.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-ionitron.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-ionitron.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-javascript.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-javascript.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-laravel.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-laravel.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-linkedin.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-linkedin.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-mastodon.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-mastodon.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-medium.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-medium.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-no-smoking.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-no-smoking.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-nodejs.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-nodejs.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-octocat.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-octocat.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-paypal.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-paypal.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-pinterest.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-pinterest.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-playstation.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-playstation.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-pwa.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-pwa.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-python.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-python.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-react.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-react.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-reddit.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-reddit.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-sass.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-sass.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-skype.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-skype.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-slack.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-slack.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-snapchat.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-snapchat.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-soundcloud.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-soundcloud.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-steam.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-steam.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-tableau.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-tableau.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-tiktok.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-tiktok.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-tux.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-tux.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-twitter.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-twitter.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-usd.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-usd.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-vimeo.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-vimeo.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-vk.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-vk.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-web-component.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-web-component.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-wechat.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-wechat.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-whatsapp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-whatsapp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-wordpress.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-wordpress.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/logo-xbox.svg` & `ionicons_python-1.0.1/ionicons_python/icons/logo-xbox.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/magnet-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/magnet-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/magnet-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/magnet-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/magnet.svg` & `ionicons_python-1.0.1/ionicons_python/icons/magnet.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mail-open-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mail-open-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mail-unread-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mail-unread-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mail-unread-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mail-unread-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mail-unread.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mail-unread.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/male-female-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/male-female-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/man-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/man-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/man.svg` & `ionicons_python-1.0.1/ionicons_python/icons/man.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/map-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/map-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/map.svg` & `ionicons_python-1.0.1/ionicons_python/icons/map.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/medal-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/medal-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/medal.svg` & `ionicons_python-1.0.1/ionicons_python/icons/medal.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/medical-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/medical-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/medical.svg` & `ionicons_python-1.0.1/ionicons_python/icons/medical.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/medkit-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/medkit-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/medkit.svg` & `ionicons_python-1.0.1/ionicons_python/icons/medkit.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/megaphone-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/megaphone-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/megaphone-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/megaphone-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/megaphone.svg` & `ionicons_python-1.0.1/ionicons_python/icons/megaphone.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mic-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mic-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mic-circle-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mic-circle-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mic-circle.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mic-circle.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mic-off-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mic-off-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mic-off-circle-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mic-off-circle-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mic-off-circle.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mic-off-circle.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mic-off-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mic-off-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mic-off-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mic-off-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mic-off.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mic-off.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mic-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mic-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mic-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mic-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/mic.svg` & `ionicons_python-1.0.1/ionicons_python/icons/mic.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/move-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/move-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/move-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/move-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/move.svg` & `ionicons_python-1.0.1/ionicons_python/icons/move.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/musical-notes-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/musical-notes-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/musical-notes-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/musical-notes-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/musical-notes.svg` & `ionicons_python-1.0.1/ionicons_python/icons/musical-notes.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/newspaper-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/newspaper-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/newspaper-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/newspaper-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/newspaper.svg` & `ionicons_python-1.0.1/ionicons_python/icons/newspaper.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/notifications-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/notifications-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/notifications-circle-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/notifications-circle-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/notifications-circle.svg` & `ionicons_python-1.0.1/ionicons_python/icons/notifications-circle.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/notifications-off-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/notifications-off-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/notifications-off-circle.svg` & `ionicons_python-1.0.1/ionicons_python/icons/notifications-off-circle.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/notifications-off-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/notifications-off-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/notifications-off.svg` & `ionicons_python-1.0.1/ionicons_python/icons/notifications-off.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/notifications-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/notifications-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/notifications.svg` & `ionicons_python-1.0.1/ionicons_python/icons/notifications.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/nuclear-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/nuclear-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/nuclear-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/nuclear-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/nuclear.svg` & `ionicons_python-1.0.1/ionicons_python/icons/nuclear.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/nutrition-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/nutrition-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/nutrition-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/nutrition-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/nutrition.svg` & `ionicons_python-1.0.1/ionicons_python/icons/nutrition.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/open-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/open-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/options-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/options-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/partly-sunny-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/partly-sunny-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/partly-sunny-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/partly-sunny-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/partly-sunny.svg` & `ionicons_python-1.0.1/ionicons_python/icons/partly-sunny.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/pause-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/pause-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/paw-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/paw-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/paw-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/paw-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/paw.svg` & `ionicons_python-1.0.1/ionicons_python/icons/paw.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/people-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/people-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/people-circle-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/people-circle-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/people-circle.svg` & `ionicons_python-1.0.1/ionicons_python/icons/people-circle.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/people-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/people-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/people.svg` & `ionicons_python-1.0.1/ionicons_python/icons/people.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/person-add-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/person-add-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/person-add.svg` & `ionicons_python-1.0.1/ionicons_python/icons/person-add.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/person-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/person-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/person-circle.svg` & `ionicons_python-1.0.1/ionicons_python/icons/person-circle.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/person-remove-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/person-remove-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/person-remove.svg` & `ionicons_python-1.0.1/ionicons_python/icons/person-remove.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/person.svg` & `ionicons_python-1.0.1/ionicons_python/icons/person.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/phone-landscape.svg` & `ionicons_python-1.0.1/ionicons_python/icons/phone-landscape.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/phone-portrait.svg` & `ionicons_python-1.0.1/ionicons_python/icons/phone-portrait.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/pint-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/pint-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/pint.svg` & `ionicons_python-1.0.1/ionicons_python/icons/pint.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/pizza-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/pizza-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/pizza-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/pizza-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/pizza.svg` & `ionicons_python-1.0.1/ionicons_python/icons/pizza.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/planet-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/planet-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/planet.svg` & `ionicons_python-1.0.1/ionicons_python/icons/planet.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/play-back-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/play-back-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/play-forward-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/play-forward-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/podium-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/podium-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/pricetags-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/pricetags-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/print-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/print-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/print-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/print-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/print.svg` & `ionicons_python-1.0.1/ionicons_python/icons/print.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/push-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/push-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/qr-code-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/qr-code-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/qr-code-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/qr-code-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/qr-code.svg` & `ionicons_python-1.0.1/ionicons_python/icons/qr-code.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/radio-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/radio-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/radio-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/radio-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/radio.svg` & `ionicons_python-1.0.1/ionicons_python/icons/radio.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/rainy-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/rainy-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/rainy-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/rainy-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/rainy.svg` & `ionicons_python-1.0.1/ionicons_python/icons/rainy.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/reader-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/reader-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/receipt-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/receipt-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/receipt.svg` & `ionicons_python-1.0.1/ionicons_python/icons/receipt.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/refresh-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/refresh-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/reload-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/reload-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/reorder-four-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/reorder-four-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/reorder-four-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/reorder-four-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/reorder-four.svg` & `ionicons_python-1.0.1/ionicons_python/icons/reorder-four.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/repeat-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/repeat-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/repeat-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/repeat-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/repeat.svg` & `ionicons_python-1.0.1/ionicons_python/icons/repeat.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/restaurant-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/restaurant-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/restaurant-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/restaurant-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/restaurant.svg` & `ionicons_python-1.0.1/ionicons_python/icons/restaurant.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/ribbon-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/ribbon-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/ribbon.svg` & `ionicons_python-1.0.1/ionicons_python/icons/ribbon.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/rocket-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/rocket-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/rocket-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/rocket-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/rocket.svg` & `ionicons_python-1.0.1/ionicons_python/icons/rocket.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/rose-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/rose-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/rose-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/rose-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/rose.svg` & `ionicons_python-1.0.1/ionicons_python/icons/rose.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/save-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/save-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/scale-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/scale-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/scale.svg` & `ionicons_python-1.0.1/ionicons_python/icons/scale.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/scan-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/scan-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/scan-circle.svg` & `ionicons_python-1.0.1/ionicons_python/icons/scan-circle.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/scan-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/scan-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/scan.svg` & `ionicons_python-1.0.1/ionicons_python/icons/scan.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/school-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/school-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/school.svg` & `ionicons_python-1.0.1/ionicons_python/icons/school.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/server-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/server-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/server-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/server-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/server.svg` & `ionicons_python-1.0.1/ionicons_python/icons/server.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/settings-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/settings-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/settings-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/settings-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/settings.svg` & `ionicons_python-1.0.1/ionicons_python/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/share-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/share-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/share-social-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/share-social-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/shield-checkmark-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/shield-checkmark-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/shield-checkmark.svg` & `ionicons_python-1.0.1/ionicons_python/icons/shield-checkmark.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/shield-half-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/shield-half-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/shirt-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/shirt-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/shirt.svg` & `ionicons_python-1.0.1/ionicons_python/icons/shirt.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/shuffle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/shuffle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/shuffle-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/shuffle-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/shuffle.svg` & `ionicons_python-1.0.1/ionicons_python/icons/shuffle.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/skull-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/skull-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/skull.svg` & `ionicons_python-1.0.1/ionicons_python/icons/skull.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/snow-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/snow-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/snow-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/snow-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/snow.svg` & `ionicons_python-1.0.1/ionicons_python/icons/snow.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/sparkles-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/sparkles-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/sparkles.svg` & `ionicons_python-1.0.1/ionicons_python/icons/sparkles.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/speedometer-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/speedometer-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/speedometer-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/speedometer-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/speedometer.svg` & `ionicons_python-1.0.1/ionicons_python/icons/speedometer.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/stats-chart-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/stats-chart-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/stats-chart.svg` & `ionicons_python-1.0.1/ionicons_python/icons/stats-chart.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/stopwatch-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/stopwatch-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/storefront-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/storefront-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/storefront-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/storefront-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/storefront.svg` & `ionicons_python-1.0.1/ionicons_python/icons/storefront.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/subway-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/subway-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/subway-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/subway-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/subway.svg` & `ionicons_python-1.0.1/ionicons_python/icons/subway.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/sunny-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/sunny-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/sunny-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/sunny-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/sunny.svg` & `ionicons_python-1.0.1/ionicons_python/icons/sunny.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/swap-horizontal-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/swap-horizontal-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/swap-horizontal-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/swap-horizontal-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/swap-horizontal.svg` & `ionicons_python-1.0.1/ionicons_python/icons/swap-horizontal.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/swap-vertical-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/swap-vertical-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/swap-vertical-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/swap-vertical-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/swap-vertical.svg` & `ionicons_python-1.0.1/ionicons_python/icons/swap-vertical.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/sync-circle-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/sync-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/sync-circle.svg` & `ionicons_python-1.0.1/ionicons_python/icons/sync-circle.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/sync-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/sync-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/sync-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/sync-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/sync.svg` & `ionicons_python-1.0.1/ionicons_python/icons/sync.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/tablet-landscape.svg` & `ionicons_python-1.0.1/ionicons_python/icons/tablet-landscape.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/tablet-portrait.svg` & `ionicons_python-1.0.1/ionicons_python/icons/tablet-portrait.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/telescope-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/telescope-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/telescope.svg` & `ionicons_python-1.0.1/ionicons_python/icons/telescope.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/tennisball-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/tennisball-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/tennisball-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/tennisball-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/tennisball.svg` & `ionicons_python-1.0.1/ionicons_python/icons/tennisball.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/text-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/text-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/text-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/text-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/text.svg` & `ionicons_python-1.0.1/ionicons_python/icons/text.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/thermometer-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/thermometer-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/thumbs-down-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/thumbs-down-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/thumbs-down-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/thumbs-down-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/thumbs-down.svg` & `ionicons_python-1.0.1/ionicons_python/icons/thumbs-down.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/thumbs-up-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/thumbs-up-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/thumbs-up.svg` & `ionicons_python-1.0.1/ionicons_python/icons/thumbs-up.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/thunderstorm-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/thunderstorm-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/thunderstorm-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/thunderstorm-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/thunderstorm.svg` & `ionicons_python-1.0.1/ionicons_python/icons/thunderstorm.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/ticket-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/ticket-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/ticket.svg` & `ionicons_python-1.0.1/ionicons_python/icons/ticket.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/timer.svg` & `ionicons_python-1.0.1/ionicons_python/icons/timer.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/today-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/today-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/today.svg` & `ionicons_python-1.0.1/ionicons_python/icons/today.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/trail-sign-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/trail-sign-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/train-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/train-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/train-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/train-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/train.svg` & `ionicons_python-1.0.1/ionicons_python/icons/train.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/transgender-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/transgender-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/transgender-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/transgender-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/transgender.svg` & `ionicons_python-1.0.1/ionicons_python/icons/transgender.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/trash-bin-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/trash-bin-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/trash-bin-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/trash-bin-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/trash-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/trash-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/trash-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/trash-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/trash.svg` & `ionicons_python-1.0.1/ionicons_python/icons/trash.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/trophy-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/trophy-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/trophy-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/trophy-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/trophy.svg` & `ionicons_python-1.0.1/ionicons_python/icons/trophy.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/umbrella-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/umbrella-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/umbrella-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/umbrella-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/umbrella.svg` & `ionicons_python-1.0.1/ionicons_python/icons/umbrella.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/videocam-off-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/videocam-off-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/videocam-off.svg` & `ionicons_python-1.0.1/ionicons_python/icons/videocam-off.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/videocam-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/videocam-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/volume-high-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/volume-high-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/volume-high-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/volume-high-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/volume-high.svg` & `ionicons_python-1.0.1/ionicons_python/icons/volume-high.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/volume-low-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/volume-low-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/volume-medium-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/volume-medium-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/volume-medium.svg` & `ionicons_python-1.0.1/ionicons_python/icons/volume-medium.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/volume-mute-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/volume-mute-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/volume-mute-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/volume-mute-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/volume-mute.svg` & `ionicons_python-1.0.1/ionicons_python/icons/volume-mute.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/walk-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/walk-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/walk-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/walk-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/walk.svg` & `ionicons_python-1.0.1/ionicons_python/icons/walk.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/wallet-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/wallet-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/wallet.svg` & `ionicons_python-1.0.1/ionicons_python/icons/wallet.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/warning-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/warning-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/wifi-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/wifi-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/wifi-sharp.svg` & `ionicons_python-1.0.1/ionicons_python/icons/wifi-sharp.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/wifi.svg` & `ionicons_python-1.0.1/ionicons_python/icons/wifi.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/wine-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/wine-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/wine.svg` & `ionicons_python-1.0.1/ionicons_python/icons/wine.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/woman-outline.svg` & `ionicons_python-1.0.1/ionicons_python/icons/woman-outline.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/icons/woman.svg` & `ionicons_python-1.0.1/ionicons_python/icons/woman.svg`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python/ionicons_icons.py` & `ionicons_python-1.0.1/ionicons_python/ionicons_icons.py`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/ionicons_python.egg-info/PKG-INFO` & `ionicons_python-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ionicons-python
-Version: 1.0.0
+Name: ionicons_python
+Version: 1.0.1
 Summary: Package containing icons taken from ionicons website.
 Home-page: https://github.com/srang992/ionicons_python
 Author: Subhradeep Rang
 Author-email: srang992@gmail.com
 License: MIT license
 Keywords: ionicons_python
 Classifier: Development Status :: 5 - Production/Stable
@@ -99,15 +99,16 @@
 ```
 if you want to know which colored icons are available, see the **Releases** section. All the icons provided here is in **.svg** format. So, if you change the size of the icon, it will still looks sharp.
 
 if you want to see all the ionicons icons available, visit [this](https://ionic.io/ionicons) website.
 
 🍃**Releases**
 ----------------
-###### **
+###### **1.0.1**
+- fixed minor bugs and done improvements.
 ###### **1.0.0**
 - This library is now Stable. You can also see some new colored icons which are taken from icons8, flaticons, etc. The icons are listed below.
 
    -  `chatgpt_icon`
    -  `gmail_icon`
    -  `google_color_icon`
    -  `google_docs_icon`
```

### Comparing `ionicons_python-1.0.0/ionicons_python.egg-info/SOURCES.txt` & `ionicons_python-1.0.1/ionicons_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ionicons_python-1.0.0/setup.py` & `ionicons_python-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,13 +22,13 @@
     ],
     description="Package containing icons taken from ionicons website.",
     long_description=readme + "\n\n" + release,
     long_description_content_type='text/markdown',
     license="MIT license",
     keywords='ionicons_python',
     name='ionicons_python',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     package_data={'ionicons_python': ['icons/*.svg', 'extra_icons/*.svg']},
     url='https://github.com/srang992/ionicons_python',
     zip_safe=False,
 )
```

