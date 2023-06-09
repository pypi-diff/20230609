# Comparing `tmp/slpkg-4.8.8.tar.gz` & `tmp/slpkg-4.8.9.tar.gz`

## Comparing `slpkg-4.8.8.tar` & `slpkg-4.8.9.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:40:58.000000 slpkg-4.8.8/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/filelists/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/filelists/multilib/
--rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-06-02 14:31:34.000000 slpkg-4.8.8/filelists/multilib/README.ERIC
--rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-06-02 14:31:34.000000 slpkg-4.8.8/filelists/multilib/glibc_packages.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-06-02 14:31:34.000000 slpkg-4.8.8/filelists/multilib/README
--rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-06-02 14:31:34.000000 slpkg-4.8.8/filelists/multilib/compat32.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-06-02 14:31:34.000000 slpkg-4.8.8/filelists/README
--rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-06-02 14:31:34.000000 slpkg-4.8.8/repositories.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slackbuild/
--rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-06-02 14:31:34.000000 slpkg-4.8.8/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      334 2023-06-02 14:31:34.000000 slpkg-4.8.8/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-06-02 14:31:34.000000 slpkg-4.8.8/slackbuild/README
--rwxr-xr-x   0 dslackw   (1000) users      (100)     4112 2023-06-02 14:31:34.000000 slpkg-4.8.8/slackbuild/slpkg.SlackBuild
--rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-06-02 14:31:34.000000 slpkg-4.8.8/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1520 2023-06-02 14:31:34.000000 slpkg-4.8.8/.pyproject.toml
--rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-06-02 14:31:34.000000 slpkg-4.8.8/requirements.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/configs/
--rw-r--r--   0 dslackw   (1000) users      (100)     8802 2023-06-02 14:31:34.000000 slpkg-4.8.8/configs/repositories.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-06-02 14:31:34.000000 slpkg-4.8.8/configs/blacklist.toml
--rw-r--r--   0 dslackw   (1000) users      (100)     4129 2023-06-02 14:31:34.000000 slpkg-4.8.8/configs/slpkg.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      381 2023-06-02 14:31:34.000000 slpkg-4.8.8/configs/rules.toml
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/
--rw-r--r--   0 dslackw   (1000) users      (100)     2337 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      765 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1961 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1565 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_sbo_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)      256 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_colors.py
--rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/check_updates_test.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1460 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1716 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_bin_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-06-02 14:31:34.000000 slpkg-4.8.8/LICENSE
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1624 2023-06-02 14:31:34.000000 slpkg-4.8.8/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)    47093 2023-06-02 14:31:34.000000 slpkg-4.8.8/ChangeLog.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/man/
--rw-r--r--   0 dslackw   (1000) users      (100)     9677 2023-06-02 14:31:34.000000 slpkg-4.8.8/man/slpkg.1
--rw-r--r--   0 dslackw   (1000) users      (100)    10867 2023-06-02 14:31:34.000000 slpkg-4.8.8/man/slpkg-fr.1
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/completion/
--rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-06-02 14:31:34.000000 slpkg-4.8.8/completion/slpkg
--rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-06-02 14:31:34.000000 slpkg-4.8.8/.gitignore
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/
--rw-r--r--   0 dslackw   (1000) users      (100)     4289 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/dialog_configs.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/binaries/
--rw-r--r--   0 dslackw   (1000) users      (100)     1892 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/binaries/required.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1439 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/binaries/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/binaries/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7698 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/binaries/install.py
--rw-r--r--   0 dslackw   (1000) users      (100)    65384 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/install_data.py
--rw-r--r--   0 dslackw   (1000) users      (100)    31419 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/repositories.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4367 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/repo_info.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/sbos/
--rw-r--r--   0 dslackw   (1000) users      (100)     1605 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/sbos/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)    11675 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/sbos/slackbuild.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1151 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/sbos/dependencies.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/sbos/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4483 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/sbos/sbo_generate.py
--rw-r--r--   0 dslackw   (1000) users      (100)    36699 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/update_repository.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2627 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/progress_bar.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3510 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/downloader.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/models/
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/models/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2655 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/models/models.py
--rw-r--r--   0 dslackw   (1000) users      (100)      887 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/rules.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/
--rw-r--r--   0 dslackw   (1000) users      (100)     6604 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/view_package.py
--rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/version.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6335 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/cli_menu.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5935 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/asciibox.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4110 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/help_commands.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)    10274 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/views.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4004 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/choose_packages.py
--rw-r--r--   0 dslackw   (1000) users      (100)      430 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/error_messages.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3637 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1350 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/logging_deps.py
--rw-r--r--   0 dslackw   (1000) users      (100)    13634 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/new_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2058 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/multi_process.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3211 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/cleanings.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1881 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/checksum.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1906 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/dialog_box.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4812 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7857 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3867 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/dependees.py
--rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/toml_error_message.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6100 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/check_updates.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6716 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/remove_packages.py
--rw-r--r--   0 dslackw   (1000) users      (100)      916 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3491 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/download_only.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4147 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/tracking.py
--rw-r--r--   0 dslackw   (1000) users      (100)      514 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/logging_config.py
--rw-r--r--   0 dslackw   (1000) users      (100)    29920 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/main.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1609 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/find_installed.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4041 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3428 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/search.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1466 2023-06-02 14:31:34.000000 slpkg-4.8.8/setup.cfg
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:40:55.000000 slpkg-4.8.8/slpkg.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)       86 2023-06-02 14:40:55.000000 slpkg-4.8.8/slpkg.egg-info/entry_points.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-06-02 14:40:55.000000 slpkg-4.8.8/slpkg.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1326 2023-06-02 14:40:55.000000 slpkg-4.8.8/slpkg.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-06-02 14:40:55.000000 slpkg-4.8.8/slpkg.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-06-02 14:40:55.000000 slpkg-4.8.8/slpkg.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1257 2023-06-02 14:40:55.000000 slpkg-4.8.8/slpkg.egg-info/PKG-INFO
--rw-r--r--   0 dslackw   (1000) users      (100)     8595 2023-06-02 14:31:34.000000 slpkg-4.8.8/README.md
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/tools/
--rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-06-02 14:31:34.000000 slpkg-4.8.8/tools/gen_sbo_txt.sh
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:23:14.000000 slpkg-4.8.9/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/filelists/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/filelists/multilib/
+-rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-06-09 14:19:35.000000 slpkg-4.8.9/filelists/multilib/README.ERIC
+-rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-06-09 14:19:35.000000 slpkg-4.8.9/filelists/multilib/glibc_packages.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-06-09 14:19:35.000000 slpkg-4.8.9/filelists/multilib/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-06-09 14:19:35.000000 slpkg-4.8.9/filelists/multilib/compat32.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-06-09 14:19:35.000000 slpkg-4.8.9/filelists/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-06-09 14:19:35.000000 slpkg-4.8.9/repositories.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slackbuild/
+-rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-06-09 14:19:35.000000 slpkg-4.8.9/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      334 2023-06-09 14:19:35.000000 slpkg-4.8.9/slackbuild/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-06-09 14:19:35.000000 slpkg-4.8.9/slackbuild/README
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     4114 2023-06-09 14:19:35.000000 slpkg-4.8.9/slackbuild/slpkg.SlackBuild
+-rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-06-09 14:19:35.000000 slpkg-4.8.9/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1520 2023-06-09 14:19:35.000000 slpkg-4.8.9/.pyproject.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-06-09 14:19:35.000000 slpkg-4.8.9/requirements.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/configs/
+-rw-r--r--   0 dslackw   (1000) users      (100)     8802 2023-06-09 14:19:35.000000 slpkg-4.8.9/configs/repositories.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-06-09 14:19:35.000000 slpkg-4.8.9/configs/blacklist.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)     4129 2023-06-09 14:19:35.000000 slpkg-4.8.9/configs/slpkg.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      381 2023-06-09 14:19:35.000000 slpkg-4.8.9/configs/rules.toml
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/
+-rw-r--r--   0 dslackw   (1000) users      (100)     2337 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      765 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1961 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1565 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_sbo_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      256 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_colors.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/check_updates_test.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1460 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1716 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_bin_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-06-09 14:19:35.000000 slpkg-4.8.9/LICENSE
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1624 2023-06-09 14:19:35.000000 slpkg-4.8.9/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)    47184 2023-06-09 14:19:35.000000 slpkg-4.8.9/ChangeLog.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/man/
+-rw-r--r--   0 dslackw   (1000) users      (100)     9677 2023-06-09 14:19:35.000000 slpkg-4.8.9/man/slpkg.1
+-rw-r--r--   0 dslackw   (1000) users      (100)    10865 2023-06-09 14:19:35.000000 slpkg-4.8.9/man/slpkg-fr.1
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/completion/
+-rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-06-09 14:19:35.000000 slpkg-4.8.9/completion/slpkg
+-rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-06-09 14:19:35.000000 slpkg-4.8.9/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/
+-rw-r--r--   0 dslackw   (1000) users      (100)     4289 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/dialog_configs.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/binaries/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1892 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/binaries/required.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1439 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/binaries/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/binaries/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7698 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/binaries/install.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    65384 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/install_data.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    31419 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/repositories.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4367 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/repo_info.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/sbos/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1605 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/sbos/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    11675 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/sbos/slackbuild.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1151 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/sbos/dependencies.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/sbos/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4483 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/sbos/sbo_generate.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    36699 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/update_repository.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2627 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/progress_bar.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3510 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/downloader.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/models/
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/models/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2655 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/models/models.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      887 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/rules.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/
+-rw-r--r--   0 dslackw   (1000) users      (100)     6604 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/view_package.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/version.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6335 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/cli_menu.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5935 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/asciibox.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4110 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/help_commands.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    10274 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/views.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4004 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/choose_packages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      430 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/error_messages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3637 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1350 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/logging_deps.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    13634 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/new_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2058 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/multi_process.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3211 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/cleanings.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1881 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/checksum.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1906 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/dialog_box.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4812 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7857 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3867 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/dependees.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/toml_error_message.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6348 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/check_updates.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6716 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/remove_packages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      916 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3491 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/download_only.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4147 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/tracking.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      514 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/logging_config.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    29920 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/main.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1609 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/find_installed.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4041 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3428 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/search.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1466 2023-06-09 14:19:35.000000 slpkg-4.8.9/setup.cfg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:23:11.000000 slpkg-4.8.9/slpkg.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)       86 2023-06-09 14:23:11.000000 slpkg-4.8.9/slpkg.egg-info/entry_points.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-06-09 14:23:11.000000 slpkg-4.8.9/slpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1326 2023-06-09 14:23:11.000000 slpkg-4.8.9/slpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-06-09 14:23:11.000000 slpkg-4.8.9/slpkg.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-06-09 14:23:11.000000 slpkg-4.8.9/slpkg.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1257 2023-06-09 14:23:11.000000 slpkg-4.8.9/slpkg.egg-info/PKG-INFO
+-rw-r--r--   0 dslackw   (1000) users      (100)     8595 2023-06-09 14:19:35.000000 slpkg-4.8.9/README.md
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/tools/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-06-09 14:19:35.000000 slpkg-4.8.9/tools/gen_sbo_txt.sh
```

### Comparing `slpkg-4.8.8/filelists/multilib/README.ERIC` & `slpkg-4.8.9/filelists/multilib/README.ERIC`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/filelists/multilib/README` & `slpkg-4.8.9/filelists/multilib/README`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/filelists/multilib/compat32.pkgs` & `slpkg-4.8.9/filelists/multilib/compat32.pkgs`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/repositories.txt` & `slpkg-4.8.9/repositories.txt`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slackbuild/slack-desc` & `slpkg-4.8.9/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slackbuild/slpkg.SlackBuild` & `slpkg-4.8.9/slackbuild/slpkg.SlackBuild`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # Grab version from __metadata_.py file
 cat ../setup.cfg | grep "version =" | tr -d "[:space:]" | cut -c9-13 | tr , .
 }
 
 cd $(dirname $0) ; CWD=$(pwd)
 
 PRGNAM=slpkg
-VERSION=${VERSION:-$(__version)} 
+VERSION=${VERSION:-$(__version)}
 BUILD=${BUILD:-1}
 TAG=${TAG:-_dsw}
 PKGTYPE=${PKGTYPE:-txz}
 INSTALL="upgradepkg --install-new"
 
 if [ -z "$ARCH" ]; then
   case "$( uname -m )" in
@@ -72,15 +72,16 @@
 
 set -e
 
 rm -rf $PKG
 mkdir -p $TMP $PKG $OUTPUT
 cd $TMP
 rm -rf $PRGNAM-$VERSION
-tar xvf $CWD/$PRGNAM-$VERSION.tar.gz || tar xvf $CWD/$PRGNAM-$VERSION.tar.bz2 || unzip $CWD/$PRGNAM-$VERSION.zip
+tar xvf $CWD/$PRGNAM-$VERSION.tar.gz || tar xvf $CWD/$PRGNAM-$VERSION.tar.bz2 \
+	|| unzip $CWD/$PRGNAM-$VERSION.zip
 cd $PRGNAM-$VERSION
 chown -R root:root .
 find -L . \
  \( -perm 777 -o -perm 775 -o -perm 750 -o -perm 711 -o -perm 555 \
   -o -perm 511 \) -exec chmod 755 {} \; -o \
  \( -perm 666 -o -perm 664 -o -perm 640 -o -perm 600 -o -perm 444 \
   -o -perm 440 -o -perm 400 \) -exec chmod 644 {} \;
```

