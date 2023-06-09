# Comparing `tmp/planemo-0.8.4.tar.gz` & `tmp/planemo-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/planemo-0.8.4.tar", last modified: Thu Apr 30 18:02:14 2015, max compression
+gzip compressed data, was "dist/planemo-0.9.0.tar", last modified: Mon May  4 00:15:19 2015, max compression
```

## Comparing `planemo-0.8.4.tar` & `planemo-0.9.0.tar`

### file list

```diff
@@ -1,144 +1,149 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/
--rw-rw-r--   0 john      (1000) john      (1000)      291 2015-04-30 18:02:14.000000 planemo-0.8.4/setup.cfg
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)       57 2015-04-30 18:02:13.000000 planemo-0.8.4/planemo.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2015-04-30 18:02:13.000000 planemo-0.8.4/planemo.egg-info/not-zip-safe
--rw-rw-r--   0 john      (1000) john      (1000)     4179 2015-04-30 18:02:13.000000 planemo-0.8.4/planemo.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)       67 2015-04-30 18:02:13.000000 planemo-0.8.4/planemo.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)    33289 2015-04-30 18:02:13.000000 planemo-0.8.4/planemo.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)        1 2015-04-30 18:02:13.000000 planemo-0.8.4/planemo.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       20 2015-04-30 18:02:13.000000 planemo-0.8.4/planemo.egg-info/top_level.txt
--rw-rw-r--   0 john      (1000) john      (1000)     1664 2015-04-29 12:43:36.000000 planemo-0.8.4/CODE_OF_CONDUCT.rst
--rw-rw-r--   0 john      (1000) john      (1000)      117 2015-04-29 12:43:36.000000 planemo-0.8.4/MANIFEST.in
--rw-rw-r--   0 john      (1000) john      (1000)     8929 2015-04-29 12:43:36.000000 planemo-0.8.4/README.rst
--rw-rw-r--   0 john      (1000) john      (1000)    33289 2015-04-30 18:02:14.000000 planemo-0.8.4/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)    11097 2014-12-09 03:06:38.000000 planemo-0.8.4/LICENSE
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo_ext/
--rw-rw-r--   0 john      (1000) john      (1000)        2 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo_ext/galaxy/
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo_ext/galaxy/util/
--rw-rw-r--   0 john      (1000) john      (1000)     2537 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/util/plugin_config.py
--rw-rw-r--   0 john      (1000) john      (1000)     1039 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/util/submodules.py
--rw-rw-r--   0 john      (1000) john      (1000)      599 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/util/directory_hash.py
--rw-rw-r--   0 john      (1000) john      (1000)     7488 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/util/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      830 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/util/bunch.py
--rw-rw-r--   0 john      (1000) john      (1000)      626 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/util/sleeper.py
--rw-rw-r--   0 john      (1000) john      (1000)     2222 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/util/odict.py
--rw-rw-r--   0 john      (1000) john      (1000)       49 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo_ext/galaxy/eggs/
--rw-rw-r--   0 john      (1000) john      (1000)      373 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/eggs/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      220 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/exceptions.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo_ext/galaxy/tools/
--rw-rw-r--   0 john      (1000) john      (1000)     3351 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/lint.py
--rw-rw-r--   0 john      (1000) john      (1000)     2312 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/loader_directory.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo_ext/galaxy/tools/linters/
--rw-rw-r--   0 john      (1000) john      (1000)     1254 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/linters/xsd_util.py
--rw-rw-r--   0 john      (1000) john      (1000)      958 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/linters/command.py
--rw-rw-r--   0 john      (1000) john      (1000)      879 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/linters/outputs.py
--rw-rw-r--   0 john      (1000) john      (1000)      543 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/linters/top_level.py
--rw-rw-r--   0 john      (1000) john      (1000)     1006 2015-04-29 12:45:41.000000 planemo-0.8.4/planemo_ext/galaxy/tools/linters/xml_order.py
--rw-rw-r--   0 john      (1000) john      (1000)      315 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/linters/xsd.py
--rw-rw-r--   0 john      (1000) john      (1000)     1371 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/linters/inputs.py
--rw-rw-r--   0 john      (1000) john      (1000)     1023 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/linters/help.py
--rw-rw-r--   0 john      (1000) john      (1000)       37 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/linters/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      988 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/linters/tests.py
--rw-rw-r--   0 john      (1000) john      (1000)     1833 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/linters/stdio.py
--rw-rw-r--   0 john      (1000) john      (1000)      990 2015-04-29 16:02:29.000000 planemo-0.8.4/planemo_ext/galaxy/tools/linters/citations.py
--rw-rw-r--   0 john      (1000) john      (1000)        0 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/
--rw-rw-r--   0 john      (1000) john      (1000)     5315 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/docker_util.py
--rw-rw-r--   0 john      (1000) john      (1000)    13204 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/containers.py
--rw-rw-r--   0 john      (1000) john      (1000)     2966 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/dependencies.py
--rw-rw-r--   0 john      (1000) john      (1000)     2493 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/dockerfiles.py
--rw-rw-r--   0 john      (1000) john      (1000)     4564 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/__init__.py
--rwxrwxr-x   0 john      (1000) john      (1000)    19588 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/brew_exts.py
--rw-rw-r--   0 john      (1000) john      (1000)     3413 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/requirements.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/resolvers/
--rw-rw-r--   0 john      (1000) john      (1000)     3022 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/resolvers/tool_shed_packages.py
--rw-rw-r--   0 john      (1000) john      (1000)     3194 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/resolvers/galaxy_packages.py
--rw-rw-r--   0 john      (1000) john      (1000)     2769 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/resolvers/resolver_mixins.py
--rw-rw-r--   0 john      (1000) john      (1000)     5246 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/resolvers/brewed_tool_shed_packages.py
--rw-rw-r--   0 john      (1000) john      (1000)     6098 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/resolvers/modules.py
--rw-rw-r--   0 john      (1000) john      (1000)      999 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/resolvers/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1947 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/resolvers/homebrew.py
--rw-rw-r--   0 john      (1000) john      (1000)     1179 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/brew_util.py
--rw-rw-r--   0 john      (1000) john      (1000)     1486 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/deps/commands.py
--rw-rw-r--   0 john      (1000) john      (1000)     6894 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo_ext/galaxy/tools/loader.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo_ext/tool_factory_2/
--rw-rw-r--   0 john      (1000) john      (1000)    44013 2015-04-30 17:46:37.000000 planemo-0.8.4/planemo_ext/tool_factory_2/rgToolFactory2.py
--rw-rw-r--   0 john      (1000) john      (1000)     2233 2015-04-30 17:46:37.000000 planemo-0.8.4/planemo_ext/tool_factory_2/getlocalrpackages.py
--rw-rw-r--   0 john      (1000) john      (1000)    21748 2015-04-30 17:47:59.000000 planemo-0.8.4/planemo_ext/tool_factory_2/rgToolFactory2.xml
--rw-rw-r--   0 john      (1000) john      (1000)    26443 2015-04-30 17:46:37.000000 planemo-0.8.4/planemo_ext/tool_factory_2/LICENSE
--rw-rw-r--   0 john      (1000) john      (1000)    18783 2015-04-30 17:59:07.000000 planemo-0.8.4/HISTORY.rst
--rw-rw-r--   0 john      (1000) john      (1000)     3372 2015-04-29 12:43:36.000000 planemo-0.8.4/setup.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo/
--rw-rw-r--   0 john      (1000) john      (1000)      977 2015-02-16 00:41:44.000000 planemo-0.8.4/planemo/github_util.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo/xml/
--rw-rw-r--   0 john      (1000) john      (1000)     2272 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/xml/validation.py
--rw-rw-r--   0 john      (1000) john      (1000)      123 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/xml/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo/xml/xsd/
--rw-rw-r--   0 john      (1000) john      (1000)     6950 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/xml/xsd/tool_dependencies.xsd
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo/xml/xsd/tool/
--rw-rw-r--   0 john      (1000) john      (1000)     1081 2015-04-20 22:28:45.000000 planemo-0.8.4/planemo/xml/xsd/tool/README.md
--rw-rw-r--   0 john      (1000) john      (1000)       13 2015-04-20 22:28:45.000000 planemo-0.8.4/planemo/xml/xsd/tool/.gitignore
--rw-rw-r--   0 john      (1000) john      (1000)      663 2015-04-20 22:28:45.000000 planemo-0.8.4/planemo/xml/xsd/tool/citations.xsd
--rw-rw-r--   0 john      (1000) john      (1000)       54 2015-04-20 22:28:45.000000 planemo-0.8.4/planemo/xml/xsd/tool/.git
--rw-rw-r--   0 john      (1000) john      (1000)     1145 2015-04-20 22:28:45.000000 planemo-0.8.4/planemo/xml/xsd/tool/citation.xsd
--rw-rw-r--   0 john      (1000) john      (1000)     1131 2015-04-20 22:28:45.000000 planemo-0.8.4/planemo/xml/xsd/tool/LICENSE
--rw-rw-r--   0 john      (1000) john      (1000)      450 2015-04-20 22:28:45.000000 planemo-0.8.4/planemo/xml/xsd/tool/Makefile
--rw-rw-r--   0 john      (1000) john      (1000)      514 2015-04-20 22:28:45.000000 planemo-0.8.4/planemo/xml/xsd/tool/test.sh
--rw-rw-r--   0 john      (1000) john      (1000)      694 2015-04-20 22:28:45.000000 planemo-0.8.4/planemo/xml/xsd/tool/galaxy.jxb
--rw-rw-r--   0 john      (1000) john      (1000)    53885 2015-04-20 22:28:45.000000 planemo-0.8.4/planemo/xml/xsd/tool/galaxy.xsd
--rw-rw-r--   0 john      (1000) john      (1000)     4915 2015-04-20 22:28:45.000000 planemo-0.8.4/planemo/xml/xsd/tool/test.urls
--rw-rw-r--   0 john      (1000) john      (1000)       82 2015-04-20 22:28:45.000000 planemo-0.8.4/planemo/xml/xsd/tool/.travis.yml
--rw-rw-r--   0 john      (1000) john      (1000)     3020 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/xml/xsd/repository_dependencies.xsd
--rw-rw-r--   0 john      (1000) john      (1000)      485 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/lint.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo/reports/
--rw-rw-r--   0 john      (1000) john      (1000)     1392 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/reports/build_report.py
--rw-rw-r--   0 john      (1000) john      (1000)        0 2015-02-16 00:41:44.000000 planemo-0.8.4/planemo/reports/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     7028 2015-04-29 16:15:49.000000 planemo-0.8.4/planemo/shed_lint.py
--rw-rw-r--   0 john      (1000) john      (1000)      529 2015-04-29 12:43:47.000000 planemo-0.8.4/planemo/config.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo/commands/
--rw-rw-r--   0 john      (1000) john      (1000)     1425 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/commands/cmd_shed_init.py
--rw-rw-r--   0 john      (1000) john      (1000)      823 2015-04-29 18:41:33.000000 planemo-0.8.4/planemo/commands/cmd_shed_lint.py
--rw-rw-r--   0 john      (1000) john      (1000)     6312 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/commands/cmd_tool_init.py
--rw-rw-r--   0 john      (1000) john      (1000)     1122 2015-03-16 17:44:16.000000 planemo-0.8.4/planemo/commands/cmd_project_init.py
--rw-rw-r--   0 john      (1000) john      (1000)      750 2014-12-09 03:06:38.000000 planemo-0.8.4/planemo/commands/cmd_brew_init.py
--rw-rw-r--   0 john      (1000) john      (1000)      898 2015-02-16 00:41:44.000000 planemo-0.8.4/planemo/commands/cmd_create_gist.py
--rw-rw-r--   0 john      (1000) john      (1000)     1415 2015-02-16 00:41:44.000000 planemo-0.8.4/planemo/commands/cmd_brew.py
--rw-rw-r--   0 john      (1000) john      (1000)     1554 2015-04-30 12:42:33.000000 planemo-0.8.4/planemo/commands/cmd_config_init.py
--rw-rw-r--   0 john      (1000) john      (1000)     1855 2014-12-09 03:06:38.000000 planemo-0.8.4/planemo/commands/cmd_travis_before_install.py
--rw-rw-r--   0 john      (1000) john      (1000)     1371 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/commands/cmd_serve.py
--rw-rw-r--   0 john      (1000) john      (1000)     1066 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/commands/cmd_tool_factory.py
--rw-rw-r--   0 john      (1000) john      (1000)     1242 2015-02-16 00:41:44.000000 planemo-0.8.4/planemo/commands/cmd_share_test.py
--rw-rw-r--   0 john      (1000) john      (1000)     2586 2015-02-16 00:41:44.000000 planemo-0.8.4/planemo/commands/cmd_travis_init.py
--rw-rw-r--   0 john      (1000) john      (1000)     1026 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/commands/cmd_shed_create.py
--rw-rw-r--   0 john      (1000) john      (1000)     2179 2014-12-09 03:06:38.000000 planemo-0.8.4/planemo/commands/cmd_docker_shell.py
--rw-rw-r--   0 john      (1000) john      (1000)      294 2014-12-09 03:06:38.000000 planemo-0.8.4/planemo/commands/cmd_syntax.py
--rw-rw-r--   0 john      (1000) john      (1000)        0 2014-12-09 03:06:38.000000 planemo-0.8.4/planemo/commands/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2558 2014-12-09 03:06:38.000000 planemo-0.8.4/planemo/commands/cmd_brew_env.py
--rw-rw-r--   0 john      (1000) john      (1000)     3128 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/commands/cmd_shed_diff.py
--rw-rw-r--   0 john      (1000) john      (1000)     3042 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/commands/cmd_normalize.py
--rw-rw-r--   0 john      (1000) john      (1000)     3025 2015-04-30 14:41:20.000000 planemo-0.8.4/planemo/commands/cmd_shed_upload.py
--rw-rw-r--   0 john      (1000) john      (1000)      703 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/commands/cmd_lint.py
--rw-rw-r--   0 john      (1000) john      (1000)      933 2015-04-22 02:38:08.000000 planemo-0.8.4/planemo/commands/cmd_shed_download.py
--rw-rw-r--   0 john      (1000) john      (1000)    11670 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/commands/cmd_test.py
--rw-rw-r--   0 john      (1000) john      (1000)     1365 2014-12-09 03:06:38.000000 planemo-0.8.4/planemo/commands/cmd_docker_build.py
--rw-rw-r--   0 john      (1000) john      (1000)     7717 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/options.py
--rw-rw-r--   0 john      (1000) john      (1000)     2219 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/tool_lint.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-04-30 18:02:14.000000 planemo-0.8.4/planemo/linters/
--rw-rw-r--   0 john      (1000) john      (1000)      802 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/linters/xsd.py
--rw-rw-r--   0 john      (1000) john      (1000)        0 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/linters/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      789 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/galaxy_serve.py
--rw-rw-r--   0 john      (1000) john      (1000)    27628 2015-04-30 17:47:58.000000 planemo-0.8.4/planemo/shed.py
--rw-rw-r--   0 john      (1000) john      (1000)      205 2015-04-30 18:00:49.000000 planemo-0.8.4/planemo/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1382 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/io.py
--rw-rw-r--   0 john      (1000) john      (1000)    14906 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/galaxy_config.py
--rw-rw-r--   0 john      (1000) john      (1000)      750 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/galaxy_run.py
--rw-rw-r--   0 john      (1000) john      (1000)     4599 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/galaxy_test.py
--rw-rw-r--   0 john      (1000) john      (1000)     3542 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/cli.py
--rw-rw-r--   0 john      (1000) john      (1000)      447 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/tools.py
--rw-rw-r--   0 john      (1000) john      (1000)      478 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/templates.py
--rw-rw-r--   0 john      (1000) john      (1000)    10071 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/tool_builder.py
--rw-rw-r--   0 john      (1000) john      (1000)      375 2015-04-29 12:43:36.000000 planemo-0.8.4/planemo/glob.py
--rw-rw-r--   0 john      (1000) john      (1000)     3471 2015-04-29 12:43:36.000000 planemo-0.8.4/CONTRIBUTING.rst
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/
+-rw-rw-r--   0 john      (1000) john      (1000)      291 2015-05-04 00:15:19.000000 planemo-0.9.0/setup.cfg
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)       57 2015-05-04 00:15:18.000000 planemo-0.9.0/planemo.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2015-05-04 00:15:18.000000 planemo-0.9.0/planemo.egg-info/not-zip-safe
+-rw-rw-r--   0 john      (1000) john      (1000)     4270 2015-05-04 00:15:18.000000 planemo-0.9.0/planemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       67 2015-05-04 00:15:18.000000 planemo-0.9.0/planemo.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)    36293 2015-05-04 00:15:18.000000 planemo-0.9.0/planemo.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2015-05-04 00:15:18.000000 planemo-0.9.0/planemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       20 2015-05-04 00:15:18.000000 planemo-0.9.0/planemo.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1000) john      (1000)     1664 2015-04-29 12:43:36.000000 planemo-0.9.0/CODE_OF_CONDUCT.rst
+-rw-rw-r--   0 john      (1000) john      (1000)      117 2015-04-29 12:43:36.000000 planemo-0.9.0/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)     9004 2015-05-01 13:22:38.000000 planemo-0.9.0/README.rst
+-rw-rw-r--   0 john      (1000) john      (1000)    36293 2015-05-04 00:15:19.000000 planemo-0.9.0/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)    11097 2014-12-09 03:06:38.000000 planemo-0.9.0/LICENSE
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo_ext/
+-rw-rw-r--   0 john      (1000) john      (1000)        2 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo_ext/galaxy/
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo_ext/galaxy/util/
+-rw-rw-r--   0 john      (1000) john      (1000)     2537 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/util/plugin_config.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1039 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/util/submodules.py
+-rw-rw-r--   0 john      (1000) john      (1000)      599 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/util/directory_hash.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7488 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/util/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)      830 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/util/bunch.py
+-rw-rw-r--   0 john      (1000) john      (1000)      626 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/util/sleeper.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2222 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/util/odict.py
+-rw-rw-r--   0 john      (1000) john      (1000)       49 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo_ext/galaxy/eggs/
+-rw-rw-r--   0 john      (1000) john      (1000)      373 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/eggs/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)      220 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/exceptions.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo_ext/galaxy/tools/
+-rw-rw-r--   0 john      (1000) john      (1000)     3351 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/lint.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2312 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/loader_directory.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo_ext/galaxy/tools/linters/
+-rw-rw-r--   0 john      (1000) john      (1000)     1254 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/linters/xsd_util.py
+-rw-rw-r--   0 john      (1000) john      (1000)      958 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/linters/command.py
+-rw-rw-r--   0 john      (1000) john      (1000)      879 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/linters/outputs.py
+-rw-rw-r--   0 john      (1000) john      (1000)      543 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/linters/top_level.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1006 2015-04-29 12:45:41.000000 planemo-0.9.0/planemo_ext/galaxy/tools/linters/xml_order.py
+-rw-rw-r--   0 john      (1000) john      (1000)      315 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/linters/xsd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1371 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/linters/inputs.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1023 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/linters/help.py
+-rw-rw-r--   0 john      (1000) john      (1000)       37 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/linters/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)      988 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/linters/tests.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1833 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/linters/stdio.py
+-rw-rw-r--   0 john      (1000) john      (1000)      990 2015-04-29 16:02:29.000000 planemo-0.9.0/planemo_ext/galaxy/tools/linters/citations.py
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/
+-rw-rw-r--   0 john      (1000) john      (1000)     5315 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/docker_util.py
+-rw-rw-r--   0 john      (1000) john      (1000)    13204 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/containers.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2966 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/dependencies.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2493 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/dockerfiles.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4564 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/__init__.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    19588 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/brew_exts.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3413 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/requirements.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/resolvers/
+-rw-rw-r--   0 john      (1000) john      (1000)     3022 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/resolvers/tool_shed_packages.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3194 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/resolvers/galaxy_packages.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2769 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/resolvers/resolver_mixins.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5246 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/resolvers/brewed_tool_shed_packages.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6098 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/resolvers/modules.py
+-rw-rw-r--   0 john      (1000) john      (1000)      999 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/resolvers/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1947 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/resolvers/homebrew.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1179 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/brew_util.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1607 2015-05-03 23:10:17.000000 planemo-0.9.0/planemo_ext/galaxy/tools/deps/commands.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6894 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo_ext/galaxy/tools/loader.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo_ext/tool_factory_2/
+-rw-rw-r--   0 john      (1000) john      (1000)    44013 2015-04-30 17:46:37.000000 planemo-0.9.0/planemo_ext/tool_factory_2/rgToolFactory2.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2233 2015-04-30 17:46:37.000000 planemo-0.9.0/planemo_ext/tool_factory_2/getlocalrpackages.py
+-rw-rw-r--   0 john      (1000) john      (1000)    21748 2015-04-30 17:47:59.000000 planemo-0.9.0/planemo_ext/tool_factory_2/rgToolFactory2.xml
+-rw-rw-r--   0 john      (1000) john      (1000)    26443 2015-04-30 17:46:37.000000 planemo-0.9.0/planemo_ext/tool_factory_2/LICENSE
+-rw-rw-r--   0 john      (1000) john      (1000)    21352 2015-05-04 00:15:01.000000 planemo-0.9.0/HISTORY.rst
+-rw-rw-r--   0 john      (1000) john      (1000)     3396 2015-05-01 16:43:50.000000 planemo-0.9.0/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo/
+-rw-rw-r--   0 john      (1000) john      (1000)      977 2015-02-16 00:41:44.000000 planemo-0.9.0/planemo/github_util.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo/xml/
+-rw-rw-r--   0 john      (1000) john      (1000)     2272 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/xml/validation.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1733 2015-05-01 14:16:18.000000 planemo-0.9.0/planemo/xml/diff.py
+-rw-rw-r--   0 john      (1000) john      (1000)      123 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/xml/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo/xml/xsd/
+-rw-rw-r--   0 john      (1000) john      (1000)     6950 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/xml/xsd/tool_dependencies.xsd
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo/xml/xsd/tool/
+-rw-rw-r--   0 john      (1000) john      (1000)     1081 2015-04-20 22:28:45.000000 planemo-0.9.0/planemo/xml/xsd/tool/README.md
+-rw-rw-r--   0 john      (1000) john      (1000)       13 2015-04-20 22:28:45.000000 planemo-0.9.0/planemo/xml/xsd/tool/.gitignore
+-rw-rw-r--   0 john      (1000) john      (1000)      663 2015-04-20 22:28:45.000000 planemo-0.9.0/planemo/xml/xsd/tool/citations.xsd
+-rw-rw-r--   0 john      (1000) john      (1000)       54 2015-04-20 22:28:45.000000 planemo-0.9.0/planemo/xml/xsd/tool/.git
+-rw-rw-r--   0 john      (1000) john      (1000)     1145 2015-04-20 22:28:45.000000 planemo-0.9.0/planemo/xml/xsd/tool/citation.xsd
+-rw-rw-r--   0 john      (1000) john      (1000)     1131 2015-04-20 22:28:45.000000 planemo-0.9.0/planemo/xml/xsd/tool/LICENSE
+-rw-rw-r--   0 john      (1000) john      (1000)      450 2015-04-20 22:28:45.000000 planemo-0.9.0/planemo/xml/xsd/tool/Makefile
+-rw-rw-r--   0 john      (1000) john      (1000)      514 2015-04-20 22:28:45.000000 planemo-0.9.0/planemo/xml/xsd/tool/test.sh
+-rw-rw-r--   0 john      (1000) john      (1000)      694 2015-04-20 22:28:45.000000 planemo-0.9.0/planemo/xml/xsd/tool/galaxy.jxb
+-rw-rw-r--   0 john      (1000) john      (1000)    53885 2015-04-20 22:28:45.000000 planemo-0.9.0/planemo/xml/xsd/tool/galaxy.xsd
+-rw-rw-r--   0 john      (1000) john      (1000)     4915 2015-04-20 22:28:45.000000 planemo-0.9.0/planemo/xml/xsd/tool/test.urls
+-rw-rw-r--   0 john      (1000) john      (1000)       82 2015-04-20 22:28:45.000000 planemo-0.9.0/planemo/xml/xsd/tool/.travis.yml
+-rw-rw-r--   0 john      (1000) john      (1000)     3020 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/xml/xsd/repository_dependencies.xsd
+-rw-rw-r--   0 john      (1000) john      (1000)      485 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/lint.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo/reports/
+-rw-rw-r--   0 john      (1000) john      (1000)     1392 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/reports/build_report.py
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2015-02-16 00:41:44.000000 planemo-0.9.0/planemo/reports/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6647 2015-05-01 17:18:21.000000 planemo-0.9.0/planemo/shed_lint.py
+-rw-rw-r--   0 john      (1000) john      (1000)      579 2015-04-30 23:37:41.000000 planemo-0.9.0/planemo/config.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo/commands/
+-rw-rw-r--   0 john      (1000) john      (1000)     1425 2015-05-01 01:29:04.000000 planemo-0.9.0/planemo/commands/cmd_shed_init.py
+-rw-rw-r--   0 john      (1000) john      (1000)      847 2015-05-01 20:28:06.000000 planemo-0.9.0/planemo/commands/cmd_shed_lint.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6312 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/commands/cmd_tool_init.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1122 2015-05-01 18:54:23.000000 planemo-0.9.0/planemo/commands/cmd_project_init.py
+-rw-rw-r--   0 john      (1000) john      (1000)      750 2014-12-09 03:06:38.000000 planemo-0.9.0/planemo/commands/cmd_brew_init.py
+-rw-rw-r--   0 john      (1000) john      (1000)      898 2015-02-16 00:41:44.000000 planemo-0.9.0/planemo/commands/cmd_create_gist.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1415 2015-02-16 00:41:44.000000 planemo-0.9.0/planemo/commands/cmd_brew.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1567 2015-04-30 23:44:26.000000 planemo-0.9.0/planemo/commands/cmd_config_init.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1855 2014-12-09 03:06:38.000000 planemo-0.9.0/planemo/commands/cmd_travis_before_install.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1401 2015-05-01 00:12:38.000000 planemo-0.9.0/planemo/commands/cmd_serve.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1096 2015-05-01 00:12:35.000000 planemo-0.9.0/planemo/commands/cmd_tool_factory.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1242 2015-02-16 00:41:44.000000 planemo-0.9.0/planemo/commands/cmd_share_test.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2586 2015-02-16 00:41:44.000000 planemo-0.9.0/planemo/commands/cmd_travis_init.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1044 2015-05-01 20:28:22.000000 planemo-0.9.0/planemo/commands/cmd_shed_create.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2179 2014-12-09 03:06:38.000000 planemo-0.9.0/planemo/commands/cmd_docker_shell.py
+-rw-rw-r--   0 john      (1000) john      (1000)      294 2014-12-09 03:06:38.000000 planemo-0.9.0/planemo/commands/cmd_syntax.py
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2014-12-09 03:06:38.000000 planemo-0.9.0/planemo/commands/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2558 2014-12-09 03:06:38.000000 planemo-0.9.0/planemo/commands/cmd_brew_env.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2014 2015-05-04 00:10:17.000000 planemo-0.9.0/planemo/commands/cmd_shed_diff.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3042 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/commands/cmd_normalize.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1722 2015-05-03 23:10:17.000000 planemo-0.9.0/planemo/commands/cmd_shed_upload.py
+-rw-rw-r--   0 john      (1000) john      (1000)      703 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/commands/cmd_lint.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1406 2015-05-01 20:28:15.000000 planemo-0.9.0/planemo/commands/cmd_shed_download.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11670 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/commands/cmd_test.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1365 2014-12-09 03:06:38.000000 planemo-0.9.0/planemo/commands/cmd_docker_build.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8848 2015-05-01 19:35:51.000000 planemo-0.9.0/planemo/options.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2219 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/tool_lint.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo/linters/
+-rw-rw-r--   0 john      (1000) john      (1000)      802 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/linters/xsd.py
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/linters/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1171 2015-05-03 23:10:17.000000 planemo-0.9.0/planemo/git.py
+-rw-rw-r--   0 john      (1000) john      (1000)      789 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/galaxy_serve.py
+-rw-rw-r--   0 john      (1000) john      (1000)      205 2015-05-04 00:15:01.000000 planemo-0.9.0/planemo/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2040 2015-05-03 23:10:17.000000 planemo-0.9.0/planemo/io.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14970 2015-05-01 19:49:15.000000 planemo-0.9.0/planemo/galaxy_config.py
+-rw-rw-r--   0 john      (1000) john      (1000)      750 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/galaxy_run.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2015-05-04 00:15:19.000000 planemo-0.9.0/planemo/shed/
+-rw-rw-r--   0 john      (1000) john      (1000)     1569 2015-05-01 14:16:18.000000 planemo-0.9.0/planemo/shed/diff.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3074 2015-05-01 01:03:02.000000 planemo-0.9.0/planemo/shed/interface.py
+-rw-rw-r--   0 john      (1000) john      (1000)    34356 2015-05-04 00:10:17.000000 planemo-0.9.0/planemo/shed/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4599 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/galaxy_test.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3542 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/cli.py
+-rw-rw-r--   0 john      (1000) john      (1000)      447 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/tools.py
+-rw-rw-r--   0 john      (1000) john      (1000)      478 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/templates.py
+-rw-rw-r--   0 john      (1000) john      (1000)    10071 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/tool_builder.py
+-rw-rw-r--   0 john      (1000) john      (1000)      375 2015-04-29 12:43:36.000000 planemo-0.9.0/planemo/glob.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3471 2015-04-29 12:43:36.000000 planemo-0.9.0/CONTRIBUTING.rst
```

### Comparing `planemo-0.8.4/planemo.egg-info/SOURCES.txt` & `planemo-0.9.0/planemo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 planemo/__init__.py
 planemo/cli.py
 planemo/config.py
 planemo/galaxy_config.py
 planemo/galaxy_run.py
 planemo/galaxy_serve.py
 planemo/galaxy_test.py
