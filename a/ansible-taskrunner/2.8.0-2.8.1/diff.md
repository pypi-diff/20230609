# Comparing `tmp/ansible_taskrunner-2.8.0.tar.gz` & `tmp/ansible_taskrunner-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_taskrunner-2.8.0.tar", last modified: Thu May 11 18:42:34 2023, max compression
+gzip compressed data, was "ansible_taskrunner-2.8.1.tar", last modified: Fri Jun  9 20:21:29 2023, max compression
```

## Comparing `ansible_taskrunner-2.8.0.tar` & `ansible_taskrunner-2.8.1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.217658 ansible_taskrunner-2.8.0/
--rw-r--r--   0 etejeda    (501) staff       (20)      313 2022-09-14 03:08:59.000000 ansible_taskrunner-2.8.0/.editorconfig
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.185647 ansible_taskrunner-2.8.0/.github/
--rw-r--r--   0 etejeda    (501) staff       (20)      344 2022-09-14 03:08:56.000000 ansible_taskrunner-2.8.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1558 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/.gitignore
--rw-r--r--   0 etejeda    (501) staff       (20)      314 2022-09-14 03:05:03.000000 ansible_taskrunner-2.8.0/.travis.yml
--rw-r--r--   0 etejeda    (501) staff       (20)      175 2022-09-14 03:04:51.000000 ansible_taskrunner-2.8.0/AUTHORS.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     3790 2022-09-14 03:04:49.000000 ansible_taskrunner-2.8.0/CONTRIBUTING.rst
--rw-r--r--   0 etejeda    (501) staff       (20)    26436 2023-03-24 15:57:41.000000 ansible_taskrunner-2.8.0/HISTORY.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1097 2022-09-14 03:04:47.000000 ansible_taskrunner-2.8.0/LICENSE
--rw-r--r--   0 etejeda    (501) staff       (20)      365 2022-09-14 03:18:38.000000 ansible_taskrunner-2.8.0/MANIFEST.in
--rw-r--r--   0 etejeda    (501) staff       (20)    11310 2023-03-07 16:33:18.000000 ansible_taskrunner-2.8.0/Makefile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)    57555 2023-05-11 18:42:34.218100 ansible_taskrunner-2.8.0/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)    58542 2023-03-15 18:52:08.000000 ansible_taskrunner-2.8.0/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)     5182 2023-03-08 21:35:43.000000 ansible_taskrunner-2.8.0/Taskfile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-05-11 18:41:42.000000 ansible_taskrunner-2.8.0/VERSION.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.188819 ansible_taskrunner-2.8.0/ansible_taskrunner/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2479 2023-03-07 16:10:01.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/cli.py
--rw-r--r--   0 etejeda    (501) staff       (20)      953 2023-05-11 18:40:42.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/config.py
--rw-r--r--   0 etejeda    (501) staff       (20)      803 2023-03-08 21:32:42.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/defaults.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.193776 ansible_taskrunner-2.8.0/ansible_taskrunner/files/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.194358 ansible_taskrunner-2.8.0/ansible_taskrunner/files/cfg/
--rw-r--r--   0 etejeda    (501) staff       (20)      159 2023-01-10 10:27:20.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/files/cfg/default.ini
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.194920 ansible_taskrunner-2.8.0/ansible_taskrunner/files/macros/
--rw-r--r--   0 etejeda    (501) staff       (20)     1116 2023-01-10 10:27:25.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/files/macros/default.mac
--rw-r--r--   0 etejeda    (501) staff       (20)      956 2023-01-10 10:27:29.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/files/start-tutorial.bat
--rw-r--r--   0 etejeda    (501) staff       (20)     1772 2023-01-10 10:27:30.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/files/tasks-console.bat
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.195448 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.195920 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/bastion_mode/
--rw-r--r--   0 etejeda    (501) staff       (20)     1354 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/bastion_mode/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.199192 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/cli/
--rw-r--r--   0 etejeda    (501) staff       (20)     6176 2023-05-11 18:40:41.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/cli/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2868 2023-03-07 15:21:06.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/cli/click_commands_create_group.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2917 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/cli/click_commands_create_init.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5235 2023-05-11 18:40:40.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/cli/click_commands_create_sub.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5660 2023-03-24 15:45:23.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/cli/click_commands_init_sub.py
--rw-r--r--   0 etejeda    (501) staff       (20)     4667 2023-03-15 18:34:45.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/cli/invocation.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.200950 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/click_extras/
--rw-r--r--   0 etejeda    (501) staff       (20)     9507 2023-05-11 18:40:42.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/click_extras/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2228 2023-03-24 15:54:02.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/click_extras/help.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2512 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/click_extras/options_advanced.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.201416 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/errorhandler/
--rw-r--r--   0 etejeda    (501) staff       (20)      738 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/errorhandler/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.201743 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/formatting/
--rw-r--r--   0 etejeda    (501) staff       (20)      787 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/formatting/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.202293 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/help/
--rw-r--r--   0 etejeda    (501) staff       (20)     2738 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/help/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.203094 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/language/
--rw-r--r--   0 etejeda    (501) staff       (20)      876 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/language/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)       19 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/language/en.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.203623 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/logger/
--rw-r--r--   0 etejeda    (501) staff       (20)      462 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/logger/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.204014 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/proc_mgmt/
--rw-r--r--   0 etejeda    (501) staff       (20)     3334 2023-04-28 19:10:32.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/proc_mgmt/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.205236 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/providers/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/providers/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)    15894 2023-03-13 18:12:26.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/providers/ansible.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2481 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/providers/bash.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2561 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/providers/vagrant.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.206503 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/sshutil/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/sshutil/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5474 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/sshutil/client.py
--rw-r--r--   0 etejeda    (501) staff       (20)    16240 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/sshutil/scp.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2949 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/libs/sshutil/sync.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1485 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/logger.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.206814 ansible_taskrunner-2.8.0/ansible_taskrunner/plugins/
--rw-r--r--   0 etejeda    (501) staff       (20)     1951 2023-01-10 10:29:26.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/plugins/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5089 2023-01-09 21:15:54.000000 ansible_taskrunner-2.8.0/ansible_taskrunner/setup.cx_freeze.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.192661 ansible_taskrunner-2.8.0/ansible_taskrunner.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)    57555 2023-05-11 18:42:33.000000 ansible_taskrunner-2.8.0/ansible_taskrunner.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     2948 2023-05-11 18:42:34.000000 ansible_taskrunner-2.8.0/ansible_taskrunner.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 18:42:33.000000 ansible_taskrunner-2.8.0/ansible_taskrunner.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       53 2023-05-11 18:42:33.000000 ansible_taskrunner-2.8.0/ansible_taskrunner.egg-info/entry_points.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-03-24 15:58:06.000000 ansible_taskrunner-2.8.0/ansible_taskrunner.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)      244 2023-05-11 18:42:33.000000 ansible_taskrunner-2.8.0/ansible_taskrunner.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       25 2023-05-11 18:42:33.000000 ansible_taskrunner-2.8.0/ansible_taskrunner.egg-info/top_level.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.209830 ansible_taskrunner-2.8.0/docs/
--rw-r--r--   0 etejeda    (501) staff       (20)      636 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/docs/Makefile
--rw-r--r--   0 etejeda    (501) staff       (20)       29 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.0/docs/authors.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     5127 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.0/docs/conf.py
--rw-r--r--   0 etejeda    (501) staff       (20)       34 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.0/docs/contributing.rst
--rw-r--r--   0 etejeda    (501) staff       (20)       29 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.0/docs/history.rst
--rw-r--r--   0 etejeda    (501) staff       (20)      335 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.0/docs/index.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     1261 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.0/docs/installation.rst
--rw-r--r--   0 etejeda    (501) staff       (20)      816 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.0/docs/make.bat
--rw-r--r--   0 etejeda    (501) staff       (20)       28 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.0/docs/readme.rst
--rw-r--r--   0 etejeda    (501) staff       (20)       98 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.0/docs/usage.rst
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.174532 ansible_taskrunner-2.8.0/examples/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.210887 ansible_taskrunner-2.8.0/examples/ansible/
--rw-r--r--   0 etejeda    (501) staff       (20)     5071 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/examples/ansible/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1967 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/examples/ansible/Taskfile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)       47 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.0/examples/ansible/config.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.211896 ansible_taskrunner-2.8.0/examples/bash/
--rw-r--r--   0 etejeda    (501) staff       (20)     2933 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/examples/bash/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1025 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/examples/bash/Taskfile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)       44 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.0/examples/bash/config.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.212286 ansible_taskrunner-2.8.0/examples/choice/
--rw-r--r--   0 etejeda    (501) staff       (20)     2300 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/examples/choice/Taskfile.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.213800 ansible_taskrunner-2.8.0/examples/custom-cli-provider/
--rw-r--r--   0 etejeda    (501) staff       (20)     3046 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.0/examples/custom-cli-provider/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1025 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/examples/custom-cli-provider/Taskfile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)       47 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.0/examples/custom-cli-provider/config.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      177 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.0/examples/custom-cli-provider/dynamic-import.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.173374 ansible_taskrunner-2.8.0/examples/custom-cli-provider/plugins/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.173562 ansible_taskrunner-2.8.0/examples/custom-cli-provider/plugins/providers/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.214133 ansible_taskrunner-2.8.0/examples/custom-cli-provider/plugins/providers/example/
--rw-r--r--   0 etejeda    (501) staff       (20)     2187 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.0/examples/custom-cli-provider/plugins/providers/example/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.214487 ansible_taskrunner-2.8.0/examples/mutually-exclusive/
--rw-r--r--   0 etejeda    (501) staff       (20)     2354 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/examples/mutually-exclusive/Taskfile.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.214864 ansible_taskrunner-2.8.0/examples/prompt/
--rw-r--r--   0 etejeda    (501) staff       (20)     2275 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/examples/prompt/Taskfile.yaml
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.216434 ansible_taskrunner-2.8.0/examples/vagrant/
--rw-r--r--   0 etejeda    (501) staff       (20)     4168 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/examples/vagrant/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)     1506 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.0/examples/vagrant/Taskfile.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)     3092 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.0/examples/vagrant/Vagrantfile
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.0/examples/vagrant/config.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      129 2023-03-07 16:28:11.000000 ansible_taskrunner-2.8.0/requirements_dev.txt
--rw-r--r--   0 etejeda    (501) staff       (20)     1591 2023-05-11 18:42:34.219112 ansible_taskrunner-2.8.0/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)       39 2022-09-14 03:03:38.000000 ansible_taskrunner-2.8.0/setup.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 18:42:34.217289 ansible_taskrunner-2.8.0/tests/
--rw-r--r--   0 etejeda    (501) staff       (20)       76 2022-09-14 03:04:16.000000 ansible_taskrunner-2.8.0/tests/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2433 2023-03-13 18:35:06.000000 ansible_taskrunner-2.8.0/tests/test_ansible_taskrunner.py
--rw-r--r--   0 etejeda    (501) staff       (20)      343 2022-09-14 03:17:41.000000 ansible_taskrunner-2.8.0/tox.ini
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.451826 ansible_taskrunner-2.8.1/
+-rw-r--r--   0 etejeda    (501) staff       (20)      313 2022-09-14 03:08:59.000000 ansible_taskrunner-2.8.1/.editorconfig
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.410633 ansible_taskrunner-2.8.1/.github/
+-rw-r--r--   0 etejeda    (501) staff       (20)      344 2022-09-14 03:08:56.000000 ansible_taskrunner-2.8.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1558 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/.gitignore
+-rw-r--r--   0 etejeda    (501) staff       (20)      314 2022-09-14 03:05:03.000000 ansible_taskrunner-2.8.1/.travis.yml
+-rw-r--r--   0 etejeda    (501) staff       (20)      175 2022-09-14 03:04:51.000000 ansible_taskrunner-2.8.1/AUTHORS.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     3790 2022-09-14 03:04:49.000000 ansible_taskrunner-2.8.1/CONTRIBUTING.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)    26436 2023-03-24 15:57:41.000000 ansible_taskrunner-2.8.1/HISTORY.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1097 2022-09-14 03:04:47.000000 ansible_taskrunner-2.8.1/LICENSE
+-rw-r--r--   0 etejeda    (501) staff       (20)      365 2022-09-14 03:18:38.000000 ansible_taskrunner-2.8.1/MANIFEST.in
+-rw-r--r--   0 etejeda    (501) staff       (20)    11310 2023-05-14 18:24:49.000000 ansible_taskrunner-2.8.1/Makefile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)    57555 2023-06-09 20:21:29.452467 ansible_taskrunner-2.8.1/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)    58542 2023-03-15 18:52:08.000000 ansible_taskrunner-2.8.1/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     5182 2023-03-08 21:35:43.000000 ansible_taskrunner-2.8.1/Taskfile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-06-09 20:21:13.000000 ansible_taskrunner-2.8.1/VERSION.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.413204 ansible_taskrunner-2.8.1/ansible_taskrunner/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2479 2023-03-07 16:10:01.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/cli.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      953 2023-06-09 16:20:10.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/config.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      803 2023-03-08 21:32:42.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/defaults.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.417372 ansible_taskrunner-2.8.1/ansible_taskrunner/files/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.417991 ansible_taskrunner-2.8.1/ansible_taskrunner/files/cfg/
+-rw-r--r--   0 etejeda    (501) staff       (20)      159 2023-01-10 10:27:20.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/files/cfg/default.ini
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.418596 ansible_taskrunner-2.8.1/ansible_taskrunner/files/macros/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1116 2023-01-10 10:27:25.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/files/macros/default.mac
+-rw-r--r--   0 etejeda    (501) staff       (20)      956 2023-01-10 10:27:29.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/files/start-tutorial.bat
+-rw-r--r--   0 etejeda    (501) staff       (20)     1772 2023-01-10 10:27:30.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/files/tasks-console.bat
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.419234 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.419494 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/bastion_mode/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1354 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/bastion_mode/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.423169 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/cli/
+-rw-r--r--   0 etejeda    (501) staff       (20)     6176 2023-05-11 18:40:41.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/cli/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2868 2023-03-07 15:21:06.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/cli/click_commands_create_group.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2917 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/cli/click_commands_create_init.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5235 2023-05-11 18:40:40.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/cli/click_commands_create_sub.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5660 2023-03-24 15:45:23.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/cli/click_commands_init_sub.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     4667 2023-03-15 18:34:45.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/cli/invocation.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.424630 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/click_extras/
+-rw-r--r--   0 etejeda    (501) staff       (20)     9616 2023-05-22 20:24:50.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/click_extras/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2228 2023-03-24 15:54:02.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/click_extras/help.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2512 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/click_extras/options_advanced.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.425131 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/errorhandler/
+-rw-r--r--   0 etejeda    (501) staff       (20)      738 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/errorhandler/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.425710 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/formatting/
+-rw-r--r--   0 etejeda    (501) staff       (20)      787 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/formatting/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.426280 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/help/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2738 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/help/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.427329 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/language/
+-rw-r--r--   0 etejeda    (501) staff       (20)      876 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/language/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)       19 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/language/en.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.427844 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/logger/
+-rw-r--r--   0 etejeda    (501) staff       (20)      462 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/logger/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.428350 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/proc_mgmt/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3334 2023-04-28 19:10:32.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/proc_mgmt/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.430069 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/providers/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/providers/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)    15894 2023-03-13 18:12:26.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/providers/ansible.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2481 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/providers/bash.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2561 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/providers/vagrant.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.431738 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/sshutil/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/sshutil/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5474 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/sshutil/client.py
+-rw-r--r--   0 etejeda    (501) staff       (20)    16240 2023-01-09 04:21:28.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/sshutil/scp.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2949 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/libs/sshutil/sync.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1444 2023-06-09 20:18:59.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/logger.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.432135 ansible_taskrunner-2.8.1/ansible_taskrunner/plugins/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1951 2023-01-10 10:29:26.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/plugins/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5089 2023-01-09 21:15:54.000000 ansible_taskrunner-2.8.1/ansible_taskrunner/setup.cx_freeze.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.416354 ansible_taskrunner-2.8.1/ansible_taskrunner.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)    57555 2023-06-09 20:21:29.000000 ansible_taskrunner-2.8.1/ansible_taskrunner.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     2948 2023-06-09 20:21:29.000000 ansible_taskrunner-2.8.1/ansible_taskrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-09 20:21:29.000000 ansible_taskrunner-2.8.1/ansible_taskrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       53 2023-06-09 20:21:29.000000 ansible_taskrunner-2.8.1/ansible_taskrunner.egg-info/entry_points.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-09 20:21:29.000000 ansible_taskrunner-2.8.1/ansible_taskrunner.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)      244 2023-06-09 20:21:29.000000 ansible_taskrunner-2.8.1/ansible_taskrunner.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       25 2023-06-09 20:21:29.000000 ansible_taskrunner-2.8.1/ansible_taskrunner.egg-info/top_level.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.437046 ansible_taskrunner-2.8.1/docs/
+-rw-r--r--   0 etejeda    (501) staff       (20)      636 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/docs/Makefile
+-rw-r--r--   0 etejeda    (501) staff       (20)       29 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.1/docs/authors.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     5127 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.1/docs/conf.py
+-rw-r--r--   0 etejeda    (501) staff       (20)       34 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.1/docs/contributing.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)       29 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.1/docs/history.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)      335 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.1/docs/index.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     1261 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.1/docs/installation.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)      816 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.1/docs/make.bat
+-rw-r--r--   0 etejeda    (501) staff       (20)       28 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.1/docs/readme.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)       98 2022-09-14 03:04:03.000000 ansible_taskrunner-2.8.1/docs/usage.rst
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.401217 ansible_taskrunner-2.8.1/examples/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.438892 ansible_taskrunner-2.8.1/examples/ansible/
+-rw-r--r--   0 etejeda    (501) staff       (20)     5071 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/examples/ansible/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1967 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/examples/ansible/Taskfile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)       47 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.1/examples/ansible/config.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.440945 ansible_taskrunner-2.8.1/examples/bash/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2933 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/examples/bash/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1025 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/examples/bash/Taskfile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)       44 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.1/examples/bash/config.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.441722 ansible_taskrunner-2.8.1/examples/choice/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2300 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/examples/choice/Taskfile.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.444329 ansible_taskrunner-2.8.1/examples/custom-cli-provider/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3046 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.1/examples/custom-cli-provider/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1025 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/examples/custom-cli-provider/Taskfile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)       47 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.1/examples/custom-cli-provider/config.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      177 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.1/examples/custom-cli-provider/dynamic-import.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.400214 ansible_taskrunner-2.8.1/examples/custom-cli-provider/plugins/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.400392 ansible_taskrunner-2.8.1/examples/custom-cli-provider/plugins/providers/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.445140 ansible_taskrunner-2.8.1/examples/custom-cli-provider/plugins/providers/example/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2187 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.1/examples/custom-cli-provider/plugins/providers/example/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.445870 ansible_taskrunner-2.8.1/examples/mutually-exclusive/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2354 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/examples/mutually-exclusive/Taskfile.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.446610 ansible_taskrunner-2.8.1/examples/prompt/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2275 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/examples/prompt/Taskfile.yaml
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.449397 ansible_taskrunner-2.8.1/examples/vagrant/
+-rw-r--r--   0 etejeda    (501) staff       (20)     4168 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/examples/vagrant/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)     1506 2023-03-07 02:31:15.000000 ansible_taskrunner-2.8.1/examples/vagrant/Taskfile.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)     3092 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.1/examples/vagrant/Vagrantfile
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2022-09-14 03:03:59.000000 ansible_taskrunner-2.8.1/examples/vagrant/config.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      129 2023-03-07 16:28:11.000000 ansible_taskrunner-2.8.1/requirements_dev.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)     1591 2023-06-09 20:21:29.454555 ansible_taskrunner-2.8.1/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)       39 2022-09-14 03:03:38.000000 ansible_taskrunner-2.8.1/setup.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:21:29.450583 ansible_taskrunner-2.8.1/tests/
+-rw-r--r--   0 etejeda    (501) staff       (20)       76 2022-09-14 03:04:16.000000 ansible_taskrunner-2.8.1/tests/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2433 2023-03-13 18:35:06.000000 ansible_taskrunner-2.8.1/tests/test_ansible_taskrunner.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      343 2022-09-14 03:17:41.000000 ansible_taskrunner-2.8.1/tox.ini
```

### Comparing `ansible_taskrunner-2.8.0/.gitignore` & `ansible_taskrunner-2.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/CONTRIBUTING.rst` & `ansible_taskrunner-2.8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/HISTORY.md` & `ansible_taskrunner-2.8.1/HISTORY.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/LICENSE` & `ansible_taskrunner-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/Makefile.yaml` & `ansible_taskrunner-2.8.1/Makefile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/PKG-INFO` & `ansible_taskrunner-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible_taskrunner
-Version: 2.8.0
+Version: 2.8.1
 Summary: Ansible Task Runner
 Home-page: https://github.com/berttejeda/ansible-taskrunner.git
 Author: Engelbert Tejeda
 Author-email: etejeda@tecknicos.com
 Keywords: ansible,playbook,wrapper,bash,python,click,task-runner,subprocess,yaml,cli,options
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ansible_taskrunner-2.8.0/README.md` & `ansible_taskrunner-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/Taskfile.yaml` & `ansible_taskrunner-2.8.1/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/cli.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/cli.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/config.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/config.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/defaults.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/defaults.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/files/macros/default.mac` & `ansible_taskrunner-2.8.1/ansible_taskrunner/files/macros/default.mac`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/files/start-tutorial.bat` & `ansible_taskrunner-2.8.1/ansible_taskrunner/files/start-tutorial.bat`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/files/tasks-console.bat` & `ansible_taskrunner-2.8.1/ansible_taskrunner/files/tasks-console.bat`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/bastion_mode/__init__.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/bastion_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/cli/__init__.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/cli/click_commands_create_group.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/cli/click_commands_create_group.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/cli/click_commands_create_init.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/cli/click_commands_create_init.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/cli/click_commands_create_sub.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/cli/click_commands_create_sub.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/cli/click_commands_init_sub.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/cli/click_commands_init_sub.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/cli/invocation.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/cli/invocation.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/click_extras/__init__.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/click_extras/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,15 @@
             option_is_flag = bool(option.get('is_flag', False))
             option_is_hidden = bool(option.get('is_hidden', False))
             option_show_choices = bool(option.get('show_choices', True))
             option_show_envvar = bool(option.get('env_var_show', True))
             option_supports_counting = bool(option.get('allow_counting', False))
             option_supports_multiple = bool(option.get('allow_multiple', False))
             option_value_from_env = option.get('env_var', None)
+            option_default_value = option.get('default', None)
             mutually_exclusive_with = option.get('mutually_exclusive_with', '')
             required_if = option.get('required_if', '')
             not_required_if = option.get('not_required_if', '')
 
             if mutually_exclusive_with and option_required:
                 logger.warning(f"Not honoring mutual exclusivity of option '{option_name}' " + \
                                f"and options with variables {mutually_exclusive_with}, as 'required' must be False")
@@ -183,14 +184,15 @@
                 *param_declarations,
                 option_variable,
                 cls=option_class,
                 confirmation_prompt=option_confirm_prompt,
                 count=option_supports_counting,
                 envvar=option_value_from_env,
                 nargs=option_nargs,
+                default=option_default_value,
                 help=option_help_effective,
                 hide_input=option_secure,
                 hidden=option_is_hidden,
                 is_flag=option_is_flag,
                 prompt=option_prompt,
                 prompt_required=option_prompt_required,
                 multiple=option_supports_multiple,
```

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/click_extras/help.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/click_extras/help.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/click_extras/options_advanced.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/click_extras/options_advanced.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/errorhandler/__init__.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/errorhandler/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/formatting/__init__.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/help/__init__.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/help/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/language/__init__.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/language/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/proc_mgmt/__init__.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/proc_mgmt/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/providers/ansible.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/providers/ansible.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/providers/bash.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/providers/bash.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/providers/vagrant.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/providers/vagrant.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/sshutil/client.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/sshutil/client.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/sshutil/scp.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/sshutil/scp.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/libs/sshutil/sync.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/libs/sshutil/sync.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/logger.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 import coloredlogs
 import os
 import sys
 
 class Logger:
 
   def __init__(self, **kwargs):
