# Comparing `tmp/minecraft-launcher-lib-5.3.tar.gz` & `tmp/minecraft-launcher-lib-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft-launcher-lib-5.3.tar", last modified: Sat Jan 21 13:07:36 2023, max compression
+gzip compressed data, was "minecraft-launcher-lib-6.0.tar", last modified: Fri Jun  9 11:27:23 2023, max compression
```

## Comparing `minecraft-launcher-lib-5.3.tar` & `minecraft-launcher-lib-6.0.tar`

### file list

```diff
@@ -1,30 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-21 13:07:36.277020 minecraft-launcher-lib-5.3/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      117 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4748 2023-01-21 13:07:36.277020 minecraft-launcher-lib-5.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3020 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-21 13:07:36.277020 minecraft-launcher-lib-5.3/minecraft_launcher_lib/
--rw-r--r--   0 root         (0) root         (0)      272 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/account.py
--rw-r--r--   0 root         (0) root         (0)     7887 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/command.py
--rw-r--r--   0 root         (0) root         (0)     1045 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     4778 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/fabric.py
--rw-r--r--   0 root         (0) root         (0)     8633 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/forge.py
--rw-r--r--   0 root         (0) root         (0)     8000 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/helper.py
--rw-r--r--   0 root         (0) root         (0)     7692 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/install.py
--rw-r--r--   0 root         (0) root         (0)     9865 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/microsoft_account.py
--rw-r--r--   0 root         (0) root         (0)     1384 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/microsoft_types.py
--rw-r--r--   0 root         (0) root         (0)     2667 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/natives.py
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/py.typed
--rw-r--r--   0 root         (0) root         (0)     4880 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/runtime.py
--rw-r--r--   0 root         (0) root         (0)     1941 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/types.py
--rw-r--r--   0 root         (0) root         (0)     6003 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/utils.py
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-21 13:07:36.277020 minecraft-launcher-lib-5.3/minecraft_launcher_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4748 2023-01-21 13:07:36.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      830 2023-01-21 13:07:36.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-21 13:07:36.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-01-21 13:07:36.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-01-21 13:07:36.000000 minecraft-launcher-lib-5.3/minecraft_launcher_lib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1845 2023-01-21 13:06:58.000000 minecraft-launcher-lib-5.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-21 13:07:36.277020 minecraft-launcher-lib-5.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:23.751604 minecraft-launcher-lib-6.0/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      117 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4987 2023-06-09 11:27:23.751604 minecraft-launcher-lib-6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:23.747604 minecraft-launcher-lib-6.0/minecraft_launcher_lib/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10512 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:23.747604 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/forge_types.py
+-rw-r--r--   0 root         (0) root         (0)      271 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/helper_types.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/install_types.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/mrpack_types.py
+-rw-r--r--   0 root         (0) root         (0)      815 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/runtime_types.py
+-rw-r--r--   0 root         (0) root         (0)     2587 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/shared_types.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/vanilla_launcher_types.py
+-rw-r--r--   0 root         (0) root         (0)    10945 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/command.py
+-rw-r--r--   0 root         (0) root         (0)     3479 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/fabric.py
+-rw-r--r--   0 root         (0) root         (0)    10464 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/forge.py
+-rw-r--r--   0 root         (0) root         (0)     9281 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/install.py
+-rw-r--r--   0 root         (0) root         (0)     4522 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/java_utils.py
+-rw-r--r--   0 root         (0) root         (0)    14509 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/microsoft_account.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/microsoft_types.py
+-rw-r--r--   0 root         (0) root         (0)     7692 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/mrpack.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/natives.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/py.typed
+-rw-r--r--   0 root         (0) root         (0)     5719 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/quilt.py
+-rw-r--r--   0 root         (0) root         (0)     7695 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/runtime.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/types.py
+-rw-r--r--   0 root         (0) root         (0)     6639 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8876 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/vanilla_launcher.py
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:23.747604 minecraft-launcher-lib-6.0/minecraft_launcher_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4987 2023-06-09 11:27:23.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-06-09 11:27:23.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 11:27:23.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-09 11:27:23.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-09 11:27:23.000000 minecraft-launcher-lib-6.0/minecraft_launcher_lib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 11:27:23.751604 minecraft-launcher-lib-6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:23.751604 minecraft-launcher-lib-6.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     5523 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_command.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_fabric.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_forge.py
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_install.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_java_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_microsoft_account.py
+-rw-r--r--   0 root         (0) root         (0)     6588 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_mrpack.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_natives.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_quilt.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_runtime.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3897 2023-06-09 11:26:51.000000 minecraft-launcher-lib-6.0/tests/test_vanilla_launcher.py
```

### Comparing `minecraft-launcher-lib-5.3/LICENSE` & `minecraft-launcher-lib-6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-5.3/PKG-INFO` & `minecraft-launcher-lib-6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-launcher-lib
-Version: 5.3
+Version: 6.0
 Summary: A library for creating a custom Minecraft launcher
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Documentation, https://minecraft-launcher-lib.readthedocs.io/en/stable/index.html
 Project-URL: Issues, https://codeberg.org/JakobDev/minecraft-launcher-lib/issues
 Project-URL: Source, https://codeberg.org/JakobDev/minecraft-launcher-lib
 Project-URL: Changelog, https://minecraft-launcher-lib.readthedocs.io/en/stable/changelog.html
@@ -93,20 +93,22 @@
 subprocess.call(minecraft_command)
 ```
 
 Features:
 - Easy installing
 - Get command to run Minecraft
 - Login to Microsoft account
-- Support Forge, Fabric and Liteloader
+- Supports [Forge](https://minecraftforge.net), [Fabric](https://fabricmc.net), [Quilt](https://quiltmc.org) and Liteloader
 - Old versions like alpha or beta supported
 - All functions have type annotations and docstrings
 - Only depents on [requests](https://pypi.org/project/requests)
 - Supports [PyPy](https://www.pypy.org)
 - Full Documention with tutorial online available
+- Supports reading and writing profiles of the Vanilla Launcher
+- Install of [mrpack modpacks](https://docs.modrinth.com/docs/modpacks/format_definition)
 - All public APIs are static typed
 - Examples available
 - OpenSource
 
 [View more examples](https://codeberg.org/JakobDev/minecraft-launcher-lib/src/branch/master/examples)
 
 [Read the documentation](https://minecraft-launcher-lib.readthedocs.io)
```

### Comparing `minecraft-launcher-lib-5.3/README.md` & `minecraft-launcher-lib-6.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -57,20 +57,22 @@
 subprocess.call(minecraft_command)
 ```
 
 Features:
 - Easy installing
 - Get command to run Minecraft
 - Login to Microsoft account
-- Support Forge, Fabric and Liteloader
+- Supports [Forge](https://minecraftforge.net), [Fabric](https://fabricmc.net), [Quilt](https://quiltmc.org) and Liteloader
 - Old versions like alpha or beta supported
 - All functions have type annotations and docstrings
 - Only depents on [requests](https://pypi.org/project/requests)
 - Supports [PyPy](https://www.pypy.org)
 - Full Documention with tutorial online available
+- Supports reading and writing profiles of the Vanilla Launcher
+- Install of [mrpack modpacks](https://docs.modrinth.com/docs/modpacks/format_definition)
 - All public APIs are static typed
 - Examples available
 - OpenSource
 
 [View more examples](https://codeberg.org/JakobDev/minecraft-launcher-lib/src/branch/master/examples)
 
 [Read the documentation](https://minecraft-launcher-lib.readthedocs.io)
```

