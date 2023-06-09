# Comparing `tmp/aioqui-2.0.1.tar.gz` & `tmp/aioqui-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioqui-2.0.1.tar", last modified: Tue May 16 21:21:00 2023, max compression
+gzip compressed data, was "aioqui-2.0.2.tar", last modified: Fri Jun  9 15:59:39 2023, max compression
```

## Comparing `aioqui-2.0.1.tar` & `aioqui-2.0.2.tar`

### file list

```diff
@@ -1,377 +1,377 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.701551 aioqui-2.0.1/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 aioqui-2.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2629 2023-05-16 21:21:00.701551 aioqui-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-15 08:21:18.000000 aioqui-2.0.1/README.md
--rw-rw-rw-   0        0        0     1488 2023-05-16 21:13:23.000000 aioqui-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 21:21:00.701551 aioqui-2.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.345984 aioqui-2.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 aioqui-2.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.348982 aioqui-2.0.1/src/aioqui/
-drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.338985 aioqui-2.0.1/src/aioqui/.assets/
-drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.648549 aioqui-2.0.1/src/aioqui/.assets/icons/
--rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/activity.svg
--rw-rw-rw-   0        0        0      357 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/airplay.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/alert-circle.svg
--rw-rw-rw-   0        0        0      411 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/alert-octagon.svg
--rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/alert-triangle.svg
--rw-rw-rw-   0        0        0      393 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/align-center.svg
--rw-rw-rw-   0        0        0      394 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/align-justify.svg
--rw-rw-rw-   0        0        0      391 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/align-left.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/align-right.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/anchor.svg
--rw-rw-rw-   0        0        0      563 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/aperture.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/archive.svg
--rw-rw-rw-   0        0        0      355 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-down-circle.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-down-left.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-down-right.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-down.svg
--rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-left-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-left.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-right-circle.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-right.svg
--rw-rw-rw-   0        0        0      352 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-up-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-up-left.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-up-right.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-up.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/at-sign.svg
--rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/award.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/bar-chart-2.svg
--rw-rw-rw-   0        0        0      348 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/bar-chart.svg
--rw-rw-rw-   0        0        0      422 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/battery-charging.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/battery.svg
--rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/bell-off.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/bell.svg
--rw-rw-rw-   0        0        0      293 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/bluetooth.svg
--rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/bold.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/book-open.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/book.svg
--rw-rw-rw-   0        0        0      282 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/bookmark.svg
--rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/box.svg
--rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/briefcase.svg
--rw-rw-rw-   0        0        0      405 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/calendar.svg
--rw-rw-rw-   0        0        0      380 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/camera-off.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/camera.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cast.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/check-circle.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/check-square.svg
--rw-rw-rw-   0        0        0      257 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/check.svg
--rw-rw-rw-   0        0        0      264 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevron-down.svg
--rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevron-left.svg
--rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevron-right.svg
--rw-rw-rw-   0        0        0      263 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevron-up.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevrons-down.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevrons-left.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevrons-right.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevrons-up.svg
--rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chrome.svg
--rw-rw-rw-   0        0        0      253 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/circle.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/clipboard.svg
--rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/clock.svg
--rw-rw-rw-   0        0        0      552 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cloud-drizzle.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cloud-lightning.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cloud-off.svg
--rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cloud-rain.svg
--rw-rw-rw-   0        0        0      567 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cloud-snow.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cloud.svg
--rw-rw-rw-   0        0        0      302 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/code.svg
--rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/codepen.svg
--rw-rw-rw-   0        0        0      633 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/codesandbox.svg
--rw-rw-rw-   0        0        0      442 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/coffee.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/columns.svg
--rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/command.svg
--rw-rw-rw-   0        0        0      337 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/compass.svg
--rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/copy.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-down-left.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-down-right.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-left-down.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-left-up.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-right-down.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-right-up.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-up-left.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-up-right.svg
--rw-rw-rw-   0        0        0      662 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cpu.svg
--rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/credit-card.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/crop.svg
--rw-rw-rw-   0        0        0      432 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/crosshair.svg
--rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/database.svg
--rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/delete.svg
--rw-rw-rw-   0        0        0      290 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/disc.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/divide-circle.svg
--rw-rw-rw-   0        0        0      414 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/divide-square.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/divide.svg
--rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/dollar-sign.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/download-cloud.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/download.svg
--rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/dribbble.svg
--rw-rw-rw-   0        0        0      269 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/droplet.svg
--rw-rw-rw-   0        0        0      286 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/edit-2.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/edit-3.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/edit.svg
--rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/external-link.svg
--rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/eye-off.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/eye.svg
--rw-rw-rw-   0        0        0      298 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/facebook.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/fast-forward.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/feather.svg
--rw-rw-rw-   0        0        0      548 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/figma.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/file-minus.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/file-plus.svg
--rw-rw-rw-   0        0        0      468 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/file-text.svg
--rw-rw-rw-   0        0        0      332 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/file.svg
--rw-rw-rw-   0        0        0      581 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/film.svg
--rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/filter.svg
--rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/flag.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/folder-minus.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/folder-plus.svg
--rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/folder.svg
--rw-rw-rw-   0        0        0      273 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/framer.svg
--rw-rw-rw-   0        0        0      385 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/frown.svg
--rw-rw-rw-   0        0        0      476 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/gift.svg
--rw-rw-rw-   0        0        0      372 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/git-branch.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/git-commit.svg
--rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/git-merge.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/git-pull-request.svg
--rw-rw-rw-   0        0        0      522 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/github.svg
--rw-rw-rw-   0        0        0      485 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/gitlab.svg
--rw-rw-rw-   0        0        0      404 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/globe.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/grid.svg
--rw-rw-rw-   0        0        0      479 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/hard-drive.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/hash.svg
--rw-rw-rw-   0        0        0      390 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/headphones.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/heart.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/help-circle.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/hexagon.svg
--rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/home.svg
--rw-rw-rw-   0        0        0      364 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/image.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/inbox.svg
--rw-rw-rw-   0        0        0      342 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/info.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/instagram.svg
--rw-rw-rw-   0        0        0      343 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/italic.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/key.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/layers.svg
--rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/layout.svg
--rw-rw-rw-   0        0        0      570 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/life-buoy.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/link-2.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/link.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/linkedin.svg
--rw-rw-rw-   0        0        0      477 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/list.svg
--rw-rw-rw-   0        0        0      609 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/loader.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/lock.svg
--rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/log-in.svg
--rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/log-out.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/mail.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/map-pin.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/map.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/maximize-2.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/maximize.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/meh.svg
--rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/menu.svg
--rw-rw-rw-   0        0        0      423 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/message-circle.svg
--rw-rw-rw-   0        0        0      300 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/message-square.svg
--rw-rw-rw-   0        0        0      489 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/mic-off.svg
--rw-rw-rw-   0        0        0      413 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/mic.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/minimize-2.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/minimize.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/minus-circle.svg
--rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/minus-square.svg
--rw-rw-rw-   0        0        0      256 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/minus.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/monitor.svg
--rw-rw-rw-   0        0        0      276 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/moon.svg
--rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/more-horizontal.svg
--rw-rw-rw-   0        0        0      336 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/more-vertical.svg
--rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/mouse-pointer.svg
--rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/move.svg
--rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/music.svg
--rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/navigation-2.svg
--rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/navigation.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/octagon.svg
--rw-rw-rw-   0        0        0      512 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/package.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/paperclip.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/pause-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/pause.svg
--rw-rw-rw-   0        0        0      386 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/pen-tool.svg
--rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/percent.svg
--rw-rw-rw-   0        0        0      571 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/phone-call.svg
--rw-rw-rw-   0        0        0      613 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/phone-forwarded.svg
--rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/phone-incoming.svg
--rw-rw-rw-   0        0        0      608 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/phone-missed.svg
--rw-rw-rw-   0        0        0      586 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/phone-off.svg
--rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/phone-outgoing.svg
--rw-rw-rw-   0        0        0      515 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/phone.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/pie-chart.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/play-circle.svg
--rw-rw-rw-   0        0        0      258 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/play.svg
--rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/plus-circle-gray.svg
--rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/plus-circle.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/plus-square.svg
--rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/plus.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/pocket.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/power.svg
--rw-rw-rw-   0        0        0      402 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/printer.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/radio.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/refresh-ccw.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/refresh-cw.svg
--rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/repeat.svg
--rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/rewind.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/rotate-ccw.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/rotate-cw.svg
--rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/rss.svg
--rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/save.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/schedule.svg
--rw-rw-rw-   0        0        0      439 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/scissors.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/search.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/send.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/server.svg
--rw-rw-rw-   0        0        0     1006 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/settings.svg
--rw-rw-rw-   0        0        0      440 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/share-2.svg
--rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/share.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/shield-off.svg
--rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/shield.svg
--rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/shopping-bag.svg
--rw-rw-rw-   0        0        0      378 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/shopping-cart.svg
--rw-rw-rw-   0        0        0      436 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/shuffle.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/sidebar.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/skip-back.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/skip-forward.svg
--rw-rw-rw-   0        0        0      994 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/slack.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/slash.svg
--rw-rw-rw-   0        0        0      606 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/sliders.svg
--rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/smartphone.svg
--rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/smile.svg
--rw-rw-rw-   0        0        0      361 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/speaker.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/square.svg
--rw-rw-rw-   0        0        0      391 2023-04-06 21:10:35.000000 aioqui-2.0.1/src/aioqui/.assets/icons/star-fill.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/star.svg
--rw-rw-rw-   0        0        0      304 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/stop-circle.svg
--rw-rw-rw-   0        0        0      645 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/sun.svg
--rw-rw-rw-   0        0        0      584 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/sunrise.svg
--rw-rw-rw-   0        0        0      583 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/sunset.svg
--rw-rw-rw-   0        0        0      335 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/table.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/tablet.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/tag.svg
--rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/target.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/terminal.svg
--rw-rw-rw-   0        0        0      292 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/thermometer.svg
--rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/thumbs-down.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/thumbs-up.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/toggle-left.svg
--rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/toggle-right.svg
--rw-rw-rw-   0        0        0      381 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/tool.svg
--rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/trash-2.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/trash.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/trello.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/trending-down.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/trending-up.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/triangle.svg
--rw-rw-rw-   0        0        0      410 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/truck.svg
--rw-rw-rw-   0        0        0      315 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/tv.svg
--rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/twitch.svg
--rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/twitter.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/type.svg
--rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/umbrella.svg
--rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/underline.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/unlock.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/upload-cloud.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/upload.svg
--rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/user-check.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/user-minus.svg
--rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/user-plus.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/user-x.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/user.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/users.svg
--rw-rw-rw-   0        0        0      374 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/video-off.svg
--rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/video.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/voicemail.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/volume-1.svg
--rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/volume-2.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/volume-x.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/volume.svg
--rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/watch.svg
--rw-rw-rw-   0        0        0      564 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/wifi-off.svg
--rw-rw-rw-   0        0        0      396 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/wifi.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/wind.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/x-circle-gray.svg
--rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/x-circle.svg
--rw-rw-rw-   0        0        0      401 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/x-octagon.svg
--rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/x-square.svg
--rw-rw-rw-   0        0        0      294 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/x.svg
--rw-rw-rw-   0        0        0      560 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/youtube.svg
--rw-rw-rw-   0        0        0      428 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/zap-off.svg
--rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/zap.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/zoom-in.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/zoom-out.svg
--rw-rw-rw-   0        0        0      177 2023-05-16 21:16:03.000000 aioqui-2.0.1/src/aioqui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.651550 aioqui-2.0.1/src/aioqui/context/
--rw-rw-rw-   0        0        0       70 2023-05-15 07:06:13.000000 aioqui-2.0.1/src/aioqui/context/__init__.py
--rw-rw-rw-   0        0        0     9795 2023-05-16 21:16:03.000000 aioqui-2.0.1/src/aioqui/context/context_obj.py
--rw-rw-rw-   0        0        0      528 2023-05-15 15:53:26.000000 aioqui-2.0.1/src/aioqui/context/contextapi.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.658551 aioqui-2.0.1/src/aioqui/misc/
--rw-rw-rw-   0        0        0      128 2023-05-15 08:51:32.000000 aioqui-2.0.1/src/aioqui/misc/__init__.py
--rw-rw-rw-   0        0        0     3736 2023-05-15 04:39:08.000000 aioqui-2.0.1/src/aioqui/misc/aiorequest.py
--rw-rw-rw-   0        0        0      978 2023-05-16 18:20:57.000000 aioqui-2.0.1/src/aioqui/misc/animation.py
--rw-rw-rw-   0        0        0     1130 2023-05-15 08:41:25.000000 aioqui-2.0.1/src/aioqui/misc/conthrq.py
--rw-rw-rw-   0        0        0     1386 2023-05-14 18:16:30.000000 aioqui-2.0.1/src/aioqui/misc/fileops.py
--rw-rw-rw-   0        0        0     2181 2023-05-14 00:12:50.000000 aioqui-2.0.1/src/aioqui/misc/qss_parser.py
--rw-rw-rw-   0        0        0      319 2023-05-15 08:04:15.000000 aioqui-2.0.1/src/aioqui/misc/utils.py
--rw-rw-rw-   0        0        0      701 2023-05-14 00:40:28.000000 aioqui-2.0.1/src/aioqui/misc/uvithread.py
--rw-rw-rw-   0        0        0     1151 2023-05-15 05:37:56.000000 aioqui-2.0.1/src/aioqui/qasyncio.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.662551 aioqui-2.0.1/src/aioqui/types/
--rw-rw-rw-   0        0        0       93 2023-05-16 21:16:03.000000 aioqui-2.0.1/src/aioqui/types/__init__.py
--rw-rw-rw-   0        0        0      257 2023-05-16 18:47:39.000000 aioqui-2.0.1/src/aioqui/types/common.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.670550 aioqui-2.0.1/src/aioqui/types/enums/
--rw-rw-rw-   0        0        0      294 2023-05-16 17:41:17.000000 aioqui-2.0.1/src/aioqui/types/enums/__init__.py
--rw-rw-rw-   0        0        0      687 2023-05-13 23:00:29.000000 aioqui-2.0.1/src/aioqui/types/enums/alignment.py
--rw-rw-rw-   0        0        0      182 2023-05-15 05:17:48.000000 aioqui-2.0.1/src/aioqui/types/enums/echo_mode.py
--rw-rw-rw-   0        0        0      227 2023-05-14 07:18:50.000000 aioqui-2.0.1/src/aioqui/types/enums/elide_mode.py
--rw-rw-rw-   0        0        0      283 2023-05-16 17:57:41.000000 aioqui-2.0.1/src/aioqui/types/enums/logic_button.py
--rw-rw-rw-   0        0        0      151 2023-05-13 23:00:29.000000 aioqui-2.0.1/src/aioqui/types/enums/orientation.py
--rw-rw-rw-   0        0        0      264 2023-05-14 00:48:52.000000 aioqui-2.0.1/src/aioqui/types/enums/scroll_policy.py
--rw-rw-rw-   0        0        0      235 2023-05-15 05:48:40.000000 aioqui-2.0.1/src/aioqui/types/enums/size_policy.py
--rw-rw-rw-   0        0        0      105 2023-05-13 23:00:29.000000 aioqui-2.0.1/src/aioqui/types/enums/window_hint.py
--rw-rw-rw-   0        0        0     3503 2023-05-15 16:06:33.000000 aioqui-2.0.1/src/aioqui/types/icon.py
--rw-rw-rw-   0        0        0      331 2023-05-15 15:26:00.000000 aioqui-2.0.1/src/aioqui/types/size.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.683550 aioqui-2.0.1/src/aioqui/widgets/
--rw-rw-rw-   0        0        0      668 2023-05-16 20:12:13.000000 aioqui-2.0.1/src/aioqui/widgets/__init__.py
--rw-rw-rw-   0        0        0      524 2023-05-16 18:48:54.000000 aioqui-2.0.1/src/aioqui/widgets/button.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.689550 aioqui-2.0.1/src/aioqui/widgets/custom/
--rw-rw-rw-   0        0        0      218 2023-05-16 21:12:59.000000 aioqui-2.0.1/src/aioqui/widgets/custom/__init__.py
--rw-rw-rw-   0        0        0     1939 2023-05-16 18:22:11.000000 aioqui-2.0.1/src/aioqui/widgets/custom/error_label.py
--rw-rw-rw-   0        0        0     2492 2023-05-16 21:10:31.000000 aioqui-2.0.1/src/aioqui/widgets/custom/image_button.py
--rw-rw-rw-   0        0        0     1423 2023-05-15 07:46:33.000000 aioqui-2.0.1/src/aioqui/widgets/custom/menu_button.py
--rw-rw-rw-   0        0        0     3079 2023-05-16 21:17:28.000000 aioqui-2.0.1/src/aioqui/widgets/custom/popup.py
--rw-rw-rw-   0        0        0     1027 2023-05-15 07:42:41.000000 aioqui-2.0.1/src/aioqui/widgets/custom/searchbar.py
--rw-rw-rw-   0        0        0     1887 2023-05-16 18:51:40.000000 aioqui-2.0.1/src/aioqui/widgets/custom/state_icon_btn.py
--rw-rw-rw-   0        0        0      712 2023-05-16 21:04:40.000000 aioqui-2.0.1/src/aioqui/widgets/date_time.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.693550 aioqui-2.0.1/src/aioqui/widgets/extensions/
--rw-rw-rw-   0        0        0      160 2023-05-15 06:44:59.000000 aioqui-2.0.1/src/aioqui/widgets/extensions/__init__.py
--rw-rw-rw-   0        0        0      746 2023-05-16 21:18:22.000000 aioqui-2.0.1/src/aioqui/widgets/extensions/input_ext.py
--rw-rw-rw-   0        0        0     1944 2023-05-16 21:18:22.000000 aioqui-2.0.1/src/aioqui/widgets/extensions/layout_ext.py
--rw-rw-rw-   0        0        0      710 2023-05-16 21:18:22.000000 aioqui-2.0.1/src/aioqui/widgets/extensions/side_menu_ext.py
--rw-rw-rw-   0        0        0     1925 2023-05-16 21:18:22.000000 aioqui-2.0.1/src/aioqui/widgets/extensions/splitter_widget_ext.py
--rw-rw-rw-   0        0        0      667 2023-05-15 07:22:27.000000 aioqui-2.0.1/src/aioqui/widgets/frame.py
--rw-rw-rw-   0        0        0     2349 2023-05-16 21:16:28.000000 aioqui-2.0.1/src/aioqui/widgets/input.py
--rw-rw-rw-   0        0        0     1347 2023-05-16 21:16:28.000000 aioqui-2.0.1/src/aioqui/widgets/label.py
--rw-rw-rw-   0        0        0     1328 2023-05-16 21:18:22.000000 aioqui-2.0.1/src/aioqui/widgets/layout.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.699550 aioqui-2.0.1/src/aioqui/widgets/qss/
--rw-rw-rw-   0        0        0      160 2023-05-16 20:13:01.000000 aioqui-2.0.1/src/aioqui/widgets/qss/__init__.py
--rw-rw-rw-   0        0        0      653 2023-05-16 20:25:11.000000 aioqui-2.0.1/src/aioqui/widgets/qss/colors.py
--rw-rw-rw-   0        0        0     1491 2023-05-16 20:59:19.000000 aioqui-2.0.1/src/aioqui/widgets/qss/date_time.py
--rw-rw-rw-   0        0        0      306 2023-05-16 21:06:26.000000 aioqui-2.0.1/src/aioqui/widgets/qss/image_button.py
--rw-rw-rw-   0        0        0      829 2023-05-16 21:12:30.000000 aioqui-2.0.1/src/aioqui/widgets/qss/popup.py
--rw-rw-rw-   0        0        0       24 2023-05-16 20:13:39.000000 aioqui-2.0.1/src/aioqui/widgets/qss/scrollbar.py
--rw-rw-rw-   0        0        0      436 2023-05-16 20:17:25.000000 aioqui-2.0.1/src/aioqui/widgets/qss/searchbar.py
--rw-rw-rw-   0        0        0     1716 2023-05-16 21:16:52.000000 aioqui-2.0.1/src/aioqui/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1184 2023-05-15 07:23:03.000000 aioqui-2.0.1/src/aioqui/widgets/selector.py
--rw-rw-rw-   0        0        0      842 2023-05-16 21:16:52.000000 aioqui-2.0.1/src/aioqui/widgets/slider.py
--rw-rw-rw-   0        0        0      270 2023-05-16 21:16:52.000000 aioqui-2.0.1/src/aioqui/widgets/spacer.py
--rw-rw-rw-   0        0        0     1560 2023-05-16 21:16:52.000000 aioqui-2.0.1/src/aioqui/widgets/splitter.py
--rw-rw-rw-   0        0        0     1139 2023-05-16 21:16:57.000000 aioqui-2.0.1/src/aioqui/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0      327 2023-05-15 07:24:09.000000 aioqui-2.0.1/src/aioqui/widgets/statusbar.py
--rw-rw-rw-   0        0        0      587 2023-05-15 07:24:24.000000 aioqui-2.0.1/src/aioqui/widgets/widget.py
--rw-rw-rw-   0        0        0      516 2023-05-16 21:17:28.000000 aioqui-2.0.1/src/aioqui/widgets/window.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.354984 aioqui-2.0.1/src/aioqui.egg-info/
--rw-rw-rw-   0        0        0     2629 2023-05-16 21:21:00.000000 aioqui-2.0.1/src/aioqui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13416 2023-05-16 21:21:00.000000 aioqui-2.0.1/src/aioqui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 21:21:00.000000 aioqui-2.0.1/src/aioqui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-16 21:21:00.000000 aioqui-2.0.1/src/aioqui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-16 21:21:00.000000 aioqui-2.0.1/src/aioqui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 15:59:39.150468 aioqui-2.0.2/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 aioqui-2.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2680 2023-06-09 15:59:39.149468 aioqui-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-15 08:21:18.000000 aioqui-2.0.2/README.md
+-rw-rw-rw-   0        0        0     1536 2023-06-09 15:59:06.000000 aioqui-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 15:59:39.150468 aioqui-2.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 15:59:38.794733 aioqui-2.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 aioqui-2.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:59:38.795784 aioqui-2.0.2/src/aioqui/
+drwxrwxrwx   0        0        0        0 2023-06-09 15:59:38.789698 aioqui-2.0.2/src/aioqui/.assets/
+drwxrwxrwx   0        0        0        0 2023-06-09 15:59:39.098467 aioqui-2.0.2/src/aioqui/.assets/icons/
+-rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/activity.svg
+-rw-rw-rw-   0        0        0      357 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/airplay.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/alert-circle.svg
+-rw-rw-rw-   0        0        0      411 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/alert-octagon.svg
+-rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/alert-triangle.svg
+-rw-rw-rw-   0        0        0      393 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/align-center.svg
+-rw-rw-rw-   0        0        0      394 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/align-justify.svg
+-rw-rw-rw-   0        0        0      391 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/align-left.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/align-right.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/anchor.svg
+-rw-rw-rw-   0        0        0      563 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/aperture.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/archive.svg
+-rw-rw-rw-   0        0        0      355 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/arrow-down-circle.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/arrow-down-left.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/arrow-down-right.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/arrow-down.svg
+-rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/arrow-left-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/arrow-left.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/arrow-right-circle.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/arrow-right.svg
+-rw-rw-rw-   0        0        0      352 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/arrow-up-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/arrow-up-left.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/arrow-up-right.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/arrow-up.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/at-sign.svg
+-rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/award.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/bar-chart-2.svg
+-rw-rw-rw-   0        0        0      348 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/bar-chart.svg
+-rw-rw-rw-   0        0        0      422 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/battery-charging.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/battery.svg
+-rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/bell-off.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/bell.svg
+-rw-rw-rw-   0        0        0      293 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/bluetooth.svg
+-rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/bold.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/book-open.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/book.svg
+-rw-rw-rw-   0        0        0      282 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/bookmark.svg
+-rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/box.svg
+-rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/briefcase.svg
+-rw-rw-rw-   0        0        0      405 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/calendar.svg
+-rw-rw-rw-   0        0        0      380 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/camera-off.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/camera.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/cast.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/check-circle.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/check-square.svg
+-rw-rw-rw-   0        0        0      257 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/check.svg
+-rw-rw-rw-   0        0        0      264 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/chevron-down.svg
+-rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/chevron-left.svg
+-rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/chevron-right.svg
+-rw-rw-rw-   0        0        0      263 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/chevron-up.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/chevrons-down.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/chevrons-left.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/chevrons-right.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/chevrons-up.svg
+-rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/chrome.svg
+-rw-rw-rw-   0        0        0      253 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/circle.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/clipboard.svg
+-rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/clock.svg
+-rw-rw-rw-   0        0        0      552 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/cloud-drizzle.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/cloud-lightning.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/cloud-off.svg
+-rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/cloud-rain.svg
+-rw-rw-rw-   0        0        0      567 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/cloud-snow.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/cloud.svg
+-rw-rw-rw-   0        0        0      302 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/code.svg
+-rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/codepen.svg
+-rw-rw-rw-   0        0        0      633 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/codesandbox.svg
+-rw-rw-rw-   0        0        0      442 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/coffee.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/columns.svg
+-rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/command.svg
+-rw-rw-rw-   0        0        0      337 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/compass.svg
+-rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/copy.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/corner-down-left.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/corner-down-right.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/corner-left-down.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/corner-left-up.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/corner-right-down.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/corner-right-up.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/corner-up-left.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/corner-up-right.svg
+-rw-rw-rw-   0        0        0      662 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/cpu.svg
+-rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/credit-card.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/crop.svg
+-rw-rw-rw-   0        0        0      432 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/crosshair.svg
+-rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/database.svg
+-rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/delete.svg
+-rw-rw-rw-   0        0        0      290 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/disc.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/divide-circle.svg
+-rw-rw-rw-   0        0        0      414 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/divide-square.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/divide.svg
+-rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/dollar-sign.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/download-cloud.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/download.svg
+-rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/dribbble.svg
+-rw-rw-rw-   0        0        0      269 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/droplet.svg
+-rw-rw-rw-   0        0        0      286 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/edit-2.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/edit-3.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/edit.svg
+-rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/external-link.svg
+-rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/eye-off.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/eye.svg
+-rw-rw-rw-   0        0        0      298 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/facebook.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/fast-forward.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/feather.svg
+-rw-rw-rw-   0        0        0      548 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/figma.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/file-minus.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/file-plus.svg
+-rw-rw-rw-   0        0        0      468 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/file-text.svg
+-rw-rw-rw-   0        0        0      332 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/file.svg
+-rw-rw-rw-   0        0        0      581 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/film.svg
+-rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/filter.svg
+-rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/flag.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/folder-minus.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/folder-plus.svg
+-rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/folder.svg
+-rw-rw-rw-   0        0        0      273 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/framer.svg
+-rw-rw-rw-   0        0        0      385 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/frown.svg
+-rw-rw-rw-   0        0        0      476 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/gift.svg
+-rw-rw-rw-   0        0        0      372 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/git-branch.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/git-commit.svg
+-rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/git-merge.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/git-pull-request.svg
+-rw-rw-rw-   0        0        0      522 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/github.svg
+-rw-rw-rw-   0        0        0      485 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/gitlab.svg
+-rw-rw-rw-   0        0        0      404 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/globe.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/grid.svg
+-rw-rw-rw-   0        0        0      479 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/hard-drive.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/hash.svg
+-rw-rw-rw-   0        0        0      390 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/headphones.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/heart.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/help-circle.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/hexagon.svg
+-rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/home.svg
+-rw-rw-rw-   0        0        0      364 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/image.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/inbox.svg
+-rw-rw-rw-   0        0        0      342 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/info.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/instagram.svg
+-rw-rw-rw-   0        0        0      343 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/italic.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/key.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/layers.svg
+-rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/layout.svg
+-rw-rw-rw-   0        0        0      570 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/life-buoy.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/link-2.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/link.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/linkedin.svg
+-rw-rw-rw-   0        0        0      477 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/list.svg
+-rw-rw-rw-   0        0        0      609 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/loader.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/lock.svg
+-rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/log-in.svg
+-rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/log-out.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/mail.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/map-pin.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/map.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/maximize-2.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/maximize.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/meh.svg
+-rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/menu.svg
+-rw-rw-rw-   0        0        0      423 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/message-circle.svg
+-rw-rw-rw-   0        0        0      300 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/message-square.svg
+-rw-rw-rw-   0        0        0      489 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/mic-off.svg
+-rw-rw-rw-   0        0        0      413 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/mic.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/minimize-2.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/minimize.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/minus-circle.svg
+-rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/minus-square.svg
+-rw-rw-rw-   0        0        0      256 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/minus.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/monitor.svg
+-rw-rw-rw-   0        0        0      276 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/moon.svg
+-rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/more-horizontal.svg
+-rw-rw-rw-   0        0        0      336 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/more-vertical.svg
+-rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/mouse-pointer.svg
+-rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/move.svg
+-rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/music.svg
+-rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/navigation-2.svg
+-rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/navigation.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/octagon.svg
+-rw-rw-rw-   0        0        0      512 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/package.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/paperclip.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/pause-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/pause.svg
+-rw-rw-rw-   0        0        0      386 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/pen-tool.svg
+-rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/percent.svg
+-rw-rw-rw-   0        0        0      571 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/phone-call.svg
+-rw-rw-rw-   0        0        0      613 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/phone-forwarded.svg
+-rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/phone-incoming.svg
+-rw-rw-rw-   0        0        0      608 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/phone-missed.svg
+-rw-rw-rw-   0        0        0      586 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/phone-off.svg
+-rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/phone-outgoing.svg
+-rw-rw-rw-   0        0        0      515 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/phone.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/pie-chart.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/play-circle.svg
+-rw-rw-rw-   0        0        0      258 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/play.svg
+-rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/plus-circle-gray.svg
+-rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/plus-circle.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/plus-square.svg
+-rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/plus.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/pocket.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/power.svg
+-rw-rw-rw-   0        0        0      402 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/printer.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/radio.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/refresh-ccw.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/refresh-cw.svg
+-rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/repeat.svg
+-rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/rewind.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/rotate-ccw.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/rotate-cw.svg
+-rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/rss.svg
+-rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/save.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/schedule.svg
+-rw-rw-rw-   0        0        0      439 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/scissors.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/search.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/send.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/server.svg
+-rw-rw-rw-   0        0        0     1006 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/settings.svg
+-rw-rw-rw-   0        0        0      440 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/share-2.svg
+-rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/share.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/shield-off.svg
+-rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/shield.svg
+-rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/shopping-bag.svg
+-rw-rw-rw-   0        0        0      378 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/shopping-cart.svg
+-rw-rw-rw-   0        0        0      436 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/shuffle.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/sidebar.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/skip-back.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/skip-forward.svg
+-rw-rw-rw-   0        0        0      994 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/slack.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/slash.svg
+-rw-rw-rw-   0        0        0      606 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/sliders.svg
+-rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/smartphone.svg
+-rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/smile.svg
+-rw-rw-rw-   0        0        0      361 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/speaker.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/square.svg
+-rw-rw-rw-   0        0        0      391 2023-04-06 21:10:35.000000 aioqui-2.0.2/src/aioqui/.assets/icons/star-fill.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/star.svg
+-rw-rw-rw-   0        0        0      304 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/stop-circle.svg
+-rw-rw-rw-   0        0        0      645 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/sun.svg
+-rw-rw-rw-   0        0        0      584 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/sunrise.svg
+-rw-rw-rw-   0        0        0      583 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/sunset.svg
+-rw-rw-rw-   0        0        0      335 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/table.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/tablet.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/tag.svg
+-rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/target.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/terminal.svg
+-rw-rw-rw-   0        0        0      292 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/thermometer.svg
+-rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/thumbs-down.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/thumbs-up.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/toggle-left.svg
+-rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/toggle-right.svg
+-rw-rw-rw-   0        0        0      381 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/tool.svg
+-rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/trash-2.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/trash.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/trello.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/trending-down.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/trending-up.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/triangle.svg
+-rw-rw-rw-   0        0        0      410 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/truck.svg
+-rw-rw-rw-   0        0        0      315 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/tv.svg
+-rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/twitch.svg
+-rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/twitter.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/type.svg
+-rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/umbrella.svg
+-rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/underline.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/unlock.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/upload-cloud.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/upload.svg
+-rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/user-check.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/user-minus.svg
+-rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/user-plus.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/user-x.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/user.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/users.svg
+-rw-rw-rw-   0        0        0      374 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/video-off.svg
+-rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/video.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/voicemail.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/volume-1.svg
+-rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/volume-2.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/volume-x.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/volume.svg
+-rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/watch.svg
+-rw-rw-rw-   0        0        0      564 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/wifi-off.svg
+-rw-rw-rw-   0        0        0      396 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/wifi.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/wind.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/x-circle-gray.svg
+-rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/x-circle.svg
+-rw-rw-rw-   0        0        0      401 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/x-octagon.svg
+-rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/x-square.svg
+-rw-rw-rw-   0        0        0      294 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/x.svg
+-rw-rw-rw-   0        0        0      560 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/youtube.svg
+-rw-rw-rw-   0        0        0      428 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/zap-off.svg
+-rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/zap.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/zoom-in.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.0.2/src/aioqui/.assets/icons/zoom-out.svg
+-rw-rw-rw-   0        0        0      181 2023-06-09 15:58:57.000000 aioqui-2.0.2/src/aioqui/__init__.py
+-rw-rw-rw-   0        0        0     1079 2023-06-09 00:29:28.000000 aioqui-2.0.2/src/aioqui/asynq.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:59:39.101467 aioqui-2.0.2/src/aioqui/context/
+-rw-rw-rw-   0        0        0       70 2023-05-15 07:06:13.000000 aioqui-2.0.2/src/aioqui/context/__init__.py
+-rw-rw-rw-   0        0        0     9868 2023-06-09 15:48:20.000000 aioqui-2.0.2/src/aioqui/context/context_obj.py
+-rw-rw-rw-   0        0        0      501 2023-06-08 23:59:03.000000 aioqui-2.0.2/src/aioqui/context/contextapi.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:59:39.109468 aioqui-2.0.2/src/aioqui/misc/
+-rw-rw-rw-   0        0        0      128 2023-05-15 08:51:32.000000 aioqui-2.0.2/src/aioqui/misc/__init__.py
+-rw-rw-rw-   0        0        0     3974 2023-06-08 23:56:39.000000 aioqui-2.0.2/src/aioqui/misc/aiorequest.py
+-rw-rw-rw-   0        0        0      975 2023-05-26 19:00:03.000000 aioqui-2.0.2/src/aioqui/misc/animation.py
+-rw-rw-rw-   0        0        0     1130 2023-05-15 08:41:25.000000 aioqui-2.0.2/src/aioqui/misc/conthrq.py
+-rw-rw-rw-   0        0        0     1386 2023-05-14 18:16:30.000000 aioqui-2.0.2/src/aioqui/misc/fileops.py
+-rw-rw-rw-   0        0        0     2181 2023-05-14 00:12:50.000000 aioqui-2.0.2/src/aioqui/misc/qss_parser.py
+-rw-rw-rw-   0        0        0      319 2023-05-15 08:04:15.000000 aioqui-2.0.2/src/aioqui/misc/utils.py
+-rw-rw-rw-   0        0        0      701 2023-05-14 00:40:28.000000 aioqui-2.0.2/src/aioqui/misc/uvithread.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:59:39.112467 aioqui-2.0.2/src/aioqui/types/
+-rw-rw-rw-   0        0        0       93 2023-05-16 21:16:03.000000 aioqui-2.0.2/src/aioqui/types/__init__.py
+-rw-rw-rw-   0        0        0      257 2023-05-16 18:47:39.000000 aioqui-2.0.2/src/aioqui/types/common.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:59:39.119468 aioqui-2.0.2/src/aioqui/types/enums/
+-rw-rw-rw-   0        0        0      294 2023-05-16 17:41:17.000000 aioqui-2.0.2/src/aioqui/types/enums/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-05-13 23:00:29.000000 aioqui-2.0.2/src/aioqui/types/enums/alignment.py
+-rw-rw-rw-   0        0        0      182 2023-05-15 05:17:48.000000 aioqui-2.0.2/src/aioqui/types/enums/echo_mode.py
+-rw-rw-rw-   0        0        0      227 2023-05-14 07:18:50.000000 aioqui-2.0.2/src/aioqui/types/enums/elide_mode.py
+-rw-rw-rw-   0        0        0      283 2023-05-16 17:57:41.000000 aioqui-2.0.2/src/aioqui/types/enums/logic_button.py
+-rw-rw-rw-   0        0        0      151 2023-05-13 23:00:29.000000 aioqui-2.0.2/src/aioqui/types/enums/orientation.py
+-rw-rw-rw-   0        0        0      264 2023-05-14 00:48:52.000000 aioqui-2.0.2/src/aioqui/types/enums/scroll_policy.py
+-rw-rw-rw-   0        0        0      235 2023-05-15 05:48:40.000000 aioqui-2.0.2/src/aioqui/types/enums/size_policy.py
+-rw-rw-rw-   0        0        0      105 2023-05-13 23:00:29.000000 aioqui-2.0.2/src/aioqui/types/enums/window_hint.py
+-rw-rw-rw-   0        0        0     3595 2023-05-26 18:03:40.000000 aioqui-2.0.2/src/aioqui/types/icon.py
+-rw-rw-rw-   0        0        0      331 2023-05-15 15:26:00.000000 aioqui-2.0.2/src/aioqui/types/size.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:59:39.132468 aioqui-2.0.2/src/aioqui/widgets/
+-rw-rw-rw-   0        0        0      668 2023-05-16 20:12:13.000000 aioqui-2.0.2/src/aioqui/widgets/__init__.py
+-rw-rw-rw-   0        0        0      524 2023-05-16 18:48:54.000000 aioqui-2.0.2/src/aioqui/widgets/button.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:59:39.138468 aioqui-2.0.2/src/aioqui/widgets/custom/
+-rw-rw-rw-   0        0        0      220 2023-06-09 00:40:35.000000 aioqui-2.0.2/src/aioqui/widgets/custom/__init__.py
+-rw-rw-rw-   0        0        0     2230 2023-06-09 00:40:35.000000 aioqui-2.0.2/src/aioqui/widgets/custom/duration_label.py
+-rw-rw-rw-   0        0        0     2489 2023-05-26 19:00:03.000000 aioqui-2.0.2/src/aioqui/widgets/custom/image_button.py
+-rw-rw-rw-   0        0        0     3060 2023-06-09 00:40:35.000000 aioqui-2.0.2/src/aioqui/widgets/custom/popup.py
+-rw-rw-rw-   0        0        0     1027 2023-05-15 07:42:41.000000 aioqui-2.0.2/src/aioqui/widgets/custom/searchbar.py
+-rw-rw-rw-   0        0        0     1736 2023-05-26 19:00:03.000000 aioqui-2.0.2/src/aioqui/widgets/custom/state_button.py
+-rw-rw-rw-   0        0        0     1447 2023-05-26 18:05:23.000000 aioqui-2.0.2/src/aioqui/widgets/custom/total_button.py
+-rw-rw-rw-   0        0        0      712 2023-05-16 21:04:40.000000 aioqui-2.0.2/src/aioqui/widgets/date_time.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:59:39.142468 aioqui-2.0.2/src/aioqui/widgets/extensions/
+-rw-rw-rw-   0        0        0      160 2023-05-15 06:44:59.000000 aioqui-2.0.2/src/aioqui/widgets/extensions/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-05-16 21:18:22.000000 aioqui-2.0.2/src/aioqui/widgets/extensions/input_ext.py
+-rw-rw-rw-   0        0        0     1944 2023-05-16 21:18:22.000000 aioqui-2.0.2/src/aioqui/widgets/extensions/layout_ext.py
+-rw-rw-rw-   0        0        0      710 2023-05-16 21:18:22.000000 aioqui-2.0.2/src/aioqui/widgets/extensions/side_menu_ext.py
+-rw-rw-rw-   0        0        0     1925 2023-05-16 21:18:22.000000 aioqui-2.0.2/src/aioqui/widgets/extensions/splitter_widget_ext.py
+-rw-rw-rw-   0        0        0      667 2023-05-15 07:22:27.000000 aioqui-2.0.2/src/aioqui/widgets/frame.py
+-rw-rw-rw-   0        0        0     2349 2023-05-16 21:16:28.000000 aioqui-2.0.2/src/aioqui/widgets/input.py
+-rw-rw-rw-   0        0        0     1347 2023-05-16 21:16:28.000000 aioqui-2.0.2/src/aioqui/widgets/label.py
+-rw-rw-rw-   0        0        0     1328 2023-05-16 21:18:22.000000 aioqui-2.0.2/src/aioqui/widgets/layout.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:59:39.148468 aioqui-2.0.2/src/aioqui/widgets/qss/
+-rw-rw-rw-   0        0        0      160 2023-05-16 20:13:01.000000 aioqui-2.0.2/src/aioqui/widgets/qss/__init__.py
+-rw-rw-rw-   0        0        0      653 2023-05-16 20:25:11.000000 aioqui-2.0.2/src/aioqui/widgets/qss/colors.py
+-rw-rw-rw-   0        0        0     1491 2023-05-16 20:59:19.000000 aioqui-2.0.2/src/aioqui/widgets/qss/date_time.py
+-rw-rw-rw-   0        0        0      306 2023-05-16 21:06:26.000000 aioqui-2.0.2/src/aioqui/widgets/qss/image_button.py
+-rw-rw-rw-   0        0        0      829 2023-05-16 21:12:30.000000 aioqui-2.0.2/src/aioqui/widgets/qss/popup.py
+-rw-rw-rw-   0        0        0       24 2023-05-16 20:13:39.000000 aioqui-2.0.2/src/aioqui/widgets/qss/scrollbar.py
+-rw-rw-rw-   0        0        0      436 2023-05-16 20:17:25.000000 aioqui-2.0.2/src/aioqui/widgets/qss/searchbar.py
+-rw-rw-rw-   0        0        0     1716 2023-05-16 21:16:52.000000 aioqui-2.0.2/src/aioqui/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1184 2023-05-15 07:23:03.000000 aioqui-2.0.2/src/aioqui/widgets/selector.py
+-rw-rw-rw-   0        0        0      842 2023-05-16 21:16:52.000000 aioqui-2.0.2/src/aioqui/widgets/slider.py
+-rw-rw-rw-   0        0        0      270 2023-05-16 21:16:52.000000 aioqui-2.0.2/src/aioqui/widgets/spacer.py
+-rw-rw-rw-   0        0        0     1560 2023-05-16 21:16:52.000000 aioqui-2.0.2/src/aioqui/widgets/splitter.py
+-rw-rw-rw-   0        0        0     1139 2023-05-16 21:16:57.000000 aioqui-2.0.2/src/aioqui/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0      327 2023-05-15 07:24:09.000000 aioqui-2.0.2/src/aioqui/widgets/statusbar.py
+-rw-rw-rw-   0        0        0      587 2023-05-15 07:24:24.000000 aioqui-2.0.2/src/aioqui/widgets/widget.py
+-rw-rw-rw-   0        0        0      470 2023-06-09 00:46:08.000000 aioqui-2.0.2/src/aioqui/widgets/window.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:59:38.800468 aioqui-2.0.2/src/aioqui.egg-info/
+-rw-rw-rw-   0        0        0     2680 2023-06-09 15:59:38.000000 aioqui-2.0.2/src/aioqui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13415 2023-06-09 15:59:38.000000 aioqui-2.0.2/src/aioqui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:59:38.000000 aioqui-2.0.2/src/aioqui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-09 15:59:38.000000 aioqui-2.0.2/src/aioqui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-09 15:59:38.000000 aioqui-2.0.2/src/aioqui.egg-info/top_level.txt
```

### Comparing `aioqui-2.0.1/LICENSE.txt` & `aioqui-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/PKG-INFO` & `aioqui-2.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioqui
-Version: 2.0.1
+Version: 2.0.2
 Summary: Asynchronous GUI framework based on PySide6
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
         