-    env_debug_is_on = os.environ.get('WEBTERMINAL_DEBUG', '').lower() in [
+    env_debug_is_on = os.environ.get('TASKS_DEBUG', '').lower() in [
     't', 'true', '1', 'on', 'y', 'yes']
     self.debug = kwargs.get('debug', False) or env_debug_is_on
     self.FORMAT_STR = "%(asctime)s %(name)s [%(levelname)s]: %(message)s"
     self.formatter = logging.Formatter(
       self.FORMAT_STR,
       datefmt='%Y-%m-%d %H:%M:%S'
     )
     self.logfile_path = kwargs.get('logfile_path')
     self.logfile_write_mode = kwargs.get('logfile_write_mode', 'a')
 
   def init_logger(self, name=None, debug=False):
     # Setup Logging
     logger = logging.getLogger(name)
     # TODO Find a better approach to this hacky method
-    if '--debug' in ' '.join(sys.argv) or self.debug:
+    if self.debug:
         logging_level = logging.DEBUG
     else:
         logging_level = logging.INFO
     logger.setLevel(logging_level)
     stdout_handler = logging.StreamHandler(sys.stdout)
     stdout_handler.setFormatter(self.formatter)
     logger.addHandler(stdout_handler)
```

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/plugins/__init__.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner/setup.cx_freeze.py` & `ansible_taskrunner-2.8.1/ansible_taskrunner/setup.cx_freeze.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner.egg-info/PKG-INFO` & `ansible_taskrunner-2.8.1/ansible_taskrunner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-taskrunner
-Version: 2.8.0
+Version: 2.8.1
 Summary: Ansible Task Runner
 Home-page: https://github.com/berttejeda/ansible-taskrunner.git
 Author: Engelbert Tejeda
 Author-email: etejeda@tecknicos.com
 Keywords: ansible,playbook,wrapper,bash,python,click,task-runner,subprocess,yaml,cli,options
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ansible_taskrunner-2.8.0/ansible_taskrunner.egg-info/SOURCES.txt` & `ansible_taskrunner-2.8.1/ansible_taskrunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/docs/Makefile` & `ansible_taskrunner-2.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/docs/conf.py` & `ansible_taskrunner-2.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/docs/installation.rst` & `ansible_taskrunner-2.8.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/docs/make.bat` & `ansible_taskrunner-2.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/examples/ansible/README.md` & `ansible_taskrunner-2.8.1/examples/ansible/README.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/examples/ansible/Taskfile.yaml` & `ansible_taskrunner-2.8.1/examples/ansible/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/examples/bash/README.md` & `ansible_taskrunner-2.8.1/examples/bash/README.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/examples/bash/Taskfile.yaml` & `ansible_taskrunner-2.8.1/examples/bash/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/examples/choice/Taskfile.yaml` & `ansible_taskrunner-2.8.1/examples/choice/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/examples/custom-cli-provider/README.md` & `ansible_taskrunner-2.8.1/examples/custom-cli-provider/README.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/examples/custom-cli-provider/Taskfile.yaml` & `ansible_taskrunner-2.8.1/examples/custom-cli-provider/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/examples/custom-cli-provider/plugins/providers/example/__init__.py` & `ansible_taskrunner-2.8.1/examples/custom-cli-provider/plugins/providers/example/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/examples/mutually-exclusive/Taskfile.yaml` & `ansible_taskrunner-2.8.1/examples/mutually-exclusive/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/examples/prompt/Taskfile.yaml` & `ansible_taskrunner-2.8.1/examples/prompt/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/examples/vagrant/README.md` & `ansible_taskrunner-2.8.1/examples/vagrant/README.md`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/examples/vagrant/Taskfile.yaml` & `ansible_taskrunner-2.8.1/examples/vagrant/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/examples/vagrant/Vagrantfile` & `ansible_taskrunner-2.8.1/examples/vagrant/Vagrantfile`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/setup.cfg` & `ansible_taskrunner-2.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ansible_taskrunner-2.8.0/tests/test_ansible_taskrunner.py` & `ansible_taskrunner-2.8.1/tests/test_ansible_taskrunner.py`

 * *Files identical despite different names*

