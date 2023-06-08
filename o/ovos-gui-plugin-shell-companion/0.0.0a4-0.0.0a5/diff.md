# Comparing `tmp/ovos-gui-plugin-shell-companion-0.0.0a4.tar.gz` & `tmp/ovos-gui-plugin-shell-companion-0.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-gui-plugin-shell-companion-0.0.0a4.tar", last modified: Thu May 25 16:25:06 2023, max compression
+gzip compressed data, was "ovos-gui-plugin-shell-companion-0.0.0a5.tar", last modified: Thu Jun  8 14:27:01 2023, max compression
```

## Comparing `ovos-gui-plugin-shell-companion-0.0.0a4.tar` & `ovos-gui-plugin-shell-companion-0.0.0a5.tar`

### file list

```diff
@@ -1,157 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:25:06.857975 ovos-gui-plugin-shell-companion-0.0.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-25 16:25:06.857975 ovos-gui-plugin-shell-companion-0.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:25:06.849975 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/color_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/cui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:25:06.845975 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:25:06.849975 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/snd/
--rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/snd/clicked.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:25:06.849975 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_HtmlFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:25:06.849975 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:25:06.849975 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/code/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js
--rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:25:06.849975 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)    18448 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    24264 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:25:06.849975 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/NameSelect.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/developer_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    20307 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/factory_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:25:06.853975 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3790 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml
--rw-r--r--   0 runner    (1001) docker     (123)    26181 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:25:06.857975 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts
--rwxr-xr-x   0 runner    (1001) docker     (123)     1969 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/wigets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:25:06.849975 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:25:06.857975 ovos-gui-plugin-shell-companion-0.0.0a4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2950 2023-05-25 16:25:06.000000 ovos-gui-plugin-shell-companion-0.0.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:27:01.317919 ovos-gui-plugin-shell-companion-0.0.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-08 14:27:01.313919 ovos-gui-plugin-shell-companion-0.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:27:01.305919 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/
+-rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/color_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/cui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/descriptions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:27:01.301919 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:27:01.305919 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/snd/
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/snd/clicked.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:27:01.305919 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_HtmlFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:27:01.305919 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:27:01.305919 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:27:01.305919 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    18448 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    24264 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:27:01.309919 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/NameSelect.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/developer_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    20307 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/factory_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:27:01.309919 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3790 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    26181 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:27:01.313919 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1969 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/wigets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:27:01.305919 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-08 14:27:01.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-06-08 14:27:01.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:27:01.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-08 14:27:01.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 14:27:01.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 14:27:01.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:27:01.000000 ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:27:01.317919 ovos-gui-plugin-shell-companion-0.0.0a5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2949 2023-06-08 14:27:00.000000 ovos-gui-plugin-shell-companion-0.0.0a5/setup.py
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/LICENSE` & `ovos-gui-plugin-shell-companion-0.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/PKG-INFO` & `ovos-gui-plugin-shell-companion-0.0.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-gui-plugin-shell-companion
-Version: 0.0.0a4
+Version: 0.0.0a5
 Summary: GUI plugin for ovos-shell
 Home-page: https://github.com/OpenVoiceOS/ovos-gui-plugin-shell-companion
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/README.md` & `ovos-gui-plugin-shell-companion-0.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/__init__.py` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import platform
 
+from ovos_bus_client.client import MessageBusClient
+
 from ovos_bus_client import Message
 from ovos_utils import network_utils
 from ovos_utils.fingerprinting import get_mycroft_version
+from ovos_utils.gui import GUIInterface
 from ovos_utils.log import LOG
 
 from ovos_gui_plugin_shell_companion.brightness import BrightnessManager
 from ovos_gui_plugin_shell_companion.color_manager import ColorManager
 from ovos_gui_plugin_shell_companion.config import get_ovos_shell_config
 from ovos_gui_plugin_shell_companion.cui import ConfigUIManager
 from ovos_gui_plugin_shell_companion.wigets import WidgetManager
@@ -15,25 +18,28 @@
 
 class OVOSShellCompanionExtension(GUIExtension):
     """OVOS-shell Extension: This extension is responsible for managing the Smart Speaker
     specific GUI behaviours. This extension adds support for Homescreens and Homescreen Mangement.
     It handles all events sent from ovos-shell
 
     Args:
+        config: plugin configuration
         bus: MessageBus instance
         gui: GUI instance
         preload_gui (bool): load GUI skills even if gui client not connected
         permanent (bool): disable unloading of GUI skills on gui client disconnections
     """
 
-    def __init__(self, config, bus=None, gui=None,
+    def __init__(self, config: dict, bus: MessageBusClient = None,
+                 gui: GUIInterface = None,
                  preload_gui=False, permanent=True):
         config["homescreen_supported"] = True
         LOG.info("OVOS Shell: Initializing")
-        super().__init__(bus, gui, config, preload_gui, permanent)
+        super().__init__(config=config, bus=bus, gui=gui,
+                         preload_gui=preload_gui, permanent=permanent)
         self.local_display_config = get_ovos_shell_config()
         self.about_page_data = []
         self.build_initial_about_page_data()
 
         self.color_manager = ColorManager(self.bus)
         self.widgets = WidgetManager(self.bus)
         self.bright = BrightnessManager(self.bus)
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/brightness.py` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/brightness.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import platform
 import subprocess
 import threading
 import time
 from datetime import timedelta
 from distutils.spawn import find_executable
 from os.path import isfile
