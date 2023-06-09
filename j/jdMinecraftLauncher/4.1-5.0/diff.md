# Comparing `tmp/jdMinecraftLauncher-4.1.tar.gz` & `tmp/jdMinecraftLauncher-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdMinecraftLauncher-4.1.tar", last modified: Wed Nov 16 15:49:52 2022, max compression
+gzip compressed data, was "jdMinecraftLauncher-5.0.tar", last modified: Fri Jun  9 20:19:20 2023, max compression
```

## Comparing `jdMinecraftLauncher-4.1.tar` & `jdMinecraftLauncher-5.0.tar`

### file list

```diff
@@ -1,32 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 15:49:52.142892 jdMinecraftLauncher-4.1/
--rw-rw-rw-   0 root         (0) root         (0)    35085 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      271 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2854 2022-11-16 15:49:52.142892 jdMinecraftLauncher-4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1347 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 15:49:52.139891 jdMinecraftLauncher-4.1/jdMinecraftLauncher/
--rw-rw-rw-   0 root         (0) root         (0)      635 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/DBusInterface.xml
--rw-rw-rw-   0 root         (0) root         (0)     2033 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/DBusService.py
--rw-rw-rw-   0 root         (0) root         (0)     7345 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/Environment.py
--rw-rw-rw-   0 root         (0) root         (0)     3544 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/Functions.py
--rw-rw-rw-   0 root         (0) root         (0)    58432 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/Icon.svg
--rw-rw-rw-   0 root         (0) root         (0)     1676 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/InstallThread.py
--rw-rw-rw-   0 root         (0) root         (0)     1428 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/MicrosoftSecrets.py
--rw-rw-rw-   0 root         (0) root         (0)     3050 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/Profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1730 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/RunMinecraft.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/Settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2536 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/jdMinecraftLauncher.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/secrets.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 15:49:52.142892 jdMinecraftLauncher-4.1/jdMinecraftLauncher/translation/
--rw-rw-rw-   0 root         (0) root         (0)     6693 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/translation/de_DE.lang
--rw-rw-rw-   0 root         (0) root         (0)     6106 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/translation/en_GB.lang
--rw-rw-rw-   0 root         (0) root         (0)        4 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 15:49:52.141892 jdMinecraftLauncher-4.1/jdMinecraftLauncher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2854 2022-11-16 15:49:52.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      876 2022-11-16 15:49:52.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-16 15:49:52.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2022-11-16 15:49:52.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       74 2022-11-16 15:49:52.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-11-16 15:49:52.000000 jdMinecraftLauncher-4.1/jdMinecraftLauncher.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1868 2022-11-16 15:49:26.000000 jdMinecraftLauncher-4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-16 15:49:52.142892 jdMinecraftLauncher-4.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 20:19:20.389675 jdMinecraftLauncher-5.0/
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35085 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      210 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-06-09 20:19:20.385675 jdMinecraftLauncher-5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 20:19:20.385675 jdMinecraftLauncher-5.0/jdMinecraftLauncher/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/DBusInterface.xml
+-rw-r--r--   0 root         (0) root         (0)     2217 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/DBusService.py
+-rw-r--r--   0 root         (0) root         (0)     6070 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/Environment.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/Functions.py
+-rw-r--r--   0 root         (0) root         (0)    58432 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/Icon.svg
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/InstallThread.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/Languages.py
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/MicrosoftSecrets.py
+-rw-r--r--   0 root         (0) root         (0)     4412 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/Profile.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/ProfileCollection.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/ProfileImporter.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/RunMinecraft.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/Settings.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/Shortcut.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 20:19:20.385675 jdMinecraftLauncher-5.0/jdMinecraftLauncher/gui/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/gui/LoginWindow.py
+-rw-r--r--   0 root         (0) root         (0)    31670 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/gui/MainWindow.py
+-rw-r--r--   0 root         (0) root         (0)    19284 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/gui/ProfileWindow.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/gui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/jdMinecraftLauncher.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/secrets.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 20:19:20.385675 jdMinecraftLauncher-5.0/jdMinecraftLauncher/translations/
+-rw-r--r--   0 root         (0) root         (0)    21558 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/translations/jdMinecraftLauncher_de.ts
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 20:19:20.385675 jdMinecraftLauncher-5.0/jdMinecraftLauncher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-06-09 20:19:20.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-06-09 20:19:20.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 20:19:20.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-09 20:19:20.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-09 20:19:20.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-09 20:19:20.000000 jdMinecraftLauncher-5.0/jdMinecraftLauncher.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2441 2023-06-09 20:14:55.000000 jdMinecraftLauncher-5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 20:19:20.389675 jdMinecraftLauncher-5.0/setup.cfg
```

### Comparing `jdMinecraftLauncher-4.1/LICENSE` & `jdMinecraftLauncher-5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jdMinecraftLauncher-4.1/PKG-INFO` & `jdMinecraftLauncher-5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jdMinecraftLauncher
-Version: 4.1
+Version: 5.0
 Summary: A classic styled Minecraft Launcher
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL v3
-Project-URL: Issues, https://gitlab.com/JakobDev/jdMinecraftLauncher/-/issues
-Project-URL: Source, https://gitlab.com/JakobDev/jdMinecraftLauncher
+Project-URL: Source, https://codeberg.org/JakobDev/jdMinecraftLauncher
+Project-URL: Issues, https://codeberg.org/JakobDev/jdMinecraftLauncher/issues
+Project-URL: Translate, https://translate.codeberg.org/projects/jdMinecraftLauncher
 Project-URL: Donation, https://ko-fi.com/jakobdev
 Keywords: JakobDev,Minecraft,Mojang,launcher,PyQt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Environment :: Other Environment
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `jdMinecraftLauncher-4.1/README.md` & `jdMinecraftLauncher-5.0/README.md`

 * *Files identical despite different names*