@@ -29,14 +29,15 @@
 Project-URL: Bug Tracker, https://github.com/cxllmerichie/aioqui/issues
 Project-URL: Repository, https://github.com/cxllmerichie/aioqui
 Project-URL: Documentation, https://github.com/cxllmerichie/aioqui/README.md
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Environment :: X11 Applications :: Qt
 Classifier: Natural Language :: English
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `aioqui-2.0.1/pyproject.toml` & `aioqui-2.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aioqui"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 maintainers = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 description = "Asynchronous GUI framework based on PySide6"
@@ -18,14 +18,16 @@
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: User Interfaces",
 
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: 3.10",
 
+    "Environment :: X11 Applications :: Qt",
+
     "Natural Language :: English",
 
     "Development Status :: 3 - Alpha",
 
     "Intended Audience :: Developers",
 
     "Operating System :: OS Independent",
```

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/aperture.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/aperture.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/cloud-drizzle.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/cloud-drizzle.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/cloud-snow.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/cloud-snow.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/codesandbox.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/codesandbox.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/cpu.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/cpu.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/figma.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/figma.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/film.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/film.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/github.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/life-buoy.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/life-buoy.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/loader.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/loader.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/package.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/package.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/phone-call.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/phone-call.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/phone-forwarded.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/phone-forwarded.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/phone-incoming.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/phone-incoming.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/phone-missed.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/phone-missed.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/phone-off.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/phone-off.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/phone-outgoing.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/phone-outgoing.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/phone.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/phone.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/settings.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/slack.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/slack.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/sliders.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/sliders.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/sun.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/sun.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/sunrise.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/sunrise.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/sunset.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/sunset.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/wifi-off.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/wifi-off.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/.assets/icons/youtube.svg` & `aioqui-2.0.2/src/aioqui/.assets/icons/youtube.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/context/context_obj.py` & `aioqui-2.0.2/src/aioqui/context/context_obj.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 from PySide6.QtCore import QObject, Qt, Signal
 from contextlib import suppress
 from loguru import logger
 import uuid
 
 from .contextapi import CONTEXT
