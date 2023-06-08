# Comparing `tmp/memfault-cli-0.8.0.tar.gz` & `tmp/memfault-cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memfault-cli-0.8.0.tar", max compression
+gzip compressed data, was "memfault-cli-0.9.0.tar", max compression
```

## Comparing `memfault-cli-0.8.0.tar` & `memfault-cli-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      267 2021-10-20 15:02:08.558356 memfault-cli-0.8.0/README.md
--rw-r--r--   0        0        0       79 2022-08-15 20:35:27.695231 memfault-cli-0.8.0/memfault_cli/__init__.py
--rw-r--r--   0        0        0      465 2022-09-02 20:14:27.749997 memfault-cli-0.8.0/memfault_cli/_version.py
--rw-r--r--   0        0        0     3145 2022-08-15 20:35:27.695231 memfault-cli-0.8.0/memfault_cli/authenticator.py
--rw-r--r--   0        0        0     2773 2022-08-15 20:35:27.695231 memfault-cli-0.8.0/memfault_cli/chunk.py
--rw-r--r--   0        0        0    19447 2022-09-19 12:17:59.490836 memfault-cli-0.8.0/memfault_cli/cli.py
--rw-r--r--   0        0        0    10891 2022-09-02 20:14:27.749997 memfault-cli-0.8.0/memfault_cli/context.py
--rw-r--r--   0        0        0     2522 2022-09-02 20:14:27.749997 memfault-cli-0.8.0/memfault_cli/deploy.py
--rw-r--r--   0        0        0      633 2022-08-15 20:35:27.695231 memfault-cli-0.8.0/memfault_cli/functools_ext.py
--rw-r--r--   0        0        0     1323 2022-09-13 17:28:36.175007 memfault-cli-0.8.0/memfault_cli/gnu_build_id.py
--rw-r--r--   0        0        0    21369 2022-09-19 12:17:59.490836 memfault-cli-0.8.0/memfault_cli/upload.py
--rw-r--r--   0        0        0     1677 2022-09-19 12:17:59.490836 memfault-cli-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 memfault-cli-0.8.0/setup.py
--rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 memfault-cli-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      267 2022-07-01 18:48:24.158978 memfault-cli-0.9.0/README.md
+-rw-r--r--   0        0        0       79 2022-07-01 18:48:24.158978 memfault-cli-0.9.0/memfault_cli/__init__.py
+-rw-r--r--   0        0        0      465 2022-09-07 08:56:09.631200 memfault-cli-0.9.0/memfault_cli/_version.py
+-rw-r--r--   0        0        0     2579 2022-09-26 12:35:31.188376 memfault-cli-0.9.0/memfault_cli/authenticator.py
+-rw-r--r--   0        0        0     2773 2022-07-01 18:48:24.158978 memfault-cli-0.9.0/memfault_cli/chunk.py
+-rw-r--r--   0        0        0    20132 2022-09-26 12:35:31.188376 memfault-cli-0.9.0/memfault_cli/cli.py
+-rw-r--r--   0        0        0    11216 2022-09-26 12:35:31.188376 memfault-cli-0.9.0/memfault_cli/context.py
+-rw-r--r--   0        0        0     2522 2022-09-07 08:56:09.631200 memfault-cli-0.9.0/memfault_cli/deploy.py
+-rw-r--r--   0        0        0     2281 2022-09-26 10:55:42.178569 memfault-cli-0.9.0/memfault_cli/elf.py
+-rw-r--r--   0        0        0      633 2022-07-01 18:48:24.158978 memfault-cli-0.9.0/memfault_cli/functools_ext.py
+-rw-r--r--   0        0        0    22740 2022-09-26 12:35:31.188376 memfault-cli-0.9.0/memfault_cli/upload.py
+-rw-r--r--   0        0        0     5712 2022-09-26 10:55:42.178569 memfault-cli-0.9.0/memfault_cli/yocto.py
+-rw-r--r--   0        0        0     1677 2022-09-26 10:55:42.178569 memfault-cli-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 memfault-cli-0.9.0/setup.py
+-rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 memfault-cli-0.9.0/PKG-INFO
```

### Comparing `memfault-cli-0.8.0/memfault_cli/authenticator.py` & `memfault-cli-0.9.0/memfault_cli/authenticator.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,38 +9,22 @@
 LOG = logging.getLogger(__name__)
 
 
 class Authenticator:
     def __init__(self, ctx: "MemfaultCliClickContext"):
         self.ctx = ctx
 