### Comparing `slpkg-4.8.8/.pyproject.toml` & `slpkg-4.8.9/.pyproject.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/configs/repositories.toml` & `slpkg-4.8.9/configs/repositories.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/configs/slpkg.toml` & `slpkg-4.8.9/configs/slpkg.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/tests/test_configs.py` & `slpkg-4.8.9/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/tests/test_checks.py` & `slpkg-4.8.9/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/tests/test_utilities.py` & `slpkg-4.8.9/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/tests/test_sbo_queries.py` & `slpkg-4.8.9/tests/test_sbo_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/tests/test_colors.py` & `slpkg-4.8.9/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/tests/check_updates_test.py` & `slpkg-4.8.9/tests/check_updates_test.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/tests/test_upgrade.py` & `slpkg-4.8.9/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/tests/test_bin_queries.py` & `slpkg-4.8.9/tests/test_bin_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/LICENSE` & `slpkg-4.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/install.sh` & `slpkg-4.8.9/install.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/ChangeLog.txt` & `slpkg-4.8.9/ChangeLog.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+4.8.9 - 06/06/2023
+Fixed
+- urllib3.exceptions.NewConnectionError (Thanks to rizitis) #173
+
 4.8.8 - 29/05/2023
 Updated:
 - France manpage
 Fixed:
 - Choose dependencies for upgraded packages
 - Build packages with the same source name:
   (nvidia-driver and nvidia-kernel use the same source NVIDIA-Linux-x86_64-<VERSION>.run)