### Comparing `minecraft-launcher-lib-5.3/minecraft_launcher_lib/fabric.py` & `minecraft-launcher-lib-6.0/minecraft_launcher_lib/fabric.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,61 @@
-from .helper import download_file, get_requests_response_cache, parse_maven_metadata, empty
+"fabric contains functions for dealing with the Fabric modloader"
+from ._helper import download_file, get_requests_response_cache, parse_maven_metadata, empty
 from .exceptions import VersionNotFound, UnsupportedVersion, ExternalProgramError
 from .types import FabricMinecraftVersion, FabricLoader, CallbackDict
 from .install import install_minecraft_version
 from typing import List, Optional, Union
 from .utils import is_version_valid
 import subprocess
 import tempfile
 import random
 import os
 
 
 def get_all_minecraft_versions() -> List[FabricMinecraftVersion]:
     """
-    Returns all available Minecraft Versions for fabric
+    Returns all available Minecraft Versions for Fabric
     """
     FABRIC_MINECARFT_VERSIONS_URL = "https://meta.fabricmc.net/v2/versions/game"
     return get_requests_response_cache(FABRIC_MINECARFT_VERSIONS_URL).json()
 
 
 def get_stable_minecraft_versions() -> List[str]:
     """
-    Returns a list which only contains the stable Minecraft versions that supports fabric
+    Returns a list which only contains the stable Minecraft versions that supports Fabric
     """
     minecraft_versions = get_all_minecraft_versions()
     stable_versions = []
     for i in minecraft_versions:
         if i["stable"] is True:
             stable_versions.append(i["version"])
     return stable_versions
 
 
 def get_latest_minecraft_version() -> str:
     """
-    Returns the latest unstable Minecraft versions that supports fabric. This could be a snapshot.
+    Returns the latest unstable Minecraft versions that supports Fabric. This could be a snapshot.
     """
     minecraft_versions = get_all_minecraft_versions()
     return minecraft_versions[0]["version"]
 
 
 def get_latest_stable_minecraft_version() -> str:
     """
-    Returns the latest stable Minecraft version that supports fabric
+    Returns the latest stable Minecraft version that supports Fabric
     """
     stable_versions = get_stable_minecraft_versions()
     return stable_versions[0]
 
 
 def is_minecraft_version_supported(version: str) -> bool:
     """
-    Checks if a Minecraft version supported by fabric
+    Checks if a Minecraft version supported by Fabric
+
+    :param version: A vanilla version
     """
     minecraft_versions = get_all_minecraft_versions()
     for i in minecraft_versions:
         if i["version"] == version:
             return True
     return False
 
@@ -77,43 +80,61 @@
     """
     Returns the latest installer version
     """
     FABRIC_INSTALLER_MAVEN_URL = "https://maven.fabricmc.net/net/fabricmc/fabric-installer/maven-metadata.xml"
     return parse_maven_metadata(FABRIC_INSTALLER_MAVEN_URL)["latest"]
 
 
-def install_fabric(minecraft_version: str, minecraft_directory: Union[str, os.PathLike], loader_version: str = None, callback: Optional[CallbackDict] = None, java: str = None) -> None:
+def install_fabric(minecraft_version: str, minecraft_directory: Union[str, os.PathLike], loader_version: Optional[str] = None, callback: Optional[CallbackDict] = None, java: Optional[Union[str, os.PathLike]] = None) -> None:
     """
-    Install a fabric version
+    Installs the Fabric modloader.
+
+    :param minecraft_version: A vanilla version that is supported by Fabric
+    :param minecraft_directory: The path to your Minecraft directory
+    :param loader_version: The fabric loader version. If not given it will use the latest
+    :param callback: The same dict as for :func:`~minecraft_launcher_lib.install.install_minecraft_version`
+    :param java: A Path to a custom Java executable
+
+    Raises a :class:`~minecraft_launcher_lib.exceptions.UnsupportedVersion` exception when the given minecraft version is not supported by Fabric.
     """
     path = str(minecraft_directory)
     if not callback:
         callback = {}
+
     # Check if the given version exists
     if not is_version_valid(minecraft_version, minecraft_directory):
         raise VersionNotFound(minecraft_version)
+
     # Check if the given Minecraft version supported
     if not is_minecraft_version_supported(minecraft_version):
         raise UnsupportedVersion(minecraft_version)
+
     # Get latest loader version if not given
     if not loader_version:
         loader_version = get_latest_loader_version()
+
     # Make sure the Minecraft version is installed
     install_minecraft_version(minecraft_version, path, callback=callback)
+
     # Get installer version
     installer_version = get_latest_installer_version()
     installer_download_url = f"https://maven.fabricmc.net/net/fabricmc/fabric-installer/{installer_version}/fabric-installer-{installer_version}.jar"
+
     # Generate a temporary path for downloading the installer
     installer_path = os.path.join(tempfile.gettempdir(), f"fabric-installer-{random.randrange(100,10000)}.tmp")
+
     # Download the installer
     download_file(installer_download_url, installer_path, callback=callback)
+
     # Run the installer see https://fabricmc.net/wiki/install#cli_installation
     callback.get("setStatus", empty)("Running fabric installer")
-    command = [java or "java", "-jar", installer_path, "client", "-dir", path, "-mcversion", minecraft_version, "-loader", loader_version, "-noprofile", "-snapshot"]
+    command = ["java" if java is None else str(java), "-jar", installer_path, "client", "-dir", path, "-mcversion", minecraft_version, "-loader", loader_version, "-noprofile", "-snapshot"]
     result = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     if result.returncode != 0:
         raise ExternalProgramError(command, result.stdout, result.stderr)
+
     # Delete the installer we don't need them anymore
     os.remove(installer_path)
+
     # Install all libs of fabric
     fabric_minecraft_version = f"fabric-loader-{loader_version}-{minecraft_version}"
     install_minecraft_version(fabric_minecraft_version, path, callback=callback)
```

### Comparing `minecraft-launcher-lib-5.3/minecraft_launcher_lib/forge.py` & `minecraft-launcher-lib-6.0/minecraft_launcher_lib/forge.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,192 +1,240 @@
-from .helper import download_file, get_library_path, get_jar_mainclass, parse_maven_metadata, empty
+"""
+.. note::
+    Before using this module, please read this comment from the forge developers:
+
+    .. code:: text
+
+        Please do not automate the download and installation of Forge.
+        Our efforts are supported by ads from the download page.
+        If you MUST automate this, please consider supporting the project through https://www.patreon.com/LexManos/
+
+    It's your choice, if you want to respect that and support forge.
+
+forge contains functions for dealing with the Forge modloader
+"""
+from ._helper import download_file, get_library_path, get_jar_mainclass, parse_maven_metadata, empty, extract_file_from_zip, get_classpath_separator
 from .install import install_minecraft_version, install_libraries
-from typing import Dict, List, Any, Union, Optional
+from ._internal_types.forge_types import ForgeInstallProfile
+from typing import List, Union, Optional
 from .exceptions import VersionNotFound
 from .types import CallbackDict
 import subprocess
-import platform
 import tempfile
 import random
 import zipfile
 import shutil
 import json
 import os
 
 __all__ = ["install_forge_version", "run_forge_installer", "list_forge_versions", "find_forge_version", "is_forge_version_valid", "supports_automatic_install"]
 
 
-def extract_file(handler: zipfile.ZipFile, zip_path: str, extract_path: str) -> None:
-    """
-    Extract a file from a zip handler into the given path
-    """
-    try:
-        os.makedirs(os.path.dirname(extract_path))
-    except Exception:
-        pass
-    with handler.open(zip_path, "r") as f:
-        with open(extract_path, "wb") as w:
-            w.write(f.read())
-
-
 def get_data_library_path(libname: str, path: str) -> str:
     """
     Turns the libname into a path
     """
     # Remove the []
     libname = libname[1:-1]
     libpath = os.path.join(path, "libraries")
     base_path, libname, version, extra = libname.split(":")
     for i in base_path.split("."):
         libpath = os.path.join(libpath, i)
     try:
         extra, fileend = extra.split("@")
     except ValueError:
         fileend = "jar"
-    libpath = os.path.join(libpath, libname, version, libname + "-" + version + "-" + extra + "." + fileend)
+    libpath = os.path.join(libpath, libname, version, f"{libname}-{version}-{extra}.{fileend}")
     return libpath
 
 
-def forge_processors(data: Dict[str, Any], minecraft_directory: Union[str, os.PathLike], lzma_path: str, installer_path: str, callback: CallbackDict, java: str = None) -> None:
+def forge_processors(data: ForgeInstallProfile, minecraft_directory: Union[str, os.PathLike], lzma_path: str, installer_path: str, callback: CallbackDict, java: str) -> None:
     """
     Run the processors of the install_profile.json
     """
     path = str(minecraft_directory)