### Comparing `jdMinecraftLauncher-4.1/jdMinecraftLauncher/DBusInterface.xml` & `jdMinecraftLauncher-5.0/jdMinecraftLauncher/DBusInterface.xml`

 * *Files 23% similar despite different names*

#### Comparing `jdMinecraftLauncher-4.1/jdMinecraftLauncher/DBusInterface.xml` & `jdMinecraftLauncher-5.0/jdMinecraftLauncher/DBusInterface.xml`

```diff
@@ -1,18 +1,21 @@
 <?xml version="1.0" encoding="utf-8"?>
-<interface name="com.gitlab.JakobDev.jdMinecraftLauncher">
+<interface name="page.codeberg.JakobDev.jdMinecraftLauncher">
   <method name="LaunchProfile">
     <arg direction="in" type="s" name="name"/>
     <arg direction="out" type="b" name="ok"/>
   </method>
   <method name="ListProfiles">
     <arg direction="out" type="as" name="profiles"/>
   </method>
+  <method name="GetProfile">
+    <arg direction="out" type="s" name="profiles"/>
+  </method>
   <method name="GetMinecraftCommand">
     <arg direction="in" type="s" name="name"/>
-    <arg direction="out" type="as" name="comman"/>
+    <arg direction="out" type="as" name="command"/>
   </method>
   <method name="GetVersion">
     <arg direction="out" type="s" name="version"/>
   </method>
   <property type="b" name="MainWindowVisible"/>
 </interface>
```

### Comparing `jdMinecraftLauncher-4.1/jdMinecraftLauncher/DBusService.py` & `jdMinecraftLauncher-5.0/jdMinecraftLauncher/DBusService.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from jdMinecraftLauncher.RunMinecraft import getMinecraftCommand
 from PyQt6.QtCore import pyqtClassInfo, pyqtSlot, pyqtProperty
 from PyQt6.QtDBus import QDBusConnection, QDBusAbstractAdaptor
 from PyQt6.QtWidgets import QApplication
 from typing import TYPE_CHECKING
+import json
 import sys
 import os
 
 
 if TYPE_CHECKING:
     from jdMinecraftLauncher.Environment import Environment
 
 
 with open(os.path.join(os.path.dirname(__file__), "DBusInterface.xml"), "r", encoding="utf-8") as f:
     interface = f.read()
 
-@pyqtClassInfo("D-Bus Interface", "com.gitlab.JakobDev.jdMinecraftLauncher")
+@pyqtClassInfo("D-Bus Interface", "page.codeberg.JakobDev.jdMinecraftLauncher")
 @pyqtClassInfo("D-Bus Introspection", interface)
 class DBusService(QDBusAbstractAdaptor):
     def __init__(self, env: "Environment", parent: QApplication):
         super().__init__(parent)
         QDBusConnection.sessionBus().registerObject("/", parent)
 
