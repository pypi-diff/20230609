# Comparing `tmp/bpkio_cli-1.4.0.tar.gz` & `tmp/bpkio_cli-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpkio_cli-1.4.0.tar", max compression
+gzip compressed data, was "bpkio_cli-1.5.0.tar", max compression
```

## Comparing `bpkio_cli-1.4.0.tar` & `bpkio_cli-1.5.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0        0 2023-06-05 14:52:28.912688 bpkio_cli-1.4.0/README.md
--rw-r--r--   0        0        0       22 2023-06-07 15:39:48.699204 bpkio_cli-1.4.0/bpkio_cli/__init__.py
--rw-r--r--   0        0        0     3871 2023-06-07 13:10:56.410462 bpkio_cli-1.4.0/bpkio_cli/app.py
--rw-r--r--   0        0        0       91 2023-06-05 14:52:28.913801 bpkio_cli-1.4.0/bpkio_cli/click_mods/__init__.py
--rw-r--r--   0        0        0      771 2023-06-05 14:52:28.914515 bpkio_cli-1.4.0/bpkio_cli/click_mods/default_last_command.py
--rw-r--r--   0        0        0     5145 2023-06-05 14:52:28.915057 bpkio_cli-1.4.0/bpkio_cli/click_mods/group_rest_resource.py
--rw-r--r--   0        0        0     1747 2023-06-05 14:52:28.915564 bpkio_cli-1.4.0/bpkio_cli/click_mods/option_eat_all.py
--rw-r--r--   0        0        0      599 2023-06-05 14:52:28.916268 bpkio_cli-1.4.0/bpkio_cli/click_options/__init__.py
--rw-r--r--   0        0        0      848 2023-06-05 14:52:28.916749 bpkio_cli-1.4.0/bpkio_cli/click_options/admin.py
--rw-r--r--   0        0        0      355 2023-06-05 14:52:28.917214 bpkio_cli-1.4.0/bpkio_cli/click_options/json.py
--rw-r--r--   0        0        0      958 2023-06-05 14:52:28.917874 bpkio_cli-1.4.0/bpkio_cli/click_options/list.py
--rw-r--r--   0        0        0      933 2023-06-05 14:52:28.918220 bpkio_cli-1.4.0/bpkio_cli/click_options/poll.py
--rw-r--r--   0        0        0      845 2023-06-06 10:33:40.520475 bpkio_cli-1.4.0/bpkio_cli/click_options/read.py
--rw-r--r--   0        0        0     1183 2023-06-05 14:52:28.919379 bpkio_cli-1.4.0/bpkio_cli/click_options/search.py
--rw-r--r--   0        0        0      445 2023-06-05 14:52:28.919891 bpkio_cli-1.4.0/bpkio_cli/click_options/table.py
--rw-r--r--   0        0        0     1161 2023-06-05 14:52:28.920409 bpkio_cli-1.4.0/bpkio_cli/click_options/urls.py
--rw-r--r--   0        0        0      656 2023-06-05 14:52:28.920820 bpkio_cli-1.4.0/bpkio_cli/commands/__init__.py
--rw-r--r--   0        0        0      751 2023-06-05 14:52:28.921064 bpkio_cli-1.4.0/bpkio_cli/commands/addons.py
--rw-r--r--   0        0        0     5246 2023-06-07 13:11:32.107723 bpkio_cli-1.4.0/bpkio_cli/commands/configure.py
--rw-r--r--   0        0        0     1766 2023-06-07 08:50:23.685205 bpkio_cli-1.4.0/bpkio_cli/commands/consumption.py
--rw-r--r--   0        0        0     4379 2023-06-05 19:39:32.652087 bpkio_cli-1.4.0/bpkio_cli/commands/creators/ad_insertion.py
--rw-r--r--   0        0        0     7921 2023-06-05 19:39:32.652047 bpkio_cli-1.4.0/bpkio_cli/commands/creators/sources.py
--rw-r--r--   0        0        0     4055 2023-06-05 19:39:32.651893 bpkio_cli-1.4.0/bpkio_cli/commands/creators/virtual_channel.py
--rw-r--r--   0        0        0     8799 2023-06-05 19:39:32.651985 bpkio_cli-1.4.0/bpkio_cli/commands/creators/virtual_channel_populate.py
--rw-r--r--   0        0        0      761 2023-06-05 14:52:28.924009 bpkio_cli-1.4.0/bpkio_cli/commands/hello.py
--rw-r--r--   0        0        0     1251 2023-06-05 14:52:28.924268 bpkio_cli-1.4.0/bpkio_cli/commands/memory.py
--rw-r--r--   0        0        0     3444 2023-06-07 13:33:49.992001 bpkio_cli-1.4.0/bpkio_cli/commands/package.py
--rw-r--r--   0        0        0    10213 2023-06-07 15:09:40.408861 bpkio_cli-1.4.0/bpkio_cli/commands/profiles.py
--rw-r--r--   0        0        0     2700 2023-06-05 14:52:28.925148 bpkio_cli-1.4.0/bpkio_cli/commands/recorder.py
--rw-r--r--   0        0        0     3669 2023-06-05 14:52:28.925467 bpkio_cli-1.4.0/bpkio_cli/commands/services.py
--rw-r--r--   0        0        0     5728 2023-06-06 14:52:14.895415 bpkio_cli-1.4.0/bpkio_cli/commands/sources.py
--rw-r--r--   0        0        0    18471 2023-06-06 10:33:54.312903 bpkio_cli-1.4.0/bpkio_cli/commands/template_crud.py
--rw-r--r--   0        0        0     7306 2023-06-05 14:52:28.926463 bpkio_cli-1.4.0/bpkio_cli/commands/template_crud_slots.py
--rw-r--r--   0        0        0      332 2023-06-05 14:52:28.926844 bpkio_cli-1.4.0/bpkio_cli/commands/tenants.py
--rw-r--r--   0        0        0     5477 2023-06-05 14:52:28.927171 bpkio_cli-1.4.0/bpkio_cli/commands/url.py
--rw-r--r--   0        0        0      359 2023-06-05 14:52:28.927398 bpkio_cli-1.4.0/bpkio_cli/commands/users.py
--rw-r--r--   0        0        0     1036 2023-06-05 14:52:28.927822 bpkio_cli-1.4.0/bpkio_cli/core/app_context.py
--rw-r--r--   0        0        0     3753 2023-06-05 14:52:28.928412 bpkio_cli-1.4.0/bpkio_cli/core/config_provider.py
--rw-r--r--   0        0        0      135 2023-06-05 14:52:28.928924 bpkio_cli-1.4.0/bpkio_cli/core/exceptions.py
--rw-r--r--   0        0        0     2565 2023-06-05 14:52:28.929158 bpkio_cli-1.4.0/bpkio_cli/core/initialize.py
--rw-r--r--   0        0        0     1718 2023-06-05 14:52:28.929630 bpkio_cli-1.4.0/bpkio_cli/core/logger.py
--rw-r--r--   0        0        0     8332 2023-06-07 15:35:22.116286 bpkio_cli-1.4.0/bpkio_cli/core/packager.py
--rw-r--r--   0        0        0     9358 2023-06-07 13:33:12.629695 bpkio_cli-1.4.0/bpkio_cli/core/resource_recorder.py
--rw-r--r--   0        0        0     2204 2023-06-05 14:52:28.930943 bpkio_cli-1.4.0/bpkio_cli/core/resource_trail.py
--rw-r--r--   0        0        0     5128 2023-06-05 14:52:28.931598 bpkio_cli-1.4.0/bpkio_cli/core/response_handler.py
--rw-r--r--   0        0        0     1234 2023-06-05 14:52:28.931905 bpkio_cli-1.4.0/bpkio_cli/core/session_recorder.py
--rw-r--r--   0        0        0      395 2023-06-05 14:52:28.932292 bpkio_cli-1.4.0/bpkio_cli/utils/__init__.py
--rw-r--r--   0        0        0     2288 2023-06-05 14:52:28.932584 bpkio_cli-1.4.0/bpkio_cli/utils/arrays.py
--rw-r--r--   0        0        0     1358 2023-06-05 14:52:28.932885 bpkio_cli-1.4.0/bpkio_cli/utils/datetimes.py
--rw-r--r--   0        0        0     1828 2023-06-05 14:52:28.933224 bpkio_cli-1.4.0/bpkio_cli/utils/editor.py
--rw-r--r--   0        0        0      494 2023-06-05 19:39:43.849589 bpkio_cli-1.4.0/bpkio_cli/utils/inquirer.py
--rw-r--r--   0        0        0      136 2023-06-05 14:52:28.933905 bpkio_cli-1.4.0/bpkio_cli/utils/json.py
--rw-r--r--   0        0        0      567 2023-06-05 14:52:28.934214 bpkio_cli-1.4.0/bpkio_cli/utils/profile_maker.py
--rw-r--r--   0        0        0    11802 2023-06-06 06:32:34.505189 bpkio_cli-1.4.0/bpkio_cli/utils/url_builders.py
--rw-r--r--   0        0        0      861 2023-06-05 14:52:28.934866 bpkio_cli-1.4.0/bpkio_cli/utils/urls.py
--rw-r--r--   0        0        0     1034 2023-06-05 14:52:28.935214 bpkio_cli-1.4.0/bpkio_cli/writers/breadcrumbs.py
--rw-r--r--   0        0        0     1667 2023-06-06 07:59:33.797067 bpkio_cli-1.4.0/bpkio_cli/writers/colorizer.py
--rw-r--r--   0        0        0     5213 2023-06-06 14:37:01.564679 bpkio_cli-1.4.0/bpkio_cli/writers/content_display.py
--rw-r--r--   0        0        0      840 2023-06-05 14:52:28.936348 bpkio_cli-1.4.0/bpkio_cli/writers/diff.py
--rw-r--r--   0        0        0      751 2023-06-06 10:33:05.139814 bpkio_cli-1.4.0/bpkio_cli/writers/formatter.py
--rw-r--r--   0        0        0     5364 2023-06-06 14:30:13.177404 bpkio_cli-1.4.0/bpkio_cli/writers/hls_formatter.py
--rw-r--r--   0        0        0      714 2023-06-05 14:52:28.938409 bpkio_cli-1.4.0/bpkio_cli/writers/json_formatter.py
--rw-r--r--   0        0        0     1665 2023-06-05 19:39:32.651931 bpkio_cli-1.4.0/bpkio_cli/writers/players.py
--rw-r--r--   0        0        0     1631 2023-06-06 14:40:13.522055 bpkio_cli-1.4.0/bpkio_cli/writers/scte35.py
--rw-r--r--   0        0        0     1865 2023-06-05 14:52:28.939530 bpkio_cli-1.4.0/bpkio_cli/writers/tables.py
--rw-r--r--   0        0        0     5368 2023-06-06 10:21:02.754933 bpkio_cli-1.4.0/bpkio_cli/writers/xml_formatter.py
--rw-r--r--   0        0        0     1243 2023-06-07 15:39:48.698279 bpkio_cli-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 bpkio_cli-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 14:52:28.912688 bpkio_cli-1.5.0/README.md
+-rw-r--r--   0        0        0       22 2023-06-09 15:48:20.061591 bpkio_cli-1.5.0/bpkio_cli/__init__.py
+-rw-r--r--   0        0        0     3880 2023-06-09 12:59:30.590598 bpkio_cli-1.5.0/bpkio_cli/app.py
+-rw-r--r--   0        0        0       91 2023-06-05 14:52:28.913801 bpkio_cli-1.5.0/bpkio_cli/click_mods/__init__.py
+-rw-r--r--   0        0        0      771 2023-06-05 14:52:28.914515 bpkio_cli-1.5.0/bpkio_cli/click_mods/default_last_command.py
+-rw-r--r--   0        0        0     5244 2023-06-08 08:20:08.800756 bpkio_cli-1.5.0/bpkio_cli/click_mods/group_rest_resource.py
+-rw-r--r--   0        0        0     1747 2023-06-05 14:52:28.915564 bpkio_cli-1.5.0/bpkio_cli/click_mods/option_eat_all.py
+-rw-r--r--   0        0        0      599 2023-06-05 14:52:28.916268 bpkio_cli-1.5.0/bpkio_cli/click_options/__init__.py
+-rw-r--r--   0        0        0      848 2023-06-05 14:52:28.916749 bpkio_cli-1.5.0/bpkio_cli/click_options/admin.py
+-rw-r--r--   0        0        0      355 2023-06-05 14:52:28.917214 bpkio_cli-1.5.0/bpkio_cli/click_options/json.py
+-rw-r--r--   0        0        0      958 2023-06-05 14:52:28.917874 bpkio_cli-1.5.0/bpkio_cli/click_options/list.py
+-rw-r--r--   0        0        0      933 2023-06-05 14:52:28.918220 bpkio_cli-1.5.0/bpkio_cli/click_options/poll.py
+-rw-r--r--   0        0        0      845 2023-06-07 15:41:46.996440 bpkio_cli-1.5.0/bpkio_cli/click_options/read.py
+-rw-r--r--   0        0        0     1183 2023-06-05 14:52:28.919379 bpkio_cli-1.5.0/bpkio_cli/click_options/search.py
+-rw-r--r--   0        0        0      445 2023-06-05 14:52:28.919891 bpkio_cli-1.5.0/bpkio_cli/click_options/table.py
+-rw-r--r--   0        0        0     1735 2023-06-09 15:29:17.087943 bpkio_cli-1.5.0/bpkio_cli/click_options/urls.py
+-rw-r--r--   0        0        0      656 2023-06-05 14:52:28.920820 bpkio_cli-1.5.0/bpkio_cli/commands/__init__.py
+-rw-r--r--   0        0        0      751 2023-06-07 16:02:26.119276 bpkio_cli-1.5.0/bpkio_cli/commands/addons.py
+-rw-r--r--   0        0        0     5246 2023-06-07 15:41:46.996745 bpkio_cli-1.5.0/bpkio_cli/commands/configure.py
+-rw-r--r--   0        0        0     1766 2023-06-07 15:41:46.997118 bpkio_cli-1.5.0/bpkio_cli/commands/consumption.py
+-rw-r--r--   0        0        0     4379 2023-06-07 15:41:46.997928 bpkio_cli-1.5.0/bpkio_cli/commands/creators/ad_insertion.py
+-rw-r--r--   0        0        0     7921 2023-06-07 15:41:46.998681 bpkio_cli-1.5.0/bpkio_cli/commands/creators/sources.py
+-rw-r--r--   0        0        0     4055 2023-06-07 15:41:46.999059 bpkio_cli-1.5.0/bpkio_cli/commands/creators/virtual_channel.py
+-rw-r--r--   0        0        0     8949 2023-06-09 12:53:03.155944 bpkio_cli-1.5.0/bpkio_cli/commands/creators/virtual_channel_populate.py
+-rw-r--r--   0        0        0      761 2023-06-05 14:52:28.924009 bpkio_cli-1.5.0/bpkio_cli/commands/hello.py
+-rw-r--r--   0        0        0     1251 2023-06-05 14:52:28.924268 bpkio_cli-1.5.0/bpkio_cli/commands/memory.py
+-rw-r--r--   0        0        0     3444 2023-06-07 15:41:46.999728 bpkio_cli-1.5.0/bpkio_cli/commands/package.py
+-rw-r--r--   0        0        0    10214 2023-06-08 07:15:15.683549 bpkio_cli-1.5.0/bpkio_cli/commands/profiles.py
+-rw-r--r--   0        0        0     2700 2023-06-05 14:52:28.925148 bpkio_cli-1.5.0/bpkio_cli/commands/recorder.py
+-rw-r--r--   0        0        0     3669 2023-06-05 14:52:28.925467 bpkio_cli-1.5.0/bpkio_cli/commands/services.py
+-rw-r--r--   0        0        0     5728 2023-06-07 15:41:47.000514 bpkio_cli-1.5.0/bpkio_cli/commands/sources.py
+-rw-r--r--   0        0        0    19372 2023-06-09 14:37:07.787776 bpkio_cli-1.5.0/bpkio_cli/commands/template_crud.py
+-rw-r--r--   0        0        0     7306 2023-06-05 14:52:28.926463 bpkio_cli-1.5.0/bpkio_cli/commands/template_crud_slots.py
+-rw-r--r--   0        0        0      332 2023-06-05 14:52:28.926844 bpkio_cli-1.5.0/bpkio_cli/commands/tenants.py
+-rw-r--r--   0        0        0     5799 2023-06-09 15:31:03.604764 bpkio_cli-1.5.0/bpkio_cli/commands/url.py
+-rw-r--r--   0        0        0      359 2023-06-05 14:52:28.927398 bpkio_cli-1.5.0/bpkio_cli/commands/users.py
+-rw-r--r--   0        0        0     1036 2023-06-05 14:52:28.927822 bpkio_cli-1.5.0/bpkio_cli/core/app_context.py
+-rw-r--r--   0        0        0     4556 2023-06-09 14:54:47.502096 bpkio_cli-1.5.0/bpkio_cli/core/config_provider.py
+-rw-r--r--   0        0        0      283 2023-06-09 10:01:38.442641 bpkio_cli-1.5.0/bpkio_cli/core/exceptions.py
+-rw-r--r--   0        0        0     2714 2023-06-09 11:12:30.963265 bpkio_cli-1.5.0/bpkio_cli/core/initialize.py
+-rw-r--r--   0        0        0     1718 2023-06-05 14:52:28.929630 bpkio_cli-1.5.0/bpkio_cli/core/logger.py
+-rw-r--r--   0        0        0     8332 2023-06-07 15:41:47.001439 bpkio_cli-1.5.0/bpkio_cli/core/packager.py
+-rw-r--r--   0        0        0     9526 2023-06-09 15:34:00.255674 bpkio_cli-1.5.0/bpkio_cli/core/resource_recorder.py
+-rw-r--r--   0        0        0     2204 2023-06-05 14:52:28.930943 bpkio_cli-1.5.0/bpkio_cli/core/resource_trail.py
+-rw-r--r--   0        0        0     5128 2023-06-05 14:52:28.931598 bpkio_cli-1.5.0/bpkio_cli/core/response_handler.py
+-rw-r--r--   0        0        0     1234 2023-06-05 14:52:28.931905 bpkio_cli-1.5.0/bpkio_cli/core/session_recorder.py
+-rw-r--r--   0        0        0      395 2023-06-05 14:52:28.932292 bpkio_cli-1.5.0/bpkio_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2288 2023-06-05 14:52:28.932584 bpkio_cli-1.5.0/bpkio_cli/utils/arrays.py
+-rw-r--r--   0        0        0     1358 2023-06-05 14:52:28.932885 bpkio_cli-1.5.0/bpkio_cli/utils/datetimes.py
+-rw-r--r--   0        0        0     1828 2023-06-05 14:52:28.933224 bpkio_cli-1.5.0/bpkio_cli/utils/editor.py
+-rw-r--r--   0        0        0      494 2023-06-07 15:41:47.002131 bpkio_cli-1.5.0/bpkio_cli/utils/inquirer.py
+-rw-r--r--   0        0        0      136 2023-06-05 14:52:28.933905 bpkio_cli-1.5.0/bpkio_cli/utils/json.py
+-rw-r--r--   0        0        0      567 2023-06-05 14:52:28.934214 bpkio_cli-1.5.0/bpkio_cli/utils/profile_maker.py
+-rw-r--r--   0        0        0    14499 2023-06-09 15:31:09.893672 bpkio_cli-1.5.0/bpkio_cli/utils/url_builders.py
+-rw-r--r--   0        0        0      861 2023-06-05 14:52:28.934866 bpkio_cli-1.5.0/bpkio_cli/utils/urls.py
+-rw-r--r--   0        0        0     1034 2023-06-05 14:52:28.935214 bpkio_cli-1.5.0/bpkio_cli/writers/breadcrumbs.py
+-rw-r--r--   0        0        0     1667 2023-06-07 15:41:47.003003 bpkio_cli-1.5.0/bpkio_cli/writers/colorizer.py
+-rw-r--r--   0        0        0     5213 2023-06-09 10:05:20.541841 bpkio_cli-1.5.0/bpkio_cli/writers/content_display.py
+-rw-r--r--   0        0        0      840 2023-06-05 14:52:28.936348 bpkio_cli-1.5.0/bpkio_cli/writers/diff.py
+-rw-r--r--   0        0        0      751 2023-06-07 15:41:47.003793 bpkio_cli-1.5.0/bpkio_cli/writers/formatter.py
+-rw-r--r--   0        0        0     5729 2023-06-09 10:04:01.517494 bpkio_cli-1.5.0/bpkio_cli/writers/hls_formatter.py
+-rw-r--r--   0        0        0      714 2023-06-05 14:52:28.938409 bpkio_cli-1.5.0/bpkio_cli/writers/json_formatter.py
+-rw-r--r--   0        0        0     1658 2023-06-09 14:52:25.540620 bpkio_cli-1.5.0/bpkio_cli/writers/players.py
+-rw-r--r--   0        0        0     1631 2023-06-07 15:41:47.004793 bpkio_cli-1.5.0/bpkio_cli/writers/scte35.py
+-rw-r--r--   0        0        0     1865 2023-06-05 14:52:28.939530 bpkio_cli-1.5.0/bpkio_cli/writers/tables.py
+-rw-r--r--   0        0        0     5741 2023-06-09 10:03:51.584951 bpkio_cli-1.5.0/bpkio_cli/writers/xml_formatter.py
+-rw-r--r--   0        0        0     1242 2023-06-09 15:48:20.060601 bpkio_cli-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 bpkio_cli-1.5.0/PKG-INFO
```

### Comparing `bpkio_cli-1.4.0/bpkio_cli/app.py` & `bpkio_cli-1.5.0/bpkio_cli/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,16 +142,16 @@
     try:
         bic()
     except Exception as e:
         if hasattr(e, "status_code"):
             st = " [{}] ".format(e.status_code)
         else:
             st = ""