+
     argument_vars = {"{MINECRAFT_JAR}": os.path.join(path, "versions", data["minecraft"], data["minecraft"] + ".jar")}
-    for key, value in data["data"].items():
-        if value["client"].startswith("[") and value["client"].endswith("]"):
-            argument_vars["{" + key + "}"] = get_data_library_path(value["client"], path)
+    for data_key, data_value in data["data"].items():
+        if data_value["client"].startswith("[") and data_value["client"].endswith("]"):
+            argument_vars["{" + data_key + "}"] = get_data_library_path(data_value["client"], path)
         else:
-            argument_vars["{" + key + "}"] = value["client"]
+            argument_vars["{" + data_key + "}"] = data_value["client"]
+
     root_path = os.path.join(tempfile.gettempdir(), "forge-root-" + str(random.randrange(1, 100000)))
     argument_vars["{INSTALLER}"] = installer_path
     argument_vars["{BINPATCH}"] = lzma_path
     argument_vars["{ROOT}"] = root_path
     argument_vars["{SIDE}"] = "client"
-    if platform.system() == "Windows":
-        classpath_seperator = ";"
-    else:
-        classpath_seperator = ":"
+
+    classpath_seperator = get_classpath_separator()
+
     callback.get("setMax", empty)(len(data["processors"]))
+
     for count, i in enumerate(data["processors"]):
         if "client" not in i.get("sides", ["client"]):
             # Skip server side only processors
             continue
         callback.get("setStatus", empty)("Running processor " + i["jar"])
         # Get the classpath
         classpath = ""
         for c in i["classpath"]:
             classpath = classpath + get_library_path(c, path) + classpath_seperator
         classpath = classpath + get_library_path(i["jar"], path)
         mainclass = get_jar_mainclass(get_library_path(i["jar"], path))
-        command = [java or "java", "-cp", classpath, mainclass]
+        command = [java, "-cp", classpath, mainclass]
         for c in i["args"]:
             var = argument_vars.get(c, c)
             if var.startswith("[") and var.endswith("]"):
                 command.append(get_library_path(var[1:-1], path))
             else:
                 command.append(var)
-        for key, value in argument_vars.items():
+        for argument_key, argument_value in argument_vars.items():
             for pos in range(len(command)):
-                command[pos] = command[pos].replace(key, value)
+                command[pos] = command[pos].replace(argument_key, argument_value)
         subprocess.call(command)
         callback.get("setProgress", empty)(count)
+
     if os.path.exists(root_path):
         shutil.rmtree(root_path)
 
 
-def install_forge_version(versionid: str, path: str, callback: Optional[CallbackDict] = None, java: Optional[str] = None) -> None:
+def install_forge_version(versionid: str, path: Union[str, os.PathLike], callback: Optional[CallbackDict] = None, java: Optional[Union[str, os.PathLike]] = None) -> None:
     """
-    Installs a forge version. Fore more information look at the documentation.
+    Installs the given Forge version
+
+    :param versionid: A Forge Version. You can get a List of Forge versions using :func:`list_forge_versions`
+    :param path: The path to your Minecraft directory
+    :param callback: The same dict as for :func:`~minecraft_launcher_lib.install.install_minecraft_version`
+    :param java: A Path to a custom Java executable
+
+    Raises a :class:`~minecraft_launcher_lib.exceptions.VersionNotFound` exception when the given forge version is not found
     """
     if callback is None:
         callback = {}
+
     FORGE_DOWNLOAD_URL = "https://files.minecraftforge.net/maven/net/minecraftforge/forge/{version}/forge-{version}-installer.jar"
     temp_file_path = os.path.join(tempfile.gettempdir(), "forge-installer-" + str(random.randrange(1, 100000)) + ".tmp")
+
     if not download_file(FORGE_DOWNLOAD_URL.format(version=versionid), temp_file_path, callback):
         raise VersionNotFound(versionid)
+
     zf = zipfile.ZipFile(temp_file_path, "r")
+
     # Read the install_profile.json
     with zf.open("install_profile.json", "r") as f:
         version_content = f.read()
-    version_data = json.loads(version_content)
-    forge_version_id = version_data["version"]
+
+    version_data: ForgeInstallProfile = json.loads(version_content)
+    forge_version_id = version_data["version"] if "version" in version_data else version_data["install"]["version"]
+    minecraft_version = version_data["minecraft"] if "minecraft" in version_data else version_data["install"]["minecraft"]
+
     # Make sure, the base version is installed
-    install_minecraft_version(version_data["minecraft"], path, callback=callback)
+    install_minecraft_version(minecraft_version, path, callback=callback)
+
     # Install all needed libs from install_profile.json
-    install_libraries(version_data, path, callback)
+    if "libraries" in version_data:
+        install_libraries(minecraft_version, version_data["libraries"], str(path), callback)
+
     # Extract the version.json
     version_json_path = os.path.join(path, "versions", forge_version_id, forge_version_id + ".json")
-    extract_file(zf, "version.json", version_json_path)
+    try:
+        extract_file_from_zip(zf, "version.json", version_json_path, minecraft_directory=path)
+    except KeyError:
+        if "versionInfo" in version_data:
+            with open(version_json_path, "w", encoding="utf-8") as f:
+                json.dump(version_data["versionInfo"], f, ensure_ascii=False, indent=4)
+
     # Extract forge libs from the installer
     forge_lib_path = os.path.join(path, "libraries", "net", "minecraftforge", "forge", versionid)
     try:
-        extract_file(zf, "maven/net/minecraftforge/forge/{version}/forge-{version}.jar".format(version=versionid), os.path.join(forge_lib_path, "forge-" + versionid + ".jar"))
-        extract_file(zf, "maven/net/minecraftforge/forge/{version}/forge-{version}-universal.jar".format(version=versionid), os.path.join(forge_lib_path, "forge-" + versionid + "-universal.jar"))
+        extract_file_from_zip(zf, "maven/net/minecraftforge/forge/{version}/forge-{version}-universal.jar".format(version=versionid), os.path.join(forge_lib_path, "forge-" + versionid + "-universal.jar"), minecraft_directory=path)
+    except KeyError:
+        pass
+    try:
+        extract_file_from_zip(zf, "forge-{version}-universal.jar".format(version=versionid), os.path.join(forge_lib_path, f"forge-{versionid}.jar"), minecraft_directory=path)
     except KeyError:
         pass
+
     # Extract the client.lzma
     lzma_path = os.path.join(tempfile.gettempdir(), "lzma-" + str(random.randrange(1, 100000)) + ".tmp")
     try:
-        extract_file(zf, "data/client.lzma", lzma_path)
+        extract_file_from_zip(zf, "data/client.lzma", lzma_path)
     except KeyError:
         pass
+
     zf.close()
+
     # Install the rest with the vanilla function
-    install_minecraft_version(forge_version_id, path, callback=callback)
+    install_minecraft_version(forge_version_id, str(path), callback=callback)
+
     # Run the processors
-    forge_processors(version_data, path, lzma_path, temp_file_path, callback, java)
+    if "processors" in version_data:
+        forge_processors(version_data, str(path), lzma_path, temp_file_path, callback, "java" if java is None else str(java))
+
     # Delete the temporary files
     os.remove(temp_file_path)
     if os.path.isfile(lzma_path):
         os.remove(lzma_path)
 
 
-def run_forge_installer(version: str, java: Optional[str] = None) -> None:
+def run_forge_installer(version: str, java: Optional[Union[str, os.PathLike]] = None) -> None:
     """
     Run the forge installer of the given forge version
+
+    :param version: A Forge Version. You can get a List of Forge versions using :func:`list_forge_versions`
+    :param java: A Path to a custom Java executable
     """
     FORGE_DOWNLOAD_URL = "https://files.minecraftforge.net/maven/net/minecraftforge/forge/{version}/forge-{version}-installer.jar"
     temp_file_path = os.path.join(tempfile.gettempdir(), "forge-" + str(random.randrange(1, 100000)) + ".tmp")