-        if not QDBusConnection.sessionBus().registerService("com.gitlab.JakobDev.jdMinecraftLauncher"):
+        if not QDBusConnection.sessionBus().registerService("page.codeberg.JakobDev.jdMinecraftLauncher"):
             print(QDBusConnection.sessionBus().lastError().message(), file=sys.stderr)
 
         self._env = env
 
     @pyqtSlot(str, result=bool)
     def LaunchProfile(self, name: str) -> bool:
         profile = self._env.getProfileByName(name)
@@ -38,17 +39,21 @@
     @pyqtSlot(result=list)
     def ListProfiles(self):
         profileList = []
         for i in self._env.profiles:
             profileList.append(i.name)
         return profileList
 
+    @pyqtSlot(result=str)
+    def GetProfile(self):
+        return json.dumps(self._env.profileCollection.getSelectedProfile().toDict())
+
     @pyqtSlot(str, result=list)
-    def GetMinecraftCommand(self, name: str):
-        profile = self._env.getProfileByName(name)
+    def GetMinecraftCommand(self, profile_id: str):
+        profile = self._env.profileCollection.getProfileByID(profile_id)
         if profile:
             return getMinecraftCommand(profile, self._env, "")
 
     @pyqtSlot(result=str)
     def GetVersion(self):
         return self._env.launcherVersion
```

### Comparing `jdMinecraftLauncher-4.1/jdMinecraftLauncher/Functions.py` & `jdMinecraftLauncher-5.0/jdMinecraftLauncher/Functions.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from PyQt6.QtWidgets import QMessageBox
 import subprocess
 import platform
 import requests
 import shutil
 import socket
 import json
+import sys
 import os
 
 
 if TYPE_CHECKING:
     from jdMinecraftLauncher.Environment import Environment
 
 
@@ -19,36 +20,29 @@
     elif platform.system() == "Darwin":
         subprocess.Popen(["open", path])
     else:
         subprocess.Popen(["xdg-open", path])
 
 
 def saveProfiles(env: "Environment"):
+    if env.args.dont_save_data:
+        return
+
     profileList = []
     for a in env.profiles:
         b = vars(a)
         c = {}
         for key, value in b.items():
             if value != env:
                 c[key] = value
         profileList.append(c)
     with open(os.path.join(env.dataDir, "profiles.json"), 'w', encoding='utf-8') as f:
         json.dump({"selectedProfile":env.selectedProfile,"profileList":profileList}, f, ensure_ascii=False, indent=4)
 
 
-def showMessageBox(title: str, text: str, env: "Environment", callback=None):
-    messageBox = QMessageBox()
-    messageBox.setWindowTitle(env.translate(title))
-    messageBox.setText(env.translate(text))
-    messageBox.setStandardButtons(QMessageBox.StandardButton.Ok)
-    if callback != None:
-        messageBox.buttonClicked.connect(callback)
-    messageBox.exec()
-
-
 def hasInternetConnection() -> bool:
     try:
         socket.create_connection(("api.mojang.com", 80))
         return True
     except OSError:
         return False
 
@@ -91,25 +85,10 @@
     return runtimeList
 
 
 def isFlatpak() -> bool:
     return os.path.isfile("/.flatpak-info")
 
 
