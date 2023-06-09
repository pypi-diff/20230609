# Comparing `tmp/pynecone-0.1.33a2.tar.gz` & `tmp/pynecone-0.1.33a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-0.1.33a2.tar", max compression
+gzip compressed data, was "pynecone-0.1.33a3.tar", max compression
```

## Comparing `pynecone-0.1.33a2.tar` & `pynecone-0.1.33a3.tar`

### file list

```diff
@@ -1,171 +1,171 @@
--rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.33a2/LICENSE
--rw-r--r--   0        0        0     7876 2023-05-18 00:14:14.758659 pynecone-0.1.33a2/README.md
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.33a2/pynecone/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1340 2023-06-07 06:32:06.269060 pynecone-0.1.33a2/pynecone/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.33a2/pynecone/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.33a2/pynecone/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.33a2/pynecone/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.33a2/pynecone/.templates/jinja/app/pcconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.33a2/pynecone/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-05-18 18:33:16.414872 pynecone-0.1.33a2/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.33a2/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     2554 2023-06-07 06:28:05.215601 pynecone-0.1.33a2/pynecone/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-05-22 21:40:04.765805 pynecone-0.1.33a2/pynecone/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.33a2/pynecone/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.33a2/pynecone/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   257247 2023-05-26 18:45:47.401731 pynecone-0.1.33a2/pynecone/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-05-26 18:45:47.402096 pynecone-0.1.33a2/pynecone/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.33a2/pynecone/.templates/web/next.config.js
--rw-r--r--   0        0        0      995 2023-06-01 03:15:26.563786 pynecone-0.1.33a2/pynecone/.templates/web/package.json
--rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.33a2/pynecone/.templates/web/pages/404.js
--rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.33a2/pynecone/.templates/web/pages/_app.js
--rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.33a2/pynecone/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0     8480 2023-06-07 06:21:32.940912 pynecone-0.1.33a2/pynecone/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1490 2023-06-07 06:05:03.874348 pynecone-0.1.33a2/pynecone/__init__.py
--rw-r--r--   0        0        0      320 2023-06-07 06:05:03.874470 pynecone-0.1.33a2/pynecone/admin.py
--rw-r--r--   0        0        0    21105 2023-06-07 06:21:03.890579 pynecone-0.1.33a2/pynecone/app.py
--rw-r--r--   0        0        0     2524 2023-05-18 00:14:14.759391 pynecone-0.1.33a2/pynecone/base.py
--rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.33a2/pynecone/compiler/__init__.py
--rw-r--r--   0        0        0     6688 2023-06-07 06:05:03.875477 pynecone-0.1.33a2/pynecone/compiler/compiler.py
--rw-r--r--   0        0        0     2642 2023-06-07 06:26:49.090764 pynecone-0.1.33a2/pynecone/compiler/templates.py
--rw-r--r--   0        0        0     7761 2023-06-01 00:32:59.071818 pynecone-0.1.33a2/pynecone/compiler/utils.py
--rw-r--r--   0        0        0     7346 2023-06-07 06:05:03.875765 pynecone-0.1.33a2/pynecone/components/__init__.py
--rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.33a2/pynecone/components/base/__init__.py
--rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.33a2/pynecone/components/base/bare.py
--rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.33a2/pynecone/components/base/body.py
--rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.33a2/pynecone/components/base/document.py
--rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.33a2/pynecone/components/base/head.py
--rw-r--r--   0        0        0      930 2023-05-15 02:04:07.607989 pynecone-0.1.33a2/pynecone/components/base/link.py
--rw-r--r--   0        0        0     1340 2023-05-15 02:04:07.608303 pynecone-0.1.33a2/pynecone/components/base/meta.py
--rw-r--r--   0        0        0    24243 2023-06-01 00:32:59.072142 pynecone-0.1.33a2/pynecone/components/component.py
--rw-r--r--   0        0        0      496 2023-05-26 18:45:47.404646 pynecone-0.1.33a2/pynecone/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.33a2/pynecone/components/datadisplay/badge.py
--rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.33a2/pynecone/components/datadisplay/code.py
--rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.33a2/pynecone/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.33a2/pynecone/components/datadisplay/divider.py
--rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.33a2/pynecone/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.33a2/pynecone/components/datadisplay/list.py
--rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.33a2/pynecone/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5793 2023-05-26 18:45:47.405454 pynecone-0.1.33a2/pynecone/components/datadisplay/table.py
--rw-r--r--   0        0        0     2188 2023-05-26 18:45:47.406072 pynecone-0.1.33a2/pynecone/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-05-26 18:45:47.406587 pynecone-0.1.33a2/pynecone/components/disclosure/__init__.py
--rw-r--r--   0        0        0     2941 2023-05-15 02:04:07.609439 pynecone-0.1.33a2/pynecone/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.33a2/pynecone/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1741 2023-05-26 18:45:47.406922 pynecone-0.1.33a2/pynecone/components/disclosure/transition.py
--rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.33a2/pynecone/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.33a2/pynecone/components/feedback/__init__.py
--rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.33a2/pynecone/components/feedback/alert.py
--rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.33a2/pynecone/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.33a2/pynecone/components/feedback/progress.py
--rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.33a2/pynecone/components/feedback/skeleton.py
--rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.33a2/pynecone/components/feedback/spinner.py
--rw-r--r--   0        0        0     1308 2023-06-07 06:05:03.876023 pynecone-0.1.33a2/pynecone/components/forms/__init__.py
--rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.33a2/pynecone/components/forms/button.py
--rw-r--r--   0        0        0     2454 2023-05-18 00:14:14.760429 pynecone-0.1.33a2/pynecone/components/forms/checkbox.py
--rw-r--r--   0        0        0      578 2023-05-18 00:14:14.760629 pynecone-0.1.33a2/pynecone/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      243 2023-06-07 06:05:03.876332 pynecone-0.1.33a2/pynecone/components/forms/date_picker.py
--rw-r--r--   0        0        0      277 2023-06-07 06:05:03.876514 pynecone-0.1.33a2/pynecone/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.760816 pynecone-0.1.33a2/pynecone/components/forms/editable.py
--rw-r--r--   0        0        0      243 2023-06-01 00:48:48.431001 pynecone-0.1.33a2/pynecone/components/forms/email.py
--rw-r--r--   0        0        0     2996 2023-05-26 18:45:47.407573 pynecone-0.1.33a2/pynecone/components/forms/form.py
--rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.33a2/pynecone/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2880 2023-05-18 00:14:14.761287 pynecone-0.1.33a2/pynecone/components/forms/input.py
--rw-r--r--   0        0        0    12667 2023-06-07 06:05:03.876768 pynecone-0.1.33a2/pynecone/components/forms/multiselect.py
--rw-r--r--   0        0        0     3897 2023-05-18 00:14:14.761460 pynecone-0.1.33a2/pynecone/components/forms/numberinput.py
--rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.33a2/pynecone/components/forms/password.py
--rw-r--r--   0        0        0     2670 2023-05-18 00:14:14.761619 pynecone-0.1.33a2/pynecone/components/forms/pininput.py
--rw-r--r--   0        0        0     3043 2023-05-18 00:14:14.761823 pynecone-0.1.33a2/pynecone/components/forms/radio.py
--rw-r--r--   0        0        0     2853 2023-05-18 00:14:14.761962 pynecone-0.1.33a2/pynecone/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3522 2023-06-07 06:05:03.877157 pynecone-0.1.33a2/pynecone/components/forms/select.py
--rw-r--r--   0        0        0     3124 2023-05-18 00:14:14.762261 pynecone-0.1.33a2/pynecone/components/forms/slider.py
--rw-r--r--   0        0        0     1552 2023-05-18 00:14:14.762398 pynecone-0.1.33a2/pynecone/components/forms/switch.py
--rw-r--r--   0        0        0     1531 2023-05-18 00:14:14.762541 pynecone-0.1.33a2/pynecone/components/forms/textarea.py
--rw-r--r--   0        0        0     2915 2023-05-18 00:14:14.762683 pynecone-0.1.33a2/pynecone/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.33a2/pynecone/components/graphing/__init__.py
--rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.33a2/pynecone/components/graphing/plotly.py
--rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.33a2/pynecone/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-05-22 21:39:53.010163 pynecone-0.1.33a2/pynecone/components/layout/__init__.py
--rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.33a2/pynecone/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      769 2023-05-15 02:04:07.614311 pynecone-0.1.33a2/pynecone/components/layout/box.py
--rw-r--r--   0        0        0     2859 2023-05-22 21:39:53.010378 pynecone-0.1.33a2/pynecone/components/layout/card.py
--rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.33a2/pynecone/components/layout/center.py
--rw-r--r--   0        0        0     3844 2023-05-18 00:14:14.762938 pynecone-0.1.33a2/pynecone/components/layout/cond.py
--rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.33a2/pynecone/components/layout/container.py
--rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.33a2/pynecone/components/layout/flex.py
--rw-r--r--   0        0        0     3167 2023-05-26 18:45:47.408238 pynecone-0.1.33a2/pynecone/components/layout/foreach.py
--rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.33a2/pynecone/components/layout/fragment.py
--rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.33a2/pynecone/components/layout/grid.py
--rw-r--r--   0        0        0      979 2023-05-30 04:03:19.236282 pynecone-0.1.33a2/pynecone/components/layout/html.py
--rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.33a2/pynecone/components/layout/responsive.py
--rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.33a2/pynecone/components/layout/spacer.py
--rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.33a2/pynecone/components/layout/stack.py
--rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.33a2/pynecone/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.33a2/pynecone/components/libs/__init__.py
--rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.33a2/pynecone/components/libs/chakra.py
--rw-r--r--   0        0        0     1391 2023-06-01 03:15:26.564372 pynecone-0.1.33a2/pynecone/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-06-01 03:15:26.564561 pynecone-0.1.33a2/pynecone/components/media/__init__.py
--rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564687 pynecone-0.1.33a2/pynecone/components/media/audio.py
--rw-r--r--   0        0        0     1524 2023-05-18 00:14:14.763360 pynecone-0.1.33a2/pynecone/components/media/avatar.py
--rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.33a2/pynecone/components/media/icon.py
--rw-r--r--   0        0        0     1774 2023-06-01 03:15:26.564867 pynecone-0.1.33a2/pynecone/components/media/image.py
--rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564984 pynecone-0.1.33a2/pynecone/components/media/video.py
--rw-r--r--   0        0        0      450 2023-06-07 06:05:03.877519 pynecone-0.1.33a2/pynecone/components/navigation/__init__.py
--rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.33a2/pynecone/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0      746 2023-06-07 06:05:03.877899 pynecone-0.1.33a2/pynecone/components/navigation/link.py
--rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.33a2/pynecone/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.33a2/pynecone/components/navigation/nextlink.py
--rw-r--r--   0        0        0     2842 2023-06-07 06:05:03.878280 pynecone-0.1.33a2/pynecone/components/navigation/stepper.py
--rw-r--r--   0        0        0      887 2023-06-07 06:05:03.878625 pynecone-0.1.33a2/pynecone/components/overlay/__init__.py
--rw-r--r--   0        0        0     5027 2023-05-18 00:14:14.763711 pynecone-0.1.33a2/pynecone/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1016 2023-06-07 06:05:03.878806 pynecone-0.1.33a2/pynecone/components/overlay/banner.py
--rw-r--r--   0        0        0     4681 2023-05-18 00:14:14.763867 pynecone-0.1.33a2/pynecone/components/overlay/drawer.py
--rw-r--r--   0        0        0     5530 2023-05-18 00:14:14.764021 pynecone-0.1.33a2/pynecone/components/overlay/menu.py
--rw-r--r--   0        0        0     4917 2023-05-18 00:14:14.764177 pynecone-0.1.33a2/pynecone/components/overlay/modal.py
--rw-r--r--   0        0        0     5688 2023-06-07 04:31:19.747990 pynecone-0.1.33a2/pynecone/components/overlay/popover.py
--rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.764530 pynecone-0.1.33a2/pynecone/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.33a2/pynecone/components/tags/__init__.py
--rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.33a2/pynecone/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.33a2/pynecone/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5018 2023-05-18 00:14:14.764773 pynecone-0.1.33a2/pynecone/components/tags/tag.py
--rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.33a2/pynecone/components/tags/tagless.py
--rw-r--r--   0        0        0      304 2023-06-01 00:32:59.073257 pynecone-0.1.33a2/pynecone/components/typography/__init__.py
--rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.33a2/pynecone/components/typography/heading.py
--rw-r--r--   0        0        0      682 2023-06-01 00:32:59.073664 pynecone-0.1.33a2/pynecone/components/typography/highlight.py
--rw-r--r--   0        0        0     3460 2023-06-07 06:05:03.879093 pynecone-0.1.33a2/pynecone/components/typography/markdown.py
--rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.33a2/pynecone/components/typography/span.py
--rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.33a2/pynecone/components/typography/text.py
--rw-r--r--   0        0        0     7021 2023-06-07 06:05:03.879346 pynecone-0.1.33a2/pynecone/config.py
--rw-r--r--   0        0        0    10219 2023-06-07 06:21:32.941182 pynecone-0.1.33a2/pynecone/constants.py
--rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.33a2/pynecone/el/__init__.py
--rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.33a2/pynecone/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.33a2/pynecone/el/constants/html.py
--rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.33a2/pynecone/el/constants/pynecone.py
--rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.33a2/pynecone/el/constants/react.py
--rw-r--r--   0        0        0     1320 2023-06-07 06:05:03.879903 pynecone-0.1.33a2/pynecone/el/element.py
--rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.33a2/pynecone/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.33a2/pynecone/el/precompile.py
--rw-r--r--   0        0        0    10977 2023-06-07 06:05:03.880324 pynecone-0.1.33a2/pynecone/event.py
--rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.33a2/pynecone/middleware/__init__.py
--rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.33a2/pynecone/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.33a2/pynecone/middleware/middleware.py
--rw-r--r--   0        0        0     2581 2023-06-07 06:05:03.880790 pynecone-0.1.33a2/pynecone/model.py
--rw-r--r--   0        0        0     8515 2023-06-07 06:05:03.881000 pynecone-0.1.33a2/pynecone/pc.py
--rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.33a2/pynecone/py.typed
--rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.33a2/pynecone/route.py
--rw-r--r--   0        0        0    30945 2023-06-07 06:21:32.941558 pynecone-0.1.33a2/pynecone/state.py
--rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.33a2/pynecone/style.py
--rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.33a2/pynecone/utils/__init__.py
--rw-r--r--   0        0        0     7394 2023-06-07 06:21:13.591977 pynecone-0.1.33a2/pynecone/utils/build.py
--rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.33a2/pynecone/utils/console.py
--rw-r--r--   0        0        0     5229 2023-06-01 03:12:42.959181 pynecone-0.1.33a2/pynecone/utils/exec.py
--rw-r--r--   0        0        0    11859 2023-06-01 03:15:26.565621 pynecone-0.1.33a2/pynecone/utils/format.py
--rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.33a2/pynecone/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.33a2/pynecone/utils/path_ops.py
--rw-r--r--   0        0        0    11355 2023-06-07 06:05:03.882688 pynecone-0.1.33a2/pynecone/utils/prerequisites.py
--rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.33a2/pynecone/utils/processes.py
--rw-r--r--   0        0        0     2397 2023-05-15 02:04:07.623496 pynecone-0.1.33a2/pynecone/utils/telemetry.py
--rw-r--r--   0        0        0     4806 2023-06-01 03:15:26.565774 pynecone-0.1.33a2/pynecone/utils/types.py
--rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.33a2/pynecone/utils/watch.py
--rw-r--r--   0        0        0    30928 2023-05-18 00:14:14.766310 pynecone-0.1.33a2/pynecone/vars.py
--rw-r--r--   0        0        0     1852 2023-06-07 06:37:30.531853 pynecone-0.1.33a2/pyproject.toml
--rw-r--r--   0        0        0     9511 1970-01-01 00:00:00.000000 pynecone-0.1.33a2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.33a3/LICENSE
+-rw-r--r--   0        0        0     7876 2023-05-18 00:14:14.758659 pynecone-0.1.33a3/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.33a3/pynecone/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1340 2023-06-07 06:32:06.269060 pynecone-0.1.33a3/pynecone/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.33a3/pynecone/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.33a3/pynecone/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.33a3/pynecone/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.33a3/pynecone/.templates/jinja/app/pcconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.33a3/pynecone/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-05-18 18:33:16.414872 pynecone-0.1.33a3/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.33a3/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3312 2023-06-09 19:48:33.040538 pynecone-0.1.33a3/pynecone/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-05-22 21:40:04.765805 pynecone-0.1.33a3/pynecone/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.33a3/pynecone/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.33a3/pynecone/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   257247 2023-05-26 18:45:47.401731 pynecone-0.1.33a3/pynecone/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-05-26 18:45:47.402096 pynecone-0.1.33a3/pynecone/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.33a3/pynecone/.templates/web/next.config.js
+-rw-r--r--   0        0        0      995 2023-06-01 03:15:26.563786 pynecone-0.1.33a3/pynecone/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.33a3/pynecone/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.33a3/pynecone/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.33a3/pynecone/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0     8450 2023-06-09 19:48:33.040820 pynecone-0.1.33a3/pynecone/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1490 2023-06-07 06:05:03.874348 pynecone-0.1.33a3/pynecone/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-07 06:05:03.874470 pynecone-0.1.33a3/pynecone/admin.py
+-rw-r--r--   0        0        0    21426 2023-06-09 19:48:39.955078 pynecone-0.1.33a3/pynecone/app.py
+-rw-r--r--   0        0        0     2548 2023-06-07 19:04:43.443201 pynecone-0.1.33a3/pynecone/base.py
+-rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.33a3/pynecone/compiler/__init__.py
+-rw-r--r--   0        0        0     6689 2023-06-09 19:48:33.041803 pynecone-0.1.33a3/pynecone/compiler/compiler.py
+-rw-r--r--   0        0        0     2642 2023-06-09 19:48:33.042227 pynecone-0.1.33a3/pynecone/compiler/templates.py
+-rw-r--r--   0        0        0     7767 2023-06-09 19:48:39.955794 pynecone-0.1.33a3/pynecone/compiler/utils.py
+-rw-r--r--   0        0        0     7346 2023-06-07 06:05:03.875765 pynecone-0.1.33a3/pynecone/components/__init__.py
+-rw-r--r--   0        0        0      229 2023-06-09 19:48:39.957002 pynecone-0.1.33a3/pynecone/components/base/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.33a3/pynecone/components/base/bare.py
+-rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.33a3/pynecone/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.33a3/pynecone/components/base/document.py
+-rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.33a3/pynecone/components/base/head.py
+-rw-r--r--   0        0        0      933 2023-06-09 19:48:39.957851 pynecone-0.1.33a3/pynecone/components/base/link.py
+-rw-r--r--   0        0        0     1412 2023-06-07 19:04:43.443671 pynecone-0.1.33a3/pynecone/components/base/meta.py
+-rw-r--r--   0        0        0    24243 2023-06-01 00:32:59.072142 pynecone-0.1.33a3/pynecone/components/component.py
+-rw-r--r--   0        0        0      496 2023-05-26 18:45:47.404646 pynecone-0.1.33a3/pynecone/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.33a3/pynecone/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.33a3/pynecone/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.33a3/pynecone/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.33a3/pynecone/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.33a3/pynecone/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.33a3/pynecone/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.33a3/pynecone/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5793 2023-05-26 18:45:47.405454 pynecone-0.1.33a3/pynecone/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2188 2023-05-26 18:45:47.406072 pynecone-0.1.33a3/pynecone/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-05-26 18:45:47.406587 pynecone-0.1.33a3/pynecone/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3517 2023-06-09 19:48:39.958158 pynecone-0.1.33a3/pynecone/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.33a3/pynecone/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1741 2023-05-26 18:45:47.406922 pynecone-0.1.33a3/pynecone/components/disclosure/transition.py
+-rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.33a3/pynecone/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.33a3/pynecone/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.33a3/pynecone/components/feedback/alert.py
+-rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.33a3/pynecone/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.33a3/pynecone/components/feedback/progress.py
+-rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.33a3/pynecone/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.33a3/pynecone/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1308 2023-06-07 06:05:03.876023 pynecone-0.1.33a3/pynecone/components/forms/__init__.py
+-rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.33a3/pynecone/components/forms/button.py
+-rw-r--r--   0        0        0     2454 2023-05-18 00:14:14.760429 pynecone-0.1.33a3/pynecone/components/forms/checkbox.py
+-rw-r--r--   0        0        0      578 2023-05-18 00:14:14.760629 pynecone-0.1.33a3/pynecone/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      243 2023-06-07 06:05:03.876332 pynecone-0.1.33a3/pynecone/components/forms/date_picker.py
+-rw-r--r--   0        0        0      277 2023-06-07 06:05:03.876514 pynecone-0.1.33a3/pynecone/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.760816 pynecone-0.1.33a3/pynecone/components/forms/editable.py
+-rw-r--r--   0        0        0      243 2023-06-01 00:48:48.431001 pynecone-0.1.33a3/pynecone/components/forms/email.py
+-rw-r--r--   0        0        0     2996 2023-05-26 18:45:47.407573 pynecone-0.1.33a3/pynecone/components/forms/form.py
+-rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.33a3/pynecone/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     2880 2023-06-09 18:42:18.512736 pynecone-0.1.33a3/pynecone/components/forms/input.py
+-rw-r--r--   0        0        0    12667 2023-06-07 06:05:03.876768 pynecone-0.1.33a3/pynecone/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3897 2023-05-18 00:14:14.761460 pynecone-0.1.33a3/pynecone/components/forms/numberinput.py
+-rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.33a3/pynecone/components/forms/password.py
+-rw-r--r--   0        0        0     2670 2023-05-18 00:14:14.761619 pynecone-0.1.33a3/pynecone/components/forms/pininput.py
+-rw-r--r--   0        0        0     3043 2023-05-18 00:14:14.761823 pynecone-0.1.33a3/pynecone/components/forms/radio.py
+-rw-r--r--   0        0        0     2853 2023-05-18 00:14:14.761962 pynecone-0.1.33a3/pynecone/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3522 2023-06-07 06:05:03.877157 pynecone-0.1.33a3/pynecone/components/forms/select.py
+-rw-r--r--   0        0        0     3124 2023-05-18 00:14:14.762261 pynecone-0.1.33a3/pynecone/components/forms/slider.py
+-rw-r--r--   0        0        0     1573 2023-06-09 19:48:39.959122 pynecone-0.1.33a3/pynecone/components/forms/switch.py
+-rw-r--r--   0        0        0     1532 2023-06-09 19:48:39.959281 pynecone-0.1.33a3/pynecone/components/forms/textarea.py
+-rw-r--r--   0        0        0     2915 2023-05-18 00:14:14.762683 pynecone-0.1.33a3/pynecone/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.33a3/pynecone/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.33a3/pynecone/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.33a3/pynecone/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-05-22 21:39:53.010163 pynecone-0.1.33a3/pynecone/components/layout/__init__.py
+-rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.33a3/pynecone/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      766 2023-06-09 19:48:39.959611 pynecone-0.1.33a3/pynecone/components/layout/box.py
+-rw-r--r--   0        0        0     2859 2023-05-22 21:39:53.010378 pynecone-0.1.33a3/pynecone/components/layout/card.py
+-rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.33a3/pynecone/components/layout/center.py
+-rw-r--r--   0        0        0     3844 2023-05-18 00:14:14.762938 pynecone-0.1.33a3/pynecone/components/layout/cond.py
+-rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.33a3/pynecone/components/layout/container.py
+-rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.33a3/pynecone/components/layout/flex.py
+-rw-r--r--   0        0        0     3167 2023-05-26 18:45:47.408238 pynecone-0.1.33a3/pynecone/components/layout/foreach.py
+-rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.33a3/pynecone/components/layout/fragment.py
+-rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.33a3/pynecone/components/layout/grid.py
+-rw-r--r--   0        0        0      979 2023-05-30 04:03:19.236282 pynecone-0.1.33a3/pynecone/components/layout/html.py
+-rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.33a3/pynecone/components/layout/responsive.py
+-rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.33a3/pynecone/components/layout/spacer.py
+-rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.33a3/pynecone/components/layout/stack.py
+-rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.33a3/pynecone/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.33a3/pynecone/components/libs/__init__.py
+-rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.33a3/pynecone/components/libs/chakra.py
+-rw-r--r--   0        0        0     1391 2023-06-01 03:15:26.564372 pynecone-0.1.33a3/pynecone/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-06-01 03:15:26.564561 pynecone-0.1.33a3/pynecone/components/media/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564687 pynecone-0.1.33a3/pynecone/components/media/audio.py
+-rw-r--r--   0        0        0     1524 2023-05-18 00:14:14.763360 pynecone-0.1.33a3/pynecone/components/media/avatar.py
+-rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.33a3/pynecone/components/media/icon.py
+-rw-r--r--   0        0        0     1774 2023-06-01 03:15:26.564867 pynecone-0.1.33a3/pynecone/components/media/image.py
+-rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564984 pynecone-0.1.33a3/pynecone/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-06-07 06:05:03.877519 pynecone-0.1.33a3/pynecone/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.33a3/pynecone/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1844 2023-06-09 19:48:39.960619 pynecone-0.1.33a3/pynecone/components/navigation/link.py
+-rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.33a3/pynecone/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.33a3/pynecone/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2842 2023-06-07 06:05:03.878280 pynecone-0.1.33a3/pynecone/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-06-07 06:05:03.878625 pynecone-0.1.33a3/pynecone/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5027 2023-05-18 00:14:14.763711 pynecone-0.1.33a3/pynecone/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1016 2023-06-07 06:05:03.878806 pynecone-0.1.33a3/pynecone/components/overlay/banner.py
+-rw-r--r--   0        0        0     4681 2023-05-18 00:14:14.763867 pynecone-0.1.33a3/pynecone/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5530 2023-05-18 00:14:14.764021 pynecone-0.1.33a3/pynecone/components/overlay/menu.py
+-rw-r--r--   0        0        0     4917 2023-05-18 00:14:14.764177 pynecone-0.1.33a3/pynecone/components/overlay/modal.py
+-rw-r--r--   0        0        0     5688 2023-06-07 04:31:19.747990 pynecone-0.1.33a3/pynecone/components/overlay/popover.py
+-rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.764530 pynecone-0.1.33a3/pynecone/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.33a3/pynecone/components/tags/__init__.py
+-rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.33a3/pynecone/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.33a3/pynecone/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5018 2023-06-09 19:48:33.042551 pynecone-0.1.33a3/pynecone/components/tags/tag.py
+-rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.33a3/pynecone/components/tags/tagless.py
+-rw-r--r--   0        0        0      304 2023-06-01 00:32:59.073257 pynecone-0.1.33a3/pynecone/components/typography/__init__.py
+-rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.33a3/pynecone/components/typography/heading.py
+-rw-r--r--   0        0        0      682 2023-06-01 00:32:59.073664 pynecone-0.1.33a3/pynecone/components/typography/highlight.py
+-rw-r--r--   0        0        0     3460 2023-06-07 06:05:03.879093 pynecone-0.1.33a3/pynecone/components/typography/markdown.py
+-rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.33a3/pynecone/components/typography/span.py
+-rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.33a3/pynecone/components/typography/text.py
+-rw-r--r--   0        0        0     6960 2023-06-09 19:48:39.960810 pynecone-0.1.33a3/pynecone/config.py
+-rw-r--r--   0        0        0    10219 2023-06-09 19:48:33.049660 pynecone-0.1.33a3/pynecone/constants.py
+-rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.33a3/pynecone/el/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.33a3/pynecone/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.33a3/pynecone/el/constants/html.py
+-rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.33a3/pynecone/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.33a3/pynecone/el/constants/react.py
+-rw-r--r--   0        0        0     1320 2023-06-07 06:05:03.879903 pynecone-0.1.33a3/pynecone/el/element.py
+-rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.33a3/pynecone/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.33a3/pynecone/el/precompile.py
+-rw-r--r--   0        0        0    10977 2023-06-07 06:05:03.880324 pynecone-0.1.33a3/pynecone/event.py
+-rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.33a3/pynecone/middleware/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.33a3/pynecone/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.33a3/pynecone/middleware/middleware.py
+-rw-r--r--   0        0        0     2388 2023-06-09 19:48:39.961091 pynecone-0.1.33a3/pynecone/model.py
+-rw-r--r--   0        0        0     8575 2023-06-07 19:04:43.444311 pynecone-0.1.33a3/pynecone/pc.py
+-rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.33a3/pynecone/py.typed
+-rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.33a3/pynecone/route.py
+-rw-r--r--   0        0        0    30945 2023-06-09 19:48:33.050053 pynecone-0.1.33a3/pynecone/state.py
+-rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.33a3/pynecone/style.py
+-rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.33a3/pynecone/utils/__init__.py
+-rw-r--r--   0        0        0     7394 2023-06-09 19:48:33.050640 pynecone-0.1.33a3/pynecone/utils/build.py
+-rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.33a3/pynecone/utils/console.py
+-rw-r--r--   0        0        0     5317 2023-06-07 19:04:43.444774 pynecone-0.1.33a3/pynecone/utils/exec.py
+-rw-r--r--   0        0        0    11859 2023-06-09 19:48:33.051324 pynecone-0.1.33a3/pynecone/utils/format.py
+-rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.33a3/pynecone/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.33a3/pynecone/utils/path_ops.py
+-rw-r--r--   0        0        0    10873 2023-06-09 19:48:39.961277 pynecone-0.1.33a3/pynecone/utils/prerequisites.py
+-rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.33a3/pynecone/utils/processes.py
+-rw-r--r--   0        0        0     2397 2023-06-09 19:48:33.052076 pynecone-0.1.33a3/pynecone/utils/telemetry.py
+-rw-r--r--   0        0        0     4806 2023-06-01 03:15:26.565774 pynecone-0.1.33a3/pynecone/utils/types.py
+-rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.33a3/pynecone/utils/watch.py
+-rw-r--r--   0        0        0    30928 2023-06-09 19:48:33.052425 pynecone-0.1.33a3/pynecone/vars.py
+-rw-r--r--   0        0        0     1874 2023-06-09 19:48:53.289852 pynecone-0.1.33a3/pyproject.toml
+-rw-r--r--   0        0        0     9511 1970-01-01 00:00:00.000000 pynecone-0.1.33a3/PKG-INFO
```

### Comparing `pynecone-0.1.33a2/LICENSE` & `pynecone-0.1.33a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/README.md` & `pynecone-0.1.33a3/README.md`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/.templates/apps/counter/counter.py` & `pynecone-0.1.33a3/pynecone/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/.templates/apps/default/default.py` & `pynecone-0.1.33a3/pynecone/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/.templates/assets/favicon.ico` & `pynecone-0.1.33a3/pynecone/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/.templates/jinja/web/pages/index.js.jinja2` & `pynecone-0.1.33a3/pynecone/.templates/jinja/web/pages/index.js.jinja2`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,87 @@
 {% extends "web/pages/base_page.js.jinja2" %}
 
 {% block declaration %}
 {% for custom_code in custom_codes %}
 {{custom_code}}
 {% endfor %}