-    download_file(FORGE_DOWNLOAD_URL.format(version=version), temp_file_path, {})
-    subprocess.call([java or "java", "-jar", temp_file_path])
+
+    if not download_file(FORGE_DOWNLOAD_URL.format(version=version), temp_file_path, {}):
+        raise VersionNotFound(version)
+
+    subprocess.call(["java" if java is None else str(java), "-jar", temp_file_path])
     os.remove(temp_file_path)
 
 
 def list_forge_versions() -> List[str]:
     """
     Returns a list of all forge versions
     """
     MAVEN_METADATA_URL = "https://files.minecraftforge.net/maven/net/minecraftforge/forge/maven-metadata.xml"
     return parse_maven_metadata(MAVEN_METADATA_URL)["versions"]
 
 
 def find_forge_version(vanilla_version: str) -> Optional[str]:
     """
     Find the latest forge version that is compatible to the given vanilla version
+
+    :param vanilla_version: A vanilla Minecraft version
     """
     version_list = list_forge_versions()
     for i in version_list:
         version_split = i.split("-")
         if version_split[0] == vanilla_version:
             return i
     return None
 
 
 def is_forge_version_valid(forge_version: str) -> bool:
     """
     Checks if a forge version is valid
+
+    :param forge_version: A Forge Version
     """
     forge_version_list = list_forge_versions()
     return forge_version in forge_version_list
 
 
 def supports_automatic_install(forge_version: str) -> bool:
     """
     Checks if install_forge_version() supports the given forge version
+
+    :param forge_version: A Forge Version
     """
     try:
         vanilla_version, forge = forge_version.split("-")
         version_split = vanilla_version.split(".")
         version_number = int(version_split[1])
         if version_number >= 13:
             return True
@@ -195,14 +243,17 @@
     except Exception:
         return False
 
 
 def forge_to_installed_version(forge_version: str) -> str:
     """
     Returns the Version under which Forge will be installed from the given Forge version.
+
+    :param forge_version: A Forge Version
+
     Raises a ValueError if the Version is invalid.
     """
     try:
         vanilla_part, forge_part = forge_version.split("-")
         return f"{vanilla_part}-forge-{forge_part}"
     except ValueError:
         raise ValueError(f"{forge_version} is not a valid forge version") from None
```

### Comparing `minecraft-launcher-lib-5.3/minecraft_launcher_lib/install.py` & `minecraft-launcher-lib-6.0/minecraft_launcher_lib/install.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,143 +1,187 @@
-from .helper import download_file, parse_rule_list, inherit_json, empty, get_user_agent
+"install allows you to install minecraft."
+from ._helper import download_file, parse_rule_list, inherit_json, empty, get_user_agent, check_path_inside_minecraft_directory
+from ._internal_types.shared_types import ClientJson, ClientJsonLibrary
 from .natives import extract_natives_file, get_natives
-from typing import Any, Dict, Optional, Union
-from .exceptions import VersionNotFound
+from ._internal_types.install_types import AssetsJson
 from .runtime import install_jvm_runtime
+from typing import List, Optional, Union
+from .exceptions import VersionNotFound
 from .types import CallbackDict
 import requests
 import shutil
 import json
 import os
 
 __all__ = ["install_minecraft_version"]
 
 
-def install_libraries(data: Dict[str, Any], path: str, callback: CallbackDict) -> None:
+def install_libraries(id: str, libraries: List[ClientJsonLibrary], path: str, callback: CallbackDict) -> None:
     """
     Install all libraries
     """
     session = requests.session()
     callback.get("setStatus", empty)("Download Libraries")
-    callback.get("setMax", empty)(len(data["libraries"]) - 1)
-    for count, i in enumerate(data["libraries"]):
+    callback.get("setMax", empty)(len(libraries) - 1)
+    for count, i in enumerate(libraries):
         # Check, if the rules allow this lib for the current system
-        if not parse_rule_list(i, "rules", {}):
+        if "rules" in i and not parse_rule_list(i["rules"], {}):
             continue
+
         # Turn the name into a path
-        currentPath = os.path.join(path, "libraries")
+        current_path = os.path.join(path, "libraries")
         if "url" in i:
             if i["url"].endswith("/"):
-                downloadUrl = i["url"][:-1]
+                download_url = i["url"][:-1]
             else:
-                downloadUrl = i["url"]
+                download_url = i["url"]
         else:
-            downloadUrl = "https://libraries.minecraft.net"
+            download_url = "https://libraries.minecraft.net"
+
         try:
-            libPath, name, version = i["name"].split(":")[0:3]
+            lib_path, name, version = i["name"].split(":")[0:3]
         except ValueError:
             continue
-        for libPart in libPath.split("."):
-            currentPath = os.path.join(currentPath, libPart)
-            downloadUrl = downloadUrl + "/" + libPart
+
+        for lib_part in lib_path.split("."):
+            current_path = os.path.join(current_path, lib_part)
+            download_url = f"{download_url}/{lib_part}"
+
         try:
             version, fileend = version.split("@")
         except ValueError:
             fileend = "jar"
-        jarFilename = name + "-" + version + "." + fileend
-        downloadUrl = downloadUrl + "/" + name + "/" + version
-        currentPath = os.path.join(currentPath, name, version)
+
+        jar_filename = f"{name}-{version}.{fileend}"
+        download_url = f"{download_url}/{name}/{version}"
+        current_path = os.path.join(current_path, name, version)
         native = get_natives(i)
+
         # Check if there is a native file
         if native != "":
-            jarFilenameNative = name + "-" + version + "-" + native + ".jar"
-        jarFilename = name + "-" + version + "." + fileend
-        downloadUrl = downloadUrl + "/" + jarFilename
+            jar_filename_native = f"{name}-{version}-{native}.jar"
+        jar_filename = f"{name}-{version}.{fileend}"
+        download_url = f"{download_url}/{jar_filename}"
+
         # Try to download the lib
         try:
-            download_file(downloadUrl, os.path.join(currentPath, jarFilename), callback=callback, session=session)
+            download_file(download_url, os.path.join(current_path, jar_filename), callback=callback, session=session, minecraft_directory=path)
         except Exception:
             pass
+
         if "downloads" not in i:
             if "extract" in i:
-                extract_natives_file(os.path.join(currentPath, jarFilenameNative), os.path.join(path, "versions", data["id"], "natives"), i["extract"])
+                extract_natives_file(os.path.join(current_path, jar_filename_native), os.path.join(path, "versions", id, "natives"), i["extract"])
             continue
+
         if "artifact" in i["downloads"]:
-            download_file(i["downloads"]["artifact"]["url"], os.path.join(path, "libraries", i["downloads"]["artifact"]["path"]), callback, sha1=i["downloads"]["artifact"]["sha1"], session=session)
+            download_file(i["downloads"]["artifact"]["url"], os.path.join(path, "libraries", i["downloads"]["artifact"]["path"]), callback, sha1=i["downloads"]["artifact"]["sha1"], session=session, minecraft_directory=path)
         if native != "":
-            download_file(i["downloads"]["classifiers"][native]["url"], os.path.join(currentPath, jarFilenameNative), callback, sha1=i["downloads"]["classifiers"][native]["sha1"], session=session)
+            download_file(i["downloads"]["classifiers"][native]["url"], os.path.join(current_path, jar_filename_native), callback, sha1=i["downloads"]["classifiers"][native]["sha1"], session=session, minecraft_directory=path)  # type: ignore
             if "extract" in i:
-                extract_natives_file(os.path.join(currentPath, jarFilenameNative), os.path.join(path, "versions", data["id"], "natives"), i["extract"])
+                extract_natives_file(os.path.join(current_path, jar_filename_native), os.path.join(path, "versions", id, "natives"), i["extract"])
+
         callback.get("setProgress", empty)(count)
 
 
-def install_assets(data: Dict[str, Any], path: str, callback: CallbackDict) -> None:
+def install_assets(data: ClientJson, path: str, callback: CallbackDict) -> None:
     """
     Install all assets
     """
-    # Old versions dosen't have this
+    # Old versions don't have this
     if "assetIndex" not in data:
         return
+
     callback.get("setStatus", empty)("Download Assets")
     session = requests.session()
