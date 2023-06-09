# Comparing `tmp/openet-core-0.0.8.tar.gz` & `tmp/openet-core-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openet-core-0.0.8.tar", last modified: Wed Feb 27 00:23:25 2019, max compression
+gzip compressed data, was "openet-core-0.1.0.tar", last modified: Fri Jun  9 20:20:17 2023, max compression
```

## Comparing `openet-core-0.0.8.tar` & `openet-core-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxrwx   0        0        0        0 2019-02-27 00:23:25.000000 openet-core-0.0.8/
--rw-rw-rw-   0        0        0    11556 2018-08-21 16:54:18.000000 openet-core-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      137 2018-11-21 16:08:52.000000 openet-core-0.0.8/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2019-02-27 00:23:25.000000 openet-core-0.0.8/openet/
-drwxrwxrwx   0        0        0        0 2019-02-27 00:23:25.000000 openet-core-0.0.8/openet/core/
--rw-rw-rw-   0        0        0     3457 2018-08-30 18:14:08.000000 openet-core-0.0.8/openet/core/api.py
--rw-rw-rw-   0        0        0     5380 2019-01-23 21:55:04.000000 openet-core-0.0.8/openet/core/common.py
--rw-rw-rw-   0        0        0    14039 2019-02-25 21:30:21.000000 openet-core-0.0.8/openet/core/interp.py
-drwxrwxrwx   0        0        0        0 2019-02-27 00:23:25.000000 openet-core-0.0.8/openet/core/tests/
--rw-rw-rw-   0        0        0      906 2018-11-21 16:08:52.000000 openet-core-0.0.8/openet/core/tests/conftest.py
--rw-rw-rw-   0        0        0     4486 2019-01-31 17:23:04.000000 openet-core-0.0.8/openet/core/tests/test_common.py
--rw-rw-rw-   0        0        0    18079 2019-02-25 20:49:28.000000 openet-core-0.0.8/openet/core/tests/test_interp.py
--rw-rw-rw-   0        0        0     2204 2019-02-20 22:53:05.000000 openet-core-0.0.8/openet/core/tests/test_utils.py
--rw-rw-rw-   0        0        0     2903 2019-02-21 00:51:22.000000 openet-core-0.0.8/openet/core/utils.py
--rw-rw-rw-   0        0        0      111 2019-02-21 01:01:39.000000 openet-core-0.0.8/openet/core/__init__.py
--rw-rw-rw-   0        0        0       66 2018-08-21 16:54:18.000000 openet-core-0.0.8/openet/__init__.py
-drwxrwxrwx   0        0        0        0 2019-02-27 00:23:25.000000 openet-core-0.0.8/openet_core.egg-info/
--rw-rw-rw-   0        0        0        1 2019-02-27 00:23:24.000000 openet-core-0.0.8/openet_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2018-11-30 15:09:00.000000 openet-core-0.0.8/openet_core.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3580 2019-02-27 00:23:24.000000 openet-core-0.0.8/openet_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       29 2019-02-27 00:23:24.000000 openet-core-0.0.8/openet_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0      516 2019-02-27 00:23:25.000000 openet-core-0.0.8/openet_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2019-02-27 00:23:24.000000 openet-core-0.0.8/openet_core.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3580 2019-02-27 00:23:25.000000 openet-core-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2514 2019-02-19 19:18:11.000000 openet-core-0.0.8/README.rst
--rw-rw-rw-   0        0        0       70 2019-02-27 00:23:25.000000 openet-core-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1749 2019-02-19 18:36:35.000000 openet-core-0.0.8/setup.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-09 20:20:17.217959 openet-core-0.1.0/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    11356 2023-06-06 21:29:21.000000 openet-core-0.1.0/LICENSE.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      132 2023-06-06 21:29:21.000000 openet-core-0.1.0/MANIFEST.in
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2980 2023-06-09 20:20:17.218009 openet-core-0.1.0/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2456 2023-06-06 21:29:21.000000 openet-core-0.1.0/README.rst
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-09 20:20:17.214129 openet-core-0.1.0/openet/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       65 2023-06-06 21:29:21.000000 openet-core-0.1.0/openet/__init__.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-09 20:20:17.215615 openet-core-0.1.0/openet/core/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      152 2023-06-07 13:41:31.000000 openet-core-0.1.0/openet/core/__init__.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3340 2023-06-06 21:29:21.000000 openet-core-0.1.0/openet/core/api.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    22474 2023-06-07 14:26:43.000000 openet-core-0.1.0/openet/core/common.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     4930 2023-06-06 21:29:21.000000 openet-core-0.1.0/openet/core/ensemble.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    50421 2023-06-07 14:26:43.000000 openet-core-0.1.0/openet/core/interpolate.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-09 20:20:17.217008 openet-core-0.1.0/openet/core/tests/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      870 2023-06-06 21:29:21.000000 openet-core-0.1.0/openet/core/tests/conftest.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    13330 2023-06-07 13:41:56.000000 openet-core-0.1.0/openet/core/tests/test_common.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     8269 2023-06-06 21:29:21.000000 openet-core-0.1.0/openet/core/tests/test_ensemble.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    43085 2023-06-07 14:26:43.000000 openet-core-0.1.0/openet/core/tests/test_interpolate.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     6650 2023-06-07 14:26:43.000000 openet-core-0.1.0/openet/core/tests/test_utils.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)    17908 2023-06-07 13:41:56.000000 openet-core-0.1.0/openet/core/utils.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)   378148 2023-06-06 21:29:21.000000 openet-core-0.1.0/openet/core/wrs2.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2023-06-09 20:20:17.217845 openet-core-0.1.0/openet_core.egg-info/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2980 2023-06-09 20:20:17.000000 openet-core-0.1.0/openet_core.egg-info/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      605 2023-06-09 20:20:17.000000 openet-core-0.1.0/openet_core.egg-info/SOURCES.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        1 2023-06-09 20:20:17.000000 openet-core-0.1.0/openet_core.egg-info/dependency_links.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        1 2023-06-06 21:45:52.000000 openet-core-0.1.0/openet_core.egg-info/not-zip-safe
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       32 2023-06-09 20:20:17.000000 openet-core-0.1.0/openet_core.egg-info/requires.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        7 2023-06-09 20:20:17.000000 openet-core-0.1.0/openet_core.egg-info/top_level.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       63 2023-06-09 20:20:17.218205 openet-core-0.1.0/setup.cfg
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     1746 2023-06-06 21:29:21.000000 openet-core-0.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `openet-core-0.0.8/LICENSE.txt` & `openet-core-0.1.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "{}"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright {yyyy} {name of copyright owner}
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "{}"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright {yyyy} {name of copyright owner}
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
    limitations under the License.
```