-
+from astral import LocationInfo
+from astral.sun import sun
 from ovos_bus_client import Message
 from ovos_config import Configuration
 from ovos_utils.events import EventSchedulerInterface
 from ovos_utils.log import LOG
 from ovos_utils.time import now_local
 from ovos_gui_plugin_shell_companion.config import get_ovos_shell_config
 
@@ -24,14 +25,16 @@
         self.device_interface = "DSI"
         self.ddcutil_detected_bus = None
         self.ddcutil_brightness_code = None
         self.auto_dim_enabled = False
         self.auto_night_mode_enabled = False
         self.timer_thread = None  # TODO - use event scheduler too
 
+        self.sunset_time = None
+        self.sunrise_time = None
         self.get_sunset_time()
 
         self.is_auto_dim_enabled()
         self.is_auto_night_mode_enabled()
 
         self.discover()
 
@@ -223,34 +226,34 @@
         else:
             pass
 
         ##### AUTO NIGHT MODE HANDLING #####
 
     def get_sunset_time(self, message=None):
         LOG.debug("Getting sunset time")
-        date = now_local()
+        now_time = now_local()
         try:
-            from astral import LocationInfo
-            from astral.sun import sun
             location = Configuration()["location"]
             lat = location["coordinate"]["latitude"]
             lon = location["coordinate"]["longitude"]
             tz = location["timezone"]["code"]
             city = LocationInfo("Some city", "Some location", tz, lat, lon)
-            s = sun(city.observer, date=date)["sunset"]
+            s = sun(city.observer, date=now_time)
             self.sunset_time = s["sunset"]
             self.sunrise_time = s["sunrise"]