-def createDesktopFile(path: str, profile_name: str):
-    try:
-        os.makedirs(path)
-    except Exception:
-        pass
-
-    with open(os.path.join(path, f"com.gitlab.JakobDev.Profile.{profile_name}.desktop"), "w", encoding="utf-8") as f:
-        f.write("[Desktop Entry]\n")
-        f.write("Type=Application\n")
-        f.write(f"Name={profile_name}\n")
-        f.write("Icon=com.gitlab.JakobDev.jdMinecraftLauncher\n")
-        f.write("Categories=Game;\n")
-        if isFlatpak():
-            f.write("Exec=" + subprocess.list2cmdline(["flatpak", "run", "com.gitlab.JakobDev.jdMinecraftLauncher", "--launch-profile", profile_name]) + "\n")
-        else:
-            f.write("Exec=" + subprocess.list2cmdline(["jdMinecraftLauncher", "--launch-profile", profile_name]) + "\n")
-
-    subprocess.run(["chmod", "+x", os.path.join(path, f"com.gitlab.JakobDev.Profile.{profile_name}.desktop")])
+def isFrozen() -> bool:
+    """Check if the App is frozen with PyInstaller"""
+    return hasattr(sys, "frozen")
```

### Comparing `jdMinecraftLauncher-4.1/jdMinecraftLauncher/Icon.svg` & `jdMinecraftLauncher-5.0/jdMinecraftLauncher/Icon.svg`

 * *Files identical despite different names*

### Comparing `jdMinecraftLauncher-4.1/jdMinecraftLauncher/InstallThread.py` & `jdMinecraftLauncher-5.0/jdMinecraftLauncher/InstallThread.py`

 * *Files identical despite different names*

### Comparing `jdMinecraftLauncher-4.1/jdMinecraftLauncher/MicrosoftSecrets.py` & `jdMinecraftLauncher-5.0/jdMinecraftLauncher/MicrosoftSecrets.py`

 * *Files identical despite different names*

### Comparing `jdMinecraftLauncher-4.1/jdMinecraftLauncher/RunMinecraft.py` & `jdMinecraftLauncher-5.0/jdMinecraftLauncher/RunMinecraft.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,39 +5,57 @@
 
 if TYPE_CHECKING:
     from jdMinecraftLauncher.Environment import Environment
     from jdMinecraftLauncher.Profile import Profile
 
 
 def getMinecraftCommand(profile: "Profile", env: "Environment", natives_path: str) -> List[str]:
-    versiontype, versionid = profile.getVersion().split(" ")
+    version = profile.getVersionID()
     options = {
         "username": env.account["name"],
         "uuid": env.account["uuid"],
         "token": env.account["accessToken"],
         "launcherName": "jdMinecraftLauncher",
         "launcherVersion": env.launcherVersion,
         "gameDirectory": profile.getGameDirectoryPath(),
     }
+
     if profile.customExecutable:
         options["executablePath"] = profile.executable
+
     if profile.customArguments:
         options["jvmArguments"] = []
         for i in profile.arguments.split(" "):
             options["jvmArguments"].append(i)
+
     if profile.customResolution:
         options["customResolution"] = True
         options["resolutionWidth"] = profile.resolutionX
         options["resolutionHeight"] = profile.resolutionY
+
     if profile.serverConnect:
         options["server"] = profile.serverIP
         if profile.serverPort != "":
             options["port"] = profile.serverPort
+
     if profile.demoMode:
         options["demo"] = True
+
+    if profile.disableMultiplayer:
+        options["disableMultiplayer"] = True
+
+    if profile.disableChat:
+        options["disableChat"] = True
+
     if natives_path != "":
         options["nativesDirectory"] = natives_path
-        minecraft_launcher_lib.natives.extract_natives(versionid,env.minecraftDir, natives_path)
-    command = minecraft_launcher_lib.command.get_minecraft_command(versionid, env.minecraftDir, options)
+        minecraft_launcher_lib.natives.extract_natives(version, env.minecraftDir, natives_path)
+
+    command = minecraft_launcher_lib.command.get_minecraft_command(version, env.minecraftDir, options)
+
+    if profile.hasMinecraftOptions:
+        command += profile.minecraftOptions.strip().split(" ")
+
     if profile.useGameMode and shutil.which("gamemoderun"):
         command.insert(0, "gamemoderun")
+
     return command