+
     # Download all assets
     download_file(data["assetIndex"]["url"], os.path.join(path, "assets", "indexes", data["assets"] + ".json"), callback, sha1=data["assetIndex"]["sha1"], session=session)
     with open(os.path.join(path, "assets", "indexes", data["assets"] + ".json")) as f:
-        assets_data = json.load(f)
+        assets_data: AssetsJson = json.load(f)
+
     # The assets has a hash. e.g. c4dbabc820f04ba685694c63359429b22e3a62b5
     # With this hash, it can be download from https://resources.download.minecraft.net/c4/c4dbabc820f04ba685694c63359429b22e3a62b5
     # And saved at assets/objects/c4/c4dbabc820f04ba685694c63359429b22e3a62b5
     callback.get("setMax", empty)(len(assets_data["objects"]) - 1)
     count = 0
-    for key, value in assets_data["objects"].items():
-        download_file("https://resources.download.minecraft.net/" + value["hash"][:2] + "/" + value["hash"], os.path.join(path, "assets", "objects", value["hash"][:2], value["hash"]), callback, sha1=value["hash"], session=session)
+    for value in assets_data["objects"].values():
+        download_file("https://resources.download.minecraft.net/" + value["hash"][:2] + "/" + value["hash"], os.path.join(path, "assets", "objects", value["hash"][:2], value["hash"]), callback, sha1=value["hash"], session=session, minecraft_directory=path)
         count += 1
         callback.get("setProgress", empty)(count)
 
 
 def do_version_install(versionid: str, path: str, callback: CallbackDict, url: Optional[str] = None, sha1: Optional[str] = None) -> None:
     """
-    Install the given version
+    Installs the given version
     """
     # Download and read versions.json
     if url:
-        download_file(url, os.path.join(path, "versions", versionid, versionid + ".json"), callback, sha1=sha1)
+        download_file(url, os.path.join(path, "versions", versionid, versionid + ".json"), callback, sha1=sha1, minecraft_directory=path)
+
     with open(os.path.join(path, "versions", versionid, versionid + ".json")) as f:
-        versiondata = json.load(f)
+        versiondata: ClientJson = json.load(f)
+
     # For Forge
     if "inheritsFrom" in versiondata:
         try:
             install_minecraft_version(versiondata["inheritsFrom"], path, callback=callback)
         except VersionNotFound:
             pass
         versiondata = inherit_json(versiondata, path)
-    install_libraries(versiondata, path, callback)
+
+    install_libraries(versiondata["id"], versiondata["libraries"], path, callback)
     install_assets(versiondata, path, callback)
+
     # Download logging config
     if "logging" in versiondata:
         if len(versiondata["logging"]) != 0:
             logger_file = os.path.join(path, "assets", "log_configs", versiondata["logging"]["client"]["file"]["id"])
-            download_file(versiondata["logging"]["client"]["file"]["url"], logger_file, callback, sha1=versiondata["logging"]["client"]["file"]["sha1"])
+            download_file(versiondata["logging"]["client"]["file"]["url"], logger_file, callback, sha1=versiondata["logging"]["client"]["file"]["sha1"], minecraft_directory=path)
+
     # Download minecraft.jar
     if "downloads" in versiondata:
-        download_file(versiondata["downloads"]["client"]["url"], os.path.join(path, "versions", versiondata["id"], versiondata["id"] + ".jar"), callback, sha1=versiondata["downloads"]["client"]["sha1"])
+        download_file(versiondata["downloads"]["client"]["url"], os.path.join(path, "versions", versiondata["id"], versiondata["id"] + ".jar"), callback, sha1=versiondata["downloads"]["client"]["sha1"], minecraft_directory=path)
+
     # Need to copy jar for old forge versions
     if not os.path.isfile(os.path.join(path, "versions", versiondata["id"], versiondata["id"] + ".jar")) and "inheritsFrom" in versiondata:
-        inheritsFrom = versiondata["inheritsFrom"]
-        shutil.copyfile(os.path.join(path, "versions", versiondata["id"], versiondata["id"] + ".jar"), os.path.join(path, "versions", inheritsFrom, inheritsFrom + ".jar"))
+        inherits_from = versiondata["inheritsFrom"]
+        inherit_path = os.path.join(path, "versions", inherits_from, f"{inherits_from}.jar")
+        check_path_inside_minecraft_directory(path, inherit_path)
+        shutil.copyfile(os.path.join(path, "versions", versiondata["id"], versiondata["id"] + ".jar"), inherit_path)
+
     # Install java runtime if needed
     if "javaVersion" in versiondata:
         callback.get("setStatus", empty)("Install java runtime")
         install_jvm_runtime(versiondata["javaVersion"]["component"], path, callback=callback)
+
     callback.get("setStatus", empty)("Installation complete")
 
 
 def install_minecraft_version(versionid: str, minecraft_directory: Union[str, os.PathLike], callback: Optional[CallbackDict] = None) -> None:
     """
-    Install a Minecraft Version. Fore more Information take a look at the documentation"
+    Installs a minecraft version into the given path. e.g. ``install_version("1.14", "/tmp/minecraft")``. Use :func:`~minecraft_launcher_lib.utils.get_minecraft_directory` to get the default Minecraft directory.
+
+    :param versionid: The Minecraft version
+    :param minecraft_directory: The path to your Minecraft directory
+    :param callback: Some functions that are called to monitor the progress (see below)
+    :raises VersionNotFound: The Minecraft version was not found
+    :raises FileOutsideMinecraftDirectory: A File should be placed outside the given Minecraft directory
+
+    ``callback`` is a dict with functions that are called with arguments to get the progress. You can use it to show the progress to the user.
+
+    .. code:: python
+
+        callback = {
+            "setStatus": some_function, # This function is called to set a text
+            "setProgress" some_function, # This function is called to set the progress.
+            "setMax": some_function, # This function is called to set to max progress.
+        }
+
+    Files that are already exists will not be replaced.
     """
     if isinstance(minecraft_directory, os.PathLike):
         minecraft_directory = str(minecraft_directory)
     if callback is None:
         callback = {}
     if os.path.isfile(os.path.join(minecraft_directory, "versions", versionid, f"{versionid}.json")):
         do_version_install(versionid, minecraft_directory, callback)
```

### Comparing `minecraft-launcher-lib-5.3/minecraft_launcher_lib/microsoft_account.py` & `minecraft-launcher-lib-6.0/minecraft_launcher_lib/microsoft_account.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,35 @@
+"""
+microsoft_account contains functions for login with a Microsoft Account. Before using this module you need to `create a Azure application <https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app>`_.
+Many thanks to wiki.vg for it's `documentation of the login process <https://wiki.vg/Microsoft_Authentication_Scheme>`_.
+You may want to read the :doc:`/tutorial/microsoft_login` tutorial before using this module.
+For a list of all types see :doc:`microsoft_types`.
+"""
 from .microsoft_types import AuthorizationTokenResponse, XBLResponse, XSTSResponse, MinecraftAuthenticateResponse, MinecraftStoreResponse, MinecraftProfileResponse, CompleteLoginResponse
 from typing import Literal, Optional, Tuple, cast
+from ._helper import get_user_agent, assert_func
 from .exceptions import InvalidRefreshToken
 from base64 import urlsafe_b64encode