-        except:
-            self.sunset_time = datetime.datetime(year=date.year, month=date.month,
-                                                 day=date.day, hour=22)
+        except Exception as e:
+            LOG.exception(f"Using default times for sunrise/sunset: {e}")
+            self.sunset_time = datetime.datetime(year=now_time.year,
+                                                 month=now_time.month,
+                                                 day=now_time.day, hour=22)
             self.sunrise_time = self.sunset_time + timedelta(hours=8)
 
         # check sunset times again in 24 hours
         self.event_scheduler.schedule_event(self.get_sunset_time,
-                                            when=date + timedelta(hours=24),
+                                            when=now_time + timedelta(hours=24),
                                             name="ovos-shell.suntimes.check")
 
     def start_auto_night_mode(self, message=None):
         if self.auto_night_mode_enabled:
             date = now_local()
             self.event_scheduler.schedule_event(self.start_auto_night_mode,
                                                 when=date + timedelta(hours=1),
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/color_manager.py` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/color_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import re
-from os.path import join
+from os.path import join, dirname
 
 from ovos_bus_client import Message
 from ovos_utils.log import LOG
 from ovos_utils.xdg_utils import xdg_config_home, xdg_data_home
 
 
 class ColorManager:
@@ -54,15 +54,15 @@
                 theme_file = open(join(xdg_config_home(), file_name), "r")
                 theme = theme_file.read()
                 theme_file.close()
             elif file_name in os.listdir(xdg_system_path):
                 theme_file = open(join(xdg_system_path, file_name), "r")
                 theme = theme_file.read()
                 theme_file.close()
-
+            # TODO: Default `theme`
             name = re.search(r"name=(.*)", theme).group(1)
             primaryColor = re.search(r"primaryColor=(.*)", theme).group(1)
             secondaryColor = re.search(r"secondaryColor=(.*)", theme).group(1)
             textColor = re.search(r"textColor=(.*)", theme).group(1)
 
             self.bus.emit(message.response({"name": name,
                                             "primaryColor": primaryColor,
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/config.py` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/config.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/cui.py` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/cui.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,30 +136,36 @@
             field["field_description"] = self.populate_field_description(
                 field["field_name"], group_name)
 
             type_str = "field"
             return [field, type_str]
 
     def populate_section_description(self, section_name, section_group):
-        with open(os.path.dirname(os.path.realpath(__file__)) + "/descriptions.json", "r") as f:
+        # TODO: Resolve file from resources
+        with open(os.path.dirname(os.path.realpath(__file__)) +
+                  "/descriptions.json", "r") as f:
             description_json = json.load(f)
             descriptions = description_json["collection"]
             for description in descriptions:
                 if description["type"] == "section":
-                    if description["key"] == section_name and description["group"] == section_group:
+                    if description["key"] == section_name and \
+                            description["group"] == section_group:
                         return description["value"]
         return ""
 
     def populate_field_description(self, field_name, field_group):
-        with open(os.path.dirname(os.path.realpath(__file__)) + "/descriptions.json", "r") as f:
+        # TODO: Resolve file from resources
+        with open(os.path.dirname(os.path.realpath(__file__)) +
+                  "/descriptions.json", "r") as f:
             description_json = json.load(f)
             descriptions = description_json["collection"]
             for description in descriptions:
                 if description["type"] == "field":
-                    if description["key"] == field_name and description["group"] == field_group:
+                    if description["key"] == field_name and \
+                            description["group"] == field_group:
                         return description["value"]
         return ""
 
     def list_groups(self, message=None):
         group_names = []
         for group in self.settings_meta["settings"]:
             group_names.append(group["group_name"])
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/snd/clicked.wav` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/snd/clicked.wav`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/FeatureRequest.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/RequestHandler.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AdditionalSettings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_AnimatedImageFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_ImageFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_TextFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/SYSTEM_UrlFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/SwipeArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/WebViewHtmlFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/WebViewUrlFrame.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/SettingsModel.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/ThemeView.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/about_page.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/code/colorUtils.js`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_generator_display.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_groups_display.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingCheckBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingListBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/configuration_ui/settingTextBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/customize_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/customize_theme.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/BrightnessSlider.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectPrimary.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSelectSecondary.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/ColorSlider.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/Palette.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/PalettesGrid.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/delegates/SetNameBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/developer_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/developer_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/display_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/factory_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/factory_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/homescreen_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/back.png`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/display.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/home.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/info.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/next.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/paint.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/power.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/restart.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/settings.png`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/ssh.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-green.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/switch-red.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/images/tick.svg`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/lupdate-generator.sh`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/settingspage.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/ssh_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/settings/wallpaper_settings.qml`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_de.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_es.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_fr.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_it.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_nl.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/SmartSpeakerExtension.GuiInterface_pt.qm`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/about_page_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_generator_display_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/configuration_groups_display_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/customize_theme_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/developer_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/display_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/homescreen_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/lrelease-generator.sh`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingListBox_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/settingspage_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/res/ui/translations/ssh_settings_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion/wigets.py` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion/wigets.py`

 * *Files identical despite different names*

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion.egg-info/PKG-INFO` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-gui-plugin-shell-companion
-Version: 0.0.0a4
+Version: 0.0.0a5
 Summary: GUI plugin for ovos-shell
 Home-page: https://github.com/OpenVoiceOS/ovos-gui-plugin-shell-companion
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt` & `ovos-gui-plugin-shell-companion-0.0.0a5/ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 ovos_gui_plugin_shell_companion/__init__.py
 ovos_gui_plugin_shell_companion/brightness.py
 ovos_gui_plugin_shell_companion/color_manager.py
 ovos_gui_plugin_shell_companion/config.py
 ovos_gui_plugin_shell_companion/cui.py
+ovos_gui_plugin_shell_companion/descriptions.json
 ovos_gui_plugin_shell_companion/version.py
 ovos_gui_plugin_shell_companion/wigets.py
 ovos_gui_plugin_shell_companion.egg-info/PKG-INFO
 ovos_gui_plugin_shell_companion.egg-info/SOURCES.txt
 ovos_gui_plugin_shell_companion.egg-info/dependency_links.txt
 ovos_gui_plugin_shell_companion.egg-info/entry_points.txt
 ovos_gui_plugin_shell_companion.egg-info/requires.txt
```

### Comparing `ovos-gui-plugin-shell-companion-0.0.0a4/setup.py` & `ovos-gui-plugin-shell-companion-0.0.0a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,9 +72,9 @@
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
-    entry_points={'ovos.plugin.phal': PLUGIN_ENTRY_POINT}
+    entry_points={'ovos.plugin.gui': PLUGIN_ENTRY_POINT}
 )
```