### Comparing `openet-core-0.0.8/openet/core/api.py` & `openet-core-0.1.0/openet/core/api.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-import sys
-
-import ee
-
-# import openet.interp as interp
-
-
-# class API():
-#     """"""
-#     def __init__(self):
-#         """"""
-#         pass
-
-
-# TODO: Make this a class eventually
-def collection(
-        et_model,
-        variable,
-        collections,
-        start_date,
-        end_date,
-        t_interval,
-        geometry,
-        **kwargs
-    ):
-    """Generic OpenET Collection
-
-    Parameters
-    ----------
-    self :
-    et_model : {'ndvi', 'ssebop'}
-        ET model.
-    variable : str
-
-    collections : list
-        GEE satellite image collection IDs.
-    start_date : str
-        ISO format inclusive start date (i.e. YYYY-MM-DD).
-    end_date : str
-        ISO format exclusive end date (i.e. YYYY-MM-DD).
-    t_interval : {'daily', 'monthly', 'annual', 'overpass'}
-        Time interval over which to interpolate and aggregate values.
-        Selecting 'overpass' will return values only for the overpass dates.
-    geometry : ee.Geometry
-        The geometry object will be used to filter the input collections.
-    kwargs :
-
-    Returns
-    -------
-    ee.ImageCollection
-
-    Notes
-    -----
-    The following is just a basic framework for what needs to happen to
-        go from input parameters to an output image collection.
-    A lot of this might make more sense in the init function above.
-
-    """
-
-    # Load the ET model
-    if et_model.lower() == 'ndvi':
-
-        # # DEADBEEF - Manually adding OpenET Model to system path
-        # # This will eventually be handled by import openet modules
-        # import os
-        # model_path = os.path.dirname(os.path.dirname(os.path.dirname(
-        #     os.path.abspath(os.path.realpath(__file__)))))
-        # print(model_path)
-        # sys.path.insert(0, os.path.join(model_path, 'openet-ndvi-test'))
-        # print(sys.path)
-
-        try:
-            import openet.ndvi as model
-        except ModuleNotFoundError:
-            print(
-                '\nThe ET model {} could not be imported'.format(et_model) +
-                '\nPlease ensure that the model has been installed')
-            return False
-        except Exception as e:
-            print('Unhandled Exception: {}'.format(e))
-            raise
-
-    elif et_model.lower() == 'ssebop':
-
-        # # DEADBEEF - Manually adding OpenET Models to system path
-        # # This will eventually be handled by import openet modules
-        # import os
-        # model_path = os.path.dirname(os.path.dirname(os.path.dirname(
-        #     os.path.abspath(os.path.realpath(__file__)))))
-        # print(model_path)
-        # sys.path.insert(0, os.path.join(model_path, 'openet-ssebop-test'))
-
-        try:
-            import openet.ssebop as model
-        except ModuleNotFoundError:
-            print(
-                '\nThe ET model {} could not be imported'.format(et_model) +
-                '\nPlease ensure that the model has been installed')
-            return False
-        except Exception as e:
-            print('Unhandled Exception: {}'.format(e))
-            raise
-
-    else:
-        # CGM - This could just be a value error exception
-        raise ValueError('unsupported et_model type')
-
-    variable_coll = model.collection(
-        variable,
-        collections,
-        start_date,
-        end_date,
-        t_interval,
-        geometry,
-        **kwargs
-    )
-    return variable_coll
+import sys
+
+import ee
+
+# import openet.interp as interp
+
+
+# class API():
+#     """"""
+#     def __init__(self):
+#         """"""
+#         pass
+
+
+# TODO: Make this a class eventually
+def collection(
+        et_model,
+        variable,
+        collections,
+        start_date,
+        end_date,
+        t_interval,
+        geometry,
+        **kwargs
+    ):
+    """Generic OpenET Collection
+
+    Parameters
+    ----------
+    self :
+    et_model : {'ndvi', 'ssebop'}
+        ET model.
+    variable : str
+
+    collections : list
+        GEE satellite image collection IDs.
+    start_date : str
+        ISO format inclusive start date (i.e. YYYY-MM-DD).
+    end_date : str
+        ISO format exclusive end date (i.e. YYYY-MM-DD).
+    t_interval : {'daily', 'monthly', 'annual', 'overpass'}
+        Time interval over which to interpolate and aggregate values.
+        Selecting 'overpass' will return values only for the overpass dates.
+    geometry : ee.Geometry
+        The geometry object will be used to filter the input collections.
+    kwargs :
+
+    Returns
+    -------
+    ee.ImageCollection
+
+    Notes
+    -----
+    The following is just a basic framework for what needs to happen to
+        go from input parameters to an output image collection.
+    A lot of this might make more sense in the init function above.
+
+    """
+
+    # Load the ET model
+    if et_model.lower() == 'ndvi':
+
+        # # DEADBEEF - Manually adding OpenET Model to system path
+        # # This will eventually be handled by import openet modules
+        # import os
+        # model_path = os.path.dirname(os.path.dirname(os.path.dirname(
+        #     os.path.abspath(os.path.realpath(__file__)))))
+        # print(model_path)
+        # sys.path.insert(0, os.path.join(model_path, 'openet-ndvi-test'))
+        # print(sys.path)
+
+        try:
+            import openet.ndvi as model
+        except ModuleNotFoundError:
+            print(
+                '\nThe ET model {} could not be imported'.format(et_model) +
+                '\nPlease ensure that the model has been installed')
+            return False
+        except Exception as e:
+            print('Unhandled Exception: {}'.format(e))
+            raise
+
+    elif et_model.lower() == 'ssebop':
+
+        # # DEADBEEF - Manually adding OpenET Models to system path
+        # # This will eventually be handled by import openet modules
+        # import os
+        # model_path = os.path.dirname(os.path.dirname(os.path.dirname(
+        #     os.path.abspath(os.path.realpath(__file__)))))
+        # print(model_path)
+        # sys.path.insert(0, os.path.join(model_path, 'openet-ssebop-test'))
+
+        try:
+            import openet.ssebop as model
+        except ModuleNotFoundError:
+            print(
+                '\nThe ET model {} could not be imported'.format(et_model) +
+                '\nPlease ensure that the model has been installed')
+            return False
+        except Exception as e:
+            print('Unhandled Exception: {}'.format(e))
+            raise
+
+    else:
+        # CGM - This could just be a value error exception
+        raise ValueError('unsupported et_model type')
+
+    variable_coll = model.collection(
+        variable,
+        collections,
+        start_date,
+        end_date,
+        t_interval,
+        geometry,
+        **kwargs
+    )
+    return variable_coll
```

### Comparing `openet-core-0.0.8/openet/core/tests/conftest.py` & `openet-core-0.1.0/openet/core/tests/conftest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-import base64
-import logging
-import os
-
-import ee
-import pytest
-
-
-@pytest.fixture(scope="session", autouse=True)
-def test_init():
-    logging.basicConfig(level=logging.DEBUG, format='%(message)s')
-    logging.debug('Test Setup')
-
-    # On Travis-CI authenticate using private key environment variable
-    if 'EE_PRIVATE_KEY_B64' in os.environ:
-        print('Writing privatekey.json from environmental variable ...')
-        content = base64.b64decode(os.environ['EE_PRIVATE_KEY_B64']).decode('ascii')
-        EE_PRIVATE_KEY_FILE = 'privatekey.json'
-        with open(EE_PRIVATE_KEY_FILE, 'w') as f:
-            f.write(content)
-        EE_CREDENTIALS = ee.ServiceAccountCredentials(
-            '', key_file=EE_PRIVATE_KEY_FILE)
-        ee.Initialize(EE_CREDENTIALS)
-    else:
-        ee.Initialize()
-
-    # Make a simple EE request
-    # logging.debug(ee.Number(1).getInfo())
+import base64
+import logging
+import os
+
+import ee
+import pytest
+
+
+@pytest.fixture(scope="session", autouse=True)
+def test_init():
+    logging.basicConfig(level=logging.DEBUG, format='%(message)s')
+    logging.getLogger('googleapiclient').setLevel(logging.ERROR)
+    logging.debug('Test Setup')
+
+    # On Travis-CI authenticate using private key environment variable
+    if 'EE_PRIVATE_KEY_B64' in os.environ:
+        print('Writing privatekey.json from environmental variable ...')
+        content = base64.b64decode(os.environ['EE_PRIVATE_KEY_B64']).decode('ascii')
+        EE_KEY_FILE = 'privatekey.json'
+        with open(EE_KEY_FILE, 'w') as f:
+            f.write(content)
+        ee.Initialize(ee.ServiceAccountCredentials('test', key_file=EE_KEY_FILE))
+    else:
+        ee.Initialize()
+
+    # Make a simple EE request
+    # logging.debug(ee.Number(1).getInfo())
```

### Comparing `openet-core-0.0.8/openet_core.egg-info/SOURCES.txt` & `openet-core-0.1.0/openet_core.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 README.rst
 setup.cfg
 setup.py
 openet/__init__.py
 openet/core/__init__.py
 openet/core/api.py
 openet/core/common.py