```

### Comparing `slpkg-4.8.8/man/slpkg.1` & `slpkg-4.8.9/man/slpkg.1`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/man/slpkg-fr.1` & `slpkg-4.8.9/man/slpkg-fr.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH slpkg 1 "Orestiada, Grèce" "slpkg 4.8.5" dslackw
+.TH slpkg 1 "Orestiada, Hellas" "slpkg 4.8.5" dslackw
 .SH NOM
 .P
 slpkg \- Utilitaire de gestion de paquets pour Slackware.
 .SH SYNOPSIS
 .P
 slpkg \c
 [\fICOMMAND\fR] [\fIOPTIONS\fR] [\fIFILELIST|PACKAGES...\fR]
@@ -168,15 +168,15 @@
 .RE
 .P
 .B -p, --pkg-version
 .RS
 Affiche la version du paquetage du référentiel. (à utiliser avec : -e, dependees, -t, tracking, -w, view)
 .RE
 .P
-.B -P, --parallèle
+.B -P, --parallel
 .RS
 Télécharger des fichiers en parallèle pour accélérer le processus.
 (à utiliser avec : -u, update, -U, upgrade, -b, build, -i, install, -d, download)
 .RE
 .P
 .B -m, --no-case
 .RS
```

### Comparing `slpkg-4.8.8/completion/slpkg` & `slpkg-4.8.9/completion/slpkg`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/dialog_configs.py` & `slpkg-4.8.9/slpkg/dialog_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/binaries/required.py` & `slpkg-4.8.9/slpkg/binaries/required.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/binaries/queries.py` & `slpkg-4.8.9/slpkg/binaries/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/binaries/install.py` & `slpkg-4.8.9/slpkg/binaries/install.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/install_data.py` & `slpkg-4.8.9/slpkg/install_data.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/repositories.py` & `slpkg-4.8.9/slpkg/repositories.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/repo_info.py` & `slpkg-4.8.9/slpkg/repo_info.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/sbos/queries.py` & `slpkg-4.8.9/slpkg/sbos/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/sbos/slackbuild.py` & `slpkg-4.8.9/slpkg/sbos/slackbuild.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/sbos/dependencies.py` & `slpkg-4.8.9/slpkg/sbos/dependencies.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/sbos/sbo_generate.py` & `slpkg-4.8.9/slpkg/sbos/sbo_generate.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/update_repository.py` & `slpkg-4.8.9/slpkg/update_repository.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/progress_bar.py` & `slpkg-4.8.9/slpkg/progress_bar.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/downloader.py` & `slpkg-4.8.9/slpkg/downloader.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/models/models.py` & `slpkg-4.8.9/slpkg/models/models.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/rules.py` & `slpkg-4.8.9/slpkg/rules.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/views/view_package.py` & `slpkg-4.8.9/slpkg/views/view_package.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/views/version.py` & `slpkg-4.8.9/slpkg/views/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (4, 8, 8)
+        self.version_info: tuple = (4, 8, 9)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'MIT License'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
 
     def view(self) -> None:
         """ Prints the version. """