-    @classmethod
-    def create_authenticator_given_context_or_raise(
-        cls, ctx: "MemfaultCliClickContext"
-    ) -> "Authenticator":
-        """
-        Given a CLI context, determine which auth system to use.
-        Simple implementation for now. If this becomes more complicated, iterate through
-        subclasses instead.
-        """
-        if ctx.obj.get("project_key"):
-            return ProjectKeyAuthenticator(ctx)
-        if ctx.obj.get("org_token"):
-            return OrgTokenAuthenticator(ctx)
-        else:
-            return BasicAuthenticator(ctx)
-
     @staticmethod
     @abstractmethod
     def project_key_auth() -> bool:
         pass
 
-    @staticmethod
+    @classmethod
     @abstractmethod
-    def required_args() -> List[str]:
+    def required_args(cls) -> List[str]:
         pass
 
     @abstractmethod
     def requests_auth_params(self) -> dict:
         pass
 
 
@@ -49,16 +33,16 @@
     Project Key Authentication with the Memfault service (Memfault-Project-Key)
     """
 
     @staticmethod
     def project_key_auth() -> bool:
         return True
 
-    @staticmethod
-    def required_args() -> List[str]:
+    @classmethod
+    def required_args(cls) -> List[str]:
         return [
             "project_key",
         ]
 
     def requests_auth_params(self) -> dict:
         return dict(headers={"Memfault-Project-Key": self.ctx.project_key})
 
@@ -80,16 +64,16 @@
                 "Please use --org-token instead of --password to pass organization auth token"
             )
 
     @staticmethod
     def project_key_auth() -> bool:
         return False
 
-    @staticmethod
-    def required_args() -> List[str]:
+    @classmethod
+    def required_args(cls) -> List[str]:
         return [
             "org",
             "project",
             "password",
         ]
 
     def requests_auth_params(self) -> dict:
@@ -103,16 +87,16 @@
     Org Token Authentication with the Memfault service, passed in with --org-token
     """
 
     @staticmethod
     def project_key_auth() -> bool:
         return False
 
-    @staticmethod
-    def required_args() -> List[str]:
+    @classmethod
+    def required_args(cls) -> List[str]:
         return [
             "org",
             "org_token",
             "project",
         ]
 
     def requests_auth_params(self) -> dict:
```

### Comparing `memfault-cli-0.8.0/memfault_cli/chunk.py` & `memfault-cli-0.9.0/memfault_cli/chunk.py`

 * *Files identical despite different names*

### Comparing `memfault-cli-0.8.0/memfault_cli/cli.py` & `memfault-cli-0.9.0/memfault_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import http.client
 import logging
 import os
-import tarfile
-import tempfile
 from base64 import b64decode
-from typing import List, Type
+from typing import List, TextIO, Type
 
 import click
 
 from ._version import version
+from .authenticator import BasicAuthenticator, OrgTokenAuthenticator, ProjectKeyAuthenticator
 from .chunk import MemfaultChunk
 from .context import MemfaultCliClickContext
 from .deploy import Deployer
 from .upload import (
     AndroidAppSymbolsUploader,
     BugreportUploader,
     CoredumpUploader,
     ElfSymbolDirectoryUploader,
     ElfSymbolUploader,
     MarUploader,
     McuSdkElfSymbolUploader,
     ReleaseArtifactUploader,
     Uploader,
     XedUploader,
+    walk_files,
 )