-        msg = "{}:{}{}".format(e.__class__.__name__, st, e)
+        msg = "{}: {}{}".format(e.__class__.__name__, st, e)
         click.secho(msg, fg="red")
 
         if hasattr(e, "original_message"):
-            click.secho("  > " + e.original_message, fg="red")
+            click.secho("  > {}".format(e.original_message), fg="red")
 
 
 if __name__ == "__main__":
     debug_entry_point()
```

### Comparing `bpkio_cli-1.4.0/bpkio_cli/click_mods/default_last_command.py` & `bpkio_cli-1.5.0/bpkio_cli/click_mods/default_last_command.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/click_mods/group_rest_resource.py` & `bpkio_cli-1.5.0/bpkio_cli/click_mods/group_rest_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,19 @@
             args[0] != ""
             and args[0] not in self.commands
             and (args[1] in self.commands or args[1] in self.alias2name)
         ):
             target_type = self._get_resource_class_for_command()
 
             # Lookup in the cache if the ID is not a recognised value
-            if not args[0].isdigit() and not args[0].startswith("-"):
+            if (
+                not args[0].isdigit()
+                and not args[0].startswith("-")
+                and not args[0].startswith("http")
+            ):
                 placeholder = args[0]
                 args[0] = ctx.obj.cache.resolve(placeholder, target_type)
                 display_context(
                     f"Resolved '{placeholder}' to {target_type.__name__} id {args[0]}",
                 )
 
             resources: ResourceTrail = ctx.obj.resources