-from ..types import QSS, Size, Event, Icon, Parent
-from src.aioqui.types.enums import Alignment, SizePolicy
+from ..types import QSS, Size, Event, Icon, Parent, Alignment, SizePolicy
 
 
 class ContextObj:
-    _emmitable_event: Signal = Signal()
+    class Emitter(QObject):
+        _event: Signal = Signal()
+
+        def _emit(self, event):
+            with suppress(Exception):
+                self._event.disconnect()
+            self._event.connect(event)
+            self._event.emit()
+
+    emitter = Emitter()
+
     __blacklist: dict[str, list[str]] = {}
 
     def __init__(self: QObject, parent: Parent = None, name: str = str(uuid.uuid4()), visible: bool = True):
         if parent and name:
             self.setObjectName(name)
             # make `self` accessible from `parent`
             self.__register(parent, name, self)
@@ -245,24 +254,21 @@
         return self
 
     def _size_warning(self: QObject) -> None:
         logger.warning(f'Review `{self.objectName()}.sized()` arguments')
 
     @staticmethod
     async def _connect_event(signal: Signal, event: Event):
-        # signal.connect(slot) is faster that using getattr(self, signalName).connect(slot)
+        # signal.connect(slot) is faster than using getattr(self, signalName).connect(slot)
         with suppress(Exception):
             signal.disconnect()
         signal.connect(event)
 
     def emit_event(self, event: Event) -> None:  # created because event might be sync, async and wrapped with asyncSlot