-openet/core/interp.py
+openet/core/ensemble.py
+openet/core/interpolate.py
 openet/core/utils.py
+openet/core/wrs2.py
 openet/core/tests/conftest.py
 openet/core/tests/test_common.py
-openet/core/tests/test_interp.py
+openet/core/tests/test_ensemble.py
+openet/core/tests/test_interpolate.py
 openet/core/tests/test_utils.py
 openet_core.egg-info/PKG-INFO
 openet_core.egg-info/SOURCES.txt
 openet_core.egg-info/dependency_links.txt
 openet_core.egg-info/not-zip-safe
 openet_core.egg-info/requires.txt
 openet_core.egg-info/top_level.txt
```

### Comparing `openet-core-0.0.8/README.rst` & `openet-core-0.1.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-=================================
-OpenET - Core Functions and Tools
-=================================
-
-|version| |build| |codecov|
-
-**WARNING: This code is in development, is being provided without support, and is subject to change at any time without notification**
-
-This repository provides core functions used by the OpenET models.
-
-Core Components
-===============
-
-Common
-------
-
-The OpenET common module provides functions that are common across many of the OpenET models.  Currently these are limited to cloud masking functions but additional functions will be added as they are identified.
-
-Examples of the cloud masking functions are provided in the "examples" folder.
-
-+ `Landsat Collection 1 TOA cloud mask <examples/landsat_toa_cloud_mask.ipynb>`__
-+ `Landsat Collection 1 SR cloud mask <examples/landsat_sr_cloud_mask.ipynb>`__
-+ `Sentinel 2 TOA cloud mask <examples/sentinel2_toa_cloud_mask.ipynb>`__
-
-Interpolation
--------------
-
-The OpenET "interp" module provides functions for interpolating the image based ET estimates from the models (primarily from Landsat images) to a daily time step then aggregating to custom time periods (such as monthly or annual).
-
-Installation
-============
-
-The OpenET core python module can be installed via pip:
-
-.. code-block:: console
-
-    pip install openet-core
-
-Dependencies
-============
-
-Modules needed to run the model:
-
- * `earthengine-api <https://github.com/google/earthengine-api>`__
-
-OpenET Namespace Package
-========================
-
-Each OpenET model will be stored in subfolders of the "openet" folder (namespace).  The benefit of the namespace package is that each ET model can be tracked in separate repositories but called as a "dot" submodule of the main openet module,
-
-.. code-block:: python
-
-    import openet.core.common
-    import openet.core.interp
-    import openet.ssebop
-
-Development and Testing
-=======================
-
-Please see the `CONTRIBUTING.rst <CONTRIBUTING.rst>`__.
-
-.. |build| image:: https://travis-ci.org/Open-ET/openet-core-beta.svg?branch=master
-   :alt: Build status
-   :target: https://travis-ci.org/Open-ET/openet-core-beta
-.. |version| image:: https://badge.fury.io/py/openet-core.svg
-   :alt: Latest version on PyPI
-   :target: https://badge.fury.io/py/openet-core
-.. |codecov| image:: https://codecov.io/gh/Open-ET/openet-core-beta/branch/master/graphs/badge.svg
-   :alt: Coverage Status
-   :target: https://codecov.io/gh/Open-ET/openet-core-beta
+=================================
+OpenET - Core Functions and Tools
+=================================
+
+|version| |build| |codecov|
+
+**WARNING: This code is in development, is being provided without support, and is subject to change at any time without notification**
+
+This repository provides core functions used by the OpenET models.
+
+Core Components
+===============
+
+Common
+------
+
+The OpenET common module provides functions that are common across many of the OpenET models.  Currently these are limited to cloud masking functions but additional functions will be added as they are identified.
+
+Examples of the cloud masking functions are provided in the "examples" folder.
+
++ `Landsat Collection 1 TOA cloud mask <examples/landsat_toa_cloud_mask.ipynb>`__
++ `Landsat Collection 1 SR cloud mask <examples/landsat_sr_cloud_mask.ipynb>`__
++ `Sentinel 2 TOA cloud mask <examples/sentinel2_toa_cloud_mask.ipynb>`__
+
+Interpolation
+-------------
+
+The OpenET "interpolate" module provides functions for interpolating the image based ET estimates from the models (primarily from Landsat images) to a daily time step then aggregating to custom time periods (such as monthly or annual).
+
+Installation
+============
+
+The OpenET core python module can be installed via pip:
+
+.. code-block:: console
+
+    pip install openet-core
+
+Dependencies
+============
+
+Modules needed to run the model:
+
+ * `earthengine-api <https://github.com/google/earthengine-api>`__
+
+OpenET Namespace Package
+========================
+
+Each OpenET model will be stored in subfolders of the "openet" folder (namespace).  The benefit of the namespace package is that each ET model can be tracked in separate repositories but called as a "dot" submodule of the main openet module,
+
+.. code-block:: python
+
+    import openet.core.common
+    import openet.core.interpolate
+    import openet.ssebop
+
+Development and Testing
+=======================
+
+Please see the `CONTRIBUTING.rst <CONTRIBUTING.rst>`__.
+
+.. |build| image:: https://github.com/Open-ET/openet-core-beta/workflows/build/badge.svg
+   :alt: Build status
+   :target: https://github.com/Open-ET/openet-core-beta
+.. |version| image:: https://badge.fury.io/py/openet-core.svg
+   :alt: Latest version on PyPI
+   :target: https://badge.fury.io/py/openet-core
+.. |codecov| image:: https://codecov.io/gh/Open-ET/openet-core-beta/branch/master/graphs/badge.svg
+   :alt: Coverage Status
+   :target: https://codecov.io/gh/Open-ET/openet-core-beta
```