```

### Comparing `slpkg-4.8.8/slpkg/views/cli_menu.py` & `slpkg-4.8.9/slpkg/views/cli_menu.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/views/asciibox.py` & `slpkg-4.8.9/slpkg/views/asciibox.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/views/help_commands.py` & `slpkg-4.8.9/slpkg/views/help_commands.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/views/views.py` & `slpkg-4.8.9/slpkg/views/views.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/choose_packages.py` & `slpkg-4.8.9/slpkg/choose_packages.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/checks.py` & `slpkg-4.8.9/slpkg/checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/logging_deps.py` & `slpkg-4.8.9/slpkg/logging_deps.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/new_configs.py` & `slpkg-4.8.9/slpkg/new_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/multi_process.py` & `slpkg-4.8.9/slpkg/multi_process.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/cleanings.py` & `slpkg-4.8.9/slpkg/cleanings.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/checksum.py` & `slpkg-4.8.9/slpkg/checksum.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/dialog_box.py` & `slpkg-4.8.9/slpkg/dialog_box.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/configs.py` & `slpkg-4.8.9/slpkg/configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/utilities.py` & `slpkg-4.8.9/slpkg/utilities.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/dependees.py` & `slpkg-4.8.9/slpkg/dependees.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/toml_error_message.py` & `slpkg-4.8.9/slpkg/toml_error_message.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/check_updates.py` & `slpkg-4.8.9/slpkg/check_updates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import os
 import logging
 from pathlib import Path
 from multiprocessing import Process