-        with suppress(Exception):
-            self._emmitable_event.disconnect()
-        self._emmitable_event.connect(event)
-        self._emmitable_event.emit()
+        self.emitter._emit(event)
 
     def _event_error(self: QObject, event: str) -> None:
         logger.error(f'event `{event}` is not implemented for `{self.objectName()}\'s` type: {type(self)}')
 
     @property
     def qss(self: QObject) -> str:
         return self.styleSheet()
```

### Comparing `aioqui-2.0.1/src/aioqui/misc/aiorequest.py` & `aioqui-2.0.2/src/aioqui/misc/aiorequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,21 @@
                 return await url
             return url
 
     @baseurl.setter
     def baseurl(self, base_url: Callable[..., str] | str):
         self.__base = base_url
 
-    async def __call__(self, method: str, url: str, **kwargs) -> Any:
+    async def __call__(
+            self,
+            method: str, url: str,
+            *,
+            evaluate: bool = False,
+            **kwargs
+    ) -> Any:
         # convert params values to str
         if params := kwargs['params']:
             for key, value in params.items():
                 kwargs['params'][key] = str(value)
         # assure that `method` supports
         assert (method := method.lower()) in ('get', 'post', 'put', 'delete')
         # request
@@ -37,14 +43,18 @@
                     data=kwargs['data']
             ) as response:
                 try:
                     return await response.json()
                 except Exception:
                     raise ValueError(await response.text())
 
