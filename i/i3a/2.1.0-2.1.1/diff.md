# Comparing `tmp/i3a-2.1.0.tar.gz` & `tmp/i3a-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i3a-2.1.0.tar", last modified: Thu May 25 07:23:59 2023, max compression
+gzip compressed data, was "i3a-2.1.1.tar", last modified: Fri Jun  9 21:25:06 2023, max compression
```

## Comparing `i3a-2.1.0.tar` & `i3a-2.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 mgoral    (1000) mgoral    (1000)        0 2023-05-25 07:23:59.606853 i3a-2.1.0/
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)      161 2021-04-28 19:43:35.000000 i3a-2.1.0/.gitignore
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)    32473 2021-04-28 19:43:35.000000 i3a-2.1.0/LICENSE
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)     4525 2023-05-25 07:23:59.606853 i3a-2.1.0/PKG-INFO
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)      135 2021-04-28 19:43:35.000000 i3a-2.1.0/Pipfile
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)     2840 2023-05-25 07:20:10.000000 i3a-2.1.0/README.md
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)       38 2023-05-25 07:23:59.606853 i3a-2.1.0/setup.cfg
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)     2027 2023-05-25 06:52:18.000000 i3a-2.1.0/setup.py
-drwxr-xr-x   0 mgoral    (1000) mgoral    (1000)        0 2023-05-25 07:23:59.606853 i3a-2.1.0/src/
-drwxr-xr-x   0 mgoral    (1000) mgoral    (1000)        0 2023-05-25 07:23:59.606853 i3a-2.1.0/src/i3a/
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)        0 2021-04-28 19:43:35.000000 i3a-2.1.0/src/i3a/__init__.py
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)      142 2023-05-25 07:23:59.000000 i3a-2.1.0/src/i3a/_version.py
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)     8511 2021-06-22 05:59:34.000000 i3a-2.1.0/src/i3a/master_stack.py
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)      943 2021-06-22 05:59:34.000000 i3a-2.1.0/src/i3a/move_to_empty.py
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)     2508 2023-05-25 07:17:39.000000 i3a-2.1.0/src/i3a/resize_compass.py
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)     7036 2021-07-26 12:22:14.000000 i3a-2.1.0/src/i3a/swallow.py
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)      668 2023-05-25 07:06:06.000000 i3a-2.1.0/src/i3a/swap.py
-drwxr-xr-x   0 mgoral    (1000) mgoral    (1000)        0 2023-05-25 07:23:59.606853 i3a-2.1.0/src/i3a.egg-info/
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)     4525 2023-05-25 07:23:59.000000 i3a-2.1.0/src/i3a.egg-info/PKG-INFO
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)      383 2023-05-25 07:23:59.000000 i3a-2.1.0/src/i3a.egg-info/SOURCES.txt
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)        1 2023-05-25 07:23:59.000000 i3a-2.1.0/src/i3a.egg-info/dependency_links.txt
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)      204 2023-05-25 07:23:59.000000 i3a-2.1.0/src/i3a.egg-info/entry_points.txt
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)       13 2023-05-25 07:23:59.000000 i3a-2.1.0/src/i3a.egg-info/requires.txt
--rw-r--r--   0 mgoral    (1000) mgoral    (1000)        4 2023-05-25 07:23:59.000000 i3a-2.1.0/src/i3a.egg-info/top_level.txt
+drwxr-xr-x   0 mgoral    (1000) mgoral    (1000)        0 2023-06-09 21:25:06.601987 i3a-2.1.1/
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)      161 2021-04-28 19:43:35.000000 i3a-2.1.1/.gitignore
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)    32473 2021-04-28 19:43:35.000000 i3a-2.1.1/LICENSE
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)     3693 2023-06-09 21:25:06.601987 i3a-2.1.1/PKG-INFO
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)      135 2021-04-28 19:43:35.000000 i3a-2.1.1/Pipfile
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)     2840 2023-05-25 07:20:10.000000 i3a-2.1.1/README.md
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)       38 2023-06-09 21:25:06.601987 i3a-2.1.1/setup.cfg
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)     2026 2023-06-09 21:23:19.000000 i3a-2.1.1/setup.py
+drwxr-xr-x   0 mgoral    (1000) mgoral    (1000)        0 2023-06-09 21:25:06.601987 i3a-2.1.1/src/
+drwxr-xr-x   0 mgoral    (1000) mgoral    (1000)        0 2023-06-09 21:25:06.601987 i3a-2.1.1/src/i3a/
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)        0 2021-04-28 19:43:35.000000 i3a-2.1.1/src/i3a/__init__.py
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)      160 2023-06-09 21:25:06.000000 i3a-2.1.1/src/i3a/_version.py
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)     8511 2021-06-22 05:59:34.000000 i3a-2.1.1/src/i3a/master_stack.py
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)      943 2021-06-22 05:59:34.000000 i3a-2.1.1/src/i3a/move_to_empty.py
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)     2508 2023-05-25 07:17:39.000000 i3a-2.1.1/src/i3a/resize_compass.py
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)     7036 2021-07-26 12:22:14.000000 i3a-2.1.1/src/i3a/swallow.py
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)      668 2023-05-25 07:06:06.000000 i3a-2.1.1/src/i3a/swap.py
+drwxr-xr-x   0 mgoral    (1000) mgoral    (1000)        0 2023-06-09 21:25:06.601987 i3a-2.1.1/src/i3a.egg-info/
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)     3693 2023-06-09 21:25:06.000000 i3a-2.1.1/src/i3a.egg-info/PKG-INFO
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)      383 2023-06-09 21:25:06.000000 i3a-2.1.1/src/i3a.egg-info/SOURCES.txt
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)        1 2023-06-09 21:25:06.000000 i3a-2.1.1/src/i3a.egg-info/dependency_links.txt
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)      203 2023-06-09 21:25:06.000000 i3a-2.1.1/src/i3a.egg-info/entry_points.txt
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)       13 2023-06-09 21:25:06.000000 i3a-2.1.1/src/i3a.egg-info/requires.txt
+-rw-r--r--   0 mgoral    (1000) mgoral    (1000)        4 2023-06-09 21:25:06.000000 i3a-2.1.1/src/i3a.egg-info/top_level.txt
```

### Comparing `i3a-2.1.0/LICENSE` & `i3a-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `i3a-2.1.0/PKG-INFO` & `i3a-2.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,129 @@
 Metadata-Version: 2.1
 Name: i3a
-Version: 2.1.0
+Version: 2.1.1
 Summary: Automatic manager for i3 tiling
 Home-page: https://git.goral.net.pl/i3a.git
 Author: Michał Góral
 Author-email: dev@goral.net.pl
 License: GPLv3+
-Description: # i3a
-        
-        i3a is a set of scripts used for automation of i3 and sway window manager
-        layouts.
-        
-        ## Automation list
-        
-        ### i3a-master-stack
-        
-        Provides automatic master-stack layout, which is known from e.g. DWM. The
-        following kinds of the layout are possible:
-        
-        - master-stack area with DWM-like stack (stack windows are split)
-        - master-stack area with i3-like stack (stack windows are actual stack)
-        
-        To use, run `i3a-master-stack` with selected options (`i3a-master-stack
-        --help` for details). One way to run it automatically is via a systemd
-        user service.
-        
-        1.  Create the following file in _~/.config/systemd/user/i3a-master-stack_:
-        
-        ```
-        [Unit]
-        Description=i3a-master-stack
-        
-        [Service]
-        ExecStart=%h/.local/bin/i3a-master-stack --stack=dwm --stack-size=35
-        Restart=on-failure
-        ```
-        
-        2.  Add the following entry to your i3 or sway configuration file:
-        
-        ```
-        exec "systemctl --user restart i3a-master-stack.service"
-        ```
-        
-        ### i3a-swap
-        
-        Swap currently focused window between master and stack areas from
-        i3a-master-stack (technically it doesn't require running i3-master-stack).
-        
-        To use it, add the following binding to your i3 or sway configuration file:
-        
-        ```
-        bindsym $mod+f exec i3a-swap
-        ```
-        
-        ### i3a-swallow
-        
-        Provides automatic "swallowing": when a program runs a child process, the
-        parent is automatically hidden (moved to the scratchpad), which looks like if
-        it was replaced, or "swallowed" by the child window. It is especially useful
-        for graphical programs (video player, document viewer etc.) run from the
-        terminal.
-        
-        Provides a means of filtering both parent programs which can be swallowed and
-        child programs which can trigger swallowing.
-        
-        To use it, run `i3a-swallow` with selected options. One way to run it
-        automatically is via a systemd user service.
-        
-        1.  Create the following file in _~/.config/systemd/user/i3a-swallow_:
-        
-        ```
-        [Unit]
-        Description=i3a-swallow
-        
-        [Service]
-        ExecStart=%h/.local/bin/i3a-swallow
-        Restart=on-failure
-        ```
-        
-        2.  Add the following entry to your i3 or sway configuration file:
-        
-        ```
-        exec "systemctl --user restart i3a-swallow.service"
-        ```
-        
-        ### i3a-move-to-empty
-        
-        Moves currently focused container to the first empty workspace. Keep in mind
-        that this script relies on numbering of the workspaces.
-        
-        To use it, add the following binding to your i3 or sway configuration file:
-        
-        ```
-        bindsym $mod+w exec i3a-move-to-empty
-        ```
-        
-        ### i3a-resize-compass
-        
-        Extension of `resize` command. Currently focused window will automatically
-        grow or shrink in a direction passed to i3a-resize-compass.
-        
-        ```
-        bindsym $mod+Up exec i3a-resize-compass up 2ppt
-        bindsym $mod+Down exec i3a-resize-compass down 2ppt
-        bindsym $mod+Right exec i3a-resize-compass right 2ppt
-        bindsym $mod+Left exec i3a-resize-compass left 2ppt
-        ```
-        
-        ## Installation
-        
-        - [PyPI](https://pypi.org/project/i3a/)
-        - [AUR](https://aur.archlinux.org/packages/i3a/) (Arch Linux - unofficial)
-        
 Platform: linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# i3a
+
+i3a is a set of scripts used for automation of i3 and sway window manager
+layouts.
+
+## Automation list
+
+### i3a-master-stack
+
+Provides automatic master-stack layout, which is known from e.g. DWM. The
+following kinds of the layout are possible:
+
+- master-stack area with DWM-like stack (stack windows are split)
+- master-stack area with i3-like stack (stack windows are actual stack)
+
+To use, run `i3a-master-stack` with selected options (`i3a-master-stack
+--help` for details). One way to run it automatically is via a systemd
+user service.
+
+1.  Create the following file in _~/.config/systemd/user/i3a-master-stack_:
+
+```
+[Unit]
+Description=i3a-master-stack
+
+[Service]
+ExecStart=%h/.local/bin/i3a-master-stack --stack=dwm --stack-size=35
+Restart=on-failure
+```
+
+2.  Add the following entry to your i3 or sway configuration file:
+
+```
+exec "systemctl --user restart i3a-master-stack.service"
+```
+
+### i3a-swap
+
+Swap currently focused window between master and stack areas from
+i3a-master-stack (technically it doesn't require running i3-master-stack).
+
+To use it, add the following binding to your i3 or sway configuration file:
+
+```
+bindsym $mod+f exec i3a-swap
+```
+
+### i3a-swallow
+
+Provides automatic "swallowing": when a program runs a child process, the
+parent is automatically hidden (moved to the scratchpad), which looks like if
+it was replaced, or "swallowed" by the child window. It is especially useful
+for graphical programs (video player, document viewer etc.) run from the
+terminal.
+
+Provides a means of filtering both parent programs which can be swallowed and
+child programs which can trigger swallowing.
+
+To use it, run `i3a-swallow` with selected options. One way to run it
+automatically is via a systemd user service.
+
+1.  Create the following file in _~/.config/systemd/user/i3a-swallow_:
+
+```
+[Unit]
+Description=i3a-swallow
+
+[Service]
+ExecStart=%h/.local/bin/i3a-swallow
+Restart=on-failure
+```
+
+2.  Add the following entry to your i3 or sway configuration file:
+
+```
+exec "systemctl --user restart i3a-swallow.service"
+```
+
+### i3a-move-to-empty
+
+Moves currently focused container to the first empty workspace. Keep in mind
+that this script relies on numbering of the workspaces.
+
+To use it, add the following binding to your i3 or sway configuration file:
+
+```
+bindsym $mod+w exec i3a-move-to-empty
+```
+
+### i3a-resize-compass
+
+Extension of `resize` command. Currently focused window will automatically
+grow or shrink in a direction passed to i3a-resize-compass.
+
+```
+bindsym $mod+Up exec i3a-resize-compass up 2ppt
+bindsym $mod+Down exec i3a-resize-compass down 2ppt
+bindsym $mod+Right exec i3a-resize-compass right 2ppt
+bindsym $mod+Left exec i3a-resize-compass left 2ppt
+```
+
+## Installation
+
+- [PyPI](https://pypi.org/project/i3a/)
+- [AUR](https://aur.archlinux.org/packages/i3a/) (Arch Linux - unofficial)
```