+from urllib3.exceptions import HTTPError
 from urllib3 import PoolManager, ProxyManager, make_headers
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.progress_bar import ProgressBar
 from slpkg.repositories import Repositories
 from slpkg.logging_config import LoggingConfig
@@ -86,29 +87,34 @@
     def ponce_repository(self) -> None:
         local_chg_txt: Path = Path(self.repos.ponce_repo_path, self.repos.ponce_repo_changelog)
         repo_chg_txt: str = f'{self.repos.ponce_repo_mirror[0]}{self.repos.ponce_repo_changelog}'
         self.compare[self.repos.ponce_repo_name] = self.compare_the_changelogs(local_chg_txt, repo_chg_txt)
 
     def compare_the_changelogs(self, local_chg_txt: Path, repo_chg_txt: str) -> bool:
         local_size: int = 0
+        repo_size: int = 0
 
         if self.proxy_address.startswith('http'):
             self.set_http_proxy_server()
 
         if self.proxy_address.startswith('socks'):
             self.set_socks_proxy_server()
 
         try:
             repo = self.http.request('GET', repo_chg_txt)
-            if local_chg_txt.is_file():
-                local_size: int = int(os.stat(local_chg_txt).st_size)
         except KeyboardInterrupt:
             raise SystemExit(1)