-from .helper import get_user_agent
 from hashlib import sha256
 import urllib.parse
 import requests
 import secrets
 
 __AUTH_URL__ = "https://login.microsoftonline.com/consumers/oauth2/v2.0/authorize"
 __TOKEN_URL__ = "https://login.microsoftonline.com/consumers/oauth2/v2.0/token"
 __SCOPE__ = "XboxLive.signin offline_access"
 
 
 def get_login_url(client_id: str, redirect_uri: str) -> str:
     """
     Generate a login url.\\
-    For a more secure alternative, use get_secure_login_data()
+    For a more secure alternative, use :func:`get_secure_login_data`
 
+    :param client_id: The Client ID of your Azure App
+    :param redirect_uri: The Redirect URI of your Azure App
     :return: The url to the website on which the user logs in
     """
     parameters = {
         "client_id": client_id,
         "response_type": "code",
         "redirect_uri": redirect_uri,
         "response_mode": "query",
@@ -37,30 +45,32 @@
     Generates the PKCE code challenge and code verifier
 
     :return: A tuple containing the code_verifier, the code_challenge and the code_challenge_method.
     """
     code_verifier = secrets.token_urlsafe(128)[:128]
     code_challenge = urlsafe_b64encode(sha256(code_verifier.encode("ascii")).digest()).decode("ascii")[:-1]
     code_challenge_method = "S256"
-    return code_verifier, code_challenge, code_challenge_method
+    return code_verifier, code_challenge, cast(Literal["plain", "S256"], code_challenge_method)
 
 
 def generate_state() -> str:
     """
     Generates a random state
     """
     return secrets.token_urlsafe(16)
 
 
 def get_secure_login_data(client_id: str, redirect_uri: str, state: Optional[str] = None) -> Tuple[str, str, str]:
     """
     Generates the login data for a secure login with pkce and state.\\
     Prevents Cross-Site Request Forgery attacks and authorization code injection attacks.
 
-    :return: The url to the website on which the user logs in, the state and the code verifier
+    :param client_id: The Client ID of your Azure App
+    :param redirect_uri: The Redirect URI of your Azure App
+    :param state: You can use a existing state. If not set, a state will be generated using :func:`generate_state`.
     """
     code_verifier, code_challenge, code_challenge_method = _generate_pkce_data()
 
     if state is None:
         state = generate_state()
 
     parameters = {
@@ -78,52 +88,64 @@
 
     return url, state, code_verifier
 
 
 def url_contains_auth_code(url: str) -> bool:
     """
     Checks if the given url contains a authorization code
+
+    :param url: The URL to check
     """
     parsed = urllib.parse.urlparse(url)
     qs = urllib.parse.parse_qs(parsed.query)
     return "code" in qs
 
 
 def get_auth_code_from_url(url: str) -> Optional[str]:
     """
     Get the authorization code from the url.\\
-    If you want to check the state, use parse_auth_code_url(), which throws errors instead of returning an optional value.
+    If you want to check the state, use :func:`parse_auth_code_url`, which throws errors instead of returning an optional value.
 
+    :param url: The URL to parse
     :return: The auth code or None if the the code is nonexistent
     """
     parsed = urllib.parse.urlparse(url)
     qs = urllib.parse.parse_qs(parsed.query)
     try:
         return qs["code"][0]
     except KeyError:
         return None
 
 
 def parse_auth_code_url(url: str, state: Optional[str]) -> str:
     """
     Parse the authorization code url and checks the state.
+
+    :param url: The URL to parse
+    :param state: If set, the function raises a AssertionError, if the state do no match the state in the URL
     :return: The auth code
     """
     parsed = urllib.parse.urlparse(url)
     qs = urllib.parse.parse_qs(parsed.query)
 
     if state is not None:
-        assert state == qs["state"][0]
+        assert_func(state == qs["state"][0])
 
     return qs["code"][0]
 
 
 def get_authorization_token(client_id: str, client_secret: Optional[str], redirect_uri: str, auth_code: str, code_verifier: Optional[str] = None) -> AuthorizationTokenResponse:
     """
-    Get the authorization token
+    Get the authorization token. This function is called during :func:`complete_login`, so you need to use this function ony if :func:`complete_login` doesnt't work for you.
+
+    :param client_id: The Client ID of your Azure App
+    :param client_secret: The Client Secret of your Azure App. This is deprecated and should not been used anymore.
+    :param redirect_uri: The Redirect URI of your Azure App
+    :param auth_code: The Code you get from :func:`parse_auth_code_url`
+    :param code_verifier: The 3rd entry in the Tuple you get from :func:`get_secure_login_data`
     """
     parameters = {
         "client_id": client_id,
         "scope": __SCOPE__,
         "code": auth_code,
         "redirect_uri": redirect_uri,
         "grant_type": "authorization_code",
@@ -141,15 +163,20 @@
     }
     r = requests.post(__TOKEN_URL__, data=parameters, headers=header)
     return r.json()
 
 
 def refresh_authorization_token(client_id: str, client_secret: Optional[str], redirect_uri: Optional[str], refresh_token: str) -> AuthorizationTokenResponse:
     """
-    Refresh the authorization token
+    Refresh the authorization token. This function is called during :func:`complete_refresh`, so you need to use this function ony if :func:`complete_refresh` doesnt't work for you.
+
+    :param client_id: The Client ID of your Azure App
+    :param client_secret: The Client Secret of your Azure App. This is deprecated and should not been used anymore.
+    :param redirect_uri: The Redirect URI of Azure App. This Parameter only exists for backwards compatibility and is not used anymore.
+    :param refresh_token: Your refresh token
     """
     parameters = {
         "client_id": client_id,
         "scope": __SCOPE__,
         "refresh_token": refresh_token,
         "grant_type": "refresh_token"
     }
@@ -166,15 +193,17 @@
     }
     r = requests.post("https://login.live.com/oauth20_token.srf", data=parameters, headers=header)
     return r.json()
 
 
 def authenticate_with_xbl(access_token: str) -> XBLResponse:
     """
-    Authenticate with Xbox Live
+    Authenticate with Xbox Live. This function is called during :func:`complete_login`, so you need to use this function ony if :func:`complete_login` doesnt't work for you.
+
+    :param access_token: The Token you get from :func:`get_authorization_token`
     """
     parameters = {
         "Properties": {
             "AuthMethod": "RPS",
             "SiteName": "user.auth.xboxlive.com",
             "RpsTicket": f"d={access_token}"
         },
@@ -188,15 +217,17 @@
     }
     r = requests.post("https://user.auth.xboxlive.com/user/authenticate", json=parameters, headers=header)
     return r.json()
 
 
 def authenticate_with_xsts(xbl_token: str) -> XSTSResponse:
     """
-    Authenticate with XSTS
+    Authenticate with XSTS. This function is called during :func:`complete_login`, so you need to use this function ony if :func:`complete_login` doesnt't work for you.
+
+    :param xbl_token: The Token you get from :func:`authenticate_with_xbl`
     """
     parameters = {
         "Properties": {
             "SandboxId": "RETAIL",
             "UserTokens": [
                 xbl_token
             ]
@@ -211,15 +242,18 @@
     }
     r = requests.post("https://xsts.auth.xboxlive.com/xsts/authorize", json=parameters, headers=header)
     return r.json()
 
 
 def authenticate_with_minecraft(userhash: str, xsts_token: str) -> MinecraftAuthenticateResponse:
     """
-    Authenticate with Minecraft
+    Authenticate with Minecraft. This function is called during :func:`complete_login`, so you need to use this function ony if :func:`complete_login` doesnt't work for you.
+
+    :param userhash: The Hash you get from :func:`authenticate_with_xbl`
+    :param xsts_token: The Token you get from :func:`authenticate_with_xsts`
     """
     parameters = {
         "identityToken": f"XBL3.0 x={userhash};{xsts_token}"
     }
     header = {
         "Content-Type": "application/json",
         "user-agent": get_user_agent(),
@@ -227,39 +261,68 @@
     }
     r = requests.post("https://api.minecraftservices.com/authentication/login_with_xbox", json=parameters, headers=header)
     return r.json()
 
 
 def get_store_information(access_token: str) -> MinecraftStoreResponse:
     """
-    Get the store information
+    Get the store information.
+
+    :param access_token: The Token you get from :func:`authenticate_with_minecraft`
     """
     header = {
         "Authorization": f"Bearer {access_token}",
         "user-agent": get_user_agent()
     }
     r = requests.get("https://api.minecraftservices.com/entitlements/mcstore", headers=header)
     return r.json()
 
 
 def get_profile(access_token: str) -> MinecraftProfileResponse:
     """
-    Get the profile
+    Get the profile. This function is called during :func:`complete_login`, so you need to use this function ony if :func:`complete_login` doesnt't work for you.
+
+    :param access_token: The Token you get from :func:`authenticate_with_minecraft`
     """
     header = {
         "Authorization": f"Bearer {access_token}",
         "user-agent": get_user_agent()
     }
     r = requests.get("https://api.minecraftservices.com/minecraft/profile", headers=header)
     return r.json()
 
 
 def complete_login(client_id: str, client_secret: Optional[str], redirect_uri: str, auth_code: str, code_verifier: Optional[str] = None) -> CompleteLoginResponse:
     """
-    Do the complete login process
+    Do the complete login process.
+
+    :param client_id: The Client ID of your Azure App
+    :param client_secret: The Client Secret of your Azure App. This is deprecated and should not been used anymore.
+    :param redirect_uri: The Redirect URI of your Azure App
+    :param auth_code: The Code you get from :func:`parse_auth_code_url`
+    :param code_verifier: The 3rd entry in the Tuple you get from :func:`get_secure_login_data`
+
+    It returns the following:
+
+    .. code:: json
+
+        {
+            "id" : "The uuid",
+            "name" : "The username",
+            "access_token": "The acces token",
+            "refresh_token": "The refresh token",
+            "skins" : [{
+                "id" : "6a6e65e5-76dd-4c3c-a625-162924514568",
+                "state" : "ACTIVE",
+                "url" : "http://textures.minecraft.net/texture/1a4af718455d4aab528e7a61f86fa25e6a369d1768dcb13f7df319a713eb810b",
+                "variant" : "CLASSIC",
+                "alias" : "STEVE"
+            } ],
+            "capes" : []
+        }
     """
     token_request = get_authorization_token(client_id, client_secret, redirect_uri, auth_code, code_verifier)
     token = token_request["access_token"]
 
     xbl_request = authenticate_with_xbl(token)
     xbl_token = xbl_request["Token"]
     userhash = xbl_request["DisplayClaims"]["xui"][0]["uhs"]
@@ -276,15 +339,22 @@
     profile["refresh_token"] = token_request["refresh_token"]
 
     return profile
 
 
 def complete_refresh(client_id: str, client_secret: Optional[str], redirect_uri: Optional[str], refresh_token: str) -> CompleteLoginResponse:
     """
-    Do the complete login process with a refresh token
+    Do the complete login process with a refresh token. It returns the same as :func:`complete_login`.
+
+    :param client_id: The Client ID of your Azure App
+    :param client_secret: The Client Secret of your Azure App. This is deprecated and should not been used anymore.
+    :param redirect_uri: The Redirect URI of Azure App. This Parameter only exists for backwards compatibility and is not used anymore.
+    :param refresh_token: Your refresh token
+
+    Raises a :class:`~minecraft_launcher_lib.exceptions.InvalidRefreshToken` exception when the refresh token is invalid.
     """
     token_request = refresh_authorization_token(client_id, client_secret, redirect_uri, refresh_token)
 
     if "error" in token_request:
         raise InvalidRefreshToken()
 
     token = token_request["access_token"]
```

### Comparing `minecraft-launcher-lib-5.3/minecraft_launcher_lib/microsoft_types.py` & `minecraft-launcher-lib-6.0/minecraft_launcher_lib/microsoft_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This module contains all Types for the :doc:`microsoft_account` module.
+It has it's own module because of the many types needed that are not used somewhere else.
+"""
 from typing import Any, Literal, TypedDict, List
 
 
 class AuthorizationTokenResponse(TypedDict):
     access_token: str
     token_type: Literal["Bearer"]
     expires_in: int
```

### Comparing `minecraft-launcher-lib-5.3/minecraft_launcher_lib/types.py` & `minecraft-launcher-lib-6.0/minecraft_launcher_lib/_internal_types/shared_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-from typing import Literal, TypedDict, List, Callable
-import datetime
+from typing import List, Dict, Union, Literal, TypedDict
 
 
-class MinecraftOptions(TypedDict, total=False):
-    username: str
-    uuid: str
-    token: str
-    executablePath: str
-    defaultExecutablePath: str
-    jvmArguments: List[str]
-    launcherName: str
-    launcherVersion: str
-    gameDirectory: str
-    demo: bool
-    customResolution: bool
-    resolutionWidth: str
-    resolutionHeight: str
-    server: str
-    port: str
-    nativesDirectory: str
-    enableLoggingConfig: bool
-    disableMultiplayer: bool
-    disableChat: bool
-
-
-class CallbackDict(TypedDict, total=False):
-    setStatus: Callable[[str], None]
-    setProgress: Callable[[int], None]
-    setMax: Callable[[int], None]
-
-
-class LatestMinecraftVersions(TypedDict):
-    release: str
-    snapshot: str
+class ClientJsonRule(TypedDict):
+    action: Literal["allow", "disallow"]
+    os: Dict[Literal["name", "arch", "vesion"], str]
+    features: Dict[Literal["has_custom_resolution", "is_demo_user", "has_quick_plays_support", "is_quick_play_singleplayer", "is_quick_play_multiplayer", "is_quick_play_realms"], bool]
 
 
-class MinecraftVersionInfo(TypedDict):
+class ClientJsonArgumentRule(TypedDict, total=False):
+    compatibilityRules: List[ClientJsonRule]
+    rules: List[ClientJsonRule]
+    value: Union[str, List[str]]
+
+
+class _ClientJsonAssetIndex(TypedDict):
     id: str
-    type: str
-    releaseTime: datetime.datetime
-    complianceLevel: int
+    sha1: str
+    size: int
+    totalSize: int
+    url: str
 
 
-class FabricMinecraftVersion(TypedDict):
-    version: str
-    stable: bool
+class _ClientJsonDownloads(TypedDict):
+    sha1: str
+    size: int
+    url: str
 
 
-class FabricLoader(TypedDict):
-    separator: str
-    build: int
-    maven: str
-    version: str
-    stable: bool
+class _ClientJsonJavaVersion(TypedDict):
+    component: str
+    majorVersion: int
 
 
-# ----
-# News
-# ----
+class _ClientJsonLibraryDownloadsArtifact(TypedDict):
+    path: str
+    url: str
+    sha1: str
+    size: int
 
 
-class _ImageBase(TypedDict):
-    content_type: Literal["image", "outgoing-link", "video"]
-    imageURL: str
+class _ClientJsonLibraryDownloads(TypedDict, total=False):
+    artifact: _ClientJsonLibraryDownloadsArtifact
+    classifiers: Dict[Literal["javadoc", "natives-linux", "natives-macos", "natives-windows", "sources"], _ClientJsonLibraryDownloadsArtifact]
 
 
-class Image(_ImageBase, total=False):
-    alt: str
-    videoURL: str
-    videoType: str
-    videoProvider: str
-    videoId: str
-    linkurl: str
-    background_color: Literal["bg-blue", "bg-green", "bg-red"]
+class ClientJsonLibrary(TypedDict, total=False):
+    name: str
+    downloads: _ClientJsonLibraryDownloads
+    extract: Dict[Literal["exclude"], List[str]]
+    rules: List[ClientJsonRule]
+    natives: Dict[Literal["linux", "osx", "windows"], str]
+    url: str
+
+
+class _ClientJsonLoggingFile(TypedDict):
+    id: str
+    sha1: str
+    size: int
+    url: str
 
 
-class Tile(TypedDict):
-    sub_header: str
-    image: Image
-    tile_size: Literal["1x1", "1x2", "2x1", "2x2", "4x2"]
-    title: str
+class _ClientJsonLogging(TypedDict):
+    argument: str
+    file: _ClientJsonLoggingFile
+    type: str
 
 
-class _ArticleBase(TypedDict):
-    default_tile: Tile
-    articleLang: Literal["en-us"]
-    primary_category: str
-    categories: List[str]
-    article_url: str
-    publish_date: str
-    tags: List[str]
+class ClientJson(TypedDict, total=False):
+    id: str
+    jar: str
+    arguments: Dict[Literal["game", "jvm"], List[Union[str, ClientJsonArgumentRule]]]
+    minecraftArguments: str
+    assetIndex: _ClientJsonAssetIndex
+    assets: str
+    downloads: Dict[Literal["client", "client_mappings", "server", "server_mappings"], _ClientJsonDownloads]
+    javaVersion: _ClientJsonJavaVersion
+    libraries: List[ClientJsonLibrary]
+    logging: Dict[Literal["client"], _ClientJsonLogging]
+    mainClass: str
+    minimumLauncherVersion: int
+    releaseTime: str
+    time: str
+    type: str
+    complianceLevel: int
+    inheritsFrom: str
 
 
-class Article(_ArticleBase, total=False):
-    preferred_tile: Tile
+class _VersionListManifestJsonVersion(TypedDict):
+    id: str
+    type: str
+    url: str
+    time: str
+    releaseTime: str
+    sha1: str
+    complianceLevel: int
 
 
-class Articles(TypedDict):
-    article_grid: List[Article]
-    article_count: int
+class VersionListManifestJson(TypedDict):
+    latest: Dict[Literal["release", "snapshot"], str]
+    versions: List[_VersionListManifestJsonVersion]
```

### Comparing `minecraft-launcher-lib-5.3/minecraft_launcher_lib/utils.py` & `minecraft-launcher-lib-6.0/minecraft_launcher_lib/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+"utils contains a few functions for helping you that doesn't fit in any other category"
 from .types import Articles, MinecraftOptions, LatestMinecraftVersions, MinecraftVersionInfo
-from .helper import get_requests_response_cache
+from ._internal_types.shared_types import ClientJson, VersionListManifestJson
+from ._helper import get_requests_response_cache
 from typing import List, Union
 from datetime import datetime
 import platform
 import requests
 import random
 import pathlib
 import shutil
@@ -31,72 +33,83 @@
     return get_requests_response_cache("https://launchermeta.mojang.com/mc/game/version_manifest_v2.json").json()["latest"]
 
 
 def get_version_list() -> List[MinecraftVersionInfo]:
     """
     Returns all versions that Mojang offers to download
     """
-    vlist = get_requests_response_cache("https://launchermeta.mojang.com/mc/game/version_manifest_v2.json").json()
-    returnlist = []
+    vlist: VersionListManifestJson = get_requests_response_cache("https://launchermeta.mojang.com/mc/game/version_manifest_v2.json").json()
+    returnlist: List[MinecraftVersionInfo] = []
     for i in vlist["versions"]:
         returnlist.append({"id": i["id"], "type": i["type"], "releaseTime": datetime.fromisoformat(i["releaseTime"]), "complianceLevel": i["complianceLevel"]})
     return returnlist
 
 
 def get_installed_versions(minecraft_directory: Union[str, os.PathLike]) -> List[MinecraftVersionInfo]:
     """
     Returns all installed versions
+
+    :param minecraft_directory: The path to your Minecraft directory
     """
     try:
         dir_list = os.listdir(os.path.join(minecraft_directory, "versions"))
     except FileNotFoundError:
         return []
-    version_list = []
+
+    version_list: List[MinecraftVersionInfo] = []
     for i in dir_list:
         if not os.path.isfile(os.path.join(minecraft_directory, "versions", i, i + ".json")):
             continue
+
         with open(os.path.join(minecraft_directory, "versions", i, i + ".json"), "r", encoding="utf-8") as f:
-            version_data = json.load(f)
+            version_data: ClientJson = json.load(f)
+
         try:
             release_time = datetime.fromisoformat(version_data["releaseTime"])
         except ValueError:
             # In case some custom client has a invalid time
             release_time = datetime.fromtimestamp(0)
+
         version_list.append({"id": version_data["id"], "type": version_data["type"], "releaseTime": release_time, "complianceLevel": version_data.get("complianceLevel", 0)})
     return version_list
 
 
 def get_available_versions(minecraft_directory: Union[str, os.PathLike]) -> List[MinecraftVersionInfo]:
     """
     Returns all installed versions and all versions that Mojang offers to download
+
+    :param minecraft_directory: The path to your Minecraft directory
     """
     version_list = []
     version_check = []
+
     for i in get_version_list():
         version_list.append(i)
         version_check.append(i["id"])
+
     for i in get_installed_versions(minecraft_directory):
         if not i["id"] in version_check:
             version_list.append(i)
+
     return version_list
 
 
 def get_java_executable() -> str:
     """
     Tries the find out the path to the default java executable
     """
     if platform.system() == "Windows":
-        if os.getenv("JAVA_HOME"):
-            return os.path.join(os.getenv("JAVA_HOME"), "bin", "javaw.exe")
+        if (java_home := os.getenv("JAVA_HOME")) is not None:
+            return os.path.join(java_home, "bin", "javaw.exe")
         elif os.path.isfile(r"C:\Program Files (x86)\Common Files\Oracle\Java\javapath\javaw.exe"):
             return r"C:\Program Files (x86)\Common Files\Oracle\Java\javapath\javaw.exe"
         else:
             return shutil.which("javaw") or "javaw"
-    elif os.getenv("JAVA_HOME"):
-        return os.path.join(os.getenv("JAVA_HOME"), "bin", "java")
+    elif (java_home := os.getenv("JAVA_HOME")) is not None:
+        return os.path.join(java_home, "bin", "java")
     elif platform.system() == "Darwin":
         return shutil.which("java") or "java"
     else:
         if os.path.islink("/etc/alternatives/java"):
             return os.readlink("/etc/alternatives/java")
         elif os.path.islink("/usr/lib/jvm/default-runtime"):
             return os.path.join("/usr", "lib", "jvm", os.readlink("/usr/lib/jvm/default-runtime"), "bin", "java")
@@ -130,39 +143,46 @@
         "token": ""
     }
 
 
 def is_version_valid(version: str, minecraft_directory: Union[str, os.PathLike]) -> bool:
     """
     Checks if the given version exists
+
+    :param version: A Minecraft version
+    :param minecraft_directory: The path to your Minecraft directory
     """
     if os.path.isdir(os.path.join(minecraft_directory, "versions", version)):
         return True
     for i in get_version_list():
         if i["id"] == version:
             return True
     return False
 
 
 def get_minecraft_news(page_size: int = 20) -> Articles:
     """
     Get the news from minecraft.net
+
+    :param page_size: The Page Size (default 20)
     """
     parameters = {
         "pageSize": page_size
     }
     header = {
         "user-agent": f"minecraft-launcher-lib/{get_library_version()}"
     }
     return requests.get("https://www.minecraft.net/content/minecraft-net/_jcr_content.articles.grid", params=parameters, headers=header).json()
 
 
 def is_vanilla_version(version: str) -> bool:
     """
     Checks if the given version is a vanilla version
+
+    :param version: A Minecraft version
     """
     for i in get_version_list():
         if i["id"] == version:
             return True
     return False