+planemo/git.py
 planemo/github_util.py
 planemo/glob.py
 planemo/io.py
 planemo/lint.py
 planemo/options.py
-planemo/shed.py
 planemo/shed_lint.py
 planemo/templates.py
 planemo/tool_builder.py
 planemo/tool_lint.py
 planemo/tools.py
 planemo.egg-info/PKG-INFO
 planemo.egg-info/SOURCES.txt
@@ -56,15 +56,19 @@
 planemo/commands/cmd_tool_init.py
 planemo/commands/cmd_travis_before_install.py
 planemo/commands/cmd_travis_init.py
 planemo/linters/__init__.py
 planemo/linters/xsd.py
 planemo/reports/__init__.py
 planemo/reports/build_report.py
+planemo/shed/__init__.py
+planemo/shed/diff.py
+planemo/shed/interface.py
 planemo/xml/__init__.py
+planemo/xml/diff.py
 planemo/xml/validation.py
 planemo/xml/xsd/repository_dependencies.xsd
 planemo/xml/xsd/tool_dependencies.xsd
 planemo/xml/xsd/tool/.git
 planemo/xml/xsd/tool/.gitignore
 planemo/xml/xsd/tool/.travis.yml
 planemo/xml/xsd/tool/LICENSE
```

### Comparing `planemo-0.8.4/planemo.egg-info/PKG-INFO` & `planemo-0.9.0/planemo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 1.1
 Name: planemo