```

### Comparing `bpkio_cli-1.4.0/bpkio_cli/click_mods/option_eat_all.py` & `bpkio_cli-1.5.0/bpkio_cli/click_mods/option_eat_all.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/click_options/__init__.py` & `bpkio_cli-1.5.0/bpkio_cli/click_options/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/click_options/admin.py` & `bpkio_cli-1.5.0/bpkio_cli/click_options/admin.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/click_options/list.py` & `bpkio_cli-1.5.0/bpkio_cli/click_options/list.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/click_options/poll.py` & `bpkio_cli-1.5.0/bpkio_cli/click_options/poll.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/click_options/read.py` & `bpkio_cli-1.5.0/bpkio_cli/click_options/read.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/click_options/search.py` & `bpkio_cli-1.5.0/bpkio_cli/click_options/search.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/__init__.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/addons.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/addons.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/configure.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/configure.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/consumption.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/consumption.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/creators/ad_insertion.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/creators/ad_insertion.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/creators/sources.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/creators/sources.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/creators/virtual_channel.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/creators/virtual_channel.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/creators/virtual_channel_populate.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/creators/virtual_channel_populate.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     VirtualChannelService,
     VirtualChannelSlotIn,
     VirtualChannelSlotType,
 )
 
 import bpkio_cli.utils.inquirer as inqdef
 from bpkio_cli.core.app_context import AppContext