+from .yocto import find_elf_files_from_image_manifest
 
 pass_memfault_cli_context = click.make_pass_decorator(MemfaultCliClickContext, ensure=True)
 click_argument_path = click.argument("path", type=click.Path(exists=True))
 click_option_concurrency = click.option(
     "--concurrency",
     required=False,
     default=8,
@@ -70,20 +71,19 @@
             httpclient_logger.log(logging.DEBUG, " ".join(args))
 
         http.client.print = httpclient_log  # type: ignore[attr-defined]
         http.client.HTTPConnection.debuglevel = 1
 
 
 def _do_upload_or_raise(
-    ctx: MemfaultCliClickContext, path: str, uploader_cls: Type[Uploader]
+    ctx: MemfaultCliClickContext, path: str, uploader_cls: Type[Uploader], **kwargs
 ) -> None:
-    authenticator = ctx.authenticator
-    ctx.check_required_cli_args(authenticator=authenticator)
+    authenticator = ctx.create_authenticator(*uploader_cls.authenticator_types)
 
-    uploader = uploader_cls(ctx=ctx, file_path=path, authenticator=authenticator)
+    uploader = uploader_cls(ctx=ctx, file_path=path, authenticator=authenticator, **kwargs)
     if not uploader.can_upload_file():
         raise click.exceptions.UsageError("Upload failed!")
     uploader.upload()
 
 
 @cli.command(name="upload-coredump")
 @click.option(
@@ -179,20 +179,23 @@
     Please use upload-aosp-symbols or upload-mcu-symbols instead!
     """
     ctx.obj.update(**kwargs)
 
     uploader: Type[Uploader]
     if os.path.isdir(path):
         uploader = ElfSymbolDirectoryUploader
+        uploader_kwargs = dict(file_paths=walk_files(path))
     elif ctx.software_info is None:
         uploader = ElfSymbolUploader
+        uploader_kwargs = dict()
     else:
         uploader = McuSdkElfSymbolUploader
+        uploader_kwargs = dict()
 
-    _do_upload_or_raise(ctx, path, uploader)
+    _do_upload_or_raise(ctx, path, uploader, **uploader_kwargs)
 
 
 @cli.command(name="upload-mar")
 @click.option(
     "--hardware-version",
     required=True,
     help="Required to identify the type of Android hardware, see https://mflt.io/34PyNGQ/#android. By default the ro.product.board property is used.",
@@ -217,37 +220,50 @@
 def upload_mar(ctx: MemfaultCliClickContext, path: str, **kwargs):
     """Upload a Memfault Archive File (mar) file for analysis."""
     ctx.obj.update(**kwargs)
     _do_upload_or_raise(ctx, path, MarUploader)
 
 
 @cli.command(name="upload-yocto-symbols")
+@click.option(
+    "--manifest",
+    "-m",
+    required=True,
+    help="""
+    The path to the image .manifest as produced by Yocto's do_rootfs (IMAGE_MANIFEST).
+    The .manifest file is expected to reside in the location where Yocto produced the file.
+    The tool will locate the symbol files to upload in the tmp/work/ directory, based on
+    the packages that are listed in the .manifest file.
+    """,
+    type=click.File(),
+)
 @click_option_concurrency
-@click_argument_path
 @pass_memfault_cli_context
-def upload_yocto_symbols(ctx: MemfaultCliClickContext, path: str, **kwargs):
+def upload_yocto_symbols(ctx: MemfaultCliClickContext, manifest: TextIO, **kwargs):
     """Upload symbols for a Yocto build.
 
-    Expects a tar image file as produced by Yocto's "tar" IMAGE_FSTYPE. To see an example
-    image containing debug symbols, take a look at the Linux SDK example project:
+    To see a full example, take a look at the Linux SDK example project:
     https://mflt.io/yocto-symbols-image
 
     Example Yocto Symbol Upload:
 
         \b
-        $ bitbake symbols-image
+        $ bitbake my-image
         $ memfault --org-token $ORG_TOKEN \\
                    --org acme-inc --project smart-sink \\
-            upload-yocto-symbols build/tmp/deploy/images/raspberrypi3/symbols-image.tar
+            upload-yocto-symbols --manifest build/tmp/deploy/images/raspberrypi3/my-image-raspberrypi3.rootfs.manifest
     """
     ctx.obj.update(**kwargs)
 
-    with tarfile.TarFile(path, "r") as tar, tempfile.TemporaryDirectory() as extraction_path:
-        tar.extractall(extraction_path)
-        _do_upload_or_raise(ctx, extraction_path, ElfSymbolDirectoryUploader)
+    ElfSymbolDirectoryUploader(
+        ctx=ctx,
+        file_path=manifest.name,  # Not used. TODO: refactor!
+        authenticator=ctx.create_authenticator(OrgTokenAuthenticator, BasicAuthenticator),
+        file_paths=find_elf_files_from_image_manifest(manifest),
+    ).upload()
 
 
 @cli.command(name="upload-mcu-symbols")
 @click.option(
     "--software-type",
     required=False,
     help="Required for MCU symbols without Build Id, see https://mflt.io/symbol-file-build-ids",
@@ -318,18 +334,20 @@
         Reference: https://mflt.io/android-os-symbol-files
     """
     ctx.obj.update(**kwargs)
 
     uploader: Type[Uploader]
     if os.path.isdir(path):
         uploader = ElfSymbolDirectoryUploader
+        uploader_kwargs = dict(file_paths=walk_files(path))
     else:
         uploader = ElfSymbolUploader
+        uploader_kwargs = dict()
 
-    _do_upload_or_raise(ctx, path, uploader)
+    _do_upload_or_raise(ctx, path, uploader, **uploader_kwargs)
 
 
 @cli.command(name="upload-android-app-symbols")
 @click.option(
     "--build-variant",
     required=True,
     help="The build variant for which to upload the Android app symbols",
@@ -470,31 +488,28 @@
                    --org acme-inc --project smart-sink \\
                    deploy-release \\
                    --release-version 1.0.0-alpha \\
                    --cohort default
     """
     ctx.obj.update(**kwargs)
 
-    ctx.check_required_cli_args(authenticator=ctx.authenticator)
+    authenticator = ctx.create_authenticator(OrgTokenAuthenticator, BasicAuthenticator)
     ctx.check_required_either(
         {"release_version"}, {"delta_from", "delta_to"}, mutually_exclusive=True
     )
     release_version = ctx.obj.get("release_version") or (
         ctx.obj["delta_from"],
         ctx.obj["delta_to"],
     )
-    deployer = Deployer(ctx=ctx, authenticator=ctx.authenticator)
+    deployer = Deployer(ctx=ctx, authenticator=authenticator)
     deployer.deploy(cohort=cohort, release_version=release_version, rollout_percent=rollout_percent)
 
 
 def _do_post_chunks_or_raise(ctx: MemfaultCliClickContext, chunks: List[bytes]):
-    authenticator = ctx.authenticator
-    ctx.check_required_cli_args(authenticator=authenticator)
-    if not authenticator.project_key_auth():
-        raise click.exceptions.UsageError("A '--project-key' is required")
+    authenticator = ctx.create_authenticator(ProjectKeyAuthenticator)
 
     MemfaultChunk(ctx, authenticator).batch_post(chunks)
     click.echo("Success")
 
 
 @cli.command("post-chunk")
 @click.option("--device-serial", show_default=True, default="TESTSERIAL")
```

### Comparing `memfault-cli-0.8.0/memfault_cli/context.py` & `memfault-cli-0.9.0/memfault_cli/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import logging
-from typing import Any, Dict, List, Optional, Set, Union
+from typing import Any, Dict, List, Optional, Set, Type, Union
 
 import click
 
 from .authenticator import Authenticator
-from .functools_ext import cached_property
 
 LOG = logging.getLogger(__name__)
 
 
 class PackageInfo:  # noqa: B903 - no data classes in Python 3.6
     def __init__(self, name: str, version_name: str, version_code: str):
         self.name = name
@@ -114,16 +113,16 @@
 
     def _find_obj_or_raise(self, name):
         value = self.obj.get(name)
         if value is None:
             raise click.exceptions.UsageError(f"Missing option {self._format_as_option(name)!r}.")
         return value
 
-    def check_required_cli_args(self, *, authenticator: Authenticator):
-        required_args = authenticator.required_args()
+    def check_required_auth_cli_args(self, *, authenticator_type: Type[Authenticator]):
+        required_args = authenticator_type.required_args()
 
         for arg in required_args:
             self._find_obj_or_raise(arg)
 
     def _format_arg_set(self, arg_set: Set[str]) -> str:
         return ", ".join([f"{self._format_as_option(arg)!r}" for arg in sorted(arg_set)])
 
@@ -147,17 +146,24 @@
 
         if len(valid_arg_sets) == 0:
             formatted_required_args = [self._format_arg_set(arg_set) for arg_set in args]
             raise click.exceptions.UsageError(
                 f"Please pass either {' or '.join(sorted(formatted_required_args))}."
             )
 
-    @cached_property
-    def authenticator(self) -> Authenticator:
-        return Authenticator.create_authenticator_given_context_or_raise(self)
+    def create_authenticator(self, *types: Type[Authenticator]) -> Authenticator:
+        assert types
+        for _type in types:
+            try:
+                self.check_required_auth_cli_args(authenticator_type=_type)
+                return _type(self)
+            except click.exceptions.UsageError:
+                pass
+        # Raise for the first missing option of the preferred authenticator type:
+        raise self.check_required_auth_cli_args(authenticator_type=types[0])
 
     @property
     def org(self):
         return self._find_obj_or_raise("org")
 
     @property
     def org_token(self) -> str:
```

### Comparing `memfault-cli-0.8.0/memfault_cli/deploy.py` & `memfault-cli-0.9.0/memfault_cli/deploy.py`

 * *Files identical despite different names*

### Comparing `memfault-cli-0.8.0/memfault_cli/functools_ext.py` & `memfault-cli-0.9.0/memfault_cli/functools_ext.py`

 * *Files identical despite different names*

### Comparing `memfault-cli-0.8.0/memfault_cli/upload.py` & `memfault-cli-0.9.0/memfault_cli/upload.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,31 +3,36 @@
 import logging
 import os
 import re
 import urllib.parse
 from abc import abstractmethod
 from concurrent.futures import ThreadPoolExecutor
 from glob import glob
-from typing import IO, Any, Dict, Generator, Optional, Tuple, Type
+from typing import IO, Dict, Iterable, List, Optional, Tuple, Type, Union
 from zipfile import is_zipfile
 
 import click
 import requests
 from elftools.elf.elffile import ELFFile
 from mflt_build_id import BuildIdInspectorAndPatcher
 from requests import Response, Session
 from requests.adapters import HTTPAdapter
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 from urllib3 import Retry
 
-from .authenticator import Authenticator
+from .authenticator import (
+    Authenticator,
+    BasicAuthenticator,
+    OrgTokenAuthenticator,
+    ProjectKeyAuthenticator,
+)
 from .context import DeltaReleaseVersion, MemfaultCliClickContext, PackageInfo
+from .elf import elf_has_debug_info, get_gnu_build_id, is_elf
 from .functools_ext import cached_property
-from .gnu_build_id import get_gnu_build_id
 
 LOG = logging.getLogger(__name__)
 
 GNU_BUILD_ID_RE = re.compile(r"Build ID: (?P<gnu_build_id>[a-f\d]+)")
 
 
 def hash_io_hexdigest(name, data: IO, chunksize=2**20) -> str:
@@ -46,25 +51,33 @@
         h.update(chunk)
     return h.hexdigest()
 
 
 def check_response(response: Response):
     if response.status_code >= 400:
         raise Exception(
-            f"Request failed with HTTP status {response.status_code}\nResponse body:\n{response.content.decode()}"
+            f"Request failed with HTTP status {response.status_code}\n"
+            f"Response body:\n{response.content.decode() if response.content else '(empty)'}"
         )
 
 
 def url_quote(value: str) -> str:
     return urllib.parse.quote(value, safe="", encoding="utf-8")
 
 
 class Uploader(metaclass=abc.ABCMeta):
+    authenticator_types: List[Type[Authenticator]]
+
     def __init__(
-        self, *, ctx: MemfaultCliClickContext, file_path: str, authenticator: Authenticator
+        self,
+        *,
+        ctx: MemfaultCliClickContext,
+        file_path: Union[str, os.PathLike],
+        authenticator: Authenticator,
+        **kwargs,
     ):
         self.ctx: MemfaultCliClickContext = ctx
         self.file_path = file_path
         self.authenticator: Authenticator = authenticator
         self.session = self._create_requests_session()
 
     @staticmethod
@@ -195,28 +208,40 @@
 
     @property
     def file_basename(self):
         return os.path.basename(self.file_path)
 
 
 class BugreportUploader(Uploader):
+    authenticator_types = [
+        ProjectKeyAuthenticator,
+        OrgTokenAuthenticator,
+        BasicAuthenticator,
+    ]
+
     def can_upload_file(self) -> bool:
         if not is_zipfile(self.file_path):
             LOG.error("%s is not a valid zip file!", self.file_path)
             return False
         return True
 
     def entity_url(self) -> str:
         if self.authenticator.project_key_auth():
             return f"{self._api_base_url()}/upload/bugreport"
         else:
             return f"{self._projects_base_url()}/bugreports"
 
 
 class CoredumpUploader(Uploader):
+    authenticator_types = [
+        ProjectKeyAuthenticator,
+        OrgTokenAuthenticator,
+        BasicAuthenticator,
+    ]
+
     def can_upload_file(self) -> bool:
         with open(self.file_path, "rb") as f:
             hdr = f.read(4).decode("ascii", errors="ignore")
             if hdr != "CORE":
                 LOG.error("%s is not a Memfault Coredump", self.file_path)
                 return False
 
@@ -233,14 +258,20 @@
             return {
                 "device_serial": self.ctx.core_info.device_serial,
             }
         return None
 
 
 class XedUploader(Uploader):
+    authenticator_types = [
+        ProjectKeyAuthenticator,
+        OrgTokenAuthenticator,
+        BasicAuthenticator,
+    ]
+
     def can_upload_file(self) -> bool:
         return True
 
     def entity_url(self) -> str:
         if self.authenticator.project_key_auth():
             return f"{self._api_base_url()}/upload/qc/x"
         else:
@@ -254,14 +285,20 @@
             "trace_attributes": [
                 {"string_key": a.string_key, "value": a.value} for a in self.ctx.attributes
             ],
         }
 
 
 class MarUploader(Uploader):
+    authenticator_types = [
+        ProjectKeyAuthenticator,
+        OrgTokenAuthenticator,
+        BasicAuthenticator,
+    ]
+
     def can_upload_file(self) -> bool:
         if not is_zipfile(self.file_path):
             LOG.error("%s is not a valid zip file!", self.file_path)
             return False
         return True
 
     def entity_url(self) -> str:
@@ -277,40 +314,37 @@
             "hardware_version": info.hardware_version,
             "software_type": info.software_type,
             "software_version": info.software_version,
         }
 
 
 class ElfSymbolUploader(Uploader):
-    gnu_build_id: str = ""
+    authenticator_types = [
+        OrgTokenAuthenticator,
+        BasicAuthenticator,
+    ]
 
-    def _is_elf(self) -> bool:
-        with open(self.file_path, "rb") as file:
-            if file.read(4) != b"\x7FELF":
-                return False
-
-        return True
-
-    def _get_gnu_build_id_and_has_debug_info(self) -> Tuple[Optional[str], bool]:
-        with open(self.file_path, "rb") as f:
-            elf = ELFFile(f)
-            return get_gnu_build_id(elf), elf.has_dwarf_info()
+    gnu_build_id: str = ""
 
     def can_upload_file(self) -> bool:
         if os.path.islink(self.file_path) and not os.path.exists(self.file_path):
             return False
 
-        if not self._is_elf():
-            LOG.info("%s: Not an ELF file", self.file_path)
-            return False
+        with open(self.file_path, "rb") as f:
+            if not is_elf(f):
+                LOG.info("%s: Not an ELF file", self.file_path)
+                return False
 
-        gnu_build_id, has_debug_info = self._get_gnu_build_id_and_has_debug_info()
-        if not gnu_build_id:
-            LOG.info("%s: looks like an ELF but does not contain a GNU Build ID", self.file_path)
-            return False
+            elf = ELFFile(f)
+            gnu_build_id, has_debug_info = get_gnu_build_id(elf), elf_has_debug_info(elf)
+            if not gnu_build_id:
+                LOG.info(
+                    "%s: looks like an ELF but does not contain a GNU Build ID", self.file_path
+                )
+                return False
 
         self.gnu_build_id = gnu_build_id
         if not has_debug_info:
             LOG.info("%s: looks like an ELF but it has no .debug_info", self.file_path)
             return False
         LOG.info(
             "%s: ELF file with .debug_info and GNU Build ID: %s", self.file_path, self.gnu_build_id
@@ -331,23 +365,28 @@
         return True
 
     def entity_url(self) -> str:
         return f"{self._projects_base_url()}/symbols"
 
 
 class McuSdkElfSymbolUploader(Uploader):
+    authenticator_types = [
+        OrgTokenAuthenticator,
+        BasicAuthenticator,
+    ]
+
     def can_upload_file(self) -> bool:
         with open(self.file_path, "rb") as file:
             if file.read(4) != b"\x7FELF":
                 LOG.info("%s: Not an ELF file", self.file_path)
                 return False
             file.seek(0)
 
             inspector = BuildIdInspectorAndPatcher(file)
-            if not inspector.elf.has_dwarf_info():
+            if not elf_has_debug_info(inspector.elf):
                 LOG.info("%s: looks like an ELF but it has no .debug_info", self.file_path)
                 return False
 
             mcu_build_id_type, mcu_build_id, mcu_build_id_short_len = inspector.get_build_info()
 
             # NB: QC symbol files have different arg requirements depending on the subsystem the
             # ELF is associated with so we offload to the Memfault backend.
@@ -392,14 +431,19 @@
                 "software_type": info.software_type,
                 **({"revision": info.revision} if info.revision else {}),
             },
         }
 
 
 class ReleaseArtifactUploader(Uploader):
+    authenticator_types = [
+        OrgTokenAuthenticator,
+        BasicAuthenticator,
+    ]
+
     def can_upload_file(self) -> bool:
         # There are no restrictions for the type of binary a customer uses for
         # a release
         return True
 
     def _is_already_uploaded(self) -> bool:
         return False
@@ -444,32 +488,43 @@
             },
             "must_pass_through": self.ctx.must_pass_through,
             "hardware_version": self.ctx.hardware_version,
             "notes": self.ctx.notes,
         }
 
 
-class DirectoryUploader(Uploader):
+def walk_files(toplevel: str) -> Iterable[str]:
+    for root, _dirs, files in os.walk(toplevel):
+        for file in files:
+            yield os.path.join(root, file)
+
+
+class ParallelUploader(Uploader):
     uploader_cls: Type[Uploader]
 
+    def __init__(
+        self,
+        *args,
+        file_paths: Iterable[Union[str, os.PathLike]],
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        self.file_paths = file_paths
+
     def can_upload_file(self) -> bool:
         if os.path.islink(self.file_path) and not os.path.exists(self.file_path):
             return False
 
         return os.path.isdir(self.file_path)
 
-    def _walk_files(self, toplevel: str) -> Generator[str, Any, Any]:
-        for root, _dirs, files in os.walk(toplevel):
-            yield from map(lambda file: os.path.join(root, file), files)
-
     def upload(self, *, progressbar=True) -> bool:
         queued_uploaders = []
         did_upload = False
 
-        for file_path in self._walk_files(self.file_path):
+        for file_path in self.file_paths:
             uploader = self.uploader_cls(
                 ctx=self.ctx, file_path=file_path, authenticator=self.authenticator
             )
             if uploader.can_upload_file():
                 queued_uploaders.append(uploader)
                 did_upload |= True
             else:
@@ -488,28 +543,38 @@
 
         return did_upload
 
     def entity_url(self) -> str:
         raise NotImplementedError
 
 
-class ElfSymbolDirectoryUploader(DirectoryUploader):
+class ElfSymbolDirectoryUploader(ParallelUploader):
     uploader_cls = ElfSymbolUploader
+    authenticator_types = [
+        OrgTokenAuthenticator,
+        BasicAuthenticator,
+    ]
 
 
 class ProguardMappingUploader(Uploader):
+    authenticator_types = [
+        OrgTokenAuthenticator,
+        BasicAuthenticator,
+    ]
+
     def __init__(
         self,
         *,
         ctx: MemfaultCliClickContext,
         file_path: str,
         authenticator: Authenticator,
         package_info: PackageInfo,
+        **kwargs,
     ):
-        super().__init__(ctx=ctx, file_path=file_path, authenticator=authenticator)
+        super().__init__(ctx=ctx, file_path=file_path, authenticator=authenticator, **kwargs)
         self.package_info = package_info
 
     def can_upload_file(self) -> bool:
         return True
 
     def entity_url(self) -> str:
         return f"{self._projects_base_url()}/symbols"
@@ -520,14 +585,19 @@
                 "version": f"{self.package_info.version_name}:{self.package_info.version_code}",
                 "software_type": self.package_info.name,
             },
         }
 
 
 class AndroidAppSymbolsUploader(Uploader):
+    authenticator_types = [
+        OrgTokenAuthenticator,
+        BasicAuthenticator,
+    ]
+
     def can_upload_file(self) -> bool:
         if not os.path.isdir(self.file_path):
             LOG.error(
                 '%s is not a directory. Please specify the Android app\'s root "build" path instead!',
                 self.file_path,
             )
             return False
@@ -591,15 +661,18 @@
         # TODO: add support for legacy ndkBuild?
         cmake_path_out = os.path.join(
             self.file_path, "intermediates", "cmake", self.ctx.build_variant
         )
         if not os.path.isdir(cmake_path_out):
             return False
         sym_dir_uploader = ElfSymbolDirectoryUploader(
-            ctx=self.ctx, file_path=cmake_path_out, authenticator=self.authenticator
+            ctx=self.ctx,
+            file_path=cmake_path_out,
+            authenticator=self.authenticator,
+            file_paths=walk_files(cmake_path_out),
         )
         return sym_dir_uploader.upload()
 
     def upload(self, *, progressbar=True) -> bool:
         did_upload = self._upload_mapping_txt() or self._upload_ndk_symbols()
         if not did_upload:
             raise click.exceptions.UsageError("No files uploaded!")
```

### Comparing `memfault-cli-0.8.0/pyproject.toml` & `memfault-cli-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "memfault-cli"
-version = "0.8.0"
+version = "0.9.0"
 description = "Memfault CLI tool"
 homepage = "https://docs.memfault.com"
 documentation = "https://docs.memfault.com/docs/ci/install-memfault-cli"
 authors = ["Memfault Inc <hello@memfault.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 memfault = 'memfault_cli.cli:main'
 
 [tool.poetry.dependencies]
 python = "^3.6"
 Click = ">=7,<9"
 requests = "^2.22.0"
 pyelftools = ">=0.26,<=0.28"
-mflt-build-id = "0.0.4"
+mflt-build-id = "0.0.5"
 # use the below for internal testing
 # see https://python-poetry.org/docs/dependency-specification/#path-dependencies
 # mflt-build-id = { path = "../../py-packages/mflt-build-id/", develop = false }
 
 more_itertools = "^8.0.2"
 pyaxmlparser = "^0.3.24"
 tqdm = "^4.44.1"
```

### Comparing `memfault-cli-0.8.0/setup.py` & `memfault-cli-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['memfault_cli']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Click>=7,<9',
- 'mflt-build-id==0.0.4',
+ 'mflt-build-id==0.0.5',
  'more_itertools>=8.0.2,<9.0.0',
  'pyaxmlparser>=0.3.24,<0.4.0',
  'pyelftools>=0.26,<=0.28',
  'requests>=2.22.0,<3.0.0',
  'tqdm>=4.44.1,<5.0.0',
  'urllib3>=1.26.7']
 
@@ -21,15 +21,15 @@
 {':python_version < "3.8"': ['importlib-metadata==4.8.3']}
 
 entry_points = \
 {'console_scripts': ['memfault = memfault_cli.cli:main']}
 
 setup_kwargs = {
     'name': 'memfault-cli',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Memfault CLI tool',
     'long_description': '# Memfault CLI tool\n\nThis package contains the `memfault` CLI tool.\n\nThe purpose of the tool is to make integration with Memfault from other systems,\nlike continuous integration servers, as easy as possible.\n\nInstall the tool and run `memfault --help` for more info!\n',
     'author': 'Memfault Inc',
     'author_email': 'hello@memfault.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://docs.memfault.com',
```

### Comparing `memfault-cli-0.8.0/PKG-INFO` & `memfault-cli-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: memfault-cli
-Version: 0.8.0
+Version: 0.9.0
 Summary: Memfault CLI tool
 Home-page: https://docs.memfault.com
 Author: Memfault Inc
 Author-email: hello@memfault.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Click (>=7,<9)
 Requires-Dist: importlib-metadata (==4.8.3); python_version < "3.8"
-Requires-Dist: mflt-build-id (==0.0.4)
+Requires-Dist: mflt-build-id (==0.0.5)
 Requires-Dist: more_itertools (>=8.0.2,<9.0.0)
 Requires-Dist: pyaxmlparser (>=0.3.24,<0.4.0)
 Requires-Dist: pyelftools (>=0.26,<=0.28)
 Requires-Dist: requests (>=2.22.0,<3.0.0)
 Requires-Dist: tqdm (>=4.44.1,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.7)
 Project-URL: Documentation, https://docs.memfault.com/docs/ci/install-memfault-cli
```