-
 {% endblock %}
 
 {% block export %}
 export default function Component() {
   const [{{state_name}}, {{state_name|react_setter}}] = useState({{initial_state|json_dumps}})
   const [{{const.result}}, {{const.result|react_setter}}] = useState({{const.initial_result|json_dumps}})
   const [notConnected, setNotConnected] = useState(false)
   const {{const.router}} = useRouter()
   const {{const.socket}} = useRef(null)
   const { isReady } = {{const.router}}
   const { {{const.color_mode}}, {{const.toggle_color_mode}} } = {{const.use_color_mode}}()
   const focusRef = useRef();
   
+  // Function to add new events to the event queue.
   const Event = (events, _e) => {
       preventDefault(_e);
-      {{state_name|react_setter}}({
-        ...{{state_name}},
-        events: [...{{state_name}}.events, ...events],
-      })
+      {{state_name|react_setter}}(state => ({
+        ...state,
+        events: [...state.events, ...events],
+      }))
   }
 
-  const File = files => {{state_name|react_setter}}({
-    ...{{state_name}},
+  // Function to add new files to be uploaded.
+  const File = files => {{state_name|react_setter}}(state => ({
+    ...state,
     files,
-  })
+  }))
 
-  useEffect(()=>{
-    if(!isReady) {
+  // Main event loop.
+  useEffect(()=> {
+    // Skip if the router is not ready.
+    if (!isReady) {
       return;
     }
+
+    // Initialize the websocket connection.
     if (!{{const.socket}}.current) {
       connect({{const.socket}}, {{state_name}}, {{state_name|react_setter}}, {{const.result}}, {{const.result|react_setter}}, {{const.router}}, {{transports}}, setNotConnected)
     }
-    const update = async () => {
-      if ({{const.result}}.{{const.state}} != null){
-        {{state_name|react_setter}}({
-          ...{{const.result}}.{{const.state}},
-          events: [...{{state_name}}.{{const.events}}, ...{{const.result}}.{{const.events}}],
-        })
-
-        {{const.result|react_setter}}({
-          {{const.state}}: null,
-          {{const.events}}: [],
-          {{const.processing}}: !{{const.result}}.{{const.final}},
-        })
-      }
 
-      await updateState({{state_name}}, {{state_name|react_setter}}, {{const.result}}, {{const.result|react_setter}}, {{const.router}}, {{const.socket}}.current)
+    // If we are not processing an event, process the next event.
+    if (!{{const.result}}.{{const.processing}}) {
+      processEvent({{state_name}}, {{state_name|react_setter}}, {{const.result}}, {{const.result|react_setter}}, {{const.router}}, {{const.socket}}.current)
+    }
+
+    // If there is a new result, update the state.
+    if ({{const.result}}.{{const.state}} != null) {
+      // Apply the new result to the state and the new events to the queue.
+      {{state_name|react_setter}}(state => ({
+        ...{{const.result}}.{{const.state}},
+        events: [...state.{{const.events}}, ...{{const.result}}.{{const.events}}],
+      }))
+
+      // Reset the result.
+      {{const.result|react_setter}}(result => ({
+        {{const.state}}: null,
+        {{const.events}}: [],
+        {{const.final}}: true,
+        {{const.processing}}: !{{const.result}}.{{const.final}},
+      }))
+
+      // Process the next event.
+      processEvent({{state_name}}, {{state_name|react_setter}}, {{const.result}}, {{const.result|react_setter}}, {{const.router}}, {{const.socket}}.current)
     }
-    if (focusRef.current)
+  })
+
+  // Set focus to the specified element.
+  useEffect(() => {
+    if (focusRef.current) {
       focusRef.current.focus();
-    update()
+    }
   })
+
+  // Route after the initial page hydration.
   useEffect(() => {
     const change_complete = () => Event([E('{{state_name}}.{{const.hydrate}}', {})])
     {{const.router}}.events.on('routeChangeComplete', change_complete)
     return () => {
       {{const.router}}.events.off('routeChangeComplete', change_complete)
     }
   }, [{{const.router}}])
```

### Comparing `pynecone-0.1.33a2/pynecone/.templates/jinja/web/pages/utils.js.jinja2` & `pynecone-0.1.33a3/pynecone/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/.templates/web/bun.lockb` & `pynecone-0.1.33a3/pynecone/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/.templates/web/package.json` & `pynecone-0.1.33a3/pynecone/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/.templates/web/pages/_app.js` & `pynecone-0.1.33a3/pynecone/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/.templates/web/styles/code/prism.js` & `pynecone-0.1.33a3/pynecone/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/.templates/web/utils/state.js` & `pynecone-0.1.33a3/pynecone/.templates/web/utils/state.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -131,40 +131,35 @@
 };
 
 /**
  * Process an event off the event queue.
  * @param event The current event
  * @param state The state with the event queue.
  * @param setResult The function to set the result.
+ *
+ * @returns Whether the event was sent.
  */
 export const applyRestEvent = async (event, state, setResult) => {
     let eventSent = false;
     if (event.handler == "uploadFiles") {
         eventSent = await uploadFiles(state, setResult, event.name);
     }
-    if (!eventSent) {
-        // If no event was sent, set processing to false and return.
-        setResult({
-            ...state,
-            final: true,
-            processing: false
-        });
-    }
+    return eventSent;
 };
 
 /**
  * Process an event off the event queue.
  * @param state The state with the event queue.
  * @param setState The function to set the state.
  * @param result The current result.
  * @param setResult The function to set the result.
  * @param router The router object.
  * @param socket The socket object to send the event on.
  */
-export const updateState = async (
+export const processEvent = async (
     state,
     setState,
     result,
     setResult,
     router,
     socket
 ) => {
@@ -175,35 +170,38 @@
 
     // Set processing to true to block other events from being processed.
     setResult({
         ...result,
         processing: true
     });
 
-    // Pop the next event off the queue and apply it.
-    const event = state.events.shift();
+    // Apply the next event in the queue.
+    const event = state.events[0];
+
     // Set new events to avoid reprocessing the same event.
-    setState({
+    setState(state => ({
         ...state,
-        events: state.events
-    });
+        events: state.events.slice(1)
+    }));
 
     // Process events with handlers via REST and all others via websockets.
+    let eventSent = false;
     if (event.handler) {
-        await applyRestEvent(event, state, setResult);
+        eventSent = await applyRestEvent(event, state, setResult);
     } else {
-        const eventSent = await applyEvent(event, router, socket);
-        if (!eventSent) {
-            // If no event was sent, set processing to false and return.
-            setResult({
-                ...state,
-                final: true,
-                processing: false
-            });
-        }
+        eventSent = await applyEvent(event, router, socket);
+    }
+
+    // If no event was sent, set processing to false.
+    if (!eventSent) {
+        setResult({
+            ...state,
+            final: true,
+            processing: false
+        });
     }
 };
 
 /**
  * Connect to a websocket and set the handlers.
  * @param socket The socket object to connect.
  * @param state The state object to apply the deltas to.
@@ -230,24 +228,24 @@
         path: endpoint["pathname"],
         transports: transports,
         autoUnref: false,
     });
 
     // Once the socket is open, hydrate the page.
     socket.current.on("connect", () => {
-        updateState(state, setState, result, setResult, router, socket.current);
+        processEvent(state, setState, result, setResult, router, socket.current);
         setNotConnected(false)
     });
 
     socket.current.on('connect_error', (error) => {
         setNotConnected(true)
     });
 
     // On each received message, apply the delta and set the result.
-    socket.current.on("event", function(update) {
+    socket.current.on("event", update => {
         update = JSON5.parse(update);
         applyDelta(state, update.delta);
         setResult({
             state: state,
             events: update.events,
             final: update.final,
             processing: true,
@@ -258,14 +256,16 @@
 /**
  * Upload files to the server.
  *
  * @param state The state to apply the delta to.
  * @param setResult The function to set the result.
  * @param handler The handler to use.
  * @param endpoint The endpoint to upload to.
+ *
+ * @returns Whether the files were uploaded.
  */
 export const uploadFiles = async (state, setResult, handler) => {
     const files = state.files;
 
     // return if there's no file to upload
     if (files.length == 0) {
         return false;
```

### Comparing `pynecone-0.1.33a2/pynecone/__init__.py` & `pynecone-0.1.33a3/pynecone/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/app.py` & `pynecone-0.1.33a3/pynecone/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 
 from pynecone import constants
 from pynecone.admin import AdminDash
 from pynecone.base import Base
 from pynecone.compiler import compiler
 from pynecone.compiler import utils as compiler_utils
 from pynecone.components.component import Component, ComponentStyle
+from pynecone.components.layout.fragment import Fragment
 from pynecone.config import get_config
-from pynecone.event import Event, EventHandler
+from pynecone.event import Event, EventHandler, EventSpec
 from pynecone.middleware import HydrateMiddleware, Middleware
 from pynecone.model import Model
 from pynecone.route import (
     DECORATED_ROUTES,
     catchall_in_route,
     catchall_prefix,
     get_route_args,
@@ -73,15 +74,15 @@
     # The styling to apply to each component.
     style: ComponentStyle = {}
 
     # Middleware to add to the app.
     middleware: List[Middleware] = []
 
     # List of event handlers to trigger when a page loads.
-    load_events: Dict[str, List[EventHandler]] = {}
+    load_events: Dict[str, List[Union[EventHandler, EventSpec]]] = {}
 
     # Admin dashboard
     admin_dash: Optional[AdminDash] = None
 
     # The component to render if there is a connection error to the server.
     connect_error_component: Optional[Component] = None
 
@@ -237,15 +238,17 @@
     def add_page(
         self,
         component: Union[Component, ComponentCallable],
         route: Optional[str] = None,
         title: str = constants.DEFAULT_TITLE,
         description: str = constants.DEFAULT_DESCRIPTION,
         image=constants.DEFAULT_IMAGE,
-        on_load: Optional[Union[EventHandler, List[EventHandler]]] = None,
+        on_load: Optional[
+            Union[EventHandler, EventSpec, List[Union[EventHandler, EventSpec]]]
+        ] = None,
         meta: List[Dict] = constants.DEFAULT_META_LIST,
         script_tags: Optional[List[Component]] = None,
     ):
         """Add a page to the app.
 
         If the component is a callable, by default the route is the name of the
         function. Otherwise, a route must be provided.
@@ -285,17 +288,24 @@
                 raise TypeError(
                     "You may be trying to use an invalid Python function on a state var. "
                     "When referencing a var inside your render code, only limited var operations are supported. "
                     "See the var operation docs here: https://pynecone.io/docs/state/vars "
                 ) from e
             raise e
 
+        # Wrap the component in a fragment.
+        component = Fragment.create(component)
+
         # Add meta information to the component.
         compiler_utils.add_meta(
-            component, title=title, image=image, description=description, meta=meta
+            component,
+            title=title,
+            image=image,
+            description=description,
+            meta=meta,
         )
 
         # Add script tags if given
         if script_tags:
             component.children.extend(script_tags)
 
         # Format the route.
@@ -307,15 +317,15 @@
 
         # Add the load events.
         if on_load:
             if not isinstance(on_load, list):
                 on_load = [on_load]
             self.load_events[route] = on_load
 
-    def get_load_events(self, route: str) -> List[EventHandler]:
+    def get_load_events(self, route: str) -> List[Union[EventHandler, EventSpec]]:
         """Get the load events for a route.
 
         Args:
             route: The route to get the load events for.
 
         Returns:
             The load events for the route.
@@ -381,15 +391,19 @@
         title = title or constants.TITLE_404
         image = image or constants.FAVICON_404
         description = description or constants.DESCRIPTION_404
 
         component = component if isinstance(component, Component) else component()
 
         compiler_utils.add_meta(
-            component, title=title, image=image, description=description, meta=meta
+            component,
+            title=title,
+            image=image,
+            description=description,
+            meta=meta,
         )
 
         froute = format.format_route
         if (froute(constants.ROOT_404) not in self.pages) and (
             not any(page.startswith("[[...") for page in self.pages)
         ):
             self.pages[froute(constants.ROOT_404)] = component
@@ -398,15 +412,15 @@
         ):
             self.pages[froute(constants.SLUG_404)] = component
 
     def setup_admin_dash(self):
         """Setup the admin dash."""
         # Get the config.
         config = get_config()
-        if config.enable_admin and config.admin_dash and config.admin_dash.models:
+        if config.admin_dash and config.admin_dash.models:
             # Build the admin dashboard
             admin = (
                 config.admin_dash.admin
                 if config.admin_dash.admin
                 else Admin(
                     engine=Model.get_db_engine(),
                     title="Pynecone Admin Dashboard",
```

### Comparing `pynecone-0.1.33a2/pynecone/base.py` & `pynecone-0.1.33a3/pynecone/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     """
 
     class Config:
         """Pydantic config."""
 
         arbitrary_types_allowed = True
         use_enum_values = True
+        extra = "allow"
 
     def json(self) -> str:
         """Convert the object to a json string.
 
         Returns:
             The object as a json string.
         """
```

### Comparing `pynecone-0.1.33a2/pynecone/compiler/compiler.py` & `pynecone-0.1.33a3/pynecone/compiler/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         ImportVar(tag="useEffect"),
         ImportVar(tag="useRef"),
         ImportVar(tag="useState"),
     },
     "next/router": {ImportVar(tag="useRouter")},
     f"/{constants.STATE_PATH}": {
         ImportVar(tag="connect"),
-        ImportVar(tag="updateState"),
+        ImportVar(tag="processEvent"),
         ImportVar(tag="uploadFiles"),
         ImportVar(tag="E"),
         ImportVar(tag="isTrue"),
         ImportVar(tag="preventDefault"),
         ImportVar(tag="refs"),
         ImportVar(tag="getRefValue"),
     },
```

### Comparing `pynecone-0.1.33a2/pynecone/compiler/templates.py` & `pynecone-0.1.33a3/pynecone/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/compiler/utils.py` & `pynecone-0.1.33a3/pynecone/compiler/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     Body,
     ColorModeScript,
     Description,
     DocumentHead,
     Head,
     Html,
     Image,
-    Link,
     Main,
     Meta,
+    RawLink,
     Script,
     Title,
 )
 from pynecone.components.component import Component, CustomComponent
 from pynecone.event import get_hydrate_event
 from pynecone.state import State
 from pynecone.style import Style
@@ -151,15 +151,15 @@
 
     Args:
         stylesheets: The list of stylesheets to include in the document root.
 
     Returns:
         The document root.
     """
-    sheets = [Link.create(rel="stylesheet", href=href) for href in stylesheets]
+    sheets = [RawLink.create(rel="stylesheet", href=href) for href in stylesheets]
     return Html.create(
         DocumentHead.create(*sheets),
         Body.create(
             ColorModeScript.create(),
             Main.create(),
             Script.create(),
         ),
```

### Comparing `pynecone-0.1.33a2/pynecone/components/__init__.py` & `pynecone-0.1.33a3/pynecone/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/base/bare.py` & `pynecone-0.1.33a3/pynecone/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/base/document.py` & `pynecone-0.1.33a3/pynecone/components/base/document.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/base/link.py` & `pynecone-0.1.33a3/pynecone/components/base/link.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Display the title of the current page."""
 
 
 from pynecone.components.component import Component
 from pynecone.vars import Var
 
 
-class Link(Component):
+class RawLink(Component):
     """A component that displays the title of the current page."""
 
     tag = "link"
 
     # The href.
     href: Var[str]
```

### Comparing `pynecone-0.1.33a2/pynecone/components/base/meta.py` & `pynecone-0.1.33a3/pynecone/components/base/meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
     # The name of metadata.
     name: Optional[str] = None
 
     # The type of metadata value.
     property: Optional[str] = None
 
+    # The type of metadata value.
+    http_equiv: Optional[str] = None
+
 
 class Description(Meta):
     """A component that displays the title of the current page."""
 
     # The type of the description.
     name: str = "description"
```

### Comparing `pynecone-0.1.33a2/pynecone/components/component.py` & `pynecone-0.1.33a3/pynecone/components/component.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/datadisplay/code.py` & `pynecone-0.1.33a3/pynecone/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/datadisplay/datatable.py` & `pynecone-0.1.33a3/pynecone/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/datadisplay/divider.py` & `pynecone-0.1.33a3/pynecone/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/datadisplay/list.py` & `pynecone-0.1.33a3/pynecone/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/datadisplay/stat.py` & `pynecone-0.1.33a3/pynecone/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/datadisplay/table.py` & `pynecone-0.1.33a3/pynecone/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/datadisplay/tag.py` & `pynecone-0.1.33a3/pynecone/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/disclosure/accordion.py` & `pynecone-0.1.33a3/pynecone/components/disclosure/accordion.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,33 +12,43 @@
 
     tag = "Accordion"
 
     # If true, multiple accordion items can be expanded at once.
     allow_multiple: Var[bool]
 
     # If true, any expanded accordion item can be collapsed again.
-    allow_toggle: Var[bool] = True  # type: ignore
+    allow_toggle: Var[bool]
 
     # The initial index(es) of the expanded accordion item(s).
     default_index: Var[Optional[List[int]]]
 
     # The index(es) of the expanded accordion item
     index: Var[Union[int, List[int]]]
 
     # If true, height animation and transitions will be disabled.
     reduce_motion: Var[bool]
 
     @classmethod
-    def create(cls, *children, items=None, icon_pos="right", **props) -> Component:
+    def create(
+        cls,
+        *children,
+        items=None,
+        icon_pos="right",
+        allow_multiple: Optional[Var[bool]] = None,
+        allow_toggle: Optional[Var[bool]] = None,
+        **props
+    ) -> Component:
         """Create an accordion component.
 
         Args:
             children: The children of the component.
             items: The items of the accordion component: list of tuples (label,panel)
             icon_pos: The position of the arrow icon of the accordion. "right", "left" or None
+            allow_multiple: The allow_multiple property of the accordion. (True or False)
+            allow_toggle: The allow_toggle property of the accordion. (True or False)
             props: The properties of the component.
 
         Returns:
             The accordion component
         """
         if len(children) == 0:
             children = []
@@ -54,14 +64,20 @@
 
                 children.append(
                     AccordionItem.create(
                         button,
                         AccordionPanel.create(panel),
                     )
                 )
+
+        # if allow_multiple is True, allow_toggle is implicitely used and does not need to be defined
+        if allow_multiple:
+            props.update({"allow_multiple": allow_multiple})
+        elif allow_toggle:
+            props.update({"allow_toggle": allow_toggle})
         return super().create(*children, **props)
 
 
 class AccordionItem(ChakraComponent):
     """A single accordion item."""
 
     tag = "AccordionItem"
```

### Comparing `pynecone-0.1.33a2/pynecone/components/disclosure/tabs.py` & `pynecone-0.1.33a3/pynecone/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/disclosure/transition.py` & `pynecone-0.1.33a3/pynecone/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/feedback/alert.py` & `pynecone-0.1.33a3/pynecone/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/feedback/circularprogress.py` & `pynecone-0.1.33a3/pynecone/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/feedback/progress.py` & `pynecone-0.1.33a3/pynecone/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/feedback/skeleton.py` & `pynecone-0.1.33a3/pynecone/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/feedback/spinner.py` & `pynecone-0.1.33a3/pynecone/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/__init__.py` & `pynecone-0.1.33a3/pynecone/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/button.py` & `pynecone-0.1.33a3/pynecone/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/checkbox.py` & `pynecone-0.1.33a3/pynecone/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/copytoclipboard.py` & `pynecone-0.1.33a3/pynecone/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/editable.py` & `pynecone-0.1.33a3/pynecone/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/form.py` & `pynecone-0.1.33a3/pynecone/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/iconbutton.py` & `pynecone-0.1.33a3/pynecone/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/input.py` & `pynecone-0.1.33a3/pynecone/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/multiselect.py` & `pynecone-0.1.33a3/pynecone/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/numberinput.py` & `pynecone-0.1.33a3/pynecone/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/pininput.py` & `pynecone-0.1.33a3/pynecone/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/radio.py` & `pynecone-0.1.33a3/pynecone/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/rangeslider.py` & `pynecone-0.1.33a3/pynecone/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/select.py` & `pynecone-0.1.33a3/pynecone/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/slider.py` & `pynecone-0.1.33a3/pynecone/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/switch.py` & `pynecone-0.1.33a3/pynecone/components/forms/switch.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 
 class Switch(ChakraComponent):
     """Toggleable switch component."""
 
     tag = "Switch"
 
-    # If true, the switch will be checked. You'll need to pass onChange to update its value (since it is now controlled)
+    # If true, the switch will be checked. You'll need to set an on_change event handler to update its value (since it is now controlled)
     is_checked: Var[bool]
 
     # If true, the switch will be disabled
     is_disabled: Var[bool]
 
-    # If true and isDisabled is passed, the switch will remain tabbable but not interactive
+    # If true and is_disabled prop is set, the switch will remain tabbable but not interactive.
     is_focusable: Var[bool]
 
     # If true, the switch is marked as invalid. Changes style of unchecked state.
     is_invalid: Var[bool]
 
     # If true, the switch will be readonly
     is_read_only: Var[bool]
```

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/textarea.py` & `pynecone-0.1.33a3/pynecone/components/forms/textarea.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     # If true, the form control will be disabled.
     is_disabled: Var[bool]
 
     # If true, the form control will be invalid.
     is_invalid: Var[bool]
 
-    # If true, the form control will be readonly.
+    # If true, the form control will be read-only.
     is_read_only: Var[bool]
 
     # If true, the form control will be required.
     is_required: Var[bool]
 
     # "outline" | "filled" | "flushed" | "unstyled"
     variant: Var[str]
```

### Comparing `pynecone-0.1.33a2/pynecone/components/forms/upload.py` & `pynecone-0.1.33a3/pynecone/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/graphing/plotly.py` & `pynecone-0.1.33a3/pynecone/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/graphing/victory.py` & `pynecone-0.1.33a3/pynecone/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/layout/__init__.py` & `pynecone-0.1.33a3/pynecone/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/layout/box.py` & `pynecone-0.1.33a3/pynecone/components/layout/box.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class Box(ChakraComponent):
     """A generic container component that can contain other components."""
 
     tag = "Box"
 
-    # The type element to render. You can specify as an image, video, or any other HTML element such as iframe.
+    # The type element to render. You can specify an image, video, or any other HTML element such as iframe.
     element: Var[str]
 
     # The source of the content.
     src: Var[str]
 
     # The alt text of the content.
     alt: Var[str]
```

### Comparing `pynecone-0.1.33a2/pynecone/components/layout/card.py` & `pynecone-0.1.33a3/pynecone/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/layout/cond.py` & `pynecone-0.1.33a3/pynecone/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/layout/flex.py` & `pynecone-0.1.33a3/pynecone/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/layout/foreach.py` & `pynecone-0.1.33a3/pynecone/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/layout/grid.py` & `pynecone-0.1.33a3/pynecone/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/layout/html.py` & `pynecone-0.1.33a3/pynecone/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/layout/responsive.py` & `pynecone-0.1.33a3/pynecone/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/layout/stack.py` & `pynecone-0.1.33a3/pynecone/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/layout/wrap.py` & `pynecone-0.1.33a3/pynecone/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/libs/react_player.py` & `pynecone-0.1.33a3/pynecone/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/media/avatar.py` & `pynecone-0.1.33a3/pynecone/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/media/icon.py` & `pynecone-0.1.33a3/pynecone/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/media/image.py` & `pynecone-0.1.33a3/pynecone/components/media/image.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/navigation/breadcrumb.py` & `pynecone-0.1.33a3/pynecone/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/navigation/linkoverlay.py` & `pynecone-0.1.33a3/pynecone/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/navigation/stepper.py` & `pynecone-0.1.33a3/pynecone/components/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/overlay/__init__.py` & `pynecone-0.1.33a3/pynecone/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/overlay/alertdialog.py` & `pynecone-0.1.33a3/pynecone/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/overlay/banner.py` & `pynecone-0.1.33a3/pynecone/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/overlay/drawer.py` & `pynecone-0.1.33a3/pynecone/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/overlay/menu.py` & `pynecone-0.1.33a3/pynecone/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/overlay/modal.py` & `pynecone-0.1.33a3/pynecone/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/overlay/popover.py` & `pynecone-0.1.33a3/pynecone/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/overlay/tooltip.py` & `pynecone-0.1.33a3/pynecone/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/tags/iter_tag.py` & `pynecone-0.1.33a3/pynecone/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/tags/tag.py` & `pynecone-0.1.33a3/pynecone/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/tags/tagless.py` & `pynecone-0.1.33a3/pynecone/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/typography/highlight.py` & `pynecone-0.1.33a3/pynecone/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/components/typography/markdown.py` & `pynecone-0.1.33a3/pynecone/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/config.py` & `pynecone-0.1.33a3/pynecone/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,17 +170,14 @@
 
     # Disable bun.
     disable_bun: bool = False
 
     # Additional frontend packages to install.
     frontend_packages: List[str] = []
 
-    # Enable the admin dash.
-    enable_admin: bool = False
-
     # The Admin Dash
     admin_dash: Optional[AdminDash] = None
 
     # Backend transport methods.
     backend_transports: Optional[
         constants.Transports
     ] = constants.Transports.WEBSOCKET_POLLING
```

### Comparing `pynecone-0.1.33a2/pynecone/constants.py` & `pynecone-0.1.33a3/pynecone/constants.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/el/constants/html.py` & `pynecone-0.1.33a3/pynecone/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/el/constants/pynecone.py` & `pynecone-0.1.33a3/pynecone/el/constants/pynecone.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/el/constants/react.py` & `pynecone-0.1.33a3/pynecone/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/el/element.py` & `pynecone-0.1.33a3/pynecone/el/element.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/el/elements/__init__.py` & `pynecone-0.1.33a3/pynecone/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/el/precompile.py` & `pynecone-0.1.33a3/pynecone/el/precompile.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/event.py` & `pynecone-0.1.33a3/pynecone/event.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/middleware/hydrate_middleware.py` & `pynecone-0.1.33a3/pynecone/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/middleware/middleware.py` & `pynecone-0.1.33a3/pynecone/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/model.py` & `pynecone-0.1.33a3/pynecone/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 
 import sqlmodel
 
 from pynecone.base import Base
 from pynecone.config import get_config
 
 
-def get_engine():
+def get_engine(url: Optional[str] = None):
     """Get the database engine.
 
+    Args:
+        url: the DB url to use.
+
     Returns:
         The database engine.
 
     Raises:
         ValueError: If the database url is None.
     """
-    url = get_config().db_url
-    enable_admin = get_config().enable_admin
-    if not url:
-        raise ValueError("No database url in config")
+    conf = get_config()
+    url = url or conf.db_url
+    if url is None:
+        raise ValueError("No database url configured")
     return sqlmodel.create_engine(
         url,
         echo=False,
-        connect_args={"check_same_thread": False} if enable_admin else {},
+        connect_args={"check_same_thread": False} if conf.admin_dash else {},
     )
 
 
 class Model(Base, sqlmodel.SQLModel):
     """Base class to define a table in the database."""
 
     # The primary key for the table.
@@ -79,26 +82,17 @@
 
         Returns:
             The select statement.
         """
         return sqlmodel.select(cls)
 
 
-def session(url=None):
+def session(url: Optional[str] = None) -> sqlmodel.Session:
     """Get a session to interact with the database.
 
     Args:
         url: The database url.
 
     Returns:
         A database session.
     """
-    enable_admin = get_config().enable_admin
-    if url is not None:
-        return sqlmodel.Session(
-            sqlmodel.create_engine(
-                url,
-                connect_args={"check_same_thread": False} if enable_admin else {},
-            ),
-        )
-    engine = get_engine()
-    return sqlmodel.Session(engine)
+    return sqlmodel.Session(get_engine(url))
```

### Comparing `pynecone-0.1.33a2/pynecone/pc.py` & `pynecone-0.1.33a3/pynecone/pc.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,18 @@
 
     if for_pc_deploy:
         # Get the app config and modify the api_url base on username and app_name.
         config.api_url = prerequisites.get_production_backend_url()
 
     # Compile the app in production mode and export it.
     console.rule("[bold]Compiling production app and preparing for export.")
+
+    if frontend:
+        build.setup_frontend(Path.cwd())
+
     app = prerequisites.get_app().app
     build.export_app(
         app,
         backend=backend,
         frontend=frontend,
         zip=zipping,
         deploy_url=config.deploy_url,
```

### Comparing `pynecone-0.1.33a2/pynecone/route.py` & `pynecone-0.1.33a3/pynecone/route.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/state.py` & `pynecone-0.1.33a3/pynecone/state.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/style.py` & `pynecone-0.1.33a3/pynecone/style.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/utils/build.py` & `pynecone-0.1.33a3/pynecone/utils/build.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/utils/console.py` & `pynecone-0.1.33a3/pynecone/utils/console.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/utils/exec.py` & `pynecone-0.1.33a3/pynecone/utils/exec.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         loglevel: The log level to use.
     """
     process = subprocess.Popen(
         run_command,
         cwd=constants.WEB_DIR,
         env=os.environ,
         stderr=subprocess.STDOUT,
-        stdout=subprocess.PIPE,
-        universal_newlines=True,
+        stdout=None if platform.system() == "Windows" else subprocess.PIPE,
+        universal_newlines=None if platform.system() == "Windows" else True,
     )
 
     current_time = datetime.now()
     if process.stdout:
         for line in process.stdout:
             if "ready started server on" in line:
                 url = line.split("url: ")[-1].strip()
```

### Comparing `pynecone-0.1.33a2/pynecone/utils/format.py` & `pynecone-0.1.33a3/pynecone/utils/format.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/utils/imports.py` & `pynecone-0.1.33a3/pynecone/utils/imports.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/utils/path_ops.py` & `pynecone-0.1.33a3/pynecone/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/utils/prerequisites.py` & `pynecone-0.1.33a3/pynecone/utils/prerequisites.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,14 +205,15 @@
 
 def initialize_web_directory():
     """Initialize the web directory on pc init."""
     console.log("Initializing the web directory.")
     path_ops.rm(os.path.join(constants.WEB_TEMPLATE_DIR, constants.NODE_MODULES))
     path_ops.rm(os.path.join(constants.WEB_TEMPLATE_DIR, constants.PACKAGE_LOCK))
     path_ops.cp(constants.WEB_TEMPLATE_DIR, constants.WEB_DIR)
+    path_ops.mkdir(constants.WEB_ASSETS_DIR)
 
     # Write the current version of distributed pynecone package to a PCVERSION_APP_FILE."""
     with open(constants.PCVERSION_APP_FILE, "w") as f:
         pynecone_json = {"version": constants.VERSION}
         json.dump(pynecone_json, f, ensure_ascii=False)
 
 
@@ -335,30 +336,21 @@
     with open(constants.PCVERSION_APP_FILE) as f:  # type: ignore
         app_version = json.load(f)["version"]
     return app_version == constants.VERSION
 
 
 def check_admin_settings():
     """Check if admin settings are set and valid for logging in cli app."""
-    admin_enabled = get_config().enable_admin
     admin_dash = get_config().admin_dash
     current_time = datetime.now()
-    if admin_enabled and admin_dash:
+    if admin_dash:
         if not admin_dash.models:
             console.print(
                 f"[yellow][Admin Dashboard][/yellow] :megaphone: Admin dashboard enabled, but no models defined in [bold magenta]pcconfig.py[/bold magenta]. Time: {current_time}"
             )
         else:
             console.print(
                 f"[yellow][Admin Dashboard][/yellow] Admin enabled, building admin dashboard. Time: {current_time}"
             )
             console.print(
                 "Admin dashboard running at: [bold green]http://localhost:8000/admin[/bold green]"
             )
-    elif admin_enabled:
-        console.print(
-            f"[yellow][Admin Dashboard][/yellow] :megaphone: Admin enabled, but no admin dashboard defined in [bold magenta]pcconfig.py[/bold magenta]. Time: {current_time}"
-        )
-    elif admin_dash:
-        console.print(
-            f"[yellow][Admin Dashboard][/yellow] :megaphone: Admin dashboard defined, but admin is not enabled in [bold magenta]pcconfig.py[/bold magenta]. Time: {current_time}"
-        )
```

### Comparing `pynecone-0.1.33a2/pynecone/utils/processes.py` & `pynecone-0.1.33a3/pynecone/utils/processes.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/utils/telemetry.py` & `pynecone-0.1.33a3/pynecone/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/utils/types.py` & `pynecone-0.1.33a3/pynecone/utils/types.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/utils/watch.py` & `pynecone-0.1.33a3/pynecone/utils/watch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pynecone/vars.py` & `pynecone-0.1.33a3/pynecone/vars.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a2/pyproject.toml` & `pynecone-0.1.33a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynecone"
-version = "0.1.33a2"
+version = "0.1.33a3"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
@@ -21,15 +21,15 @@
 packages = [
     {include = "pynecone"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 cloudpickle = "^2.2.1"
-fastapi = "^0.92.0"
+fastapi = "^0.96.0"
 gunicorn = "^20.1.0"
 httpx = "^0.23.0"
 jinja2 = "^3.1.2"
 plotly = "^5.13.0"
 psutil = "^5.9.4"
 pydantic = "^1.10.2"
 python-multipart = "^0.0.5"
@@ -54,14 +54,15 @@
 pytest-cov = "^4.0.0"
 black = "^22.10.0"
 ruff = "^0.0.244"
 pandas = [
     {version = "^1.5.3", python = ">=3.8,<4.0"},
     {version = "^1.1", python = ">=3.7, <3.8"}
 ]
+asynctest = "^0.13.0"
 pre-commit = {version = "^3.2.1", python = ">=3.8,<4.0"}
 
 [tool.poetry.scripts]
 pc = "pynecone.pc:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `pynecone-0.1.33a2/PKG-INFO` & `pynecone-0.1.33a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone
-Version: 0.1.33a2
+Version: 0.1.33a3
 Summary: Web apps in pure Python.
 Home-page: https://pynecone.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
-Requires-Dist: fastapi (>=0.92.0,<0.93.0)
+Requires-Dist: fastapi (>=0.96.0,<0.97.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: plotly (>=5.13.0,<6.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: python-dotenv (>=0.13.0,<0.14.0)
```