+from bpkio_cli.core.config_provider import ConfigProvider
 from bpkio_cli.utils.datetimes import (
     parse_date_expression_as_utc,
     parse_duration_expression,
 )
 
 
 def populate_virtual_channel_slots_command():
@@ -149,15 +150,17 @@
             if source_id == "ADBREAK":
                 default_duration = adbreak_default_duration
 
             if source:
                 if source.type == SourceType.LIVE:
                     default_duration = "10 min"
                 else:
-                    handler: ContentHandler = factory.create_handler(source.full_url)
+                    handler: ContentHandler = factory.create_handler(
+                        source.full_url, user_agent=ConfigProvider().get_user_agent()
+                    )
                     default_duration = str(handler.get_duration())
 
             if source_id != "SKIP":
                 # ask for duration to insert
                 duration = inquirer.text(
                     message="Duration",
                     default=default_duration,
```

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/hello.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/hello.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/memory.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/memory.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/package.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/package.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/profiles.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
     search_fields,
     json,
     select_fields,
     sort_fields,
 ):
     search_def = bic_options.validate_search(single_term, search_terms, search_fields)
 
-    profiles = obj.api.transcoding_profiles.search(filters=search_def, tenantId=tenant)
+    profiles = obj.api.transcoding_profiles.search(filters=search_def, tenant_id=tenant)
 
     obj.response_handler.treat_list_resources(
         profiles,
         select_fields=select_fields,
         sort_fields=sort_fields,
         json=json,
     )
```

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/recorder.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/recorder.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/services.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/services.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/sources.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/sources.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/template_crud.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/template_crud.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,32 +77,38 @@
         # Record the resource
         if ctx.obj.cache and hasattr(resource, "id"):
             ctx.obj.cache.record(resource)
 
         return resource
 
     def get_content_handler(
-        resource, replacement_fqdn=None, extra_url=None, subplaylist_index=None
+        resource,
+        replacement_fqdn=None,
+        extra_url=None,
+        subplaylist_index=None,
+        user_agent=None,
     ):
         api = click.get_current_context().obj.api
 
         if isinstance(resource, SourceIn):
             return get_source_handler(
                 resource,
                 extra_url=extra_url,
                 subplaylist_index=subplaylist_index,
+                user_agent=user_agent,
             )
 
         if isinstance(resource, ServiceIn):
             return get_service_handler(
                 resource,
                 replacement_fqdn=replacement_fqdn,
                 extra_url=extra_url,
                 subplaylist_index=subplaylist_index,
                 api=api,
+                user_agent=user_agent,
             )
 
     # === GROUP ===
 
     @cloup.group(
         name=name,
         help=f"Manage {resource_title}s",
@@ -277,19 +283,24 @@
         # --- URL Command
         @cloup.command(help="Retrieve the full URL of the resource")
         @bic_options.url
         def url(
             sub: int,
             url: str,
             fqdn: str,
+            user_agent: str,
             **kwargs,
         ):
             resource = retrieve_resource()
             handler = get_content_handler(
-                resource, replacement_fqdn=fqdn, extra_url=url, subplaylist_index=sub
+                resource,
+                replacement_fqdn=fqdn,
+                extra_url=url,
+                subplaylist_index=sub,
+                user_agent=user_agent,
             )
 
             if handler:
                 click.secho(handler.url, fg="yellow")
 
         content_section.add_command(url)
 
@@ -316,20 +327,25 @@
         @bic_options.url
         @click.pass_obj
         def table(
             obj: AppContext,
             sub: int,
             url: str,
             fqdn: str,
+            user_agent: str,
             header: bool = True,
             **kwargs,
         ):
             resource = retrieve_resource()
             handler = get_content_handler(
-                resource, replacement_fqdn=fqdn, extra_url=url, subplaylist_index=sub
+                resource,
+                replacement_fqdn=fqdn,
+                extra_url=url,
+                subplaylist_index=sub,
+                user_agent=user_agent,
             )
             if handler:
                 try:
                     display_content(
                         handler=handler,
                         max=1,
                         interval=0,
@@ -352,24 +368,29 @@
         @bic_options.table
         @click.pass_obj
         def read(
             obj: AppContext,
             sub: int,
             url: str,
             fqdn: str,
+            user_agent: str,
             table: bool,
             raw: bool,
             top: int = 0,
             tail: int = 0,
             header: bool = True,
             pager: bool = False,
         ):
             resource = retrieve_resource()
             handler = get_content_handler(
-                resource, replacement_fqdn=fqdn, extra_url=url, subplaylist_index=sub
+                resource,
+                replacement_fqdn=fqdn,
+                extra_url=url,
+                subplaylist_index=sub,
+                user_agent=user_agent,
             )
             if handler:
                 try:
                     display_content(
                         handler=handler,
                         max=1,
                         interval=0,
@@ -395,27 +416,32 @@
         @bic_options.url
         @bic_options.table
         @bic_options.poll
         def poll(
             sub: int,
             url: str,
             fqdn: str,
+            user_agent: str,
             max: int,
             interval: int,
             raw: bool,
             diff: bool,
             top: bool,
             tail: bool,
             clear: bool,
             table: bool,
             pager: bool,
         ):
             resource = retrieve_resource()
             handler = get_content_handler(
-                resource, replacement_fqdn=fqdn, extra_url=url, subplaylist_index=sub
+                resource,
+                replacement_fqdn=fqdn,
+                extra_url=url,
+                subplaylist_index=sub,
+                user_agent=user_agent,
             )
 
             if handler:
                 display_content(
                     handler,
                     max=max,
                     interval=interval,
@@ -443,18 +469,24 @@
             default="CONFIG",
             help="The template for a player URL",
             type=str,
             is_flag=False,
             flag_value="CHOICE",
         )
         @click.pass_obj
-        def play(obj: AppContext, fqdn: str, url: str, sub: int, player: str):
+        def play(
+            obj: AppContext, fqdn: str, url: str, user_agent: str, sub: int, player: str
+        ):
             resource = retrieve_resource()
             handler = get_content_handler(
-                resource, replacement_fqdn=fqdn, extra_url=url, subplaylist_index=sub
+                resource,
+                replacement_fqdn=fqdn,
+                extra_url=url,
+                subplaylist_index=sub,
+                user_agent=user_agent,
             )
             if player == "CONFIG":
                 player = obj.config.get("player")
 
             if player == "CHOICE":
                 player = StreamPlayer.prompt_player()
 
@@ -487,19 +519,29 @@
             is_flag=True,
             default=False,
             help="Save the profile to a file",
         )
         @bic_options.url
         @click.pass_obj
         def profile(
-            obj: AppContext, fqdn: str, url: str, sub: int, with_table: bool, save: bool
+            obj: AppContext,
+            fqdn: str,
+            url: str,
+            user_agent: str,
+            sub: int,
+            with_table: bool,
+            save: bool,
         ):
             resource = retrieve_resource()
             handler = get_content_handler(
-                resource, replacement_fqdn=fqdn, extra_url=url, subplaylist_index=sub
+                resource,
+                replacement_fqdn=fqdn,
+                extra_url=url,
+                subplaylist_index=sub,
+                user_agent=user_agent,
             )
 
             profile = make_transcoding_profile(handler)
 
             if with_table:
                 display_table(profile["transcoding"]["jobs"])
             else:
```

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/template_crud_slots.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/template_crud_slots.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/commands/url.py` & `bpkio_cli-1.5.0/bpkio_cli/commands/url.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,32 +10,40 @@
 from bpkio_cli.commands.sources import create as source_create
 from bpkio_cli.core.app_context import AppContext
 from bpkio_cli.core.config_provider import ConfigProvider
 from bpkio_cli.utils.profile_maker import make_transcoding_profile
 from bpkio_cli.writers.content_display import display_content
 from bpkio_cli.writers.players import StreamPlayer
 from bpkio_cli.writers.tables import display_table
+from bpkio_cli.utils.url_builders import ask_for_user_agent
 
 
 def determine_source_type(full_url) -> SourceType | None:
     source_type = SourceTypeDetector.determine_source_type(full_url)
     if not source_type:
         click.secho(
             "Could not determine the type of source for that URL", fg="red", bold="true"
         )
         return None
     else:
         return source_type
 
 
-def get_handler(sub: int | None = None) -> ContentHandler:
+def get_handler(
+    sub: int | None = None, user_agent: str | None = None
+) -> ContentHandler:
     ctx = click.get_current_context()
     url = ctx.obj.resources.last()
 
-    handler: ContentHandler = factory.create_handler(url)
+    if user_agent == "SELECT":
+        ask_for_user_agent(url)
+
+    handler: ContentHandler = factory.create_handler(
+        url, user_agent=ConfigProvider().get_user_agent(user_agent)
+    )
 
     if not sub:
         return handler
     else:
         if not handler.has_children():
             raise click.UsageError(
                 "`--sub` cannot be used with this source, as it has no children URLs"
@@ -89,17 +97,24 @@
     help="Loads and displays the content of a URL"
     ", optionally highlighted with relevant information"
 )
 @bic_options.read
 @bic_options.url
 @bic_options.table
 def read(
-    sub: int, table: bool, raw: bool, top: bool, tail: bool, pager: bool, **kwargs
+    sub: int,
+    table: bool,
+    raw: bool,
+    top: bool,
+    tail: bool,
+    pager: bool,
+    user_agent: str,
+    **kwargs,
 ):
-    handler = get_handler(sub)
+    handler = get_handler(sub, user_agent)
 
     display_content(
         handler=handler,
         max=1,
         interval=0,
         table=table,
         raw=raw,
@@ -113,25 +128,26 @@
 @cloup.command(help="Similar to `read`, but regularly re-load the URL's content")
 @bic_options.read
 @bic_options.url
 @bic_options.poll
 @bic_options.table
 def poll(
     sub: int,
+    user_agent: str,
     max: int,
     interval: int,
     raw: bool,
     diff: bool,
     top: bool,
     tail: bool,
     clear: bool,
     table: bool,
     **kwargs,
 ):
-    handler = get_handler(sub)
+    handler = get_handler(sub, user_agent)
 
     display_content(
         handler=handler,
         max=max,
         interval=interval,
         table=table,
         raw=raw,
```

### Comparing `bpkio_cli-1.4.0/bpkio_cli/core/app_context.py` & `bpkio_cli-1.5.0/bpkio_cli/core/app_context.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/core/config_provider.py` & `bpkio_cli-1.5.0/bpkio_cli/core/config_provider.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,22 +8,31 @@
         self.config_path = os.path.expanduser(config_path)
         self.config = configparser.ConfigParser()
         self.temporary = dict()  # For temporary or overrides values
         self.initialize()
 
     def initialize(self):
         default_values = {
-            "settings": {"player": "browser", "editor": "vim", "verbose": "2"},
+            "settings": {
+                "player": "browser",
+                "editor": "vim",
+                "verbose": "2",
+                "user-agent": "chrome",
+            },
             "pygments": {"style": "monokai", "linenos": "0"},
             "players": {
                 "browser": "{url}",
                 "demo": "https://theoplayer.ridgeline.fr/?url1={url}&title1={name}&autoplay=true",
                 "hls": "https://hlsjs.video-dev.org/demo/?src={url}",
                 "dash": "https://reference.dashif.org/dash.js/nightly/samples/dash-if-reference-player/index.html?mpd={url}",
             },
+            "user-agents": {
+                "chrome": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.110 Safari/537.36",
+                "safari": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/15.4 Safari/605.1.15",
+            },
         }
 
         if not os.path.exists(self.config_path):
             self.config.read_dict(default_values)
             self.save_config()
         else:
             self.config.read(self.config_path)
@@ -37,15 +46,15 @@
                         self._set(key, value, section)
 
     def get(self, key, cast_type=None, section="settings"):
         if key in self.temporary:
             value = self.temporary[key]
         else:
             value = self.config.get(section, key)
-        
+
         return self.cast_value(value, cast_type)
 
     def cast_value(self, value, cast_type):
         if cast_type is None:
             return value
         elif cast_type == bool:
             return value.lower() in {"true", "1"}
@@ -76,22 +85,21 @@
             case "player":
                 self.set_player(value)
             case _:
                 if key not in self.config["settings"]:
                     raise ValueError(f"There is no setting called '{key}'.")
 
                 self._set(key, value)
-                
+
     def set_temporary(self, key, value):
         self.temporary[key] = value
 
     def save_config(self):
         with open(self.config_path, "w") as config_file:
             self.config.write(config_file)
-            
 
     # --- Specific config parameters ---
 
     def set_player(self, value):
         if value in self.config["players"]:
             self._set("player", value)
         else:
@@ -100,7 +108,18 @@
     def add_player(self, label, player_string):
         self.config.set("players", label, player_string)
         self.save_config()
 
     def list_players(self) -> Dict[str, Any]:
         return self.get_section_items("players")
 
+    def get_user_agent(self, label=None):
+        if not label:
+            label = self.get("user-agent")
+        if label not in self.config["user-agents"]:
+            # allows passing a user-agent string directly
+            return label
+
+        return self.get(label, section="user-agents")
+
+    def list_user_agents(self) -> Dict[str, Any]:
+        return self.get_section_items("user-agents")
```

### Comparing `bpkio_cli-1.4.0/bpkio_cli/core/initialize.py` & `bpkio_cli-1.5.0/bpkio_cli/core/initialize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import os
+from importlib.metadata import version
 
 import click
 from bpkio_api import BroadpeakIoApi
 from bpkio_api.credential_provider import TenantProfileProvider
 from bpkio_api.models import BaseResource
 
 from bpkio_cli.core.app_context import AppContext
 from bpkio_cli.core.logger import get_child_logger
 
 logger = get_child_logger("init")
 
+user_agent = f"bpkio-cli/{version('bpkio-cli')}"
+
 
 def initialize(
     requires_api: bool,
     tenant: str | int | None = None,
     use_cache: bool = True,
     use_prompts: bool = True,
 ) -> AppContext:
@@ -51,15 +54,18 @@
     if os.path.exists(session_sentinel):
         # open it and extract the path to the session file.
         with open(session_sentinel, "r") as f:
             session_file = f.read()
 
     if requires_api:
         api = BroadpeakIoApi(
-            tenant=tenant, use_cache=use_cache, session_file=session_file
+            tenant=tenant,
+            use_cache=use_cache,
+            session_file=session_file,
+            user_agent=user_agent,
         )
         app_context = AppContext(api=api, tenant_provider=TenantProfileProvider())
         app_context.config.set_temporary("use_prompts", use_prompts)
 
         if app_context.config.get("verbose", int) > 0:
             full_tenant = api.get_self_tenant()
             app_context.tenant = full_tenant
```

### Comparing `bpkio_cli-1.4.0/bpkio_cli/core/logger.py` & `bpkio_cli-1.5.0/bpkio_cli/core/logger.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/core/packager.py` & `bpkio_cli-1.5.0/bpkio_cli/core/packager.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/core/resource_recorder.py` & `bpkio_cli-1.5.0/bpkio_cli/core/resource_recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,37 +167,43 @@
             resources = [r for r in resources if isinstance(r, BaseModel)]
         return resources
 
     def list_lists(self):
         """Return a list of all lists in the cache"""
         return self._cache_lists
 
+    def _make_key(self, item):
+        if hasattr(item, "summary"):
+            return item.summary
+        else:
+            return str(item)
+
     def record_metadata(self, item, key, value):
         """Records metadata against an item"""
-        item_key = item.summary
+        item_key = self._make_key(item)
         if item_key not in self._cache_metadata:
             self._cache_metadata[item_key] = dict()
 
         if key not in self._cache_metadata[item_key]:
             self._cache_metadata[item_key][key] = MoveToFrontList(maxlen=10)
 
         self._cache_metadata[item_key][key].add(value)
 
     def get_metadata(self, item, key):
         """Returns the metadata for an item"""
-        item_key = item.summary
+        item_key = self._make_key(item)
         if item_key in self._cache_metadata:
             lst: MoveToFrontList = self._cache_metadata[item_key].get(key)
             if lst:
                 return lst.values()
         return None
 
     def remove_metadata(self, item, key, value):
         """Removes metadata for an item"""
-        item_key = item.summary
+        item_key = self._make_key(item)
         if item_key in self._cache_metadata:
             lst: MoveToFrontList = self._cache_metadata[item_key].get(key)
             if lst:
                 lst.remove(value)
                 self._cache_metadata[item_key][key] = lst
                 return lst
         return None
```

### Comparing `bpkio_cli-1.4.0/bpkio_cli/core/resource_trail.py` & `bpkio_cli-1.5.0/bpkio_cli/core/resource_trail.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/core/response_handler.py` & `bpkio_cli-1.5.0/bpkio_cli/core/response_handler.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/core/session_recorder.py` & `bpkio_cli-1.5.0/bpkio_cli/core/session_recorder.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/utils/arrays.py` & `bpkio_cli-1.5.0/bpkio_cli/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/utils/datetimes.py` & `bpkio_cli-1.5.0/bpkio_cli/utils/datetimes.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/utils/editor.py` & `bpkio_cli-1.5.0/bpkio_cli/utils/editor.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/utils/profile_maker.py` & `bpkio_cli-1.5.0/bpkio_cli/utils/profile_maker.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/utils/url_builders.py` & `bpkio_cli-1.5.0/bpkio_cli/utils/url_builders.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,38 +12,47 @@
     SourceIn,
     SourceType,
     VirtualChannelService,
 )
 
 import bpkio_cli.utils.inquirer as inqdef
 from bpkio_cli.core.app_context import AppContext
+from bpkio_cli.core.config_provider import ConfigProvider
 from bpkio_cli.utils.urls import add_query_parameters, validate_ipv4_or_domain
 
 NEW = "-- add new --"
 DELETED = "__DELETED__"
 UNSET = "__UNSET__"
 
 
 def get_source_handler(
-    source: SourceIn, extra_url: Optional[str], subplaylist_index: Optional[int]
+    source: SourceIn,
+    extra_url: Optional[str],
+    subplaylist_index: Optional[int],
+    user_agent: Optional[str],
 ) -> ContentHandler:
     if isinstance(source, AssetCatalogSourceIn):
         # Ask for extra portion of URL if it wasn't supplied
         if not extra_url:
             extra_url = ask_for_asset_catalog_sub_path(source)
 
     url_to_read = source.make_full_url(extra_url)
 
     if isinstance(source, AdServerSourceIn):
         # Fill query parameters
         if not extra_url or "?" not in url_to_read:
             filled_params = ask_for_adserver_query_params(source)
             url_to_read = add_query_parameters(url_to_read, filled_params)
 
-    handler: ContentHandler = factory.create_handler(url_to_read)
+    if user_agent == "SELECT":
+        user_agent = ask_for_user_agent(source)
+
+    handler: ContentHandler = factory.create_handler(
+        url_to_read, user_agent=ConfigProvider().get_user_agent(user_agent)
+    )
     if subplaylist_index:
         if not handler.has_children():
             raise click.UsageError(
                 "`--sub` cannot be used with this source, as it has no children URLs"
             )
         handler = handler.get_child(subplaylist_index)
 
@@ -52,14 +61,15 @@
 
 def get_service_handler(
     service,
     api,
     replacement_fqdn: Optional[str],
     extra_url: Optional[str],
     subplaylist_index: Optional[int],
+    user_agent: Optional[str],
 ) -> ContentHandler:
     """Calculates the URL to call for a Service, based on its type and Source"""
     url_to_read = service.make_full_url()
 
     if isinstance(service, AdInsertionService):
         source_type = service.source.type
         source_id = service.source.id
@@ -98,15 +108,22 @@
             queries = {k: v for k, v in (x.split("=") for x in query_string.split("&"))}
 
         filled_params = ask_for_adserver_query_params(
             ad_config.adServer, existing_params=queries, for_service=True
         )
         url_to_read = add_query_parameters(url_to_read, filled_params)
 
-    handler: ContentHandler = factory.create_handler(url_to_read, from_url_only=True)
+    if user_agent == "SELECT":
+        user_agent = ask_for_user_agent(service)
+
+    handler: ContentHandler = factory.create_handler(
+        url_to_read,
+        from_url_only=True,
+        user_agent=ConfigProvider().get_user_agent(user_agent),
+    )
     if subplaylist_index:
         if not handler.has_children():
             raise click.UsageError(
                 "`--sub` cannot be used with this source, as it has no children URLs"
             )
         handler = handler.get_child(subplaylist_index)
 
@@ -278,14 +295,17 @@
 
     else:
         if cached_values:
             extra_url = cached_values[0]
         else:
             extra_url = source.assetSample
 
+        click.secho("> Sub-path: ", fg="white", nl=False)
+        click.secho(extra_url, fg="blue", bold=True)
+
     metadata_cache.record_metadata(source, "subPath", extra_url)
 
     return extra_url
 
 
 def ask_for_fqdn(service):
     fqdn = None
@@ -314,10 +334,71 @@
 
     else:
         if cached_fqdns:
             fqdn = cached_fqdns[0]
         else:
             fqdn = "CUSTOM_FQDN"
 
+        click.secho("> FQDN: ", fg="white", nl=False)
+        click.secho(fqdn, fg="blue", bold=True)
+
     metadata_cache.record_metadata(service, "fqdn", fqdn)
 
     return fqdn
+
+
+def ask_for_user_agent(resource):
+    ua = UNSET
+    obj: AppContext = click.get_current_context().obj
+    metadata_cache = obj.cache
+    cached_useragents = metadata_cache.get_metadata(resource, "user_agent")
+
+    if obj.config.get("use_prompts"):
+        click.echo()
+        while ua in [UNSET, DELETED]:
+            if cached_useragents:
+                ua_prompt = inquirer.select(
+                    message="User agent to use: ",
+                    choices=cached_useragents + [NEW],
+                    multiselect=False,
+                    default=cached_useragents[0],
+                    long_instruction="Keyboard: 'd' = delete the selected value | "
+                    "'ctrl-s' = skip all prompts, using last or default value",
+                    **inqdef.select_markers(),
+                )
+
+                @ua_prompt.register_kb("d")
+                def _handle_delete(event):
+                    choice_value = ua_prompt.result_value
+
+                    metadata_cache.remove_metadata(resource, "user_agent", choice_value)
+                    event.app.exit(result=DELETED)
+
+                @ua_prompt.register_kb("c-s")
+                def _handle_skip_all(event):
+                    choice_value = ua_prompt.result_value
+                    obj.config.set_temporary("use_prompts", False)
+                    click.secho(choice_value, fg="bright_blue")
+
+                    event.app.exit(result=choice_value)
+
+                ua = ua_prompt.execute()
+
+            if not cached_useragents or ua == NEW:
+                ua = inquirer.text(
+                    message="User agent (label or full string)",
+                    default="",
+                    **inqdef.markers(0),
+                ).execute()
+
+    else:
+        if cached_useragents:
+            ua = cached_useragents[0]
+        else:
+            ua = None
+
+        click.secho("> User-Agent: ", fg="white", nl=False)
+        click.secho(ua, fg="blue", bold=True)
+
+    metadata_cache.record_metadata(resource, "user_agent", ua)
+
+    return ua
```

### Comparing `bpkio_cli-1.4.0/bpkio_cli/utils/urls.py` & `bpkio_cli-1.5.0/bpkio_cli/utils/urls.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/writers/breadcrumbs.py` & `bpkio_cli-1.5.0/bpkio_cli/writers/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/writers/colorizer.py` & `bpkio_cli-1.5.0/bpkio_cli/writers/colorizer.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/writers/content_display.py` & `bpkio_cli-1.5.0/bpkio_cli/writers/content_display.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/writers/diff.py` & `bpkio_cli-1.5.0/bpkio_cli/writers/diff.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/writers/formatter.py` & `bpkio_cli-1.5.0/bpkio_cli/writers/formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/writers/hls_formatter.py` & `bpkio_cli-1.5.0/bpkio_cli/writers/hls_formatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 
 from bpkio_api.helpers.handlers import HLSHandler
 from colorama import Fore, Style, init
+from bpkio_cli.core.exceptions import UnexepctedContentError
 
 import bpkio_cli.writers.scte35 as scte35
 from bpkio_cli.writers.colorizer import Colorizer as CL
 from bpkio_cli.writers.formatter import OutputFormatter
 
 init()
 
@@ -27,19 +28,26 @@
 
     def format(self, mode="standard", top: int = 0, tail: int = 0):
         if top and top > 0:
             self.top = top
         if tail and tail > 0:
             self.tail = tail
 
-        match mode:
-            case "raw":
-                return self._content
-            case "standard":
-                return self.highlight()
+        try:
+            match mode:
+                case "raw":
+                    return self._content
+                case "standard":
+                    return self.highlight()
+        except Exception:
+            raise UnexepctedContentError(
+                message="Error formatting the content. "
+                "It does not appear to be a valid HLS document.\n"
+                "Raw content: \n{}".format(self.handler.content)
+            )
 
     def highlight(self):
         """Highlights specific HLS elements of interest"""
 
         nodes_to_highlight = {
             "#EXT-X-DATERANGE": CL.high2,
             "#EXT-OATCLS-SCTE35": CL.high2,
```

### Comparing `bpkio_cli-1.4.0/bpkio_cli/writers/json_formatter.py` & `bpkio_cli-1.5.0/bpkio_cli/writers/json_formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/writers/players.py` & `bpkio_cli-1.5.0/bpkio_cli/writers/players.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,12 +37,12 @@
 
     def available_player_templates(self):
         return self.config_provider.list_players().keys()
 
     @staticmethod
     def prompt_player():
         player = inquirer.fuzzy(
-            message="What (top-level) resources do you want to include in the package?  ",
+            message="What player (or page) do you want to open this resoure in?  ",
             choices=[p for p in StreamPlayer().available_player_templates()],
             **select_markers(),
         ).execute()
         return player
```

### Comparing `bpkio_cli-1.4.0/bpkio_cli/writers/scte35.py` & `bpkio_cli-1.5.0/bpkio_cli/writers/scte35.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/writers/tables.py` & `bpkio_cli-1.5.0/bpkio_cli/writers/tables.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.4.0/bpkio_cli/writers/xml_formatter.py` & `bpkio_cli-1.5.0/bpkio_cli/writers/xml_formatter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 import re
 from xml.sax.saxutils import escape
 
 from bpkio_api.helpers.handlers import XMLHandler
 from lxml import etree
 
+from bpkio_cli.core.exceptions import UnexepctedContentError
 from bpkio_cli.writers.colorizer import Colorizer as CL
 from bpkio_cli.writers.formatter import OutputFormatter
 
 
 class XMLFormatter(OutputFormatter):
     def __init__(self, handler: XMLHandler) -> None:
         super().__init__()
         self.handler = handler
 
     def format(self, mode="standard", top: int = 0, tail: int = 0):
-        match mode:
-            case "raw":
-                output = self.raw()
-            case "standard":
-                output = self.pretty_print()
-
-        output = self.trim(output, top, tail)
-        return output
+        try:
+            match mode:
+                case "raw":
+                    output = self.raw()
+                case "standard":
+                    output = self.pretty_print()
+
+            output = self.trim(output, top, tail)
+            return output
+        except Exception:
+            raise UnexepctedContentError(
+                message="Error formatting the content. "
+                "It does not appear to be a valid XML document.\n"
+                "Raw content: \n{}".format(self.handler.content)
+            )
 
     def raw(self):
         # Pretty-print the XML using the ElementTree's tostring() method
         # return etree.tostring(self.handler.xml_document, pretty_print=True)
 
         return self.handler.content.decode()
```

### Comparing `bpkio_cli-1.4.0/pyproject.toml` & `bpkio_cli-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "bpkio-cli"
-version = "1.4.0"
+version = "1.5.0"
 description = "A command line interface to the broadpeak.io APIs, with additional helpers"
 authors = ["Fabre Lambeau <fabre.lambeau@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "bpkio_cli" }]
 
 [tool.poetry-dynamic-versioning]
-enable = false
+enable = true
 vcs = "git"
 style = "semver"
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["*/__init__.py", "*/__version__.py", "*/_version.py"]
 
 [tool.poetry.dependencies]
-bpkio-python-sdk = "^1.3.0"
+bpkio-python-sdk = "^1.4.0"
 python = "^3.10"
 click = "^8.1.3"
 colorama = "^0.4.6"
 # inquirerpy = { git = "https://github.com/kazhala/InquirerPy" }
 inquirerpy = "^0.3.4"
 tabulate = "^0.9.0"
 arrow = "^1.2.3"
```

### Comparing `bpkio_cli-1.4.0/PKG-INFO` & `bpkio_cli-1.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bpkio-cli
-Version: 1.4.0
+Version: 1.5.0
 Summary: A command line interface to the broadpeak.io APIs, with additional helpers
 Author: Fabre Lambeau
 Author-email: fabre.lambeau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
-Requires-Dist: bpkio-python-sdk (>=1.3.0,<2.0.0)
+Requires-Dist: bpkio-python-sdk (>=1.4.0,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cloup (>=2.0.0.post1,<3.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: diskcache (>=5.4.0,<6.0.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
```