### Comparing `i3a-2.1.0/README.md` & `i3a-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `i3a-2.1.0/setup.py` & `i3a-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
           long_description_content_type='text/markdown',
           use_scm_version={'write_to': 'src/i3a/_version.py'},
           license='GPLv3+',
           author='Michał Góral',
           author_email='dev@goral.net.pl',
           url='https://git.goral.net.pl/i3a.git',
           platforms=['linux'],
-          python_requires='>=3.7,<3.10',
+          python_requires='>=3.7,<4.0',
           setup_requires=['setuptools_scm'],
           install_requires=[
               'i3ipc==2.2.1',
           ],
 
           # https://pypi.python.org/pypi?%3Aaction=list_classifiers
           classifiers=['Development Status :: 5 - Production/Stable',
```

### Comparing `i3a-2.1.0/src/i3a/master_stack.py` & `i3a-2.1.1/src/i3a/master_stack.py`

 * *Files identical despite different names*

### Comparing `i3a-2.1.0/src/i3a/move_to_empty.py` & `i3a-2.1.1/src/i3a/move_to_empty.py`

 * *Files identical despite different names*

### Comparing `i3a-2.1.0/src/i3a/resize_compass.py` & `i3a-2.1.1/src/i3a/resize_compass.py`

 * *Files identical despite different names*

### Comparing `i3a-2.1.0/src/i3a/swallow.py` & `i3a-2.1.1/src/i3a/swallow.py`

 * *Files identical despite different names*

### Comparing `i3a-2.1.0/src/i3a/swap.py` & `i3a-2.1.1/src/i3a/swap.py`

 * *Files identical despite different names*

### Comparing `i3a-2.1.0/src/i3a.egg-info/PKG-INFO` & `i3a-2.1.1/src/i3a.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,129 @@
 Metadata-Version: 2.1
 Name: i3a
-Version: 2.1.0
+Version: 2.1.1
 Summary: Automatic manager for i3 tiling
 Home-page: https://git.goral.net.pl/i3a.git
 Author: Michał Góral
 Author-email: dev@goral.net.pl
 License: GPLv3+
-Description: # i3a
-        
-        i3a is a set of scripts used for automation of i3 and sway window manager
-        layouts.
-        
-        ## Automation list
-        
-        ### i3a-master-stack
-        
-        Provides automatic master-stack layout, which is known from e.g. DWM. The
-        following kinds of the layout are possible:
-        
-        - master-stack area with DWM-like stack (stack windows are split)
-        - master-stack area with i3-like stack (stack windows are actual stack)
-        
-        To use, run `i3a-master-stack` with selected options (`i3a-master-stack
-        --help` for details). One way to run it automatically is via a systemd
-        user service.
-        
-        1.  Create the following file in _~/.config/systemd/user/i3a-master-stack_:
-        
-        ```
-        [Unit]
-        Description=i3a-master-stack
-        
-        [Service]
-        ExecStart=%h/.local/bin/i3a-master-stack --stack=dwm --stack-size=35
-        Restart=on-failure
-        ```
-        
-        2.  Add the following entry to your i3 or sway configuration file:
-        
-        ```
-        exec "systemctl --user restart i3a-master-stack.service"
-        ```
-        
-        ### i3a-swap
-        
-        Swap currently focused window between master and stack areas from
-        i3a-master-stack (technically it doesn't require running i3-master-stack).
-        
-        To use it, add the following binding to your i3 or sway configuration file:
-        
-        ```
-        bindsym $mod+f exec i3a-swap
-        ```
-        
-        ### i3a-swallow
-        
-        Provides automatic "swallowing": when a program runs a child process, the
-        parent is automatically hidden (moved to the scratchpad), which looks like if
-        it was replaced, or "swallowed" by the child window. It is especially useful
-        for graphical programs (video player, document viewer etc.) run from the
-        terminal.
-        
-        Provides a means of filtering both parent programs which can be swallowed and
-        child programs which can trigger swallowing.
-        
-        To use it, run `i3a-swallow` with selected options. One way to run it
-        automatically is via a systemd user service.
-        
-        1.  Create the following file in _~/.config/systemd/user/i3a-swallow_:
-        
-        ```
-        [Unit]
-        Description=i3a-swallow
-        
-        [Service]
-        ExecStart=%h/.local/bin/i3a-swallow
-        Restart=on-failure
-        ```
-        
-        2.  Add the following entry to your i3 or sway configuration file:
-        
-        ```
-        exec "systemctl --user restart i3a-swallow.service"
-        ```
-        
-        ### i3a-move-to-empty
-        
-        Moves currently focused container to the first empty workspace. Keep in mind
-        that this script relies on numbering of the workspaces.
-        
-        To use it, add the following binding to your i3 or sway configuration file:
-        
-        ```
-        bindsym $mod+w exec i3a-move-to-empty
-        ```
-        
-        ### i3a-resize-compass
-        
-        Extension of `resize` command. Currently focused window will automatically
-        grow or shrink in a direction passed to i3a-resize-compass.
-        
-        ```
-        bindsym $mod+Up exec i3a-resize-compass up 2ppt
-        bindsym $mod+Down exec i3a-resize-compass down 2ppt
-        bindsym $mod+Right exec i3a-resize-compass right 2ppt
-        bindsym $mod+Left exec i3a-resize-compass left 2ppt
-        ```
-        
-        ## Installation
-        
-        - [PyPI](https://pypi.org/project/i3a/)
-        - [AUR](https://aur.archlinux.org/packages/i3a/) (Arch Linux - unofficial)
-        
 Platform: linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# i3a
+
+i3a is a set of scripts used for automation of i3 and sway window manager
+layouts.
+
+## Automation list
+
+### i3a-master-stack
+
+Provides automatic master-stack layout, which is known from e.g. DWM. The
+following kinds of the layout are possible:
+
+- master-stack area with DWM-like stack (stack windows are split)
+- master-stack area with i3-like stack (stack windows are actual stack)
+
+To use, run `i3a-master-stack` with selected options (`i3a-master-stack
+--help` for details). One way to run it automatically is via a systemd
+user service.
+
+1.  Create the following file in _~/.config/systemd/user/i3a-master-stack_:
+
+```
+[Unit]
+Description=i3a-master-stack
+
+[Service]
+ExecStart=%h/.local/bin/i3a-master-stack --stack=dwm --stack-size=35
+Restart=on-failure
+```
+
+2.  Add the following entry to your i3 or sway configuration file:
+
+```
+exec "systemctl --user restart i3a-master-stack.service"
+```
+
+### i3a-swap
+
+Swap currently focused window between master and stack areas from
+i3a-master-stack (technically it doesn't require running i3-master-stack).
+
+To use it, add the following binding to your i3 or sway configuration file:
+
+```
+bindsym $mod+f exec i3a-swap
+```
+
+### i3a-swallow
+
+Provides automatic "swallowing": when a program runs a child process, the
+parent is automatically hidden (moved to the scratchpad), which looks like if
+it was replaced, or "swallowed" by the child window. It is especially useful
+for graphical programs (video player, document viewer etc.) run from the
+terminal.
+
+Provides a means of filtering both parent programs which can be swallowed and
+child programs which can trigger swallowing.
+
+To use it, run `i3a-swallow` with selected options. One way to run it
+automatically is via a systemd user service.
+
+1.  Create the following file in _~/.config/systemd/user/i3a-swallow_:
+
+```
+[Unit]
+Description=i3a-swallow
+
+[Service]
+ExecStart=%h/.local/bin/i3a-swallow
+Restart=on-failure
+```
+
+2.  Add the following entry to your i3 or sway configuration file:
+
+```
+exec "systemctl --user restart i3a-swallow.service"
+```
+
+### i3a-move-to-empty
+
+Moves currently focused container to the first empty workspace. Keep in mind
+that this script relies on numbering of the workspaces.
+
+To use it, add the following binding to your i3 or sway configuration file:
+
+```
+bindsym $mod+w exec i3a-move-to-empty
+```
+
+### i3a-resize-compass
+
+Extension of `resize` command. Currently focused window will automatically
+grow or shrink in a direction passed to i3a-resize-compass.
+
+```
+bindsym $mod+Up exec i3a-resize-compass up 2ppt
+bindsym $mod+Down exec i3a-resize-compass down 2ppt
+bindsym $mod+Right exec i3a-resize-compass right 2ppt
+bindsym $mod+Left exec i3a-resize-compass left 2ppt
+```
+
+## Installation
+
+- [PyPI](https://pypi.org/project/i3a/)
+- [AUR](https://aur.archlinux.org/packages/i3a/) (Arch Linux - unofficial)
```