-Version: 0.8.4
+Version: 0.9.0
 Summary: Command-line utilities to assist in building tools for the Galaxy project (http://galaxyproject.org/).
 Home-page: https://github.com/galaxyproject/planemo
 Author: Galaxy Project and Community
 Author-email: jmchilton@gmail.com
 License: AFL
-Description: ===============================
-        Planemo
-        ===============================
+Description: .. figure:: https://raw.githubusercontent.com/jmchilton/planemo/master/docs/planemo_logo.png
+           :alt: Planemo Logo
+           :align: center
+           :figwidth: 100%
         
         .. image:: https://readthedocs.org/projects/pip/badge/?version=latest
            :target: https://planemo.readthedocs.org
         
         .. image:: https://badge.fury.io/py/planemo.svg
            :target: https://pypi.python.org/pypi/planemo/
         
         .. image:: https://travis-ci.org/galaxyproject/planemo.png?branch=master
            :target: https://travis-ci.org/galaxyproject/planemo
         
         .. image:: https://coveralls.io/repos/galaxyproject/planemo/badge.svg?branch=master
            :target: https://coveralls.io/r/galaxyproject/planemo?branch=master
         
         
-        Command-line utilities to assist in building tools for the Galaxy_ project.
+        Command-line utilities to assist in building and publishing Galaxy_ tools.
         
         * Free software: Academic Free License version 3.0
         * Documentation: https://planemo.readthedocs.org.
         * Code: https://github.com/galaxyproject/planemo
         
         Quick Start
         -----------
@@ -220,34 +221,65 @@
             /home/john/.linuxbrew/Cellar/bowtie2/2.1.0/bin/bowtie2
         
         For more information see the documentation for the `brew
         <http://planemo.readthedocs.org/en/latest/commands.html#brew-command>`__
         and `brew_env
         <http://planemo.readthedocs.org/en/latest/commands.html#brew_env-command>`__ commands.
         
-        .. _Galaxy: (http://galaxyproject.org/)
+        .. _Galaxy: http://galaxyproject.org/
         .. _GitHub: https://github.com/
         .. _Docker: https://www.docker.com/
         .. _Homebrew: http://brew.sh/
         .. _linuxbrew: https://github.com/Homebrew/linuxbrew
         .. _Vagrant: https://www.vagrantup.com/
-        .. _Travis CI: <http://travis-ci.org/>
+        .. _Travis CI: http://travis-ci.org/
         .. _`tools-devteam`: https://github.com/galaxyproject/tools-devteam
         .. _`tools-iuc`: https://github.com/galaxyproject/tools-iuc
         .. _Publishing to the Tool Shed: http://planemo.readthedocs.org/en/latest/publishing.html
         
         
         
         
         History
         -------
         
         .. to_doc
         
         ---------------------
+        0.9.0 (2015-05-03)
+        ---------------------
+        
+        * Add new logo to the README thanks to @petrkadlec from `puradesign.cz
+          <http://puradesign.cz/en>`__ and @carlfeberhard from the Galaxy Project.
+          `Issue 108`_
+        * Implement smarter ``shed_diff`` command - it now produces a meaningful
+          exit codes and doesn't report differences if these correspond to attributes
+          that will be automatically populated by the Tool Shed. `Issue 167`_
+        * Use new smarter ``shed_diff`` code to implement a new ``--check_diff``
+          option for ``shed_upload`` - to check for meaningful differences before
+          updating repositories. `Issue 168`_
+        * Record git commit hash during ``shed_upload`` if the ``.shed.yml`` is
+          located in a git repository. `Issue 170`_
+        * Allow ``shed_`` operations to operate on git URLs directly. `Issue 169`_
+        * Fail if missing file inclusion statements encountered during ``.shed.yml``
+          repository resolution - bug reported by @peterjc. `Issue 158`_
+        * Improved exception handling for tool shed operations including new 
+          ``--fail_fast`` command-line option. * `Issue 114`_, `Pull Request 173`_
+        * Implement more validation when using the ``shed_init`` command. 1cd0e2d_
+        * Add ``-r/--recursive`` option to ``shed_download`` and ``shed_diff`` 
+          commands and allow these commands to work with ``.shed.yml`` files defining
+          multipe repositories. 40a1f57_
+        * Add ``--port`` option to the ``serve`` and ``tool_factory`` commands.
+          15804be_
+        * Fix problem introduced with ``setup.py`` during the 0.9.0 development cycle
+          - thanks to @peterjc. `Pull Request 171`_
+        * Fix clone bug introduced during 0.9.0 development cycle - thanks to
+          @bgruening. `Pull Request 175`_
+        
+        ---------------------
         0.8.4 (2015-04-30)
         ---------------------
         
         * Fix for Travis CI testing picking up invalid tests (reported by @takadonet). `Issue 161`_
         * Fix tar ordering for consistency (always sort by name) - thanks to @peterjc.  `Pull Request 164`_, `Issue 159`_
         * Fix exception handling related to tool shed operations - thanks to @peterjc. `Pull Request 155`_, b86fe1f_
         
@@ -480,14 +512,27 @@
         0.0.1 (2014-10-04)
         ---------------------
         
         * Initial work on the project - commands for testing, linting, serving Galaxy
           tools - and more experimental features involving Docker and Homebrew. 7d07782_
         
         .. github_links
+        .. _Issue 114: https://github.com/galaxyproject/planemo/issues/114
+        .. _Pull Request 173: https://github.com/galaxyproject/planemo/pull/173
+        .. _Issue 108: https://github.com/galaxyproject/planemo/issues/108
+        .. _15804be: https://github.com/galaxyproject/planemo/commit/15804be
+        .. _Issue 158: https://github.com/galaxyproject/planemo/issues/158
+        .. _Pull Request 171: https://github.com/galaxyproject/planemo/pull/171
+        .. _1cd0e2d: https://github.com/galaxyproject/planemo/commit/1cd0e2d
+        .. _40a1f57: https://github.com/galaxyproject/planemo/commit/40a1f57
+        .. _Pull Request 175: https://github.com/galaxyproject/planemo/pull/175
+        .. _Issue 167: https://github.com/galaxyproject/planemo/issues/167
+        .. _Issue 170: https://github.com/galaxyproject/planemo/issues/170
+        .. _Issue 169: https://github.com/galaxyproject/planemo/issues/169
+        .. _Issue 168: https://github.com/galaxyproject/planemo/issues/168
         .. _b86fe1f: https://github.com/galaxyproject/planemo/commit/b86fe1f
         .. _Pull Request 155: https://github.com/galaxyproject/planemo/pull/155
         .. _Pull Request 164: https://github.com/galaxyproject/planemo/pull/164
         .. _Issue 159: https://github.com/galaxyproject/planemo/issues/159
         .. _Issue 161: https://github.com/galaxyproject/planemo/issues/161
         .. _a2ee135: https://github.com/galaxyproject/planemo/commit/a2ee135
         .. _9ff0d2d: https://github.com/galaxyproject/planemo/commit/9ff0d2d
```

### Comparing `planemo-0.8.4/CODE_OF_CONDUCT.rst` & `planemo-0.9.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/README.rst` & `planemo-0.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-===============================
-Planemo
-===============================
+.. figure:: https://raw.githubusercontent.com/jmchilton/planemo/master/docs/planemo_logo.png
+   :alt: Planemo Logo
+   :align: center
+   :figwidth: 100%
 
 .. image:: https://readthedocs.org/projects/pip/badge/?version=latest
    :target: https://planemo.readthedocs.org
 
 .. image:: https://badge.fury.io/py/planemo.svg
    :target: https://pypi.python.org/pypi/planemo/
 
 .. image:: https://travis-ci.org/galaxyproject/planemo.png?branch=master
    :target: https://travis-ci.org/galaxyproject/planemo
 
 .. image:: https://coveralls.io/repos/galaxyproject/planemo/badge.svg?branch=master
    :target: https://coveralls.io/r/galaxyproject/planemo?branch=master
 
 
-Command-line utilities to assist in building tools for the Galaxy_ project.
+Command-line utilities to assist in building and publishing Galaxy_ tools.
 
 * Free software: Academic Free License version 3.0
 * Documentation: https://planemo.readthedocs.org.
 * Code: https://github.com/galaxyproject/planemo
 
 Quick Start
 -----------
@@ -212,17 +213,17 @@
     /home/john/.linuxbrew/Cellar/bowtie2/2.1.0/bin/bowtie2
 
 For more information see the documentation for the `brew
 <http://planemo.readthedocs.org/en/latest/commands.html#brew-command>`__
 and `brew_env
 <http://planemo.readthedocs.org/en/latest/commands.html#brew_env-command>`__ commands.
 
-.. _Galaxy: (http://galaxyproject.org/)
+.. _Galaxy: http://galaxyproject.org/
 .. _GitHub: https://github.com/
 .. _Docker: https://www.docker.com/
 .. _Homebrew: http://brew.sh/
 .. _linuxbrew: https://github.com/Homebrew/linuxbrew
 .. _Vagrant: https://www.vagrantup.com/
-.. _Travis CI: <http://travis-ci.org/>
+.. _Travis CI: http://travis-ci.org/
 .. _`tools-devteam`: https://github.com/galaxyproject/tools-devteam
 .. _`tools-iuc`: https://github.com/galaxyproject/tools-iuc
 .. _Publishing to the Tool Shed: http://planemo.readthedocs.org/en/latest/publishing.html
```

### Comparing `planemo-0.8.4/PKG-INFO` & `planemo-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 1.1
 Name: planemo
-Version: 0.8.4
+Version: 0.9.0
 Summary: Command-line utilities to assist in building tools for the Galaxy project (http://galaxyproject.org/).
 Home-page: https://github.com/galaxyproject/planemo
 Author: Galaxy Project and Community
 Author-email: jmchilton@gmail.com
 License: AFL
-Description: ===============================
-        Planemo
-        ===============================
+Description: .. figure:: https://raw.githubusercontent.com/jmchilton/planemo/master/docs/planemo_logo.png
+           :alt: Planemo Logo
+           :align: center
+           :figwidth: 100%
         
         .. image:: https://readthedocs.org/projects/pip/badge/?version=latest
            :target: https://planemo.readthedocs.org
         
         .. image:: https://badge.fury.io/py/planemo.svg
            :target: https://pypi.python.org/pypi/planemo/
         
         .. image:: https://travis-ci.org/galaxyproject/planemo.png?branch=master
            :target: https://travis-ci.org/galaxyproject/planemo
         
         .. image:: https://coveralls.io/repos/galaxyproject/planemo/badge.svg?branch=master
            :target: https://coveralls.io/r/galaxyproject/planemo?branch=master
         
         
-        Command-line utilities to assist in building tools for the Galaxy_ project.
+        Command-line utilities to assist in building and publishing Galaxy_ tools.
         
         * Free software: Academic Free License version 3.0
         * Documentation: https://planemo.readthedocs.org.
         * Code: https://github.com/galaxyproject/planemo
         
         Quick Start
         -----------
@@ -220,34 +221,65 @@
             /home/john/.linuxbrew/Cellar/bowtie2/2.1.0/bin/bowtie2
         
         For more information see the documentation for the `brew
         <http://planemo.readthedocs.org/en/latest/commands.html#brew-command>`__
         and `brew_env
         <http://planemo.readthedocs.org/en/latest/commands.html#brew_env-command>`__ commands.
         
-        .. _Galaxy: (http://galaxyproject.org/)
+        .. _Galaxy: http://galaxyproject.org/
         .. _GitHub: https://github.com/
         .. _Docker: https://www.docker.com/
         .. _Homebrew: http://brew.sh/
         .. _linuxbrew: https://github.com/Homebrew/linuxbrew
         .. _Vagrant: https://www.vagrantup.com/
-        .. _Travis CI: <http://travis-ci.org/>
+        .. _Travis CI: http://travis-ci.org/
         .. _`tools-devteam`: https://github.com/galaxyproject/tools-devteam
         .. _`tools-iuc`: https://github.com/galaxyproject/tools-iuc
         .. _Publishing to the Tool Shed: http://planemo.readthedocs.org/en/latest/publishing.html
         
         
         
         
         History
         -------
         
         .. to_doc
         
         ---------------------
+        0.9.0 (2015-05-03)
+        ---------------------
+        
+        * Add new logo to the README thanks to @petrkadlec from `puradesign.cz
+          <http://puradesign.cz/en>`__ and @carlfeberhard from the Galaxy Project.
+          `Issue 108`_
+        * Implement smarter ``shed_diff`` command - it now produces a meaningful
+          exit codes and doesn't report differences if these correspond to attributes
+          that will be automatically populated by the Tool Shed. `Issue 167`_
+        * Use new smarter ``shed_diff`` code to implement a new ``--check_diff``
+          option for ``shed_upload`` - to check for meaningful differences before
+          updating repositories. `Issue 168`_
+        * Record git commit hash during ``shed_upload`` if the ``.shed.yml`` is
+          located in a git repository. `Issue 170`_
+        * Allow ``shed_`` operations to operate on git URLs directly. `Issue 169`_
+        * Fail if missing file inclusion statements encountered during ``.shed.yml``
+          repository resolution - bug reported by @peterjc. `Issue 158`_
+        * Improved exception handling for tool shed operations including new 
+          ``--fail_fast`` command-line option. * `Issue 114`_, `Pull Request 173`_
+        * Implement more validation when using the ``shed_init`` command. 1cd0e2d_
+        * Add ``-r/--recursive`` option to ``shed_download`` and ``shed_diff`` 
+          commands and allow these commands to work with ``.shed.yml`` files defining
+          multipe repositories. 40a1f57_
+        * Add ``--port`` option to the ``serve`` and ``tool_factory`` commands.
+          15804be_
+        * Fix problem introduced with ``setup.py`` during the 0.9.0 development cycle
+          - thanks to @peterjc. `Pull Request 171`_
+        * Fix clone bug introduced during 0.9.0 development cycle - thanks to
+          @bgruening. `Pull Request 175`_
+        
+        ---------------------
         0.8.4 (2015-04-30)
         ---------------------
         
         * Fix for Travis CI testing picking up invalid tests (reported by @takadonet). `Issue 161`_
         * Fix tar ordering for consistency (always sort by name) - thanks to @peterjc.  `Pull Request 164`_, `Issue 159`_
         * Fix exception handling related to tool shed operations - thanks to @peterjc. `Pull Request 155`_, b86fe1f_
         
@@ -480,14 +512,27 @@
         0.0.1 (2014-10-04)
         ---------------------
         
         * Initial work on the project - commands for testing, linting, serving Galaxy
           tools - and more experimental features involving Docker and Homebrew. 7d07782_
         
         .. github_links
+        .. _Issue 114: https://github.com/galaxyproject/planemo/issues/114
+        .. _Pull Request 173: https://github.com/galaxyproject/planemo/pull/173
+        .. _Issue 108: https://github.com/galaxyproject/planemo/issues/108
+        .. _15804be: https://github.com/galaxyproject/planemo/commit/15804be
+        .. _Issue 158: https://github.com/galaxyproject/planemo/issues/158
+        .. _Pull Request 171: https://github.com/galaxyproject/planemo/pull/171
+        .. _1cd0e2d: https://github.com/galaxyproject/planemo/commit/1cd0e2d
+        .. _40a1f57: https://github.com/galaxyproject/planemo/commit/40a1f57
+        .. _Pull Request 175: https://github.com/galaxyproject/planemo/pull/175
+        .. _Issue 167: https://github.com/galaxyproject/planemo/issues/167
+        .. _Issue 170: https://github.com/galaxyproject/planemo/issues/170
+        .. _Issue 169: https://github.com/galaxyproject/planemo/issues/169
+        .. _Issue 168: https://github.com/galaxyproject/planemo/issues/168
         .. _b86fe1f: https://github.com/galaxyproject/planemo/commit/b86fe1f
         .. _Pull Request 155: https://github.com/galaxyproject/planemo/pull/155
         .. _Pull Request 164: https://github.com/galaxyproject/planemo/pull/164
         .. _Issue 159: https://github.com/galaxyproject/planemo/issues/159
         .. _Issue 161: https://github.com/galaxyproject/planemo/issues/161
         .. _a2ee135: https://github.com/galaxyproject/planemo/commit/a2ee135
         .. _9ff0d2d: https://github.com/galaxyproject/planemo/commit/9ff0d2d
```

### Comparing `planemo-0.8.4/LICENSE` & `planemo-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/util/plugin_config.py` & `planemo-0.9.0/planemo_ext/galaxy/util/plugin_config.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/util/submodules.py` & `planemo-0.9.0/planemo_ext/galaxy/util/submodules.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/util/directory_hash.py` & `planemo-0.9.0/planemo_ext/galaxy/util/directory_hash.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/util/__init__.py` & `planemo-0.9.0/planemo_ext/galaxy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/util/bunch.py` & `planemo-0.9.0/planemo_ext/galaxy/util/bunch.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/util/sleeper.py` & `planemo-0.9.0/planemo_ext/galaxy/util/sleeper.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/util/odict.py` & `planemo-0.9.0/planemo_ext/galaxy/util/odict.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/lint.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/lint.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/loader_directory.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/loader_directory.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/linters/xsd_util.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/linters/xsd_util.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/linters/command.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/linters/command.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/linters/outputs.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/linters/outputs.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/linters/top_level.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/linters/top_level.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/linters/xml_order.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/linters/xml_order.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/linters/inputs.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/linters/inputs.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/linters/help.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/linters/help.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/linters/tests.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/linters/tests.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/linters/stdio.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/linters/stdio.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/linters/citations.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/linters/citations.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/docker_util.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/docker_util.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/containers.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/containers.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/dependencies.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/dependencies.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/dockerfiles.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/dockerfiles.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/__init__.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/__init__.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/brew_exts.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/brew_exts.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/requirements.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/requirements.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/resolvers/tool_shed_packages.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/resolvers/tool_shed_packages.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/resolvers/galaxy_packages.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/resolvers/galaxy_packages.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/resolvers/resolver_mixins.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/resolvers/resolver_mixins.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/resolvers/brewed_tool_shed_packages.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/resolvers/brewed_tool_shed_packages.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/resolvers/modules.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/resolvers/modules.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/resolvers/__init__.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/resolvers/homebrew.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/resolvers/homebrew.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/brew_util.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/brew_util.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/deps/commands.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/deps/commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import os
 import subprocess
 
 
 def shell(cmds, env=None):
+    p = shell_process(cmds, env)
+    return p.wait()
+
+
+def shell_process(cmds, env=None, **kwds):
     popen_kwds = dict(
         shell=True,
     )
+    popen_kwds.update(**kwds)
     if env:
         new_env = os.environ.copy()
         new_env.update(env)
         popen_kwds["env"] = new_env
     p = subprocess.Popen(cmds, **popen_kwds)
-    return p.wait()
+    return p
 
 
 def execute(cmds):
     return __wait(cmds, shell=False)
 
 
 def which(file):
```

### Comparing `planemo-0.8.4/planemo_ext/galaxy/tools/loader.py` & `planemo-0.9.0/planemo_ext/galaxy/tools/loader.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/tool_factory_2/rgToolFactory2.py` & `planemo-0.9.0/planemo_ext/tool_factory_2/rgToolFactory2.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/tool_factory_2/getlocalrpackages.py` & `planemo-0.9.0/planemo_ext/tool_factory_2/getlocalrpackages.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/tool_factory_2/rgToolFactory2.xml` & `planemo-0.9.0/planemo_ext/tool_factory_2/rgToolFactory2.xml`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo_ext/tool_factory_2/LICENSE` & `planemo-0.9.0/planemo_ext/tool_factory_2/LICENSE`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/HISTORY.rst` & `planemo-0.9.0/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,45 @@
 
 History
 -------
 
 .. to_doc
 
 ---------------------
+0.9.0 (2015-05-03)
+---------------------
+
+* Add new logo to the README thanks to @petrkadlec from `puradesign.cz
+  <http://puradesign.cz/en>`__ and @carlfeberhard from the Galaxy Project.
+  `Issue 108`_
+* Implement smarter ``shed_diff`` command - it now produces a meaningful
+  exit codes and doesn't report differences if these correspond to attributes
+  that will be automatically populated by the Tool Shed. `Issue 167`_
+* Use new smarter ``shed_diff`` code to implement a new ``--check_diff``
+  option for ``shed_upload`` - to check for meaningful differences before
+  updating repositories. `Issue 168`_
+* Record git commit hash during ``shed_upload`` if the ``.shed.yml`` is
+  located in a git repository. `Issue 170`_
+* Allow ``shed_`` operations to operate on git URLs directly. `Issue 169`_
+* Fail if missing file inclusion statements encountered during ``.shed.yml``
+  repository resolution - bug reported by @peterjc. `Issue 158`_
+* Improved exception handling for tool shed operations including new 
+  ``--fail_fast`` command-line option. * `Issue 114`_, `Pull Request 173`_
+* Implement more validation when using the ``shed_init`` command. 1cd0e2d_
+* Add ``-r/--recursive`` option to ``shed_download`` and ``shed_diff`` 
+  commands and allow these commands to work with ``.shed.yml`` files defining
+  multipe repositories. 40a1f57_
+* Add ``--port`` option to the ``serve`` and ``tool_factory`` commands.
+  15804be_
+* Fix problem introduced with ``setup.py`` during the 0.9.0 development cycle
+  - thanks to @peterjc. `Pull Request 171`_
+* Fix clone bug introduced during 0.9.0 development cycle - thanks to
+  @bgruening. `Pull Request 175`_
+
+---------------------
 0.8.4 (2015-04-30)
 ---------------------
 
 * Fix for Travis CI testing picking up invalid tests (reported by @takadonet). `Issue 161`_
 * Fix tar ordering for consistency (always sort by name) - thanks to @peterjc.  `Pull Request 164`_, `Issue 159`_
 * Fix exception handling related to tool shed operations - thanks to @peterjc. `Pull Request 155`_, b86fe1f_
 
@@ -242,14 +273,27 @@
 0.0.1 (2014-10-04)
 ---------------------
 
 * Initial work on the project - commands for testing, linting, serving Galaxy
   tools - and more experimental features involving Docker and Homebrew. 7d07782_
 
 .. github_links
+.. _Issue 114: https://github.com/galaxyproject/planemo/issues/114
+.. _Pull Request 173: https://github.com/galaxyproject/planemo/pull/173
+.. _Issue 108: https://github.com/galaxyproject/planemo/issues/108
+.. _15804be: https://github.com/galaxyproject/planemo/commit/15804be
+.. _Issue 158: https://github.com/galaxyproject/planemo/issues/158
+.. _Pull Request 171: https://github.com/galaxyproject/planemo/pull/171
+.. _1cd0e2d: https://github.com/galaxyproject/planemo/commit/1cd0e2d
+.. _40a1f57: https://github.com/galaxyproject/planemo/commit/40a1f57
+.. _Pull Request 175: https://github.com/galaxyproject/planemo/pull/175
+.. _Issue 167: https://github.com/galaxyproject/planemo/issues/167
+.. _Issue 170: https://github.com/galaxyproject/planemo/issues/170
+.. _Issue 169: https://github.com/galaxyproject/planemo/issues/169
+.. _Issue 168: https://github.com/galaxyproject/planemo/issues/168
 .. _b86fe1f: https://github.com/galaxyproject/planemo/commit/b86fe1f
 .. _Pull Request 155: https://github.com/galaxyproject/planemo/pull/155
 .. _Pull Request 164: https://github.com/galaxyproject/planemo/pull/164
 .. _Issue 159: https://github.com/galaxyproject/planemo/issues/159
 .. _Issue 161: https://github.com/galaxyproject/planemo/issues/161
 .. _a2ee135: https://github.com/galaxyproject/planemo/commit/a2ee135
 .. _9ff0d2d: https://github.com/galaxyproject/planemo/commit/9ff0d2d
```

### Comparing `planemo-0.8.4/setup.py` & `planemo-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     author_email='jmchilton@gmail.com',
     url='https://github.com/galaxyproject/planemo',
     packages=[
         'planemo',
         'planemo.commands',
         'planemo.linters',
         'planemo.reports',
+        'planemo.shed',
         'planemo.xml',
         'planemo_ext',
         'planemo_ext.galaxy',
         'planemo_ext.galaxy.eggs',
         'planemo_ext.galaxy.tools',
         'planemo_ext.galaxy.tools.linters',
         'planemo_ext.galaxy.tools.deps',
```

### Comparing `planemo-0.8.4/planemo/github_util.py` & `planemo-0.9.0/planemo/github_util.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/xml/validation.py` & `planemo-0.9.0/planemo/xml/validation.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/xml/xsd/tool_dependencies.xsd` & `planemo-0.9.0/planemo/xml/xsd/tool_dependencies.xsd`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/xml/xsd/tool/README.md` & `planemo-0.9.0/planemo/xml/xsd/tool/README.md`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/xml/xsd/tool/citations.xsd` & `planemo-0.9.0/planemo/xml/xsd/tool/citations.xsd`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/xml/xsd/tool/citation.xsd` & `planemo-0.9.0/planemo/xml/xsd/tool/citation.xsd`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/xml/xsd/tool/LICENSE` & `planemo-0.9.0/planemo/xml/xsd/tool/LICENSE`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/xml/xsd/tool/test.sh` & `planemo-0.9.0/planemo/xml/xsd/tool/test.sh`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/xml/xsd/tool/galaxy.jxb` & `planemo-0.9.0/planemo/xml/xsd/tool/galaxy.jxb`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/xml/xsd/tool/galaxy.xsd` & `planemo-0.9.0/planemo/xml/xsd/tool/galaxy.xsd`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/xml/xsd/tool/test.urls` & `planemo-0.9.0/planemo/xml/xsd/tool/test.urls`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/xml/xsd/repository_dependencies.xsd` & `planemo-0.9.0/planemo/xml/xsd/repository_dependencies.xsd`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/reports/build_report.py` & `planemo-0.9.0/planemo/reports/build_report.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/shed_lint.py` & `planemo-0.9.0/planemo/shed_lint.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
-import re
 import yaml
 from galaxy.tools.lint import LintContext
 from galaxy.tools.linters.help import rst_invalid
 from planemo.lint import lint_xsd
 from planemo.shed import (
     path_to_repo_name,
     REPO_TYPE_UNRESTRICTED,
     REPO_TYPE_TOOL_DEP,
     REPO_TYPE_SUITE,
     CURRENT_CATEGORIES,
+    validate_repo_owner,
+    validate_repo_name,
 )
 from planemo.tool_lint import (
     build_lint_args,
     yield_tool_xmls,
 )
 from planemo.xml import XSDS_PATH
 
@@ -22,46 +23,51 @@
 from planemo.io import error
 
 from galaxy.tools.lint import lint_xml_with
 
 TOOL_DEPENDENCIES_XSD = os.path.join(XSDS_PATH, "tool_dependencies.xsd")
 REPO_DEPENDENCIES_XSD = os.path.join(XSDS_PATH, "repository_dependencies.xsd")
 
-# TODO: sync this with tool shed impl someday
-VALID_REPOSITORYNAME_RE = re.compile("^[a-z0-9\_]+$")
-VALID_PUBLICNAME_RE = re.compile("^[a-z0-9\-]+$")
 
 VALID_REPOSITORY_TYPES = [
     REPO_TYPE_UNRESTRICTED,
     REPO_TYPE_TOOL_DEP,
     REPO_TYPE_SUITE,
 ]
 
 
-def lint_repository(ctx, path, **kwds):
+def lint_repository(ctx, realized_repository, **kwds):
+    # TODO: this really needs to start working with realized path.
+    path = realized_repository.real_path
     info("Linting repository %s" % path)
     lint_args = build_lint_args(ctx, **kwds)
     lint_ctx = LintContext(lint_args["level"])
     lint_ctx.lint(
-        "tool_dependencies",
+        "lint_expansion",
+        lint_expansion,
+        realized_repository,
+    )
+
+    lint_ctx.lint(
+        "lint_tool_dependencies",
         lint_tool_dependencies,
         path,
     )
     lint_ctx.lint(
-        "repository_dependencies",
+        "lint_repository_dependencies",
         lint_repository_dependencies,
         path,
     )
     lint_ctx.lint(
-        "shed_yaml",
+        "lint_shed_yaml",
         lint_shed_yaml,
         path,
     )
     lint_ctx.lint(
-        "readme",
+        "lint_readme",
         lint_readme,
         path,
     )
     if kwds["tools"]:
         for (tool_path, tool_xml) in yield_tool_xmls(ctx, path,
                                                      recursive=True):
             info("+Linting tool %s" % tool_path)
@@ -72,14 +78,23 @@
             )
     failed = lint_ctx.failed(lint_args["fail_level"])
     if failed:
         error("Failed linting")
     return 1 if failed else 0
 
 
+def lint_expansion(realized_repository, lint_ctx):
+    missing = realized_repository.missing
+    if missing:
+        msg = "Failed to expand inclusions %s" % missing
+        lint_ctx.warn(msg)
+    else:
+        lint_ctx.info("Included files all found.")
+
+
 def lint_readme(path, lint_ctx):
     readme_rst = os.path.join(path, "README.rst")
     readme = os.path.join(path, "README")
     readme_txt = os.path.join(path, "README.txt")
 
     readme_found = False
     for readme in [readme_rst, readme, readme_txt]:
@@ -133,14 +148,15 @@
     if not os.path.exists(shed_yaml):
         lint_ctx.info("No .shed.yml file found, skipping.")
         return
     try:
         shed_contents = yaml.load(open(shed_yaml, "r"))
     except Exception as e:
         lint_ctx.warn("Failed to parse .shed.yml file [%s]" % str(e))
+        return
     lint_ctx.info(".shed.yml found and appears to be valid YAML.")
     _lint_shed_contents(lint_ctx, path, shed_contents)
 
 
 def _lint_shed_contents(lint_ctx, path, shed_contents):
     name = shed_contents.get("name", None)
     effective_name = name or path_to_repo_name(path)
@@ -148,16 +164,16 @@
     def _lint_if_present(key, func, *args):
         value = shed_contents.get(key, None)
         if value is not None:
             msg = func(value, *args)
             if msg:
                 lint_ctx.warn(msg)
 
-    _lint_if_present("owner", _validate_repo_owner)
-    _lint_if_present("name", _validate_repo_name)
+    _lint_if_present("owner", validate_repo_owner)
+    _lint_if_present("name", validate_repo_name)
     _lint_if_present("type", _validate_repo_type, effective_name)
     _lint_if_present("categories", _validate_categories)
 
 
 def _validate_repo_type(repo_type, name):
     if repo_type not in VALID_REPOSITORY_TYPES:
         return "Invalid repository type specified [%s]" % repo_type
@@ -172,37 +188,14 @@
                 "starting with suite_")
     if name.startswith("package_") or name.startswith("suite_"):
         if repo_type == "unrestricted":
             return ("Repository name indicated specialized repository type "
                     "but repository is listed as unrestricted.")
 
 
-def _validate_repo_name(name):
-    msg = None
-    if len(name) < 2:
-        msg = "Repository names must be at least 2 characters in length."
-    if len(name) > 80:
-        msg = "Repository names cannot be more than 80 characters in length."
-    if not VALID_REPOSITORYNAME_RE.match(name):
-        msg = ("Repository names must contain only lower-case letters, "
-               "numbers and underscore.")
-    return msg
-
-
-def _validate_repo_owner(owner):
-    msg = None
-    if len(owner) < 3:
-        msg = "Owner must be at least 3 characters in length"
-    if len(owner) > 255:
-        msg = "Owner cannot be more than 255 characters in length"
-    if not(VALID_PUBLICNAME_RE.match(owner)):
-        msg = "Owner must contain only lower-case letters, numbers and '-'"
-    return msg
-
-
 def _validate_categories(categories):
     msg = None
     if len(categories) == 0:
         msg = "Repository should specify one or more categories."
     else:
         for category in categories:
             unknown_categories = []
```

### Comparing `planemo-0.8.4/planemo/config.py` & `planemo-0.9.0/planemo/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 import yaml
 
+PLANEMO_CONFIG_ENV_PROP = "PLANEMO_GLOBAL_CONFIG_PATH"
 DEFAULT_CONFIG = {
 }
 
 
 def global_config_path(config_path=None):
     if not config_path:
         config_path = os.environ.get(
-            "PLANEMO_GLOBAL_CONFIG_PATH",
+            PLANEMO_CONFIG_ENV_PROP,
             "~/.planemo.yml"
         )
         config_path = os.path.expanduser(config_path)
     return config_path
 
 
 def read_global_config(config_path):
```

### Comparing `planemo-0.8.4/planemo/commands/cmd_shed_init.py` & `planemo-0.9.0/planemo/commands/cmd_shed_init.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/commands/cmd_shed_lint.py` & `planemo-0.9.0/planemo/commands/cmd_shed_lint.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 from planemo.cli import pass_context
 from planemo import options
 from planemo import shed
 from planemo import shed_lint
 
 
 @click.command('shed_lint')
-@options.optional_project_arg(exists=True)
+@options.shed_project_arg()
 @options.report_level_option()
 @options.fail_level_option()
 @options.click.option(
     '--tools',
     is_flag=True,
     default=False,
     help=("Lint tools discovered in the process of linting repositories.")
 )
 @options.lint_xsd_option()
 @options.recursive_shed_option()
+@options.shed_fail_fast_option()
 @pass_context
 def cli(ctx, path, **kwds):
     """Check a Tool Shed repository for common problems.
     """
     def lint(realized_repository):
-        path = realized_repository.real_path
-        return shed_lint.lint_repository(ctx, path, **kwds)
+        return shed_lint.lint_repository(ctx, realized_repository, **kwds)
 
+    kwds["fail_on_missing"] = False
     exit_code = shed.for_each_repository(lint, path, **kwds)
     sys.exit(exit_code)
```

### Comparing `planemo-0.8.4/planemo/commands/cmd_tool_init.py` & `planemo-0.9.0/planemo/commands/cmd_tool_init.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/commands/cmd_project_init.py` & `planemo-0.9.0/planemo/commands/cmd_project_init.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/commands/cmd_brew_init.py` & `planemo-0.9.0/planemo/commands/cmd_brew_init.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/commands/cmd_create_gist.py` & `planemo-0.9.0/planemo/commands/cmd_create_gist.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/commands/cmd_brew.py` & `planemo-0.9.0/planemo/commands/cmd_brew.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/commands/cmd_config_init.py` & `planemo-0.9.0/planemo/commands/cmd_config_init.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 """
 import os
+import sys
 
 import click
 
 from planemo.cli import pass_context
 from planemo import options
 from planemo import config
 from planemo.io import warn, info
@@ -49,11 +50,11 @@
 def cli(ctx, path, template=None, **kwds):
     """Help initialize global configuration (in home directory) for Planemo.
     """
     # TODO: prompt for values someday.
     config_path = config.global_config_path()
     if os.path.exists(config_path):
         warn("File %s already exists, exiting." % config_path)
-        return -1
+        sys.exit(1)
     with open(config_path, "w") as f:
         f.write(CONFIG_TEMPLATE)
         info(SUCCESS_MESSAGE % config_path)
```

### Comparing `planemo-0.8.4/planemo/commands/cmd_travis_before_install.py` & `planemo-0.9.0/planemo/commands/cmd_travis_before_install.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/commands/cmd_serve.py` & `planemo-0.9.0/planemo/commands/cmd_serve.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from planemo import galaxy_serve
 from planemo import options
 
 
 @click.command('serve')
 @options.optional_tools_arg()
 @options.galaxy_root_option()
+@options.galaxy_port_option()
 @options.install_galaxy_option()
 @options.no_cache_galaxy_option()
 @options.no_cleanup_option()
 @options.test_data_option()
 @options.dependency_resolvers_option()
 @options.job_config_option()
 @options.tool_dependency_dir_option()
```

### Comparing `planemo-0.8.4/planemo/commands/cmd_tool_factory.py` & `planemo-0.9.0/planemo/commands/cmd_tool_factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from planemo.cli import pass_context
 from planemo import options
 from planemo import galaxy_serve
 
 
 @click.command('tool_factory')
 @options.galaxy_root_option()
+@options.galaxy_port_option()
 @options.install_galaxy_option()
 @options.no_cache_galaxy_option()
 @options.no_cleanup_option()
 @options.test_data_option()
 @options.dependency_resolvers_option()
 @options.job_config_option()
 @options.tool_dependency_dir_option()
```

### Comparing `planemo-0.8.4/planemo/commands/cmd_share_test.py` & `planemo-0.9.0/planemo/commands/cmd_share_test.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/commands/cmd_travis_init.py` & `planemo-0.9.0/planemo/commands/cmd_travis_init.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/commands/cmd_shed_create.py` & `planemo-0.9.0/planemo/commands/cmd_shed_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 from planemo.cli import pass_context
 from planemo import options
 from planemo import shed
 from planemo.io import info
 
 
 @click.command("shed_create")
-@options.optional_project_arg(exists=True)
+@options.shed_project_arg()
 @options.shed_owner_option()
 @options.shed_name_option()
 @options.shed_target_option()
 @options.shed_key_option()
 @options.shed_email_option()
 @options.shed_password_option()
 @options.recursive_shed_option()
+@options.shed_fail_fast_option()
 @pass_context
 def cli(ctx, path, **kwds):
     """Create a repository in a Galaxy Tool Shed from a ``.shed.yml`` file.
     """
     tsi = shed.tool_shed_client(ctx, **kwds)
 
     def create(realized_reposiotry):
```

### Comparing `planemo-0.8.4/planemo/commands/cmd_docker_shell.py` & `planemo-0.9.0/planemo/commands/cmd_docker_shell.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/commands/cmd_brew_env.py` & `planemo-0.9.0/planemo/commands/cmd_brew_env.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/commands/cmd_shed_diff.py` & `planemo-0.9.0/planemo/commands/cmd_shed_diff.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 """
 """
-import os
-import shutil
-import tempfile
+import sys
 
 import click
 
 from planemo.cli import pass_context
-from planemo.io import shell
 from planemo import options
 from planemo import shed
 
 
 @click.command("shed_diff")
-@options.optional_project_arg(exists=True)
+@options.shed_project_arg()
 @options.shed_owner_option()
 @options.shed_name_option()
 @options.shed_target_option()
+@options.shed_fail_fast_option()
 @click.option(
     "-o", "--output",
     type=click.Path(file_okay=True, resolve_path=True),
     help="Send diff output to specified file.",
     default=None,
 )
 @click.option(
     '--shed_target_source',
     help="Source Tool Shed to diff against (will ignore local project info"
          " specified). To compare the main Tool Shed against the test, set"
          " this to testtoolshed.",
     default=None,
 )
+@click.option(
+    "--raw",
+    is_flag=True,
+    help="Do not attempt smart diff of XML to filter out attributes "
+         "populated by the Tool Shed.",
+)
+@options.recursive_shed_option()
 @pass_context
 def cli(ctx, path, **kwds):
     """Produce diff between local repository and Tool Shed contents.
 
     By default, this will produce a diff between this repository and what
     would be uploaded to the Tool Shed with the `shed_upload` command - but
     this command can be made to compare other combinations of repositories.
@@ -46,57 +51,12 @@
         % # diff for the test Tool Shed and main Tool Shed
         % planemo shed_diff --shed_target_source testtoolshed
         % # diff for two an explicitly specified repositories (ignores
         % # current project's shed YAML file.)
         % planemo shed_diff --owner peterjc --name blast_rbh
             --shed_target_source testtoolshed
     """
-    working = tempfile.mkdtemp(prefix="tool_shed_diff_")
-    try:
-        diff_in(ctx, working, path, **kwds)
-    finally:
-        shutil.rmtree(working)
-
-
-def diff_in(ctx, working, path, **kwds):
-    shed_target_source = kwds.get("shed_target_source", None)
-
-    label_a = "_%s_" % (shed_target_source if shed_target_source else "local")
-    shed_target = kwds.get("shed_target", "B")
-    if "/" in shed_target:
-        shed_target = "custom_shed"
-    label_b = "_%s_" % shed_target
-
-    mine = os.path.join(working, label_a)
-    other = os.path.join(working, label_b)
-
-    tsi = shed.tool_shed_client(ctx, read_only=True, **kwds)
-    shed.download_tarball(
-        ctx,
-        tsi,
-        path,
-        destination=other,
-        clean=True,
-        **kwds
-    )
-
-    if shed_target_source:
-        new_kwds = kwds.copy()
-        new_kwds["shed_target"] = shed_target_source
-        tsi = shed.tool_shed_client(ctx, read_only=True, **new_kwds)
-        shed.download_tarball(
-            ctx,
-            tsi,
-            path,
-            destination=mine,
-            clean=True,
-            **new_kwds
-        )
-    else:
-        tar_path = shed.build_tarball(path)
-        cmd_template = 'mkdir "%s"; tar -xzf "%s" -C "%s"; rm -rf %s'
-        shell(cmd_template % (mine, tar_path, mine, tar_path))
-
-    cmd = 'cd "%s"; diff -r %s %s' % (working, label_a, label_b)
-    if kwds["output"]:
-        cmd += "> '%s'" % kwds["output"]
-    shell(cmd)
+    def diff(realized_repository):
+        return shed.diff_repo(ctx, realized_repository, **kwds)
+
+    exit_code = shed.for_each_repository(diff, path, **kwds)
+    sys.exit(exit_code)
```

### Comparing `planemo-0.8.4/planemo/commands/cmd_normalize.py` & `planemo-0.9.0/planemo/commands/cmd_normalize.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/commands/cmd_lint.py` & `planemo-0.9.0/planemo/commands/cmd_lint.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/commands/cmd_test.py` & `planemo-0.9.0/planemo/commands/cmd_test.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/commands/cmd_docker_build.py` & `planemo-0.9.0/planemo/commands/cmd_docker_build.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/options.py` & `planemo-0.9.0/planemo/options.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,23 @@
     return click.option(
         "--galaxy_root",
         type=click.Path(exists=True, file_okay=False, resolve_path=True),
         help='Root of development galaxy directory to execute command with.'
     )
 
 
+def galaxy_port_option():
+    return click.option(
+        "--port",
+        type=int,
+        default="9090",
+        help='Port to serve Galaxy on (default is 9090).'
+    )
+
+
 def dependency_resolvers_option():
     return click.option(
         "--dependency_resolvers_config_file",
         type=click.Path(
             exists=True,
             file_okay=True,
             dir_okay=False,
@@ -152,14 +161,42 @@
         metavar="TOOL_PATH",
         default=".",
         type=arg_type,
         nargs=nargs,
     )
 
 
+class ProjectOrRepositry(click.Path):
+
+    def __init__(self, **kwds):
+        super(ProjectOrRepositry, self).__init__(**kwds)
+
+    def convert(self, value, param, ctx):
+        if value and value.startswith("git:") or value.startswith("git+"):
+            return value
+        else:
+            return super(ProjectOrRepositry, self).convert(value, param, ctx)
+
+
+def shed_project_arg():
+    arg_type = ProjectOrRepositry(
+        exists=True,
+        file_okay=False,
+        dir_okay=True,
+        writable=True,
+        resolve_path=True,
+    )
+    return click.argument(
+        'path',
+        metavar="PROJECT",
+        default=".",
+        type=arg_type,
+    )
+
+
 def optional_project_arg(exists=True):
     arg_type = click.Path(
         exists=exists,
         file_okay=False,
         dir_okay=True,
         writable=True,
         resolve_path=True,
@@ -259,14 +296,24 @@
     return click.option(
         '--shed_password',
         help="Password for Tool Shed auth (required unless shed_key is "
              "specified)."
     )
 
 
+def shed_fail_fast_option():
+    return click.option(
+        '--fail_fast',
+        is_flag=True,
+        default=False,
+        help="If multiple repositories are specified and an error occurs "
+             "stop immediately instead of processing remaining repositories."
+    )
+
+
 def lint_xsd_option():
     return click.option(
         '--xsd',
         is_flag=True,
         default=False,
         help=("Include experimental tool XSD validation in linting "
               "process (requires xmllint on PATH or lxml installed).")
```

### Comparing `planemo-0.8.4/planemo/tool_lint.py` & `planemo-0.9.0/planemo/tool_lint.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/linters/xsd.py` & `planemo-0.9.0/planemo/linters/xsd.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/galaxy_serve.py` & `planemo-0.9.0/planemo/galaxy_serve.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/shed.py` & `planemo-0.9.0/planemo/shed/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,47 @@
+from collections import namedtuple
+import contextlib
 import copy
 import fnmatch
-from planemo import glob
 import hashlib
 import json
 import os
+import re
+import shutil
+import sys
 import tarfile
 from tempfile import (
     mkstemp,
-    mkdtemp,
 )
-import shutil
 
 from six import iteritems
 import yaml
 
-try:
-    from bioblend import toolshed
-except ImportError:
-    toolshed = None
-
 from planemo.io import (
     error,
-    untar_to,
+    shell,
+    info,
     can_write_to_path,
+    temp_directory,
 )
+from planemo import git
+from planemo import glob
 from planemo.tools import load_tool_elements_from_path
 from planemo import templates
 
+from .interface import (
+    username,
+    tool_shed_instance,
+    find_repository,
+    api_exception_to_message,
+    find_category_ids,
+    download_tar,
+)
+from .diff import diff_and_remove
+
 SHED_CONFIG_NAME = '.shed.yml'
 REPO_DEPENDENCIES_CONFIG_NAME = "repository_dependencies.xml"
 TOOL_DEPENDENCIES_CONFIG_NAME = "tool_dependencies.xml"
 
 NO_REPOSITORIES_MESSAGE = ("Could not find any .shed.yml files or a --name to "
                            "describe the target repository.")
 NAME_INVALID_MESSAGE = ("Cannot use --name argument when multiple directories "
@@ -40,14 +51,16 @@
                              "with value discovered in .shed.yml.")
 PARSING_PROBLEM = ("Problem parsing file .shed.yml in directory %s, skipping "
                    "repository. Message: [%s].")
 AUTO_REPO_CONFLICT_MESSAGE = ("Cannot specify both auto_tool_repositories and "
                               "repositories in .shed.yml at this time.")
 AUTO_NAME_CONFLICT_MESSAGE = ("Cannot specify both auto_tool_repositories and "
                               "in .shed.yml and --name on the command-line.")
+REALIZAION_PROBLEMS_MESSAGE = ("Problem encountered executing action for one or more "
+                               "repositories.")
 # Planemo generated or consumed files that do not need to be uploaded to the
 # tool shed.
 PLANEMO_FILES = [
     "shed_upload.tar.gz",
     "tool_test_output.json",
     "tool_test_output.html",
     ".travis",
@@ -55,26 +68,22 @@
     ".shed.yml"
 ]
 SHED_SHORT_NAMES = {
     "toolshed": "https://toolshed.g2.bx.psu.edu/",
     "testtoolshed": "https://testtoolshed.g2.bx.psu.edu/",
     "local": "http://localhost:9009/"
 }
-REPOSITORY_DOWNLOAD_TEMPLATE = (
-    "%srepository/download?repository_id=%s"
-    "&changeset_revision=default&file_type=gz"
-)
-BIOBLEND_UNAVAILABLE = ("This functionality requires the bioblend library "
-                        " which is unavailable, please install `pip install "
-                        "bioblend`")
-
 REPO_TYPE_UNRESTRICTED = "unrestricted"
 REPO_TYPE_TOOL_DEP = "tool_dependency_definition"
 REPO_TYPE_SUITE = "repository_suite_definition"
 
+# TODO: sync this with tool shed impl someday
+VALID_REPOSITORYNAME_RE = re.compile("^[a-z0-9\_]+$")
+VALID_PUBLICNAME_RE = re.compile("^[a-z0-9\-]+$")
+
 # Generate with python scripts/categories.py
 CURRENT_CATEGORIES = [
     "Assembly",
     "ChIP-seq",
     "Combinatorial Selections",
     "Computational chemistry",
     "Convert Formats",
@@ -112,15 +121,18 @@
     if not os.path.exists(path):
         os.makedirs(path)
     shed_config_path = os.path.join(path, SHED_CONFIG_NAME)
     if not can_write_to_path(shed_config_path, **kwds):
         # .shed.yml exists and no --force sent.
         return 1
 
-    _create_shed_config(ctx, shed_config_path, **kwds)
+    create_failed = _create_shed_config(ctx, shed_config_path, **kwds)
+    if create_failed:
+        return 1
+
     repo_dependencies_path = os.path.join(path, REPO_DEPENDENCIES_CONFIG_NAME)
     from_workflow = kwds.get("from_workflow", None)
 
     if from_workflow:
         workflow_name = os.path.basename(from_workflow)
         workflow_target = os.path.join(path, workflow_name)
         if not os.path.exists(workflow_target):
@@ -133,30 +145,143 @@
         repository_dependencies = RepositoryDependencies()
         repository_dependencies.repo_pairs = repo_pairs
         repository_dependencies.write_to_path(repo_dependencies_path)
 
     return 0
 
 
+def upload_repository(ctx, realized_repository, **kwds):
+    """Upload a tool directory as a tarball to a tool shed.
+    """
+    path = realized_repository.path
+    tar_path = kwds.get("tar", None)
+    if not tar_path:
+        tar_path = build_tarball(path, **kwds)
+    if kwds["tar_only"]:
+        name = realized_repository.pattern_to_file_name("shed_upload.tar.gz")
+        shell("cp '%s' '%s'" % (tar_path, name))
+        return 0
+    tsi = tool_shed_client(ctx, **kwds)
+    update_kwds = {}
+    _update_commit_message(ctx, realized_repository, update_kwds, **kwds)
+
+    repo_id = realized_repository.find_repository_id(ctx, tsi)
+    if repo_id is None and kwds["force_repository_creation"]:
+        repo_id = realized_repository.create(ctx, tsi)
+    # failing to create the repo, give up
+    if repo_id is None:
+        return -1
+
+    if kwds["check_diff"]:
+        is_diff = diff_repo(ctx, realized_repository, **kwds)
+        if not is_diff:
+            name = realized_repository.name
+            info("Repositry [%s] not different, skipping upload." % name)
+            return 0
+
+    # TODO: support updating repo information if it changes in the config file
+    try:
+        tsi.repositories.update_repository(repo_id, tar_path, **update_kwds)
+    except Exception as e:
+        message = api_exception_to_message(e)
+        error("Could not update %s" % realized_repository.name)
+        error(message)
+        return -1
+    info("Repository %s updated successfully." % realized_repository.name)
+    return 0
+
+
+def _update_commit_message(ctx, realized_repository, update_kwds, **kwds):
+    message = kwds.get("message", None)
+    git_rev = realized_repository.git_rev(ctx)
+    git_repo = realized_repository.git_repo(ctx)
+    if message is None:
+        message = "planemo upload"
+        if git_repo:
+            message += " for repository %s" % git_repo
+        if git_rev:
+            message += " commit %s" % git_rev
+    update_kwds["commit_message"] = message
+
+
+def diff_repo(ctx, realized_repository, **kwds):
+    with temp_directory("tool_shed_diff_") as working:
+        return _diff_in(ctx, working, realized_repository, **kwds)
+
+
+def _diff_in(ctx, working, realized_repository, **kwds):
+    path = realized_repository.path
+    shed_target_source = kwds.get("shed_target_source", None)
+
+    label_a = "_%s_" % (shed_target_source if shed_target_source else "local")
+    shed_target = kwds.get("shed_target", "B")
+    if "/" in shed_target:
+        shed_target = "custom_shed"
+    label_b = "_%s_" % shed_target
+
+    mine = os.path.join(working, label_a)
+    other = os.path.join(working, label_b)
+
+    tsi = tool_shed_client(ctx, read_only=True, **kwds)
+    download_tarball(
+        ctx,
+        tsi,
+        realized_repository,
+        destination=other,
+        clean=True,
+        **kwds
+    )
+    if shed_target_source:
+        new_kwds = kwds.copy()
+        new_kwds["shed_target"] = shed_target_source
+        tsi = tool_shed_client(ctx, read_only=True, **new_kwds)
+        download_tarball(
+            ctx,
+            tsi,
+            realized_repository,
+            destination=mine,
+            clean=True,
+            **new_kwds
+        )
+    else:
+        tar_path = build_tarball(path)
+        cmd_template = 'mkdir "%s"; tar -xzf "%s" -C "%s"; rm -rf %s'
+        shell(cmd_template % (mine, tar_path, mine, tar_path))
+
+    output = kwds.get("output", None)
+    raw = kwds.get("raw", False)
+    is_diff = 0
+    if not raw:
+        if output:
+            with open(output, "w") as f:
+                is_diff = diff_and_remove(working, label_a, label_b, f)
+        else:
+            is_diff = diff_and_remove(working, label_a, label_b, sys.stdout)
+
+    cmd = 'cd "%s"; diff -r %s %s' % (working, label_a, label_b)
+    if output:
+        cmd += ">> '%s'" % output
+    exit = shell(cmd) or is_diff
+    return exit
+
+
 def shed_repo_config(path, name=None):
     shed_yaml_path = os.path.join(path, SHED_CONFIG_NAME)
     config = {}
     if os.path.exists(shed_yaml_path):
         with open(shed_yaml_path, "r") as f:
             config = yaml.load(f)
 
     if config is None:  # yaml may yield None
         config = {}
     _expand_raw_config(config, path, name=name)
     return config
 
 
 def tool_shed_client(ctx=None, **kwds):
-    if toolshed is None:
-        raise Exception(BIOBLEND_UNAVAILABLE)
     read_only = kwds.get("read_only", False)
     shed_target = kwds.get("shed_target")
     global_config = getattr(ctx, "global_config", {})
     if global_config and "sheds" in global_config:
         sheds_config = global_config["sheds"]
         shed_config = sheds_config.get(shed_target, {})
     else:
@@ -170,21 +295,15 @@
         key = None
         email = None
         password = None
     else:
         key = prop("key")
         email = prop("email")
         password = prop("password")
-    tsi = toolshed.ToolShedInstance(
-        url=url,
-        key=key,
-        email=email,
-        password=password
-    )
-    return tsi
+    return tool_shed_instance(url, key, email, password)
 
 
 def find_repository_id(ctx, tsi, path, **kwds):
     repo_config = kwds.get("config", None)
     if repo_config is None:
         name = kwds.get("name", None)
         repo_config = shed_repo_config(path, name=name)
@@ -196,14 +315,16 @@
 
 
 def _find_repository_id(ctx, tsi, name, repo_config, **kwds):
     global_config = getattr(ctx, "global_config", {})
     owner = kwds.get("owner", None) or repo_config.get("owner", None)
     if owner is None:
         owner = global_config.get("shed_username", None)
+    if owner is None:
+        owner = username(tsi)
 
     matching_repository = find_repository(tsi, owner, name)
     if matching_repository is None:
         if not kwds.get("allow_none", False):
             message = "Failed to find repository for owner/name %s/%s"
             raise Exception(message % (owner, name))
         else:
@@ -227,25 +348,27 @@
 
     if repos and auto_tool_repos:
         raise Exception(AUTO_REPO_CONFLICT_MESSAGE)
     if auto_tool_repos and name_input:
         raise Exception(AUTO_NAME_CONFLICT_MESSAGE)
     if auto_tool_repos:
         repos = _build_auto_tool_repos(path, config, auto_tool_repos)
+    if suite_config:
+        if repos is None:
+            repos = {}
+        _build_suite_repo(config, repos, suite_config)
     # If repositories aren't defined, just define a single
     # one based on calculated name and including everything
     # by default.
     if repos is None:
         repos = {
             config["name"]: {
                 "include": default_include
             }
         }
-    if suite_config:
-        _build_suite_repo(config, repos, suite_config)
     config["repositories"] = repos
 
 
 def _build_auto_tool_repos(path, config, auto_tool_repos):
     default_include = config.get("include", ["**"])
     tool_els = list(load_tool_elements_from_path(path, recursive=True))
     paths = list(map(lambda pair: pair[0], tool_els))
@@ -309,27 +432,14 @@
         "description": description,
     }
     if long_description:
         repo["long_description"] = long_description
     repos[name] = repo
 
 
-def find_repository(tsi, owner, name):
-    repos = tsi.repositories.get_repositories()
-
-    def matches(r):
-        return r["owner"] == owner and r["name"] == name
-
-    matching_repos = list(filter(matches, repos))
-    if not matching_repos:
-        return None
-    else:
-        return matching_repos[0]
-
-
 def create_repository_for(ctx, tsi, name, repo_config):
     description = repo_config.get("description", None)
     long_description = repo_config.get("long_description", None)
     repo_type = shed_repo_type(repo_config, name)
     remote_repository_url = repo_config.get("remote_repository_url", None)
     homepage_url = repo_config.get("homepage_url", None)
     categories = repo_config.get("categories", [])
@@ -348,60 +458,37 @@
         remote_repository_url=remote_repository_url,
         homepage_url=homepage_url,
         category_ids=category_ids
     )
     return repo
 
 
-def find_category_ids(tsi, categories):
-    """ Translate human readable category names into their associated IDs.
-    """
-    category_list = tsi.repositories.get_categories()
-
-    category_ids = []
-    for cat in categories:
-        matching_cats = [x for x in category_list if x['name'] == cat]
-        if not matching_cats:
-            message = "Failed to find category %s" % cat
-            raise Exception(message)
-        category_ids.append(matching_cats[0]['id'])
-    return category_ids
-
-
-def download_tarball(ctx, tsi, path, **kwds):
-    destination = kwds.get('destination', 'shed_download.tar.gz')
-    repo_id = find_repository_id(ctx, tsi, path, **kwds)
-    base_url = tsi.base_url
-    if not base_url.endswith("/"):
-        base_url += "/"
-    download_url = REPOSITORY_DOWNLOAD_TEMPLATE % (base_url, repo_id)
+def download_tarball(ctx, tsi, realized_repository, **kwds):
+    repo_id = realized_repository.find_repository_id(ctx, tsi)
+    if repo_id is None:
+        message = "Unable to find repository id, cannot download."
+        error(message)
+        raise Exception(message)
+    destination_pattern = kwds.get('destination', 'shed_download.tar.gz')
+    destination = realized_repository.pattern_to_file_name(destination_pattern)
     to_directory = not destination.endswith("gz")
-    if to_directory:
-        untar_args = "-xzf - -C %s --strip-components 1" % destination
-    else:
-        untar_args = None
-    untar_to(download_url, destination, untar_args)
+    download_tar(tsi, repo_id, destination, to_directory=to_directory)
     if to_directory:
         clean = kwds.get("clean", False)
         if clean:
             archival_file = os.path.join(destination, ".hg_archival.txt")
             if os.path.exists(archival_file):
                 os.remove(archival_file)
 
 
 def build_tarball(realized_path, **kwds):
     """Build a tool-shed tar ball for the specified path, caller is
     responsible for deleting this file.
     """
 
-    # Not really how realize_effective_repositories was meant to be used.
-    # It should be pushed up a level into the thing that is uploading tar
-    # balls to iterate over them - but placing it here for now because
-    # it address some bugs.
-
     # Simplest solution to sorting the files is to use a list,
     files = []
     for dirpath, dirnames, filenames in os.walk(realized_path):
         for f in filenames:
             files.append(os.path.join(dirpath, f))
     files.sort()
 
@@ -417,39 +504,31 @@
     finally:
         os.close(fd)
     return temp_path
 
 
 def for_each_repository(function, path, **kwds):
     ret_codes = []
-    effective_repositories = realize_effective_repositories(path, **kwds)
-    for realized_repository in effective_repositories:
-        ret_codes.append(
-            function(realized_repository)
-        )
+    with _path_on_disk(path) as raw_path:
+        try:
+            for realized_repository in _realize_effective_repositories(
+                raw_path, **kwds
+            ):
+                ret_codes.append(
+                    function(realized_repository)
+                )
+        except RealizationException:
+            error(REALIZAION_PROBLEMS_MESSAGE)
+            return 254
+
     # "Good" returns are Nones, everything else is a -1 and should be
     # passed upwards.
     return 0 if all((not x) for x in ret_codes) else -1
 
 
-def username(tsi):
-    user = _user(tsi)
-    return user["username"]
-
-
-def _user(tsi):
-    """ Fetch user information from the ToolShed API for given
-    key.
-    """
-    # TODO: this should be done with an actual bioblend method,
-    # see https://github.com/galaxyproject/bioblend/issues/130.
-    response = tsi.make_get_request(tsi.url + "/users")
-    return response.json()[0]
-
-
 def path_to_repo_name(path):
     return os.path.basename(os.path.abspath(path))
 
 
 def shed_repo_type(config, name):
     repo_type = config.get("type", None)
     if repo_type is None and name.startswith("package_"):
@@ -464,38 +543,60 @@
 def _tool_shed_url(kwds):
     url = kwds.get("shed_target")
     if url in SHED_SHORT_NAMES:
         url = SHED_SHORT_NAMES[url]
     return url
 
 
-def realize_effective_repositories(path, **kwds):
+def _realize_effective_repositories(path, **kwds):
     """ Expands folders in a source code repository into tool shed
     repositories.
 
     Each folder may have nested repositories and each folder may corresponding
     to many repositories (for instance if a folder has n tools in the source
     code repository but are published to the tool shed as one repository per
     tool).
     """
     raw_repo_objects = _find_raw_repositories(path, **kwds)
-    temp_directory = mkdtemp()
-    try:
+    failed = False
+    with temp_directory() as base_dir:
         for raw_repo_object in raw_repo_objects:
-            for realized_repo in raw_repo_object.realizations(temp_directory):
+            if isinstance(raw_repo_object, Exception):
+                _handle_realization_error(raw_repo_object, **kwds)
+                failed = True
+                continue
+
+            realized_repos = raw_repo_object.realizations(
+                base_dir,
+                kwds.get("fail_on_missing", True)
+            )
+            for realized_repo in realized_repos:
+                if isinstance(realized_repo, Exception):
+                    _handle_realization_error(realized_repo, **kwds)
+                    failed = True
+                    continue
                 yield realized_repo
-    finally:
-        shutil.rmtree(temp_directory)
+    if failed:
+        raise RealizationException()
 
 
 def _create_shed_config(ctx, path, **kwds):
     name = kwds.get("name", None) or path_to_repo_name(os.path.dirname(path))
+    name_invalid = validate_repo_name(name)
+    if name_invalid:
+        error(name_invalid)
+        return 1
+
     owner = kwds.get("owner", None)
     if owner is None:
         owner = ctx.global_config.get("shed_username", None)
+    owner_invalid = validate_repo_owner(owner)
+    if owner_invalid:
+        error(owner_invalid)
+        return 1
     description = kwds.get("description", None) or name
     long_description = kwds.get("long_description", None)
     remote_repository_url = kwds.get("remote_repository_url", None)
     homepage_url = kwds.get("homepage_url", None)
     categories = kwds.get("category", [])
     config = dict(
         name=name,
@@ -535,29 +636,50 @@
         owner = tool_repo_parts[0]
         name = tool_repo_parts[1]
         repo_pairs.add((owner, name))
 
     return repo_pairs
 
 
+@contextlib.contextmanager
+def _path_on_disk(path):
+    git_path = None
+    if path.startswith("git:"):
+        git_path = path
+    elif path.startswith("git+"):
+        git_path = path[len("git+"):]
+    if git_path is None:
+        yield path
+    else:
+        with temp_directory() as git_repo:
+            # TODO: pass ctx down through
+            git.clone(None, git_path, git_repo)
+            yield git_repo
+
+
 def _find_raw_repositories(path, **kwds):
     name = kwds.get("name", None)
     recursive = kwds.get("recursive", False)
 
     shed_file_dirs = []
     if recursive:
         for base_path, dirnames, filenames in os.walk(path):
             for filename in fnmatch.filter(filenames, SHED_CONFIG_NAME):
                 shed_file_dirs.append(base_path)
     elif os.path.exists(os.path.join(path, SHED_CONFIG_NAME)):
         shed_file_dirs.append(path)
 
     config_name = None
     if len(shed_file_dirs) == 1:
-        config = shed_repo_config(shed_file_dirs[0], name=name)
+        shed_file_dir = shed_file_dirs[0]
+        try:
+            config = shed_repo_config(shed_file_dir, name=name)
+        except Exception as e:
+            error_message = PARSING_PROBLEM % (shed_file_dir, e)
+            return [RuntimeError(error_message)]
         config_name = config.get("name", None)
 
     if len(shed_file_dirs) > 1 and name is not None:
         raise Exception(NAME_INVALID_MESSAGE)
     if config_name is not None and name is not None:
         if config_name != name:
             raise Exception(CONFLICTING_NAMES_MESSAGE)
@@ -571,27 +693,27 @@
     """
     From specific directories with .shed.yml files or specified directly from
     the comman-line build abstract description of directories that should be
     expanded out into shed repositories.
     """
     multiple = len(raw_dirs) > 1
     name = kwds.get("name", None)
-    skip_errors = kwds.get("skip_errors", False)
 
+    # List of RawRepositoryDirectories or parsing failures if
+    # fail_fast is not enabled.
     raw_repo_objects = []
     for raw_dir in raw_dirs:
         try:
             config = shed_repo_config(raw_dir, name=name)
         except Exception as e:
-            if skip_errors:
-                error_message = PARSING_PROBLEM % (raw_dir, e)
-                error(error_message)
-                continue
-            else:
-                raise
+            error_message = PARSING_PROBLEM % (raw_dir, e)
+            exception = RuntimeError(error_message)
+            _handle_realization_error(exception, **kwds)
+            raw_repo_objects.append(exception)
+            continue
         raw_repo_object = RawRepositoryDirectory(raw_dir, config, multiple)
         raw_repo_objects.append(raw_repo_object)
     return raw_repo_objects
 
 
 class RepositoryDependencies(object):
     """ Abstraction for shed repository_dependencies.xml files.
@@ -599,15 +721,15 @@
 
     def __init__(self):
         self.description = ""
         self.repo_pairs = []
 
     def __str__(self):
         contents = '<repositories description="%s">' % self.description
-        line_template = '  <repository owner="%s" name="%s" />'
+        line_template = '  <repository owner="%s" name="%s" />\n'
         for (owner, name) in self.repo_pairs:
             contents += line_template % (owner, name)
         contents += "</repositories>"
         return contents
 
     def write_to_path(self, path):
         with open(path, "w") as f:
@@ -622,32 +744,38 @@
         self.name = config["name"]
         self.type = shed_repo_type(config, self.name)
         self.multiple = multiple  # operation over many repos?
 
     def _hash(self, name):
         return hashlib.md5(name.encode('utf-8')).hexdigest()
 
-    def realizations(self, parent_directory):
+    def realizations(self, parent_directory, fail_on_missing=True):
         names = self._repo_names()
 
         for name in names:
             directory = os.path.join(parent_directory, self._hash(name), name)
             multiple = self.multiple or len(names) > 1
             if not os.path.exists(directory):
                 os.makedirs(directory)
-            yield self._realize_to(directory, name, multiple)
+            yield self._realize_to(directory, name, multiple, fail_on_missing)
 
-    def _realize_to(self, directory, name, multiple):
+    def _realize_to(self, directory, name, multiple, fail_on_missing):
         ignore_list = []
         config = self._realize_config(name)
         excludes = _shed_config_excludes(config)
         for exclude in excludes:
             ignore_list.extend(_glob(self.path, exclude))
 
-        for realized_file in self._realized_files(name):
+        realized_files = self._realized_files(name)
+        missing = realized_files.include_failures
+        if missing and fail_on_missing:
+            msg = "Failed to include files for %s" % missing
+            return RuntimeError(msg)
+
+        for realized_file in realized_files.files:
             relative_dest = realized_file.relative_dest
             implicit_ignore = self._implicit_ignores(relative_dest)
             explicit_ignore = (realized_file.absolute_src in ignore_list)
             if implicit_ignore or explicit_ignore:
                 continue
             realized_file.realize_to(directory)
 
@@ -656,29 +784,32 @@
             with open(path, "w") as f:
                 f.write(contents)
 
         return RealizedRepositry(
             realized_path=directory,
             real_path=self.path,
             config=config,
-            multiple=multiple
+            multiple=multiple,
+            missing=missing,
         )
 
     def _repo_names(self):
         return self.config.get("repositories").keys()
 
     def _realized_files(self, name):
         config = self._realize_config(name)
         realized_files = []
+        missing = []
         for include in config["include"]:
-            realized_files.extend(
-                RealizedFile.realized_files_for(self.path, include)
-            )
-        for realized_file in realized_files:
-            yield realized_file
+            included = RealizedFile.realized_files_for(self.path, include)
+            if not included:
+                missing.append(include)
+            else:
+                realized_files.extend(included)
+        return RealizedFiles(realized_files, missing)
 
     def _realize_config(self, name):
         config = copy.deepcopy(self.config)
         config["name"] = name
         repo_config = config.get("repositories", {}).get(name, {})
         config.update(repo_config)
         if "repositories" in config:
@@ -699,14 +830,16 @@
         name = os.path.basename(relative_path)
         if relative_path.startswith(".git"):
             return True
         elif name in PLANEMO_FILES:
             return True
         return False
 
+RealizedFiles = namedtuple("RealizedFiles", ["files", "include_failures"])
+
 
 class RealizedFile(object):
 
     def __init__(self, src_root, src, dest, dest_is_file, strip_components):
         self.src_root = src_root
         self.src = src
         self.dest = dest
@@ -771,20 +904,40 @@
         return "RealizedFile[src={},dest={},dest_file={}]".format(
             self.src, self.dest, self.dest_is_file
         )
 
 
 class RealizedRepositry(object):
 
-    def __init__(self, realized_path, real_path, config, multiple):
+    def __init__(self, realized_path, real_path, config, multiple, missing):
         self.path = realized_path
         self.real_path = real_path
         self.config = config
         self.name = config["name"]
         self.multiple = multiple
+        self.missing = missing
+
+    def git_rev(self, ctx):
+        return git.rev_if_git(ctx, self.real_path)
+
+    def git_repo(self, ctx):
+        return self.config.get("remote_repository_url", None)
+
+    def pattern_to_file_name(self, pattern):
+        if not self.multiple:
+            return pattern
+
+        name = self.config["name"]
+        suffix = "_%s" % name.replace("-", "_")
+
+        if "." not in pattern:
+            return pattern + suffix
+        else:
+            parts = pattern.split(".", 1)
+            return parts[0] + suffix + "." + parts[1]
 
     def find_repository_id(self, ctx, tsi):
         try:
             repo_id = _find_repository_id(
                 ctx,
                 tsi,
                 name=self.name,
@@ -816,30 +969,83 @@
                 upstream_error = json.loads(e.read())
                 error(upstream_error['err_msg'])
             except Exception:
                 error(str(e))
             return None
 
 
-def api_exception_to_message(e):
-    message = str(e)
-    if hasattr(e, "read"):
-        message = e.read()
-        try:
-            # Galaxy passes nice JSON messages as their errors, which bioblend
-            # blindly returns. Attempt to parse those.
-            upstream_error = json.loads(message)
-            message = upstream_error['err_msg']
-        except Exception:
-            pass
-    return message
-
-
 def _glob(path, pattern):
     pattern = os.path.join(path, pattern)
     if os.path.isdir(pattern):
         pattern = "%s/**" % pattern
     return glob.glob(pattern)
 
 
 def _shed_config_excludes(config):
     return config.get('ignore', []) + config.get('exclude', [])
+
+
+def _handle_realization_error(exception, **kwds):
+    fail_fast = kwds.get("fail_fast", False)
+    if fail_fast:
+        raise exception
+    else:
+        error(str(exception))
+
+
+def validate_repo_name(name):
+    def _build_error(descript):
+        return "Repository name [%s] invalid. %s" % (name, descript)
+
+    msg = None
+    if len(name) < 2:
+        msg = _build_error(
+            "Repository names must be at least 2 characters in length."
+        )
+    if len(name) > 80:
+        msg = _build_error(
+            "Repository names cannot be more than 80 characters in length."
+        )
+    if not VALID_REPOSITORYNAME_RE.match(name):
+        msg = _build_error(
+            "Repository names must contain only lower-case letters, "
+            "numbers and underscore."
+        )
+    return msg
+
+
+def validate_repo_owner(owner):
+    def _build_error(descript):
+        return "Owner [%s] invalid. %s" % (owner, descript)
+    msg = None
+    if len(owner) < 3:
+        msg = _build_error("Owner must be at least 3 characters in length")
+    if len(owner) > 255:
+        msg = _build_error(
+            "Owner cannot be more than 255 characters in length"
+        )
+    if not(VALID_PUBLICNAME_RE.match(owner)):
+        msg = _build_error(
+            "Owner must contain only lower-case letters, numbers and '-'"
+        )
+    return msg
+
+
+class RealizationException(Exception):
+    """ This exception indicates there was a problem while
+    realizing effective repositories for a shed command. As a
+    precondition - the user has already been informed with error().
+    """
+
+__all__ = [
+    'for_each_repository',
+    'api_exception_to_message',
+    'tool_shed_client',
+    'diff',
+    'download_tarball',
+    'shed_init',
+    'CURRENT_CATEGORIES',
+    'path_to_repo_name',
+    'REPO_TYPE_UNRESTRICTED',
+    'REPO_TYPE_TOOL_DEP',
+    'REPO_TYPE_SUITE',
+]
```

### Comparing `planemo-0.8.4/planemo/io.py` & `planemo-0.9.0/planemo/io.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 from __future__ import print_function
+import contextlib
 import os
+import shutil
 import sys
+import tempfile
 
 import click
 from galaxy.tools.deps import commands
 from galaxy.tools.deps.commands import which
 
 
+def communicate(cmds, **kwds):
+    info(cmds)
+    p = commands.shell_process(cmds, **kwds)
+    ret_val = p.communicate()
+    if p.returncode != 0:
+        template = "Problem executing commands {0} - ({1}, {2})"
+        msg = template.format(cmds, ret_val[0], ret_val[1])
+        raise RuntimeError(msg)
+    return ret_val
+
+
 def shell(cmds, **kwds):
     info(cmds)
     return commands.shell(cmds, **kwds)
 
 
 def info(message, *args):
     if args:
@@ -40,21 +54,35 @@
 def _echo(message, err=False):
     if sys.version_info[0] == 2:
         click.echo(message, err=err)
     else:
         print(message)
 
 
+def write_file(path, content):
+    with open(path, "w") as f:
+        f.write(content)
+
+
 def untar_to(url, path, tar_args):
     if which("wget"):
         download_cmd = "wget -q --recursive -O - '%s'"
     else:
         download_cmd = "curl '%s'"
     download_cmd = download_cmd % url
     if tar_args:
         if not os.path.exists(path):
             os.makedirs(path)
 
         untar_cmd = "tar %s" % tar_args
         shell("%s | %s" % (download_cmd, untar_cmd))
     else:
         shell("%s > '%s'" % (download_cmd, path))
+
+
+@contextlib.contextmanager
+def temp_directory(prefix="planemo_tmp_"):
+    temp_dir = tempfile.mkdtemp(prefix=prefix)
+    try:
+        yield temp_dir
+    finally:
+        shutil.rmtree(temp_dir)
```

### Comparing `planemo-0.8.4/planemo/galaxy_config.py` & `planemo-0.9.0/planemo/galaxy_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from six.moves.urllib.request import urlretrieve
 
 import click
 
 from planemo import galaxy_run
 from planemo.io import warn
 from planemo.io import shell
+from planemo import git
 
 NO_TEST_DATA_MESSAGE = (
     "planemo couldn't find a target test-data directory, you should likely "
     "create a test-data directory or pass an explicit path using --test_data."
 )
 
 WEB_SERVER_CONFIG_TEMPLATE = """
@@ -327,15 +328,15 @@
     _install_with_command(config_directory, command)
 
 
 def _install_galaxy_via_git(ctx, config_directory, kwds):
     _ensure_galaxy_repository_available(ctx)
     workspace = ctx.workspace
     gx_repo = os.path.join(workspace, "gx_repo")
-    command = "git clone %s galaxy-dev" % (gx_repo)
+    command = git.command_clone(ctx, gx_repo, "galaxy-dev")
     _install_with_command(config_directory, command)
 
 
 def _install_with_command(config_directory, command):
     install_cmds = [
         "cd %s" % config_directory,
         command,
@@ -350,15 +351,16 @@
     workspace = ctx.workspace
     gx_repo = os.path.join(workspace, "gx_repo")
     if os.path.exists(gx_repo):
         # Attempt fetch - but don't fail if not interweb, etc...
         shell("git --git-dir %s fetch >/dev/null 2>&1" % gx_repo)
     else:
         remote_repo = "https://github.com/galaxyproject/galaxy"
-        shell("git clone --bare %s %s" % (remote_repo, gx_repo))
+        command = git.command_clone(ctx, remote_repo, gx_repo, bare=True)
+        shell(command)
 
 
 def _build_env_for_galaxy(properties, template_args):
     env = {}
     for key, value in iteritems(properties):
         var = "GALAXY_CONFIG_OVERRIDE_%s" % key.upper()
         value = _sub(value, template_args)
```

### Comparing `planemo-0.8.4/planemo/galaxy_run.py` & `planemo-0.9.0/planemo/galaxy_run.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/galaxy_test.py` & `planemo-0.9.0/planemo/galaxy_test.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/cli.py` & `planemo-0.9.0/planemo/cli.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/planemo/tool_builder.py` & `planemo-0.9.0/planemo/tool_builder.py`

 * *Files identical despite different names*

### Comparing `planemo-0.8.4/CONTRIBUTING.rst` & `planemo-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