+    async def __evaluate(self, response):
+        # evaluate str repr of uuid to uuid, "b''" to b'' and so on
+        return response
+
     async def get(
             self,
             url: str,
             *,
             params: dict[str, Any] = None,
             headers: dict[str, Any] = None,
             body: dict[str, Any] = None,
```

### Comparing `aioqui-2.0.1/src/aioqui/misc/animation.py` & `aioqui-2.0.2/src/aioqui/misc/animation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PySide6.QtCore import QPropertyAnimation, Property, QObject
 from typing import Any, Callable
 
-from ..qasyncio import asyncSlot
+from ..asynq import asyncSlot
 
 
 async def create(  # uncompleted
         obj: QObject,
         pname: str,
         ptype: type,
         duration: float,
```

### Comparing `aioqui-2.0.1/src/aioqui/misc/conthrq.py` & `aioqui-2.0.2/src/aioqui/misc/conthrq.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/misc/fileops.py` & `aioqui-2.0.2/src/aioqui/misc/fileops.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/misc/qss_parser.py` & `aioqui-2.0.2/src/aioqui/misc/qss_parser.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/misc/uvithread.py` & `aioqui-2.0.2/src/aioqui/misc/uvithread.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/qasyncio.py` & `aioqui-2.0.2/src/aioqui/asynq.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,30 @@
+from qasync import QApplication, run as qrun, asyncSlot  # to import `asyncSlot` from `asynq`
+from asyncio import exceptions, Future, AbstractEventLoop, get_event_loop
 from typing import Callable, Awaitable
-import functools
-import asyncio
-import qasync
+from functools import partial
 import sys
-from qasync import asyncSlot  # to import `asyncSlot` from `qasyncio`
 
 
-class AsyncApp:
-    @staticmethod
-    def run(amain: Callable[[], Awaitable[None]]) -> None:
-        async def wrap():
-            def close_future(future: asyncio.Future, loop: asyncio.AbstractEventLoop) -> None:
-                loop.call_later(10, future.cancel)
-                future.cancel()
-            future = asyncio.Future()
-            if hasattr(qapp := qasync.QApplication.instance(), 'aboutToQuit'):
-                getattr(qapp, 'aboutToQuit').connect(functools.partial(close_future, future, asyncio.get_event_loop()))
-            await amain()
-            await future
-
-        try:
-            qasync.run(wrap())
-        except asyncio.exceptions.CancelledError:
-            sys.exit(0)
+def run(amain: Callable[[], Awaitable[None]]) -> None:
+    async def wrap():
+        def close_future(future: Future, loop: AbstractEventLoop) -> None:
+            loop.call_later(10, future.cancel)
+            future.cancel()
+
+        future = Future()
+        if hasattr(qapp := QApplication.instance(), 'aboutToQuit'):
+            getattr(qapp, 'aboutToQuit').connect(partial(close_future, future, get_event_loop()))
+        await amain()
+        await future
+
+    try:
+        qrun(wrap())
+    except exceptions.CancelledError:
+        sys.exit(0)
 
 
 # def to_async_slot(to_call):
 #     @asyncSlot()
 #     async def wrapped():
 #         print(type(to_call))
 #         if to_call.__class__.__name__ in ('function', 'method'):
```

### Comparing `aioqui-2.0.1/src/aioqui/types/enums/alignment.py` & `aioqui-2.0.2/src/aioqui/types/enums/alignment.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/types/icon.py` & `aioqui-2.0.2/src/aioqui/types/icon.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,7 +92,11 @@
         image = QImage(icon.icon.pixmap(QSize(512, 512)).toImage())
         buffer = QBuffer()
         buffer.open(QIODevice.WriteOnly)
         image.save(buffer, 'JPG')
         image_bytes = buffer.data()
         buffer.close()
         return image_bytes
+
+    @classmethod
+    def default(cls) -> 'Icon':
+        return Icon(instance=QIcon())
```

### Comparing `aioqui-2.0.1/src/aioqui/widgets/__init__.py` & `aioqui-2.0.2/src/aioqui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/button.py` & `aioqui-2.0.2/src/aioqui/widgets/button.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/custom/error_label.py` & `aioqui-2.0.2/src/aioqui/widgets/custom/duration_label.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from PySide6.QtCore import QPropertyAnimation, Property
 from time import sleep
 
 from ...misc import ConditionalThreadQueue
 from ..label import Label
-from ...qasyncio import asyncSlot
+from ...asynq import asyncSlot
 from ...types import Parent
 
 
-class ErrorLabel(Label):
-    __duration: float = 0.5
+class DurationLabel(Label):
     __ctq: ConditionalThreadQueue = ConditionalThreadQueue()
+    __duration: float = 0.5
+    __rgb: tuple[int, int, int] = (255, 0, 0)
+    __oprng: tuple[float, float] = (0.0, 1.0)
 
     def __init__(self, parent: Parent, name: str = None, visible: bool = True):
         super().__init__(parent, name if name else self.__class__.__name__, visible)
 
     async def init(
             self, *,
-            _=None,
+            rgb: tuple[int, int, int] = (255, 0, 0), oprng: tuple[float, float] = (0.0, 1.0),
             **kwargs
-    ) -> 'ErrorLabel':
+    ) -> 'DurationLabel':
+        self.__rgb = rgb
+        self.__oprng = oprng
         return await Label.init(self, **kwargs)
 
     def setText(self, text: str, delay: float = 2, duration: int = 0.5) -> None:
         if delay == 0:  # if delay is 0, just set the text
             return Label.setText(self, '')
 
         if not text:  # text == '' means instantly clear the text and hide label without `post` action
@@ -41,20 +45,20 @@
         self.__duration = duration
         self.__ctq.new(pre, post)
 
     @asyncSlot()
     async def reduce(self):
         self.animation = QPropertyAnimation(self, b"_opacity")
         self.animation.setDuration(int(self.__duration * 1000))
-        self.animation.setStartValue(1.0)
-        self.animation.setEndValue(0.0)
+        self.animation.setStartValue(self.__oprng[0])
+        self.animation.setEndValue(self.__oprng[1])
         self.animation.start()
 
     def _get_opacity(self):
         return self.__opacity
 
     def _set_opacity(self, opacity: float):
         self.__opacity = opacity
-        self.setStyleSheet(f'color: rgba(255, 0, 0, {opacity});')
+        self.setStyleSheet(f'color: rgba({self.__rgb[0]}, {self.__rgb[1]}, {self.__rgb[2]}, {opacity});')
 
     __opacity: float = 1
     _opacity: Property = Property(float, _get_opacity, _set_opacity)
```

### Comparing `aioqui-2.0.1/src/aioqui/widgets/custom/image_button.py` & `aioqui-2.0.2/src/aioqui/widgets/custom/image_button.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from PySide6.QtGui import QIcon
 from contextlib import suppress
 
 from ..button import Button
 from .popup import Popup
 from ...types import Icon, Size, Parent, Event, DefaultEvent
-from ...qasyncio import asyncSlot
+from ...asynq import asyncSlot
 from ...misc import fileops
 from ..qss.popup import qss
 
 
 class ImageButton(Button):
     RemoveBtn: Button
```

### Comparing `aioqui-2.0.1/src/aioqui/widgets/custom/menu_button.py` & `aioqui-2.0.2/src/aioqui/widgets/custom/total_button.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 from ..button import Button
 from ..label import Label
 from ..layout import Layout
 from ...types import Icon, Size
 
 
-class MenuButton(Button):
+class TotalButton(Button):
     IconBtn: Button
     TextLbl: Label
     TotalLbl: Label
 
     def __init__(self, parent: QWidget, name: str = None, visible: bool = True):
         super().__init__(parent, name if name else self.__class__.__name__, visible)
 
     async def init(
             self, *,
-            icon: Icon, text: str, total: int = 0,
+            icon: Icon = Icon.default(), text: str = '', total: int = 0,
             **kwargs
-    ) -> 'MenuButton':
+    ) -> 'TotalButton':
         self.setLayout(await Layout.horizontal().init(
             margins=(10, 5, 10, 5), spacing=10,
             items=[
                 IconBtn := await Button(self, f'{self.objectName()}IconBtn').init(
                     icon=icon, disabled=True, fixed_size=Size(icon.size.width(), icon.size.height())
                 ), Layout.Left,
                 TextLbl := await Label(self, f'{self.objectName()}TextLbl').init(
```

### Comparing `aioqui-2.0.1/src/aioqui/widgets/custom/popup.py` & `aioqui-2.0.2/src/aioqui/widgets/custom/popup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 from ...types import Parent, Event, DefaultEvent, QSS, LogicButton
 
 
 class Popup(LogicButton, Frame):
     def __init__(self, parent: Parent, name: str = None, qss: QSS = None, *,
                  message: str = '', buttons: Iterable[LogicButton] = (LogicButton.YES, LogicButton.NO),
                  on_success: Event = DefaultEvent, on_failure: Event = DefaultEvent):
-        super().__init__(parent, name if name else self.__class__.__name__)
-        self.qss = qss
+        super().__init__(parent, name if name else self.__class__.__name__, qss)
         self.message: str = message
         self.buttons: Iterable[LogicButton] = buttons
         self.on_success: Event = on_success
         self.on_failure: Event = on_failure
         self.hide()
 
     @asyncSlot()
```

### Comparing `aioqui-2.0.1/src/aioqui/widgets/custom/searchbar.py` & `aioqui-2.0.2/src/aioqui/widgets/custom/searchbar.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/date_time.py` & `aioqui-2.0.2/src/aioqui/widgets/date_time.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/extensions/input_ext.py` & `aioqui-2.0.2/src/aioqui/widgets/extensions/input_ext.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/extensions/layout_ext.py` & `aioqui-2.0.2/src/aioqui/widgets/extensions/layout_ext.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/extensions/side_menu_ext.py` & `aioqui-2.0.2/src/aioqui/widgets/extensions/side_menu_ext.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/extensions/splitter_widget_ext.py` & `aioqui-2.0.2/src/aioqui/widgets/extensions/splitter_widget_ext.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/frame.py` & `aioqui-2.0.2/src/aioqui/widgets/frame.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/input.py` & `aioqui-2.0.2/src/aioqui/widgets/input.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/label.py` & `aioqui-2.0.2/src/aioqui/widgets/label.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/layout.py` & `aioqui-2.0.2/src/aioqui/widgets/layout.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/qss/colors.py` & `aioqui-2.0.2/src/aioqui/widgets/qss/colors.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/qss/date_time.py` & `aioqui-2.0.2/src/aioqui/widgets/qss/date_time.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/qss/popup.py` & `aioqui-2.0.2/src/aioqui/widgets/qss/popup.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/scroll_area.py` & `aioqui-2.0.2/src/aioqui/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/selector.py` & `aioqui-2.0.2/src/aioqui/widgets/selector.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/slider.py` & `aioqui-2.0.2/src/aioqui/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/splitter.py` & `aioqui-2.0.2/src/aioqui/widgets/splitter.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/stacked_widget.py` & `aioqui-2.0.2/src/aioqui/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui/widgets/widget.py` & `aioqui-2.0.2/src/aioqui/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.1/src/aioqui.egg-info/PKG-INFO` & `aioqui-2.0.2/src/aioqui.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioqui
-Version: 2.0.1
+Version: 2.0.2
 Summary: Asynchronous GUI framework based on PySide6
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
         
@@ -29,14 +29,15 @@
 Project-URL: Bug Tracker, https://github.com/cxllmerichie/aioqui/issues
 Project-URL: Repository, https://github.com/cxllmerichie/aioqui
 Project-URL: Documentation, https://github.com/cxllmerichie/aioqui/README.md
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Environment :: X11 Applications :: Qt
 Classifier: Natural Language :: English
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `aioqui-2.0.1/src/aioqui.egg-info/SOURCES.txt` & `aioqui-2.0.2/src/aioqui.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/__init__.py
 src/aioqui/__init__.py
-src/aioqui/qasyncio.py
+src/aioqui/asynq.py
 src/aioqui.egg-info/PKG-INFO
 src/aioqui.egg-info/SOURCES.txt
 src/aioqui.egg-info/dependency_links.txt
 src/aioqui.egg-info/requires.txt
 src/aioqui.egg-info/top_level.txt
 src/aioqui/.assets/icons/activity.svg
 src/aioqui/.assets/icons/airplay.svg
@@ -337,20 +337,20 @@
 src/aioqui/widgets/spacer.py
 src/aioqui/widgets/splitter.py
 src/aioqui/widgets/stacked_widget.py
 src/aioqui/widgets/statusbar.py
 src/aioqui/widgets/widget.py
 src/aioqui/widgets/window.py
 src/aioqui/widgets/custom/__init__.py
-src/aioqui/widgets/custom/error_label.py
+src/aioqui/widgets/custom/duration_label.py
 src/aioqui/widgets/custom/image_button.py
-src/aioqui/widgets/custom/menu_button.py
 src/aioqui/widgets/custom/popup.py
 src/aioqui/widgets/custom/searchbar.py
-src/aioqui/widgets/custom/state_icon_btn.py
+src/aioqui/widgets/custom/state_button.py
+src/aioqui/widgets/custom/total_button.py
 src/aioqui/widgets/extensions/__init__.py
 src/aioqui/widgets/extensions/input_ext.py
 src/aioqui/widgets/extensions/layout_ext.py
 src/aioqui/widgets/extensions/side_menu_ext.py
 src/aioqui/widgets/extensions/splitter_widget_ext.py
 src/aioqui/widgets/qss/__init__.py
 src/aioqui/widgets/qss/colors.py
```