```

### Comparing `minecraft-launcher-lib-5.3/minecraft_launcher_lib.egg-info/PKG-INFO` & `minecraft-launcher-lib-6.0/minecraft_launcher_lib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-launcher-lib
-Version: 5.3
+Version: 6.0
 Summary: A library for creating a custom Minecraft launcher
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Documentation, https://minecraft-launcher-lib.readthedocs.io/en/stable/index.html
 Project-URL: Issues, https://codeberg.org/JakobDev/minecraft-launcher-lib/issues
 Project-URL: Source, https://codeberg.org/JakobDev/minecraft-launcher-lib
 Project-URL: Changelog, https://minecraft-launcher-lib.readthedocs.io/en/stable/changelog.html
@@ -93,20 +93,22 @@
 subprocess.call(minecraft_command)
 ```
 
 Features:
 - Easy installing
 - Get command to run Minecraft
 - Login to Microsoft account
-- Support Forge, Fabric and Liteloader
+- Supports [Forge](https://minecraftforge.net), [Fabric](https://fabricmc.net), [Quilt](https://quiltmc.org) and Liteloader
 - Old versions like alpha or beta supported
 - All functions have type annotations and docstrings
 - Only depents on [requests](https://pypi.org/project/requests)
 - Supports [PyPy](https://www.pypy.org)
 - Full Documention with tutorial online available
+- Supports reading and writing profiles of the Vanilla Launcher
+- Install of [mrpack modpacks](https://docs.modrinth.com/docs/modpacks/format_definition)
 - All public APIs are static typed
 - Examples available
 - OpenSource
 
 [View more examples](https://codeberg.org/JakobDev/minecraft-launcher-lib/src/branch/master/examples)
 
 [Read the documentation](https://minecraft-launcher-lib.readthedocs.io)
```

### Comparing `minecraft-launcher-lib-5.3/pyproject.toml` & `minecraft-launcher-lib-6.0/pyproject.toml`

 * *Files identical despite different names*