+        except HTTPError:
+            print(f'\n\n{self.endc}{self.prog_name}: {self.bred}Error:{self.endc} '
+                  f'Failed to connect to {repo_chg_txt}\n')
+        else:
+            repo_size: int = int(repo.headers['Content-Length'])
 
-        repo_size: int = int(repo.headers['Content-Length'])
+        if local_chg_txt.is_file():
+            local_size: int = int(os.stat(local_chg_txt).st_size)
 
         logger = logging.getLogger(LoggingConfig.date_time)
         logger.info(f'{self.__class__.__name__}: '
                     f'{self.__class__.compare_the_changelogs.__name__}: '
                     f'{local_chg_txt=}, {local_size=}, '
                     f'{repo_chg_txt=}, {repo_size=}, '
                     f'{local_size != repo_size}')
```

### Comparing `slpkg-4.8.8/slpkg/remove_packages.py` & `slpkg-4.8.9/slpkg/remove_packages.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/blacklist.py` & `slpkg-4.8.9/slpkg/blacklist.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/download_only.py` & `slpkg-4.8.9/slpkg/download_only.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/tracking.py` & `slpkg-4.8.9/slpkg/tracking.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/logging_config.py` & `slpkg-4.8.9/slpkg/logging_config.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/main.py` & `slpkg-4.8.9/slpkg/main.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/find_installed.py` & `slpkg-4.8.9/slpkg/find_installed.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/upgrade.py` & `slpkg-4.8.9/slpkg/upgrade.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg/search.py` & `slpkg-4.8.9/slpkg/search.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/setup.cfg` & `slpkg-4.8.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = slpkg
-version = 4.8.8
+version = 4.8.9
 license_file = LICENSE
 author = Dimitris Zlatanidis
 author_email = dslackw@gmail.com
 description = Package manager utility for Slackware Linux.
 long_description = file:README.rst
 url = https://dslackw.gitlab.io/slpkg/
 project_urls =
```

### Comparing `slpkg-4.8.8/slpkg.egg-info/SOURCES.txt` & `slpkg-4.8.9/slpkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.8/slpkg.egg-info/PKG-INFO` & `slpkg-4.8.9/slpkg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 4.8.8
+Version: 4.8.9
 Summary: Package manager utility for Slackware Linux.
 Home-page: https://dslackw.gitlab.io/slpkg/
 Author: Dimitris Zlatanidis
 Author-email: dslackw@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://dslackw.gitlab.io/slpkg/
 Project-URL: Documentation, https://dslackw.gitlab.io/slpkg/
```

### Comparing `slpkg-4.8.8/README.md` & `slpkg-4.8.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 $ slpkg tracking --pkg-version Flask awscli pychess
 ```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_tracking.png" width="900">
 
 ### Installation
 
 ```
-$ tar xvf slpkg-4.8.8.tar.gz
-$ cd slpkg-4.8.8
+$ tar xvf slpkg-4.8.9.tar.gz
+$ cd slpkg-4.8.9
 $ ./install.sh
 ```
 
 ### Requirements
 
 ```
 SQLAlchemy >= 1.4.46
@@ -82,15 +82,15 @@
 
 The majority of trials have been made in Slackware x86_64 'stable' environment.
 
 
 ### Command Line Tool Usage
 
 ```
-slpkg - version 4.8.8
+slpkg - version 4.8.9
 
 USAGE:
   slpkg [COMMAND] [OPTIONS] [FILELIST|PACKAGES...]
 
 DESCRIPTION:
   Package manager utility for Slackware.
```

### Comparing `slpkg-4.8.8/tools/gen_sbo_txt.sh` & `slpkg-4.8.9/tools/gen_sbo_txt.sh`

 * *Files identical despite different names*