```

### Comparing `jdMinecraftLauncher-4.1/jdMinecraftLauncher.egg-info/PKG-INFO` & `jdMinecraftLauncher-5.0/jdMinecraftLauncher.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jdMinecraftLauncher
-Version: 4.1
+Version: 5.0
 Summary: A classic styled Minecraft Launcher
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL v3
-Project-URL: Issues, https://gitlab.com/JakobDev/jdMinecraftLauncher/-/issues
-Project-URL: Source, https://gitlab.com/JakobDev/jdMinecraftLauncher
+Project-URL: Source, https://codeberg.org/JakobDev/jdMinecraftLauncher
+Project-URL: Issues, https://codeberg.org/JakobDev/jdMinecraftLauncher/issues
+Project-URL: Translate, https://translate.codeberg.org/projects/jdMinecraftLauncher
 Project-URL: Donation, https://ko-fi.com/jakobdev
 Keywords: JakobDev,Minecraft,Mojang,launcher,PyQt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Environment :: Other Environment
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `jdMinecraftLauncher-4.1/jdMinecraftLauncher.egg-info/SOURCES.txt` & `jdMinecraftLauncher-5.0/jdMinecraftLauncher.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,34 @@
+BuildBackend.py
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 jdMinecraftLauncher/DBusInterface.xml
 jdMinecraftLauncher/DBusService.py
 jdMinecraftLauncher/Environment.py
 jdMinecraftLauncher/Functions.py
 jdMinecraftLauncher/Icon.svg
 jdMinecraftLauncher/InstallThread.py
+jdMinecraftLauncher/Languages.py
 jdMinecraftLauncher/MicrosoftSecrets.py
 jdMinecraftLauncher/Profile.py
+jdMinecraftLauncher/ProfileCollection.py
+jdMinecraftLauncher/ProfileImporter.py
 jdMinecraftLauncher/RunMinecraft.py
 jdMinecraftLauncher/Settings.py
+jdMinecraftLauncher/Shortcut.py
 jdMinecraftLauncher/__init__.py
 jdMinecraftLauncher/jdMinecraftLauncher.py
 jdMinecraftLauncher/secrets.json
 jdMinecraftLauncher/version.txt
 jdMinecraftLauncher.egg-info/PKG-INFO
 jdMinecraftLauncher.egg-info/SOURCES.txt
 jdMinecraftLauncher.egg-info/dependency_links.txt
 jdMinecraftLauncher.egg-info/entry_points.txt
 jdMinecraftLauncher.egg-info/requires.txt
 jdMinecraftLauncher.egg-info/top_level.txt
-jdMinecraftLauncher/translation/de_DE.lang
-jdMinecraftLauncher/translation/en_GB.lang
+jdMinecraftLauncher/gui/LoginWindow.py
+jdMinecraftLauncher/gui/MainWindow.py
+jdMinecraftLauncher/gui/ProfileWindow.py
+jdMinecraftLauncher/gui/__init__.py
+jdMinecraftLauncher/translations/jdMinecraftLauncher_de.ts
```

### Comparing `jdMinecraftLauncher-4.1/pyproject.toml` & `jdMinecraftLauncher-5.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
+requires = ["setuptools", "PyQt6", "wheel"]
+build-backend = "BuildBackend"
+backend-path = ["."]
 
 [project]
 name = "jdMinecraftLauncher"
 description = "A classic styled Minecraft Launcher"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["JakobDev", "Minecraft", "Mojang", "launcher", "PyQt"]
@@ -34,25 +35,38 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: Implementation :: CPython"
 ]
 dependencies = [
     "PyQt6",
     "PyQt6-WebEngine",
     "minecraft-launcher-lib",
-    "jdTranslationHelper",
     "requests"
 ]
 dynamic = ["version"]
 
 [project.urls]
-Issues = "https://gitlab.com/JakobDev/jdMinecraftLauncher/-/issues"
-Source = "https://gitlab.com/JakobDev/jdMinecraftLauncher"
+Source = "https://codeberg.org/JakobDev/jdMinecraftLauncher"
+Issues = "https://codeberg.org/JakobDev/jdMinecraftLauncher/issues"
+Translate = "https://translate.codeberg.org/projects/jdMinecraftLauncher"
 Donation = "https://ko-fi.com/jakobdev"
 
 [project.scripts]
 jdMinecraftLauncher = "jdMinecraftLauncher.jdMinecraftLauncher:main"
 
-[tool.setuptools]
-packages = ["jdMinecraftLauncher"]
+[tool.setuptools.package-dir]
+jdMinecraftLauncher = "jdMinecraftLauncher"
 
 [tool.setuptools.dynamic]
 version = { file = "jdMinecraftLauncher/version.txt" }
+
+[tool.pyproject-appimage]
+script = "jdMinecraftLauncher"
+output = "jdMinecraftLauncher.AppImage"
+icon = "jdMinecraftLauncher/Icon.svg"
+rename-icon = "page.codeberg.JakobDev.jdMinecraftLauncher.png"
+desktop-entry = "deploy/page.codeberg.JakobDev.jdMinecraftLauncher.desktop"
+gettext-desktop-entry = true
+appstream = "deploy/page.codeberg.JakobDev.jdMinecraftLauncher.metainfo.xml"
+gettext-appstream = true
+gettext-directory = "deploy/translations"
+python-version = "3.11"
+
```

