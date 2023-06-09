# Comparing `tmp/machineconfig-1.4.tar.gz` & `tmp/machineconfig-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineconfig-1.4.tar", last modified: Sat Apr  1 06:43:05 2023, max compression
+gzip compressed data, was "machineconfig-1.5.tar", last modified: Fri Jun  9 00:20:22 2023, max compression
```

## Comparing `machineconfig-1.4.tar` & `machineconfig-1.5.tar`

### file list

```diff
@@ -1,399 +1,408 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.275316 machineconfig-1.4/
--rw-rw-rw-   0        0        0      232 2023-03-04 22:55:51.000000 machineconfig-1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5289 2023-04-01 06:43:05.275316 machineconfig-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4775 2023-04-01 05:32:36.000000 machineconfig-1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-01 06:43:05.275316 machineconfig-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1016 2023-03-05 00:54:04.000000 machineconfig-1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.911539 machineconfig-1.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.938049 machineconfig-1.4/src/machineconfig/
--rw-rw-rw-   0        0        0      121 2023-04-01 05:54:45.000000 machineconfig-1.4/src/machineconfig/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.945091 machineconfig-1.4/src/machineconfig/jobs/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.945091 machineconfig-1.4/src/machineconfig/jobs/__pycache__/
--rw-rw-rw-   0        0        0      158 2023-03-05 00:35:45.000000 machineconfig-1.4/src/machineconfig/jobs/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.912888 machineconfig-1.4/src/machineconfig/jobs/linux/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.955926 machineconfig-1.4/src/machineconfig/jobs/linux/archive/
--rw-rw-rw-   0        0        0      519 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/jobs/linux/archive/get_latest_release.sh
--rw-rw-rw-   0        0        0      670 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/linux/archive/install_bandwich.sh
--rw-rw-rw-   0        0        0      687 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/linux/archive/install_diskonaut.sh
--rw-rw-rw-   0        0        0      352 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/linux/archive/install_kondo.sh
--rw-rw-rw-   0        0        0      662 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/linux/archive/install_nu.sh
--rw-rw-rw-   0        0        0      606 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/linux/archive/install_zellij.sh
--rw-rw-rw-   0        0        0      654 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/jobs/linux/archive/lf.sh
--rw-rw-rw-   0        0        0     1335 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/jobs/linux/archive/quirks.sh
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.964934 machineconfig-1.4/src/machineconfig/jobs/python/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.970399 machineconfig-1.4/src/machineconfig/jobs/python/__pycache__/
--rw-rw-rw-   0        0        0      165 2023-03-05 00:35:45.000000 machineconfig-1.4/src/machineconfig/jobs/python/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     3752 2023-03-30 04:11:37.000000 machineconfig-1.4/src/machineconfig/jobs/python/__pycache__/python_linux_installers_all.cpython-39.pyc
--rw-rw-rw-   0        0        0      679 2023-03-13 07:34:55.000000 machineconfig-1.4/src/machineconfig/jobs/python/__pycache__/python_ve_symlink.cpython-39.pyc
--rw-rw-rw-   0        0        0     1200 2023-03-28 23:28:03.000000 machineconfig-1.4/src/machineconfig/jobs/python/__pycache__/python_windows_installers_all.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.970399 machineconfig-1.4/src/machineconfig/jobs/python/archive/
--rw-rw-rw-   0        0        0      258 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python/archive/python_tools.txt
--rw-rw-rw-   0        0        0     7357 2023-03-05 03:20:36.000000 machineconfig-1.4/src/machineconfig/jobs/python/check_installations.py
--rw-rw-rw-   0        0        0      625 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python/create_bootable_media.py
--rw-rw-rw-   0        0        0     1742 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python/python_cargo_build_share.py
--rw-rw-rw-   0        0        0     3303 2023-03-29 00:59:04.000000 machineconfig-1.4/src/machineconfig/jobs/python/python_linux_installers_all.py
--rw-rw-rw-   0        0        0     2820 2023-03-31 01:04:52.000000 machineconfig-1.4/src/machineconfig/jobs/python/python_ve_installer.py
--rw-rw-rw-   0        0        0      872 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python/python_ve_symlink.py
--rw-rw-rw-   0        0        0      789 2023-03-28 23:12:01.000000 machineconfig-1.4/src/machineconfig/jobs/python/python_windows_installers_all.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.989737 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.991354 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/__pycache__/
--rw-rw-rw-   0        0        0      184 2023-03-05 00:35:45.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.995621 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/archive/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/archive/__init__.py
--rw-rw-rw-   0        0        0      490 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/archive/nvim.py
--rw-rw-rw-   0        0        0     1024 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/archive/strongbox.py
--rw-rw-rw-   0        0        0      720 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/archive/vtm.py
--rw-rw-rw-   0        0        0     1230 2023-03-28 22:15:27.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/broot.py
--rw-rw-rw-   0        0        0      939 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/cpufetch.py
--rw-rw-rw-   0        0        0     1940 2023-03-28 22:15:27.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/delta.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.009374 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/
--rw-rw-rw-   0        0        0        0 2023-03-27 21:24:54.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/__init__.py
--rw-rw-rw-   0        0        0      960 2023-03-28 22:16:59.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/bw.py
--rw-rw-rw-   0        0        0      722 2023-03-30 04:14:00.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/evcxr.py
--rw-rw-rw-   0        0        0      802 2023-03-28 22:20:23.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/kondo.py
--rw-rw-rw-   0        0        0     1900 2023-03-28 23:27:59.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/lvim.py
--rw-rw-rw-   0        0        0      462 2023-04-01 03:13:32.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/opencommit.py
--rw-rw-rw-   0        0        0     1119 2023-03-28 23:27:59.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/qrcp.py
--rw-rw-rw-   0        0        0      760 2023-03-28 23:27:59.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/qrscan.py
--rw-rw-rw-   0        0        0     1016 2023-03-28 23:27:59.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/rust-analyzer.py
--rw-rw-rw-   0        0        0      746 2023-03-28 23:27:59.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/termscp.py
--rw-rw-rw-   0        0        0      969 2023-03-28 23:27:59.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/tldr.py
--rw-rw-rw-   0        0        0      984 2023-03-28 23:27:59.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/tokei.py
--rw-rw-rw-   0        0        0      946 2023-03-28 22:12:20.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/diskonaut.py
--rw-rw-rw-   0        0        0      747 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dua.py
--rw-rw-rw-   0        0        0      893 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/gitui.py
--rw-rw-rw-   0        0        0      745 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/gopass.py
--rw-rw-rw-   0        0        0     1946 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/helix.py
--rw-rw-rw-   0        0        0     1027 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/lf.py
--rw-rw-rw-   0        0        0      664 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/mprocs.py
--rw-rw-rw-   0        0        0      690 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/navi.py
--rw-rw-rw-   0        0        0     1205 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/ots.py
--rw-rw-rw-   0        0        0      965 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/ouch.py
--rw-rw-rw-   0        0        0      757 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/pomodoro.py
--rw-rw-rw-   0        0        0      701 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/procs.py
--rw-rw-rw-   0        0        0      689 2023-03-28 22:16:59.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/rclone.py
--rw-rw-rw-   0        0        0     1143 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/tere.py
--rw-rw-rw-   0        0        0      712 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/watchexec.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.023501 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.023501 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/__pycache__/
--rw-rw-rw-   0        0        0      182 2023-03-05 00:35:45.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.025603 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/archive/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/archive/__init__.py
--rw-rw-rw-   0        0        0      548 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/archive/ranger.py
--rw-rw-rw-   0        0        0      626 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/bottom.py
--rw-rw-rw-   0        0        0      582 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/btop.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.031207 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/dev/
--rw-rw-rw-   0        0        0        0 2023-03-27 21:24:54.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/dev/__init__.py
--rw-rw-rw-   0        0        0      207 2023-03-28 23:27:59.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/dev/bandwhich.py
--rw-rw-rw-   0        0        0      680 2023-03-28 23:27:59.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/dev/bytehound.py
--rw-rw-rw-   0        0        0      569 2023-03-28 23:27:59.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/dev/nnn.py
--rw-rw-rw-   0        0        0      497 2023-03-29 01:53:24.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/gotty.py
--rw-rw-rw-   0        0        0     1139 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/joshuto.py
--rw-rw-rw-   0        0        0      402 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/mcfly.py
--rw-rw-rw-   0        0        0      508 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/skim.py
--rw-rw-rw-   0        0        0      511 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/topgrade.py
--rw-rw-rw-   0        0        0      642 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/viu.py
--rw-rw-rw-   0        0        0      759 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/xplr.py
--rw-rw-rw-   0        0        0     1145 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/zellij.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.042006 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.042512 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/__pycache__/
--rw-rw-rw-   0        0        0      184 2023-03-05 00:35:45.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.046067 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/archive/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/archive/__init__.py
--rw-rw-rw-   0        0        0      425 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/archive/ntop.py
--rw-rw-rw-   0        0        0       66 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/archive/readme.md
--rw-rw-rw-   0        0        0      356 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/bat.py
--rw-rw-rw-   0        0        0      789 2023-03-28 22:15:27.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/boxes.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.050332 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/dev/
--rw-rw-rw-   0        0        0        0 2023-03-27 21:24:54.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/dev/__init__.py
--rw-rw-rw-   0        0        0      560 2023-03-28 23:27:59.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/dev/bypass_paywall.py
--rw-rw-rw-   0        0        0      790 2023-03-28 23:27:59.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/dev/obs_background_removal_plugin.py
--rw-rw-rw-   0        0        0      514 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/fd.py
--rw-rw-rw-   0        0        0      715 2023-03-28 22:15:27.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/fzf.py
--rw-rw-rw-   0        0        0      438 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/rg.py
--rw-rw-rw-   0        0        0      422 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/ugrep.py
--rw-rw-rw-   0        0        0      624 2023-03-28 22:15:27.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/zoomit.py
--rw-rw-rw-   0        0        0      405 2023-03-28 21:18:51.000000 machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/zoxide.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.051762 machineconfig-1.4/src/machineconfig/jobs/windows/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.054948 machineconfig-1.4/src/machineconfig/jobs/windows/arhive/
--rw-rw-rw-   0        0        0      681 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/windows/arhive/archive_pygraphviz.ps1
--rw-rw-rw-   0        0        0      276 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/windows/arhive/openssh-server_add_key.ps1
--rw-rw-rw-   0        0        0      759 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/windows/arhive/openssh-server_copy-ssh-id.ps1
--rw-rw-rw-   0        0        0      477 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/windows/start_terminal.ps1
--rwxrwxrwx   0        0        0       97 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/jobs/windows/startup_file.cmd
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.057568 machineconfig-1.4/src/machineconfig/profile/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/profile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.060447 machineconfig-1.4/src/machineconfig/profile/__pycache__/
--rw-rw-rw-   0        0        0      161 2023-03-05 00:24:30.000000 machineconfig-1.4/src/machineconfig/profile/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     6546 2023-03-15 11:01:02.000000 machineconfig-1.4/src/machineconfig/profile/__pycache__/create.cpython-39.pyc
--rw-rw-rw-   0        0        0     9363 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/profile/create.py
--rw-rw-rw-   0        0        0      406 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/profile/fix_shell_profiles.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.919817 machineconfig-1.4/src/machineconfig/profile/patches/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.066415 machineconfig-1.4/src/machineconfig/profile/patches/linux/
--rw-rw-rw-   0        0        0       70 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/profile/patches/linux/mcfly.sh
--rw-rw-rw-   0        0        0       50 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/profile/patches/linux/xming.sh
--rw-rw-rw-   0        0        0       76 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/profile/patches/linux/zoxide.sh
--rw-rw-rw-   0        0        0      613 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/profile/patches/linux/zzellij.sh
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.067686 machineconfig-1.4/src/machineconfig/profile/patches/windows/
--rw-rw-rw-   0        0        0      241 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/profile/patches/windows/zoxide.ps1
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.921826 machineconfig-1.4/src/machineconfig/profile/records/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.067686 machineconfig-1.4/src/machineconfig/profile/records/generic/
--rw-rw-rw-   0        0        0      150 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/profile/records/generic/shares.toml
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.069638 machineconfig-1.4/src/machineconfig/profile/records/linux/
--rw-rw-rw-   0        0        0     1732 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/profile/records/linux/safe_cli_apps.json
--rw-rw-rw-   0        0        0       65 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/profile/records/linux/safe_cli_apps_url.txt
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.072541 machineconfig-1.4/src/machineconfig/profile/records/windows/
--rw-rw-rw-   0        0        0      423 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/profile/records/windows/safe_cli_apps.csv
--rw-rw-rw-   0        0        0     4597 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/profile/records/windows/safe_cli_apps.json
--rw-rw-rw-   0        0        0       65 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/profile/records/windows/safe_cli_apps_url.txt
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.074582 machineconfig-1.4/src/machineconfig/scripts/
--rw-rw-rw-   0        0        0       79 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.074582 machineconfig-1.4/src/machineconfig/scripts/__pycache__/
--rw-rw-rw-   0        0        0      231 2023-03-05 00:35:45.000000 machineconfig-1.4/src/machineconfig/scripts/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.101747 machineconfig-1.4/src/machineconfig/scripts/linux/
--rw-rw-rw-   0        0        0     1603 2023-04-01 05:50:14.000000 machineconfig-1.4/src/machineconfig/scripts/linux/activate_ve
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.105045 machineconfig-1.4/src/machineconfig/scripts/linux/archive/
--rw-rw-rw-   0        0        0     1137 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/archive/dotfiles_pull
--rw-rw-rw-   0        0        0     2559 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/archive/dotfiles_push
--rw-rw-rw-   0        0        0        0 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/archive/secure_pull
--rw-rw-rw-   0        0        0     2516 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/archive/secure_push
--rw-rw-rw-   0        0        0      183 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/choose_shell_theme
--rw-rw-rw-   0        0        0      557 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/cloud_mount
--rw-rw-rw-   0        0        0      135 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/cloud_repo_sync
--rw-rw-rw-   0        0        0      123 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/cloud_rx
--rw-rw-rw-   0        0        0      123 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/cloud_sx
--rw-rw-rw-   0        0        0      556 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/cloud_sync
--rw-rw-rw-   0        0        0      242 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/linux/croshell
--rw-rw-rw-   0        0        0      462 2023-03-17 01:03:26.000000 machineconfig-1.4/src/machineconfig/scripts/linux/devops
--rw-rw-rw-   0        0        0      783 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/fresh_lvim_installation
--rw-rw-rw-   0        0        0      125 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/linux/ftprx
--rw-rw-rw-   0        0        0      121 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/linux/ftpsx
--rw-rw-rw-   0        0        0      853 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/linux/fzf2g
--rw-rw-rw-   0        0        0      696 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/linux/fzfag
--rw-rw-rw-   0        0        0     1115 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/linux/fzffg
--rw-rw-rw-   0        0        0     1215 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/linux/fzfg
--rw-rw-rw-   0        0        0     2695 2023-04-01 06:30:24.000000 machineconfig-1.4/src/machineconfig/scripts/linux/mount_drive
--rw-rw-rw-   0        0        0     2341 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/mount_nfs
--rw-rw-rw-   0        0        0     2800 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/mount_nw_drive
--rw-rw-rw-   0        0        0      522 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/repos
--rw-rw-rw-   0        0        0      137 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/sk_rg
--rw-rw-rw-   0        0        0      345 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/linux/tmate_conn
--rw-rw-rw-   0        0        0      479 2023-03-30 22:29:06.000000 machineconfig-1.4/src/machineconfig/scripts/linux/tmate_start
--rw-rw-rw-   0        0        0      663 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/transfer.sh
--rw-rw-rw-   0        0        0      134 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/linux/transfer_wsl_win
--rw-rw-rw-   0        0        0     1366 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/linux/z_ls
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.141768 machineconfig-1.4/src/machineconfig/scripts/python/
--rw-rw-rw-   0        0        0       79 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.150899 machineconfig-1.4/src/machineconfig/scripts/python/__pycache__/
--rw-rw-rw-   0        0        0      238 2023-03-05 00:35:45.000000 machineconfig-1.4/src/machineconfig/scripts/python/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2086 2023-04-01 06:33:14.000000 machineconfig-1.4/src/machineconfig/scripts/python/__pycache__/cloud_mount.cpython-39.pyc
--rw-rw-rw-   0        0        0     1794 2023-03-05 00:41:39.000000 machineconfig-1.4/src/machineconfig/scripts/python/__pycache__/cloud_rx.cpython-39.pyc
--rw-rw-rw-   0        0        0     1722 2023-04-01 01:25:14.000000 machineconfig-1.4/src/machineconfig/scripts/python/__pycache__/cloud_sx.cpython-39.pyc
--rw-rw-rw-   0        0        0     2133 2023-04-01 06:01:00.000000 machineconfig-1.4/src/machineconfig/scripts/python/__pycache__/devops_backup_retrieve.cpython-39.pyc
--rw-rw-rw-   0        0        0     3147 2023-03-31 01:06:28.000000 machineconfig-1.4/src/machineconfig/scripts/python/__pycache__/devops_devapps_install.cpython-39.pyc
--rw-rw-rw-   0        0        0     2233 2023-03-31 02:05:22.000000 machineconfig-1.4/src/machineconfig/scripts/python/__pycache__/devops_update_repos.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.156228 machineconfig-1.4/src/machineconfig/scripts/python/archive/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/archive/__init__.py
--rw-rw-rw-   0        0        0     2070 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/archive/bu_gdrive_rx.py
--rw-rw-rw-   0        0        0     2246 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/archive/bu_gdrive_sx.py
--rw-rw-rw-   0        0        0     2996 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/archive/bu_onedrive_rx.py
--rw-rw-rw-   0        0        0     2291 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/archive/bu_onedrive_sx.py
--rw-rw-rw-   0        0        0     1145 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/choose_ohmybash_theme.py
--rw-rw-rw-   0        0        0     1919 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/choose_ohmyposh_theme.py
--rw-rw-rw-   0        0        0     1979 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/scripts/python/cloud_mount.py
--rw-rw-rw-   0        0        0     4491 2023-04-01 05:36:05.000000 machineconfig-1.4/src/machineconfig/scripts/python/cloud_repo_sync.py
--rw-rw-rw-   0        0        0     2252 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/cloud_rx.py
--rw-rw-rw-   0        0        0     1980 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/cloud_sx.py
--rw-rw-rw-   0        0        0     3441 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/cloud_sync.py
--rw-rw-rw-   0        0        0     3560 2023-04-01 06:04:21.000000 machineconfig-1.4/src/machineconfig/scripts/python/devops.py
--rw-rw-rw-   0        0        0     1462 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/devops_add_identity.py
--rw-rw-rw-   0        0        0     2527 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/devops_add_ssh_key.py
--rw-rw-rw-   0        0        0     2201 2023-04-01 06:00:22.000000 machineconfig-1.4/src/machineconfig/scripts/python/devops_backup_retrieve.py
--rw-rw-rw-   0        0        0     3780 2023-03-30 04:19:46.000000 machineconfig-1.4/src/machineconfig/scripts/python/devops_devapps_install.py
--rw-rw-rw-   0        0        0     2212 2023-04-01 00:11:02.000000 machineconfig-1.4/src/machineconfig/scripts/python/devops_update_repos.py
--rw-rw-rw-   0        0        0     1568 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/dotfile.py
--rw-rw-rw-   0        0        0     1477 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/ftprx.py
--rw-rw-rw-   0        0        0     1343 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/ftpsx.py
--rw-rw-rw-   0        0        0      558 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/im2text.py
--rw-rw-rw-   0        0        0       36 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/mount_nfs.py
--rw-rw-rw-   0        0        0      463 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/mount_ssh.py
--rw-rw-rw-   0        0        0     1396 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/onetimeshare.py
--rw-rw-rw-   0        0        0     1920 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/pomodoro.py
--rw-rw-rw-   0        0        0     5787 2023-04-01 05:28:37.000000 machineconfig-1.4/src/machineconfig/scripts/python/repos.py
--rw-rw-rw-   0        0        0      641 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/snapshot.py
--rw-rw-rw-   0        0        0      821 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/tmate_conn.py
--rw-rw-rw-   0        0        0      933 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/tmate_start.py
--rw-rw-rw-   0        0        0     1945 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/transfer_wsl_win.py
--rw-rw-rw-   0        0        0     1989 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/python/wifi_conn.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.185539 machineconfig-1.4/src/machineconfig/scripts/windows/
--rw-rw-rw-   0        0        0     1596 2023-04-01 05:45:52.000000 machineconfig-1.4/src/machineconfig/scripts/windows/activate_ve.ps1
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.190851 machineconfig-1.4/src/machineconfig/scripts/windows/archive/
--rw-rw-rw-   0        0        0      299 2023-03-19 23:10:45.000000 machineconfig-1.4/src/machineconfig/scripts/windows/archive/gource2vid.ps1
--rw-rw-rw-   0        0        0      623 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/archive/lvim_fresh_installation.ps1
--rw-rw-rw-   0        0        0     1651 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/archive/secure_pull.ps1
--rw-rw-rw-   0        0        0     2744 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/archive/secure_push.ps1
--rw-rw-rw-   0        0        0      333 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/choose_shell_theme.ps1
--rw-rw-rw-   0        0        0      575 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/cloud_mount.ps1
--rw-rw-rw-   0        0        0      134 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/cloud_repo_sync.ps1
--rw-rw-rw-   0        0        0      166 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/cloud_rx.ps1
--rw-rw-rw-   0        0        0      166 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/cloud_sx.ps1
--rw-rw-rw-   0        0        0      323 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/cloud_sync.ps1
--rw-rw-rw-   0        0        0      545 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/croshell.ps1
--rw-rw-rw-   0        0        0      684 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/devops.ps1
--rw-rw-rw-   0        0        0      160 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/dotfile.ps1
--rw-rw-rw-   0        0        0       85 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/fire.ps1
--rw-rw-rw-   0        0        0      327 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/fix_rclone_link.ps1
--rw-rw-rw-   0        0        0      158 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/ftprx.ps1
--rw-rw-rw-   0        0        0      224 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/ftpsx.ps1
--rw-rw-rw-   0        0        0      123 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/fzfb.ps1
--rw-rw-rw-   0        0        0       29 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/fzfg.ps1
--rw-rw-rw-   0        0        0       51 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/grep.ps1
--rw-rw-rw-   0        0        0      811 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/im2text.ps1
--rw-rw-rw-   0        0        0     2094 2023-03-13 08:14:50.000000 machineconfig-1.4/src/machineconfig/scripts/windows/mount_nfs.ps1
--rw-rw-rw-   0        0        0       53 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/nano.ps1
--rw-rw-rw-   0        0        0      152 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/neofetch.ps1
--rw-rw-rw-   0        0        0      178 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/pomodoro.ps1
--rw-rw-rw-   0        0        0      285 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/py2exe.ps1
--rw-rw-rw-   0        0        0      220 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/reload_path.ps1
--rw-rw-rw-   0        0        0      763 2023-03-17 01:04:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/repos.ps1
--rw-rw-rw-   0        0        0      161 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/snapshot.ps1
--rw-rw-rw-   0        0        0      200 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/tmate_conn.ps1
--rwxrwxrwx   0        0        0     1062 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/transfer_sh.cmd
--rw-rw-rw-   0        0        0      263 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/unlock_bitlocker.ps1
--rw-rw-rw-   0        0        0      197 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/wifi_conn.ps1
--rw-rw-rw-   0        0        0     1766 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/wsl_rdp_windows_port_forwarding.ps1
--rw-rw-rw-   0        0        0     2744 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/wsl_ssh_windows_port_forwarding.ps1
--rw-rw-rw-   0        0        0      171 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/scripts/windows/wsl_windows_transfer.ps1
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.931848 machineconfig-1.4/src/machineconfig/settings/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.193548 machineconfig-1.4/src/machineconfig/settings/broot/
--rw-rw-rw-   0        0        0      599 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/broot/br.sh
--rw-rw-rw-   0        0        0      909 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/broot/brootcd.ps1
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.194600 machineconfig-1.4/src/machineconfig/settings/helix/
--rw-rw-rw-   0        0        0      200 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/helix/config.toml
--rw-rw-rw-   0        0        0      336 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/helix/languages.toml
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.926061 machineconfig-1.4/src/machineconfig/settings/lf/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.199474 machineconfig-1.4/src/machineconfig/settings/lf/linux/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.205538 machineconfig-1.4/src/machineconfig/settings/lf/linux/autocall/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/linux/autocall/delete.sh
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/linux/autocall/on-cd.sh
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/linux/autocall/on-quit.sh
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/linux/autocall/open.sh
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/linux/autocall/paste.sh
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/linux/autocall/pre-cd.sh
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/linux/autocall/rename.sh
--rw-rw-rw-   0        0        0     3570 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/linux/colors
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.209796 machineconfig-1.4/src/machineconfig/settings/lf/linux/exe/
--rw-rw-rw-   0        0        0      388 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/settings/lf/linux/exe/fzf_nano.sh
--rw-rw-rw-   0        0        0       90 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/settings/lf/linux/exe/leftpane_previewer.sh
--rw-rw-rw-   0        0        0      795 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/settings/lf/linux/exe/lfcd.sh
--rw-rw-rw-   0        0        0       95 2023-03-26 01:52:23.000000 machineconfig-1.4/src/machineconfig/settings/lf/linux/exe/previewer.sh
--rw-rw-rw-   0        0        0     7504 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/linux/icons
--rw-rw-rw-   0        0        0     4991 2023-03-17 04:41:42.000000 machineconfig-1.4/src/machineconfig/settings/lf/linux/lfrc
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.223119 machineconfig-1.4/src/machineconfig/settings/lf/windows/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.226470 machineconfig-1.4/src/machineconfig/settings/lf/windows/autocall/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/autocall/delete.ps1
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/autocall/on-cd.ps1
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/autocall/on-quit.ps1
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/autocall/open.ps1
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/autocall/paste.ps1
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/autocall/pre-cd.ps1
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/autocall/rename.ps1
--rw-rw-rw-   0        0        0      207 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/cd_tere.ps1
--rw-rw-rw-   0        0        0      163 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/cd_zoxide.ps1
--rw-rw-rw-   0        0        0      145 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/cd_zoxide2.ps1
--rw-rw-rw-   0        0        0     3150 2023-03-19 03:41:28.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/colors
--rw-rw-rw-   0        0        0      401 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/fzf_edit.ps1
--rw-rw-rw-   0        0        0     7504 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/icons
--rw-rw-rw-   0        0        0       90 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/leftpane_previewer.ps1
--rw-rw-rw-   0        0        0      996 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/lfcd.ps1
--rw-rw-rw-   0        0        0     4486 2023-03-17 04:49:37.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/lfrc
--rw-rw-rw-   0        0        0       59 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/mkdir.ps1
--rw-rw-rw-   0        0        0       65 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/mkfile.ps1
--rw-rw-rw-   0        0        0      213 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/previewer.ps1
--rw-rw-rw-   0        0        0        4 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lf/windows/tst.ps1
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.927410 machineconfig-1.4/src/machineconfig/settings/lvim/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.927410 machineconfig-1.4/src/machineconfig/settings/lvim/generic/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.230243 machineconfig-1.4/src/machineconfig/settings/lvim/generic/plugins_config/
--rw-rw-rw-   0        0        0      625 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lvim/generic/plugins_config/.flake8
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.927410 machineconfig-1.4/src/machineconfig/settings/lvim/windows/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.232556 machineconfig-1.4/src/machineconfig/settings/lvim/windows/archive/
--rw-rw-rw-   0        0        0      815 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lvim/windows/archive/config_additional.lua
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.927410 machineconfig-1.4/src/machineconfig/settings/lvim/windows/lua/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.232556 machineconfig-1.4/src/machineconfig/settings/lvim/windows/lua/user/
--rw-rw-rw-   0        0        0      282 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/lvim/windows/lua/user/custom_config.lua
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.929220 machineconfig-1.4/src/machineconfig/settings/mprocs/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.234180 machineconfig-1.4/src/machineconfig/settings/mprocs/windows/
--rw-rw-rw-   0        0        0      915 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/mprocs/windows/mprocs.yaml
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.930624 machineconfig-1.4/src/machineconfig/settings/shells/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.234180 machineconfig-1.4/src/machineconfig/settings/shells/bash/
--rw-rw-rw-   0        0        0     1145 2023-04-01 05:27:22.000000 machineconfig-1.4/src/machineconfig/settings/shells/bash/init.sh
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.237485 machineconfig-1.4/src/machineconfig/settings/shells/nushell/
--rw-rw-rw-   0        0        0    21214 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/shells/nushell/config.nu
--rw-rw-rw-   0        0        0     2044 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/shells/nushell/env.nu
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.238493 machineconfig-1.4/src/machineconfig/settings/shells/pwsh/
--rw-rw-rw-   0        0        0     1618 2023-03-30 22:29:06.000000 machineconfig-1.4/src/machineconfig/settings/shells/pwsh/init.ps1
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.238999 machineconfig-1.4/src/machineconfig/settings/shells/wt/
--rw-rw-rw-   0        0        0    13738 2023-03-30 01:22:19.000000 machineconfig-1.4/src/machineconfig/settings/shells/wt/settings.json
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.930624 machineconfig-1.4/src/machineconfig/settings/svim/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.238999 machineconfig-1.4/src/machineconfig/settings/svim/linux/
--rw-rw-rw-   0        0        0     1496 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/svim/linux/init.toml
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.238999 machineconfig-1.4/src/machineconfig/settings/svim/windows/
--rw-rw-rw-   0        0        0     1484 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/svim/windows/init.toml
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.238999 machineconfig-1.4/src/machineconfig/settings/tere/
--rw-rw-rw-   0        0        0      183 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/tere/terecd.ps1
--rw-rw-rw-   0        0        0       95 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/tere/terecd.sh
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.245809 machineconfig-1.4/src/machineconfig/settings/tmux/
--rw-rw-rw-   0        0        0       60 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/tmux/.tmate.conf
--rw-rw-rw-   0        0        0      100 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/tmux/.tmux.conf
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.245809 machineconfig-1.4/src/machineconfig/settings/wsl/
--rw-rw-rw-   0        0        0     1313 2023-03-19 03:41:28.000000 machineconfig-1.4/src/machineconfig/settings/wsl/.wslconfig
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.250558 machineconfig-1.4/src/machineconfig/settings/zellij/
--rw-rw-rw-   0        0        0    10624 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/zellij/config.kdl
--rw-rw-rw-   0        0        0    10644 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/zellij/config.orig.kdl
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.251854 machineconfig-1.4/src/machineconfig/settings/zellij/layouts/
--rw-rw-rw-   0        0        0      662 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/zellij/layouts/st.kdl
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.251854 machineconfig-1.4/src/machineconfig/settings/zellij/themes/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/settings/zellij/themes/mytheme.kdl
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.934438 machineconfig-1.4/src/machineconfig/setup_linux/
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.252929 machineconfig-1.4/src/machineconfig/setup_linux/nix/
--rw-rw-rw-   0        0        0     4540 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/setup_linux/nix/cli_installation.sh
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.256371 machineconfig-1.4/src/machineconfig/setup_linux/others/
--rw-rw-rw-   0        0        0      424 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/setup_linux/others/archive
--rw-rw-rw-   0        0        0      479 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/setup_linux/others/chrome.sh
--rw-rw-rw-   0        0        0      424 2023-03-30 22:29:06.000000 machineconfig-1.4/src/machineconfig/setup_linux/others/openssh-server_add_pub_key.sh
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.262066 machineconfig-1.4/src/machineconfig/setup_linux/web_shortcuts/
--rw-rw-rw-   0        0        0      930 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/setup_linux/web_shortcuts/all.sh
--rw-rw-rw-   0        0        0     1534 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/setup_linux/web_shortcuts/ascii_art.sh
--rw-rw-rw-   0        0        0      606 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/setup_linux/web_shortcuts/croshell.sh
--rw-rw-rw-   0        0        0      573 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/setup_linux/web_shortcuts/ssh.sh
--rw-rw-rw-   0        0        0      447 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/setup_linux/web_shortcuts/update_system.sh
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.263126 machineconfig-1.4/src/machineconfig/setup_windows/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/setup_windows/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.263126 machineconfig-1.4/src/machineconfig/setup_windows/others/
--rw-rw-rw-   0        0        0      318 2023-03-29 22:18:40.000000 machineconfig-1.4/src/machineconfig/setup_windows/others/docker.ps1
--rw-rw-rw-   0        0        0       78 2023-03-05 08:45:12.000000 machineconfig-1.4/src/machineconfig/setup_windows/others/obs.ps1
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.268747 machineconfig-1.4/src/machineconfig/setup_windows/web_shortcuts/
--rw-rw-rw-   0        0        0      854 2023-03-30 22:29:06.000000 machineconfig-1.4/src/machineconfig/setup_windows/web_shortcuts/all.ps1
--rw-rw-rw-   0        0        0     1200 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/setup_windows/web_shortcuts/ascii_art.ps1
--rw-rw-rw-   0        0        0      770 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/setup_windows/web_shortcuts/croshell.ps1
--rw-rw-rw-   0        0        0      328 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/setup_windows/web_shortcuts/ssh.ps1
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.272860 machineconfig-1.4/src/machineconfig/setup_windows/wt_and_pwsh/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/setup_windows/wt_and_pwsh/__init__.py
--rw-rw-rw-   0        0        0      705 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/setup_windows/wt_and_pwsh/install_fonts.ps1
--rw-rw-rw-   0        0        0     2242 2023-03-05 01:43:35.000000 machineconfig-1.4/src/machineconfig/setup_windows/wt_and_pwsh/set_pwsh_theme.py
--rw-rw-rw-   0        0        0     6097 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/setup_windows/wt_and_pwsh/set_wt_settings.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:05.275316 machineconfig-1.4/src/machineconfig/utils/
--rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/utils/__init__.py
--rw-rw-rw-   0        0        0      205 2023-03-04 22:55:51.000000 machineconfig-1.4/src/machineconfig/utils/to_exe.py
--rw-rw-rw-   0        0        0    10946 2023-04-01 06:04:52.000000 machineconfig-1.4/src/machineconfig/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-01 06:43:04.943504 machineconfig-1.4/src/machineconfig.egg-info/
--rw-rw-rw-   0        0        0     5289 2023-04-01 06:43:04.000000 machineconfig-1.4/src/machineconfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    16679 2023-04-01 06:43:04.000000 machineconfig-1.4/src/machineconfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 06:43:04.000000 machineconfig-1.4/src/machineconfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-01 06:43:04.000000 machineconfig-1.4/src/machineconfig.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-01 06:43:04.000000 machineconfig-1.4/src/machineconfig.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.388409 machineconfig-1.5/
+-rw-rw-rw-   0        0        0      232 2023-03-04 22:55:51.000000 machineconfig-1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     5289 2023-06-09 00:20:22.387004 machineconfig-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4775 2023-04-01 05:32:36.000000 machineconfig-1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 00:20:22.388409 machineconfig-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      971 2023-05-18 10:20:13.000000 machineconfig-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.013504 machineconfig-1.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.043572 machineconfig-1.5/src/machineconfig/
+-rw-rw-rw-   0        0        0       67 2023-06-09 00:19:40.000000 machineconfig-1.5/src/machineconfig/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.050745 machineconfig-1.5/src/machineconfig/jobs/
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.050745 machineconfig-1.5/src/machineconfig/jobs/__pycache__/
+-rw-rw-rw-   0        0        0      158 2023-03-05 00:35:45.000000 machineconfig-1.5/src/machineconfig/jobs/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.014630 machineconfig-1.5/src/machineconfig/jobs/linux/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.061018 machineconfig-1.5/src/machineconfig/jobs/linux/archive/
+-rw-rw-rw-   0        0        0      519 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/jobs/linux/archive/get_latest_release.sh
+-rw-rw-rw-   0        0        0      670 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/linux/archive/install_bandwich.sh
+-rw-rw-rw-   0        0        0      687 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/linux/archive/install_diskonaut.sh
+-rw-rw-rw-   0        0        0      352 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/linux/archive/install_kondo.sh
+-rw-rw-rw-   0        0        0      662 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/linux/archive/install_nu.sh
+-rw-rw-rw-   0        0        0      606 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/linux/archive/install_zellij.sh
+-rw-rw-rw-   0        0        0      654 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/jobs/linux/archive/lf.sh
+-rw-rw-rw-   0        0        0     1335 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/jobs/linux/archive/quirks.sh
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.072609 machineconfig-1.5/src/machineconfig/jobs/python/
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/python/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.077119 machineconfig-1.5/src/machineconfig/jobs/python/__pycache__/
+-rw-rw-rw-   0        0        0      165 2023-03-05 00:35:45.000000 machineconfig-1.5/src/machineconfig/jobs/python/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3752 2023-03-30 04:11:37.000000 machineconfig-1.5/src/machineconfig/jobs/python/__pycache__/python_linux_installers_all.cpython-39.pyc
+-rw-rw-rw-   0        0        0      679 2023-03-13 07:34:55.000000 machineconfig-1.5/src/machineconfig/jobs/python/__pycache__/python_ve_symlink.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1200 2023-03-28 23:28:03.000000 machineconfig-1.5/src/machineconfig/jobs/python/__pycache__/python_windows_installers_all.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.078626 machineconfig-1.5/src/machineconfig/jobs/python/archive/
+-rw-rw-rw-   0        0        0      299 2023-04-26 01:20:08.000000 machineconfig-1.5/src/machineconfig/jobs/python/archive/python_tools.txt
+-rw-rw-rw-   0        0        0     7357 2023-03-05 03:20:36.000000 machineconfig-1.5/src/machineconfig/jobs/python/check_installations.py
+-rw-rw-rw-   0        0        0      625 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/python/create_bootable_media.py
+-rw-rw-rw-   0        0        0     1296 2023-04-09 00:03:14.000000 machineconfig-1.5/src/machineconfig/jobs/python/create_zellij_template.py
+-rw-rw-rw-   0        0        0     1742 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/python/python_cargo_build_share.py
+-rw-rw-rw-   0        0        0     3303 2023-03-29 00:59:04.000000 machineconfig-1.5/src/machineconfig/jobs/python/python_linux_installers_all.py
+-rw-rw-rw-   0        0        0     2826 2023-04-11 07:14:49.000000 machineconfig-1.5/src/machineconfig/jobs/python/python_ve_installer.py
+-rw-rw-rw-   0        0        0      872 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/python/python_ve_symlink.py
+-rw-rw-rw-   0        0        0      789 2023-03-28 23:12:01.000000 machineconfig-1.5/src/machineconfig/jobs/python/python_windows_installers_all.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.104597 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.106007 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/__pycache__/
+-rw-rw-rw-   0        0        0      184 2023-03-05 00:35:45.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.109195 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/archive/
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/archive/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/archive/nvim.py
+-rw-rw-rw-   0        0        0     1024 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/archive/strongbox.py
+-rw-rw-rw-   0        0        0     1230 2023-03-28 22:15:27.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/broot.py
+-rw-rw-rw-   0        0        0     1098 2023-05-18 09:24:40.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/browsh.py
+-rw-rw-rw-   0        0        0      857 2023-06-08 23:20:31.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/chatgpt.py
+-rw-rw-rw-   0        0        0      939 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/cpufetch.py
+-rw-rw-rw-   0        0        0     1940 2023-03-28 22:15:27.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/delta.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.127287 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/
+-rw-rw-rw-   0        0        0        0 2023-03-27 21:24:54.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/__init__.py
+-rw-rw-rw-   0        0        0      754 2023-04-26 01:20:08.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/autogpt.py
+-rw-rw-rw-   0        0        0      960 2023-03-28 22:16:59.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/bw.py
+-rw-rw-rw-   0        0        0      722 2023-03-30 04:14:00.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/evcxr.py
+-rw-rw-rw-   0        0        0      802 2023-03-28 22:20:23.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/kondo.py
+-rw-rw-rw-   0        0        0     2498 2023-05-07 09:04:38.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/lvim.py
+-rw-rw-rw-   0        0        0     1087 2023-04-08 23:43:48.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/ngrok.py
+-rw-rw-rw-   0        0        0      476 2023-04-03 04:25:43.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/opencommit.py
+-rw-rw-rw-   0        0        0     1119 2023-03-28 23:27:59.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/qrcp.py
+-rw-rw-rw-   0        0        0      760 2023-03-28 23:27:59.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/qrscan.py
+-rw-rw-rw-   0        0        0     1016 2023-03-28 23:27:59.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/rust-analyzer.py
+-rw-rw-rw-   0        0        0      746 2023-03-28 23:27:59.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/termscp.py
+-rw-rw-rw-   0        0        0      969 2023-03-28 23:27:59.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/tldr.py
+-rw-rw-rw-   0        0        0      984 2023-03-28 23:27:59.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/tokei.py
+-rw-rw-rw-   0        0        0      946 2023-03-28 22:12:20.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/diskonaut.py
+-rw-rw-rw-   0        0        0      747 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dua.py
+-rw-rw-rw-   0        0        0      893 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/gitui.py
+-rw-rw-rw-   0        0        0      745 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/gopass.py
+-rw-rw-rw-   0        0        0     1946 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/helix.py
+-rw-rw-rw-   0        0        0     1027 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/lf.py
+-rw-rw-rw-   0        0        0      664 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/mprocs.py
+-rw-rw-rw-   0        0        0      690 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/navi.py
+-rw-rw-rw-   0        0        0     1205 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/ots.py
+-rw-rw-rw-   0        0        0      965 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/ouch.py
+-rw-rw-rw-   0        0        0      757 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/pomodoro.py
+-rw-rw-rw-   0        0        0      701 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/procs.py
+-rw-rw-rw-   0        0        0      689 2023-03-28 22:16:59.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/rclone.py
+-rw-rw-rw-   0        0        0     1143 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/tere.py
+-rw-rw-rw-   0        0        0      818 2023-04-26 01:20:08.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/vtm.py
+-rw-rw-rw-   0        0        0      712 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/watchexec.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.139147 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.140523 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/__pycache__/
+-rw-rw-rw-   0        0        0      182 2023-03-05 00:35:45.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.142717 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/archive/
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/archive/__init__.py
+-rw-rw-rw-   0        0        0      548 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/archive/ranger.py
+-rw-rw-rw-   0        0        0      626 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/bottom.py
+-rw-rw-rw-   0        0        0      582 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/btop.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.146159 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/dev/
+-rw-rw-rw-   0        0        0        0 2023-03-27 21:24:54.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/dev/__init__.py
+-rw-rw-rw-   0        0        0      207 2023-03-28 23:27:59.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/dev/bandwhich.py
+-rw-rw-rw-   0        0        0      680 2023-03-28 23:27:59.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/dev/bytehound.py
+-rw-rw-rw-   0        0        0      569 2023-03-28 23:27:59.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/dev/nnn.py
+-rw-rw-rw-   0        0        0      497 2023-03-29 01:53:24.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/gotty.py
+-rw-rw-rw-   0        0        0     1139 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/joshuto.py
+-rw-rw-rw-   0        0        0      402 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/mcfly.py
+-rw-rw-rw-   0        0        0      508 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/skim.py
+-rw-rw-rw-   0        0        0      511 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/topgrade.py
+-rw-rw-rw-   0        0        0      642 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/viu.py
+-rw-rw-rw-   0        0        0      759 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/xplr.py
+-rw-rw-rw-   0        0        0     1145 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/zellij.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.156551 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.158059 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/__pycache__/
+-rw-rw-rw-   0        0        0      184 2023-03-05 00:35:45.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.160603 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/archive/
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/archive/__init__.py
+-rw-rw-rw-   0        0        0      425 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/archive/ntop.py
+-rw-rw-rw-   0        0        0       66 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/archive/readme.md
+-rw-rw-rw-   0        0        0      356 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/bat.py
+-rw-rw-rw-   0        0        0      789 2023-03-28 22:15:27.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/boxes.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.162882 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/dev/
+-rw-rw-rw-   0        0        0        0 2023-03-27 21:24:54.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/dev/__init__.py
+-rw-rw-rw-   0        0        0      560 2023-03-28 23:27:59.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/dev/bypass_paywall.py
+-rw-rw-rw-   0        0        0      790 2023-03-28 23:27:59.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/dev/obs_background_removal_plugin.py
+-rw-rw-rw-   0        0        0      514 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/fd.py
+-rw-rw-rw-   0        0        0      715 2023-03-28 22:15:27.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/fzf.py
+-rw-rw-rw-   0        0        0      438 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/rg.py
+-rw-rw-rw-   0        0        0      422 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/ugrep.py
+-rw-rw-rw-   0        0        0      624 2023-03-28 22:15:27.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/zoomit.py
+-rw-rw-rw-   0        0        0      405 2023-03-28 21:18:51.000000 machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/zoxide.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.165412 machineconfig-1.5/src/machineconfig/jobs/windows/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.168420 machineconfig-1.5/src/machineconfig/jobs/windows/arhive/
+-rw-rw-rw-   0        0        0      681 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/windows/arhive/archive_pygraphviz.ps1
+-rw-rw-rw-   0        0        0      276 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/windows/arhive/openssh-server_add_key.ps1
+-rw-rw-rw-   0        0        0      759 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/windows/arhive/openssh-server_copy-ssh-id.ps1
+-rw-rw-rw-   0        0        0      477 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/windows/start_terminal.ps1
+-rwxrwxrwx   0        0        0       97 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/jobs/windows/startup_file.cmd
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.173038 machineconfig-1.5/src/machineconfig/profile/
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/profile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.174044 machineconfig-1.5/src/machineconfig/profile/__pycache__/
+-rw-rw-rw-   0        0        0      161 2023-03-05 00:24:30.000000 machineconfig-1.5/src/machineconfig/profile/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6546 2023-03-15 11:01:02.000000 machineconfig-1.5/src/machineconfig/profile/__pycache__/create.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9363 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/profile/create.py
+-rw-rw-rw-   0        0        0      406 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/profile/fix_shell_profiles.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.023698 machineconfig-1.5/src/machineconfig/profile/patches/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.179572 machineconfig-1.5/src/machineconfig/profile/patches/linux/
+-rw-rw-rw-   0        0        0       70 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/profile/patches/linux/mcfly.sh
+-rw-rw-rw-   0        0        0       50 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/profile/patches/linux/xming.sh
+-rw-rw-rw-   0        0        0       76 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/profile/patches/linux/zoxide.sh
+-rw-rw-rw-   0        0        0      613 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/profile/patches/linux/zzellij.sh
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.180721 machineconfig-1.5/src/machineconfig/profile/patches/windows/
+-rw-rw-rw-   0        0        0      241 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/profile/patches/windows/zoxide.ps1
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.024759 machineconfig-1.5/src/machineconfig/profile/records/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.180721 machineconfig-1.5/src/machineconfig/profile/records/generic/
+-rw-rw-rw-   0        0        0      150 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/profile/records/generic/shares.toml
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.184390 machineconfig-1.5/src/machineconfig/profile/records/linux/
+-rw-rw-rw-   0        0        0     1732 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/profile/records/linux/safe_cli_apps.json
+-rw-rw-rw-   0        0        0       65 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/profile/records/linux/safe_cli_apps_url.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.188295 machineconfig-1.5/src/machineconfig/profile/records/windows/
+-rw-rw-rw-   0        0        0      423 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/profile/records/windows/safe_cli_apps.csv
+-rw-rw-rw-   0        0        0     4597 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/profile/records/windows/safe_cli_apps.json
+-rw-rw-rw-   0        0        0       65 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/profile/records/windows/safe_cli_apps_url.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.189314 machineconfig-1.5/src/machineconfig/scripts/
+-rw-rw-rw-   0        0        0       79 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.190408 machineconfig-1.5/src/machineconfig/scripts/__pycache__/
+-rw-rw-rw-   0        0        0      231 2023-03-05 00:35:45.000000 machineconfig-1.5/src/machineconfig/scripts/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.215520 machineconfig-1.5/src/machineconfig/scripts/linux/
+-rw-rw-rw-   0        0        0     1603 2023-04-01 05:50:14.000000 machineconfig-1.5/src/machineconfig/scripts/linux/activate_ve
+-rw-rw-rw-   0        0        0      183 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/scripts/linux/choose_shell_theme
+-rw-rw-rw-   0        0        0      557 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/scripts/linux/cloud_mount
+-rw-rw-rw-   0        0        0      135 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/scripts/linux/cloud_repo_sync
+-rw-rw-rw-   0        0        0      123 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/scripts/linux/cloud_rx
+-rw-rw-rw-   0        0        0      123 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/scripts/linux/cloud_sx
+-rw-rw-rw-   0        0        0      556 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/scripts/linux/cloud_sync
+-rw-rw-rw-   0        0        0      242 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/linux/croshell
+-rw-rw-rw-   0        0        0      484 2023-04-16 04:35:03.000000 machineconfig-1.5/src/machineconfig/scripts/linux/devops
+-rw-rw-rw-   0        0        0      289 2023-04-26 01:20:08.000000 machineconfig-1.5/src/machineconfig/scripts/linux/fire
+-rw-rw-rw-   0        0        0      125 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/linux/ftprx
+-rw-rw-rw-   0        0        0      121 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/linux/ftpsx
+-rw-rw-rw-   0        0        0      853 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/linux/fzf2g
+-rw-rw-rw-   0        0        0      696 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/linux/fzfag
+-rw-rw-rw-   0        0        0     1115 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/linux/fzffg
+-rw-rw-rw-   0        0        0     1215 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/linux/fzfg
+-rw-rw-rw-   0        0        0      214 2023-04-08 23:43:48.000000 machineconfig-1.5/src/machineconfig/scripts/linux/launch_multiple_machines
+-rw-rw-rw-   0        0        0     2757 2023-04-08 23:43:48.000000 machineconfig-1.5/src/machineconfig/scripts/linux/mount_drive
+-rw-rw-rw-   0        0        0     2341 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/scripts/linux/mount_nfs
+-rw-rw-rw-   0        0        0     2800 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/scripts/linux/mount_nw_drive
+-rw-rw-rw-   0        0        0      522 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/scripts/linux/repos
+-rw-rw-rw-   0        0        0      137 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/scripts/linux/sk_rg
+-rw-rw-rw-   0        0        0      437 2023-04-08 23:43:48.000000 machineconfig-1.5/src/machineconfig/scripts/linux/tmate_conn
+-rw-rw-rw-   0        0        0      513 2023-04-08 23:43:48.000000 machineconfig-1.5/src/machineconfig/scripts/linux/tmate_start
+-rw-rw-rw-   0        0        0      663 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/scripts/linux/transfer.sh
+-rw-rw-rw-   0        0        0      134 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/linux/transfer_wsl_win
+-rw-rw-rw-   0        0        0     1366 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/scripts/linux/z_ls
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.250344 machineconfig-1.5/src/machineconfig/scripts/python/
+-rw-rw-rw-   0        0        0        0 2023-04-08 23:43:48.000000 machineconfig-1.5/src/machineconfig/scripts/python/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.263031 machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/
+-rw-rw-rw-   0        0        0      168 2023-04-09 00:19:23.000000 machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1019 2023-05-24 02:05:22.000000 machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/chatgpt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2086 2023-04-01 06:33:14.000000 machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/cloud_mount.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1794 2023-03-05 00:41:39.000000 machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/cloud_rx.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1763 2023-04-09 02:17:26.000000 machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/cloud_sx.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3167 2023-04-04 00:27:27.000000 machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/devops.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2133 2023-04-01 06:01:00.000000 machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/devops_backup_retrieve.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3658 2023-04-09 01:18:39.000000 machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/devops_devapps_install.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2172 2023-05-17 08:24:01.000000 machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/devops_update_repos.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4137 2023-04-09 00:53:56.000000 machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/fire_jobs.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1873 2023-04-17 05:38:29.000000 machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/pomodoro.cpython-39.pyc
+-rw-rw-rw-   0        0        0      737 2023-05-27 16:35:58.000000 machineconfig-1.5/src/machineconfig/scripts/python/chatgpt.py
+-rw-rw-rw-   0        0        0     1145 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/choose_ohmybash_theme.py
+-rw-rw-rw-   0        0        0     1919 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/choose_ohmyposh_theme.py
+-rw-rw-rw-   0        0        0     1979 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/scripts/python/cloud_mount.py
+-rw-rw-rw-   0        0        0     6147 2023-06-08 23:20:31.000000 machineconfig-1.5/src/machineconfig/scripts/python/cloud_repo_sync.py
+-rw-rw-rw-   0        0        0     2252 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/cloud_rx.py
+-rw-rw-rw-   0        0        0     1980 2023-04-09 02:18:50.000000 machineconfig-1.5/src/machineconfig/scripts/python/cloud_sx.py
+-rw-rw-rw-   0        0        0     3443 2023-05-12 02:03:01.000000 machineconfig-1.5/src/machineconfig/scripts/python/cloud_sync.py
+-rw-rw-rw-   0        0        0     3901 2023-05-12 01:54:52.000000 machineconfig-1.5/src/machineconfig/scripts/python/devops.py
+-rw-rw-rw-   0        0        0     1462 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/devops_add_identity.py
+-rw-rw-rw-   0        0        0     2527 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/devops_add_ssh_key.py
+-rw-rw-rw-   0        0        0     2201 2023-04-01 06:00:22.000000 machineconfig-1.5/src/machineconfig/scripts/python/devops_backup_retrieve.py
+-rw-rw-rw-   0        0        0     4488 2023-04-08 23:43:48.000000 machineconfig-1.5/src/machineconfig/scripts/python/devops_devapps_install.py
+-rw-rw-rw-   0        0        0     2541 2023-05-12 01:35:13.000000 machineconfig-1.5/src/machineconfig/scripts/python/devops_update_repos.py
+-rw-rw-rw-   0        0        0     1568 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/dotfile.py
+-rw-rw-rw-   0        0        0     4982 2023-04-16 04:35:03.000000 machineconfig-1.5/src/machineconfig/scripts/python/fire_jobs.py
+-rw-rw-rw-   0        0        0     1477 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/ftprx.py
+-rw-rw-rw-   0        0        0     1343 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/ftpsx.py
+-rw-rw-rw-   0        0        0      558 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/im2text.py
+-rw-rw-rw-   0        0        0       36 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/mount_nfs.py
+-rw-rw-rw-   0        0        0      463 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/mount_ssh.py
+-rw-rw-rw-   0        0        0     1396 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/onetimeshare.py
+-rw-rw-rw-   0        0        0     1920 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/pomodoro.py
+-rw-rw-rw-   0        0        0     5813 2023-05-12 02:06:41.000000 machineconfig-1.5/src/machineconfig/scripts/python/repos.py
+-rw-rw-rw-   0        0        0      641 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/snapshot.py
+-rw-rw-rw-   0        0        0      821 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/tmate_conn.py
+-rw-rw-rw-   0        0        0      933 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/tmate_start.py
+-rw-rw-rw-   0        0        0     1945 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/python/transfer_wsl_win.py
+-rw-rw-rw-   0        0        0     2009 2023-05-12 01:43:30.000000 machineconfig-1.5/src/machineconfig/scripts/python/wifi_conn.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.300467 machineconfig-1.5/src/machineconfig/scripts/windows/
+-rw-rw-rw-   0        0        0     1704 2023-04-08 23:43:48.000000 machineconfig-1.5/src/machineconfig/scripts/windows/activate_ve.ps1
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.302777 machineconfig-1.5/src/machineconfig/scripts/windows/archive/
+-rw-rw-rw-   0        0        0      299 2023-03-19 23:10:45.000000 machineconfig-1.5/src/machineconfig/scripts/windows/archive/gource2vid.ps1
+-rw-rw-rw-   0        0        0     1651 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/archive/secure_pull.ps1
+-rw-rw-rw-   0        0        0     2744 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/archive/secure_push.ps1
+-rw-rw-rw-   0        0        0      243 2023-05-07 09:04:38.000000 machineconfig-1.5/src/machineconfig/scripts/windows/chatgpt.ps1
+-rw-rw-rw-   0        0        0      333 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/choose_shell_theme.ps1
+-rw-rw-rw-   0        0        0      577 2023-04-11 07:14:49.000000 machineconfig-1.5/src/machineconfig/scripts/windows/cloud_mount.ps1
+-rw-rw-rw-   0        0        0      134 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/cloud_repo_sync.ps1
+-rw-rw-rw-   0        0        0      166 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/cloud_rx.ps1
+-rw-rw-rw-   0        0        0      166 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/cloud_sx.ps1
+-rw-rw-rw-   0        0        0      323 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/cloud_sync.ps1
+-rw-rw-rw-   0        0        0      545 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/croshell.ps1
+-rw-rw-rw-   0        0        0      789 2023-04-04 00:33:12.000000 machineconfig-1.5/src/machineconfig/scripts/windows/devops.ps1
+-rw-rw-rw-   0        0        0      160 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/dotfile.ps1
+-rw-rw-rw-   0        0        0      369 2023-04-04 22:55:32.000000 machineconfig-1.5/src/machineconfig/scripts/windows/fire.ps1
+-rw-rw-rw-   0        0        0      327 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/fix_rclone_link.ps1
+-rw-rw-rw-   0        0        0      158 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/ftprx.ps1
+-rw-rw-rw-   0        0        0      224 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/ftpsx.ps1
+-rw-rw-rw-   0        0        0      123 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/fzfb.ps1
+-rw-rw-rw-   0        0        0       29 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/fzfg.ps1
+-rw-rw-rw-   0        0        0       51 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/grep.ps1
+-rw-rw-rw-   0        0        0      811 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/im2text.ps1
+-rw-rw-rw-   0        0        0      133 2023-04-26 01:20:08.000000 machineconfig-1.5/src/machineconfig/scripts/windows/kill_process.ps1
+-rw-rw-rw-   0        0        0     2094 2023-03-13 08:14:50.000000 machineconfig-1.5/src/machineconfig/scripts/windows/mount_nfs.ps1
+-rw-rw-rw-   0        0        0       53 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/nano.ps1
+-rw-rw-rw-   0        0        0      152 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/neofetch.ps1
+-rw-rw-rw-   0        0        0      178 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/pomodoro.ps1
+-rw-rw-rw-   0        0        0      285 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/py2exe.ps1
+-rw-rw-rw-   0        0        0      220 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/reload_path.ps1
+-rw-rw-rw-   0        0        0      763 2023-03-17 01:04:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/repos.ps1
+-rw-rw-rw-   0        0        0      161 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/snapshot.ps1
+-rw-rw-rw-   0        0        0      200 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/tmate_conn.ps1
+-rwxrwxrwx   0        0        0     1062 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/transfer_sh.cmd
+-rw-rw-rw-   0        0        0      263 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/unlock_bitlocker.ps1
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.303986 machineconfig-1.5/src/machineconfig/scripts/windows/utils/
+-rw-rw-rw-   0        0        0      174 2023-04-11 07:14:49.000000 machineconfig-1.5/src/machineconfig/scripts/windows/utils/op_script_delete.ps1
+-rw-rw-rw-   0        0        0      193 2023-04-08 23:43:48.000000 machineconfig-1.5/src/machineconfig/scripts/windows/wifi_conn.ps1
+-rw-rw-rw-   0        0        0     1766 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/wsl_rdp_windows_port_forwarding.ps1
+-rw-rw-rw-   0        0        0     2744 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/wsl_ssh_windows_port_forwarding.ps1
+-rw-rw-rw-   0        0        0      171 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/scripts/windows/wsl_windows_transfer.ps1
+-rw-rw-rw-   0        0        0       68 2023-04-26 01:20:08.000000 machineconfig-1.5/src/machineconfig/scripts/windows/wts.ps1
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.038031 machineconfig-1.5/src/machineconfig/settings/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.306233 machineconfig-1.5/src/machineconfig/settings/broot/
+-rw-rw-rw-   0        0        0      599 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/broot/br.sh
+-rw-rw-rw-   0        0        0      909 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/broot/brootcd.ps1
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.308286 machineconfig-1.5/src/machineconfig/settings/helix/
+-rw-rw-rw-   0        0        0      200 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/helix/config.toml
+-rw-rw-rw-   0        0        0      428 2023-06-08 23:20:31.000000 machineconfig-1.5/src/machineconfig/settings/helix/languages.toml
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.030480 machineconfig-1.5/src/machineconfig/settings/lf/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.311321 machineconfig-1.5/src/machineconfig/settings/lf/linux/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.315776 machineconfig-1.5/src/machineconfig/settings/lf/linux/autocall/
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/linux/autocall/delete.sh
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/linux/autocall/on-cd.sh
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/linux/autocall/on-quit.sh
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/linux/autocall/open.sh
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/linux/autocall/paste.sh
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/linux/autocall/pre-cd.sh
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/linux/autocall/rename.sh
+-rw-rw-rw-   0        0        0     4344 2023-04-26 01:20:08.000000 machineconfig-1.5/src/machineconfig/settings/lf/linux/colors
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.319116 machineconfig-1.5/src/machineconfig/settings/lf/linux/exe/
+-rw-rw-rw-   0        0        0      388 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/settings/lf/linux/exe/fzf_nano.sh
+-rw-rw-rw-   0        0        0       90 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/settings/lf/linux/exe/leftpane_previewer.sh
+-rw-rw-rw-   0        0        0      795 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/settings/lf/linux/exe/lfcd.sh
+-rw-rw-rw-   0        0        0       95 2023-03-26 01:52:23.000000 machineconfig-1.5/src/machineconfig/settings/lf/linux/exe/previewer.sh
+-rw-rw-rw-   0        0        0     7504 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/linux/icons
+-rw-rw-rw-   0        0        0     4991 2023-03-17 04:41:42.000000 machineconfig-1.5/src/machineconfig/settings/lf/linux/lfrc
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.331202 machineconfig-1.5/src/machineconfig/settings/lf/windows/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.336620 machineconfig-1.5/src/machineconfig/settings/lf/windows/autocall/
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/autocall/delete.ps1
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/autocall/on-cd.ps1
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/autocall/on-quit.ps1
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/autocall/open.ps1
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/autocall/paste.ps1
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/autocall/pre-cd.ps1
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/autocall/rename.ps1
+-rw-rw-rw-   0        0        0      207 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/cd_tere.ps1
+-rw-rw-rw-   0        0        0      163 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/cd_zoxide.ps1
+-rw-rw-rw-   0        0        0      145 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/cd_zoxide2.ps1
+-rw-rw-rw-   0        0        0     3150 2023-03-19 03:41:28.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/colors
+-rw-rw-rw-   0        0        0      401 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/fzf_edit.ps1
+-rw-rw-rw-   0        0        0     7504 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/icons
+-rw-rw-rw-   0        0        0       90 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/leftpane_previewer.ps1
+-rw-rw-rw-   0        0        0      996 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/lfcd.ps1
+-rw-rw-rw-   0        0        0     4486 2023-03-17 04:49:37.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/lfrc
+-rw-rw-rw-   0        0        0       59 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/mkdir.ps1
+-rw-rw-rw-   0        0        0       65 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/mkfile.ps1
+-rw-rw-rw-   0        0        0      213 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/previewer.ps1
+-rw-rw-rw-   0        0        0        4 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lf/windows/tst.ps1
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.031792 machineconfig-1.5/src/machineconfig/settings/lvim/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.031792 machineconfig-1.5/src/machineconfig/settings/lvim/generic/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.336620 machineconfig-1.5/src/machineconfig/settings/lvim/generic/plugins_config/
+-rw-rw-rw-   0        0        0      626 2023-04-16 04:35:03.000000 machineconfig-1.5/src/machineconfig/settings/lvim/generic/plugins_config/.flake8
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.033062 machineconfig-1.5/src/machineconfig/settings/lvim/windows/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.338126 machineconfig-1.5/src/machineconfig/settings/lvim/windows/archive/
+-rw-rw-rw-   0        0        0      815 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lvim/windows/archive/config_additional.lua
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.033062 machineconfig-1.5/src/machineconfig/settings/lvim/windows/lua/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.339191 machineconfig-1.5/src/machineconfig/settings/lvim/windows/lua/user/
+-rw-rw-rw-   0        0        0      282 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/lvim/windows/lua/user/custom_config.lua
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.033569 machineconfig-1.5/src/machineconfig/settings/mprocs/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.341850 machineconfig-1.5/src/machineconfig/settings/mprocs/windows/
+-rw-rw-rw-   0        0        0      915 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/mprocs/windows/mprocs.yaml
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.035114 machineconfig-1.5/src/machineconfig/settings/shells/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.343022 machineconfig-1.5/src/machineconfig/settings/shells/bash/
+-rw-rw-rw-   0        0        0     1340 2023-04-26 01:20:08.000000 machineconfig-1.5/src/machineconfig/settings/shells/bash/init.sh
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.344574 machineconfig-1.5/src/machineconfig/settings/shells/nushell/
+-rw-rw-rw-   0        0        0    21214 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/shells/nushell/config.nu
+-rw-rw-rw-   0        0        0     2044 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/shells/nushell/env.nu
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.345580 machineconfig-1.5/src/machineconfig/settings/shells/pwsh/
+-rw-rw-rw-   0        0        0     1647 2023-04-11 07:14:49.000000 machineconfig-1.5/src/machineconfig/settings/shells/pwsh/init.ps1
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.346579 machineconfig-1.5/src/machineconfig/settings/shells/vtm/
+-rw-rw-rw-   0        0        0    18559 2023-04-26 01:20:08.000000 machineconfig-1.5/src/machineconfig/settings/shells/vtm/settings.xml
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.348085 machineconfig-1.5/src/machineconfig/settings/shells/wt/
+-rw-rw-rw-   0        0        0    13192 2023-04-26 01:20:08.000000 machineconfig-1.5/src/machineconfig/settings/shells/wt/settings.json
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.036524 machineconfig-1.5/src/machineconfig/settings/svim/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.349108 machineconfig-1.5/src/machineconfig/settings/svim/linux/
+-rw-rw-rw-   0        0        0     1496 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/svim/linux/init.toml
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.350234 machineconfig-1.5/src/machineconfig/settings/svim/windows/
+-rw-rw-rw-   0        0        0     1484 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/svim/windows/init.toml
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.351671 machineconfig-1.5/src/machineconfig/settings/tere/
+-rw-rw-rw-   0        0        0      183 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/tere/terecd.ps1
+-rw-rw-rw-   0        0        0       95 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/tere/terecd.sh
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.352677 machineconfig-1.5/src/machineconfig/settings/tmux/
+-rw-rw-rw-   0        0        0       60 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/tmux/.tmate.conf
+-rw-rw-rw-   0        0        0      100 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/tmux/.tmux.conf
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.353677 machineconfig-1.5/src/machineconfig/settings/wsl/
+-rw-rw-rw-   0        0        0     1314 2023-04-03 04:25:43.000000 machineconfig-1.5/src/machineconfig/settings/wsl/.wslconfig
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.355823 machineconfig-1.5/src/machineconfig/settings/zellij/
+-rw-rw-rw-   0        0        0    10624 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/zellij/config.kdl
+-rw-rw-rw-   0        0        0    10644 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/zellij/config.orig.kdl
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.356850 machineconfig-1.5/src/machineconfig/settings/zellij/layouts/
+-rw-rw-rw-   0        0        0      316 2023-04-08 23:43:48.000000 machineconfig-1.5/src/machineconfig/settings/zellij/layouts/hist
+-rw-rw-rw-   0        0        0      571 2023-04-19 23:50:38.000000 machineconfig-1.5/src/machineconfig/settings/zellij/layouts/st.kdl
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.358355 machineconfig-1.5/src/machineconfig/settings/zellij/themes/
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/settings/zellij/themes/mytheme.kdl
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.040090 machineconfig-1.5/src/machineconfig/setup_linux/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.359360 machineconfig-1.5/src/machineconfig/setup_linux/nix/
+-rw-rw-rw-   0        0        0     4540 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/setup_linux/nix/cli_installation.sh
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.362958 machineconfig-1.5/src/machineconfig/setup_linux/others/
+-rw-rw-rw-   0        0        0      424 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/setup_linux/others/archive
+-rw-rw-rw-   0        0        0      479 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/setup_linux/others/chrome.sh
+-rw-rw-rw-   0        0        0      424 2023-03-30 22:29:06.000000 machineconfig-1.5/src/machineconfig/setup_linux/others/openssh-server_add_pub_key.sh
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.368260 machineconfig-1.5/src/machineconfig/setup_linux/web_shortcuts/
+-rw-rw-rw-   0        0        0      930 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/setup_linux/web_shortcuts/all.sh
+-rw-rw-rw-   0        0        0     1534 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/setup_linux/web_shortcuts/ascii_art.sh
+-rw-rw-rw-   0        0        0      606 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/setup_linux/web_shortcuts/croshell.sh
+-rw-rw-rw-   0        0        0      573 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/setup_linux/web_shortcuts/ssh.sh
+-rw-rw-rw-   0        0        0      447 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/setup_linux/web_shortcuts/update_system.sh
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.368260 machineconfig-1.5/src/machineconfig/setup_windows/
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/setup_windows/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.372713 machineconfig-1.5/src/machineconfig/setup_windows/others/
+-rw-rw-rw-   0        0        0      318 2023-03-29 22:18:40.000000 machineconfig-1.5/src/machineconfig/setup_windows/others/docker.ps1
+-rw-rw-rw-   0        0        0       78 2023-03-05 08:45:12.000000 machineconfig-1.5/src/machineconfig/setup_windows/others/obs.ps1
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.378130 machineconfig-1.5/src/machineconfig/setup_windows/web_shortcuts/
+-rw-rw-rw-   0        0        0      854 2023-03-30 22:29:06.000000 machineconfig-1.5/src/machineconfig/setup_windows/web_shortcuts/all.ps1
+-rw-rw-rw-   0        0        0     1200 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/setup_windows/web_shortcuts/ascii_art.ps1
+-rw-rw-rw-   0        0        0      770 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/setup_windows/web_shortcuts/croshell.ps1
+-rw-rw-rw-   0        0        0      328 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/setup_windows/web_shortcuts/ssh.ps1
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.382212 machineconfig-1.5/src/machineconfig/setup_windows/wt_and_pwsh/
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/setup_windows/wt_and_pwsh/__init__.py
+-rw-rw-rw-   0        0        0      705 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/setup_windows/wt_and_pwsh/install_fonts.ps1
+-rw-rw-rw-   0        0        0     2242 2023-03-05 01:43:35.000000 machineconfig-1.5/src/machineconfig/setup_windows/wt_and_pwsh/set_pwsh_theme.py
+-rw-rw-rw-   0        0        0     6097 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/setup_windows/wt_and_pwsh/set_wt_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.385916 machineconfig-1.5/src/machineconfig/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/utils/__init__.py
+-rw-rw-rw-   0        0        0     2969 2023-05-10 23:52:37.000000 machineconfig-1.5/src/machineconfig/utils/procs.py
+-rw-rw-rw-   0        0        0      205 2023-03-04 22:55:51.000000 machineconfig-1.5/src/machineconfig/utils/to_exe.py
+-rw-rw-rw-   0        0        0    12285 2023-05-18 09:15:06.000000 machineconfig-1.5/src/machineconfig/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:20:22.049233 machineconfig-1.5/src/machineconfig.egg-info/
+-rw-rw-rw-   0        0        0     5289 2023-06-09 00:20:21.000000 machineconfig-1.5/src/machineconfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    17138 2023-06-09 00:20:21.000000 machineconfig-1.5/src/machineconfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 00:20:21.000000 machineconfig-1.5/src/machineconfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-09 00:20:21.000000 machineconfig-1.5/src/machineconfig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 00:20:21.000000 machineconfig-1.5/src/machineconfig.egg-info/top_level.txt
```

### Comparing `machineconfig-1.4/PKG-INFO` & `machineconfig-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineconfig
-Version: 1.4
+Version: 1.5
 Summary: Dotfiles management package
 Home-page: https://github.com/thisismygitrepo/machineconfig
 Author: Alex Al-Saffar
 Author-email: programmer@usa.com
 Project-URL: Bug Tracker, https://github.com/thisismygitrepo/machineconfig/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `machineconfig-1.4/README.md` & `machineconfig-1.5/README.md`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/setup.py` & `machineconfig-1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import setuptools
 from src.machineconfig import __version__
-
+# this is a comment
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="machineconfig",
     version=__version__,
     author="Alex Al-Saffar",
@@ -27,8 +27,7 @@
     python_requires=">=3.9",
     install_requires=[
     "rich",
     ],
     
 )
 
-# todo create a link to where this setup is. in .machoneconfig
```

### Comparing `machineconfig-1.4/src/machineconfig/jobs/linux/archive/get_latest_release.sh` & `machineconfig-1.5/src/machineconfig/jobs/linux/archive/get_latest_release.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/linux/archive/install_bandwich.sh` & `machineconfig-1.5/src/machineconfig/jobs/linux/archive/install_bandwich.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/linux/archive/install_diskonaut.sh` & `machineconfig-1.5/src/machineconfig/jobs/linux/archive/install_diskonaut.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/linux/archive/install_nu.sh` & `machineconfig-1.5/src/machineconfig/jobs/linux/archive/install_nu.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/linux/archive/install_zellij.sh` & `machineconfig-1.5/src/machineconfig/jobs/linux/archive/install_zellij.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/linux/archive/lf.sh` & `machineconfig-1.5/src/machineconfig/jobs/linux/archive/lf.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/linux/archive/quirks.sh` & `machineconfig-1.5/src/machineconfig/jobs/linux/archive/quirks.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python/__pycache__/python_linux_installers_all.cpython-39.pyc` & `machineconfig-1.5/src/machineconfig/jobs/python/__pycache__/python_linux_installers_all.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python/__pycache__/python_ve_symlink.cpython-39.pyc` & `machineconfig-1.5/src/machineconfig/jobs/python/__pycache__/python_ve_symlink.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python/__pycache__/python_windows_installers_all.cpython-39.pyc` & `machineconfig-1.5/src/machineconfig/jobs/python/__pycache__/python_windows_installers_all.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python/check_installations.py` & `machineconfig-1.5/src/machineconfig/jobs/python/check_installations.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python/create_bootable_media.py` & `machineconfig-1.5/src/machineconfig/jobs/python/create_bootable_media.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python/python_cargo_build_share.py` & `machineconfig-1.5/src/machineconfig/jobs/python/python_cargo_build_share.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python/python_linux_installers_all.py` & `machineconfig-1.5/src/machineconfig/jobs/python/python_linux_installers_all.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python/python_ve_installer.py` & `machineconfig-1.5/src/machineconfig/jobs/python/python_ve_installer.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,13 +60,14 @@
     scripts = scripts.replace(predef_script, lines)
 
     if repos == "y":
         text = lib_root.joinpath(f"setup_{system.lower()}/repos.{'ps1' if system == 'Windows' else 'sh'}").read_text()
         text = tb.modify_text(txt_raw=text, txt_search="ve_name=", txt_alt=f"{variable_prefix}ve_name='{env_name}'", replace_line=True)
         scripts += text
 
-    write_shell_script(scripts, desc="Script to create ve environment")
-    return None
+#    write_shell_script(scripts, desc="Script to create ve environment")
+    return scripts
 
 
 if __name__ == '__main__':
     pass
+
```

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python/python_ve_symlink.py` & `machineconfig-1.5/src/machineconfig/jobs/python/python_ve_symlink.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python/python_windows_installers_all.py` & `machineconfig-1.5/src/machineconfig/jobs/python/python_windows_installers_all.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/archive/strongbox.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/archive/strongbox.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/broot.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/broot.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/cpufetch.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/cpufetch.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/delta.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/delta.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/bw.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/bw.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/evcxr.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/evcxr.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/kondo.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/kondo.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/lvim.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/lvim.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,28 +8,53 @@
 
 
 def main(version=None):
     _ = version
     if system() == "Windows":
         tb.P.home().joinpath(r"AppData/Local/lvim").delete(sure=True)
         # tb.P.home().joinpath("AppData/Roaming/lunarvim").delete(sure=True)
-        install_script = "$LV_BRANCH='release-1.2/neovim-0.8'; Invoke-WebRequest https://raw.githubusercontent.com/LunarVim/LunarVim/master/utils/installer/install.ps1 -UseBasicParsing | Invoke-Expression"
+        install_script = """pwsh -c "`$LV_BRANCH='release-1.3/neovim-0.9'; iwr https://raw.githubusercontent.com/LunarVim/LunarVim/release-1.3/neovim-0.9/utils/installer/install.ps1 -UseBasicParsing | iex" """
         # install_script = "Invoke-WebRequest    https://raw.githubusercontent.com/LunarVim/LunarVim/master/utils/installer/install.ps1 -UseBasicParsing | Invoke-Expression"
         uninstall_script = "Invoke-WebRequest https://raw.githubusercontent.com/LunarVim/LunarVim/master/utils/installer/uninstall.ps1 -UseBasicParsing | Invoke-Expression"
-        script = f"""{uninstall_script} ; {install_script}
+        script = f"""
+# uninstall then install latest stable release as per https://www.lunarvim.org/docs/installation
+{uninstall_script}
+{install_script}        
 cd ~/AppData/Local
+rm lvim -Force  # kill bad symlinks there
 git clone https://github.com/ChristianChiarulli/lvim
+pip install pynvim
+pip install flake8
+pip install black
 """
-        # tb.T().run(script, shell="pwsh")
         # tb.P(r"AppData/Local/lvim").joinpath("config.lua").append_text(tb.P(machineconfig.__file__).joinpath("src/machineconfig/settings/lvim_windows/config_additional.lua").read_text())
         return script
     else:
         tb.P.home().joinpath(".config/lvim").delete(sure=True)
-        install_script = "LV_BRANCH='release-1.2/neovim-0.8' bash <(curl -s https://raw.githubusercontent.com/lunarvim/lunarvim/master/utils/installer/install.sh)"
-        # install_script = r"bash <(curl -s https://raw.githubusercontent.com/LunarVim/LunarVim/rolling/utils/installer/install-neovim-from-release)"
-        # script = install_script
-        # tb.T().run(script, shell="pwsh")
+        install_script = f"""
+
+# uninstall then install latest stable release:
+# from https://www.lunarvim.org/docs/installation
+bash <(curl -s https://raw.githubusercontent.com/lunarvim/lunarvim/master/utils/installer/uninstall.sh)
+sudo rm -rdf ~/.config/lvim || true  # kill bad symlinks there
+LV_BRANCH='release-1.3/neovim-0.9' bash <(curl -s https://raw.githubusercontent.com/LunarVim/LunarVim/release-1.3/neovim-0.9/utils/installer/install.sh)
+export lvim="$HOME/.local/bin/lvim"
+
+# config from Chris
+sudo rm -rdf ~/.config/lvim || true # kill bad symlinks there
+cd ~/.config
+git clone https://github.com/ChristianChiarulli/lvim
+sudo apt install xsel
+
+pip install pynvim
+pip install flake8
+
+#lvim --headless + 'autocmd User PackerComplete quitall' +PackerSync
+# :PackerSync
+# :Copilot setup
+
+"""
         return install_script
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/qrcp.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/qrcp.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/qrscan.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/qrscan.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/rust-analyzer.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/rust-analyzer.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/termscp.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/termscp.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/tldr.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/tldr.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dev/tokei.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dev/tokei.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/diskonaut.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/diskonaut.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/dua.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/dua.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/gitui.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/gitui.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/gopass.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/gopass.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/helix.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/helix.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/lf.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/lf.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/mprocs.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/mprocs.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/navi.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/navi.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/ots.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/ots.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/ouch.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/ouch.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/pomodoro.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/pomodoro.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/procs.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/procs.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/rclone.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/rclone.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/tere.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/tere.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_generic_installers/watchexec.py` & `machineconfig-1.5/src/machineconfig/jobs/python_generic_installers/watchexec.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/archive/ranger.py` & `machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/archive/ranger.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/bottom.py` & `machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/bottom.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/btop.py` & `machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/btop.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/dev/bytehound.py` & `machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/dev/bytehound.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/dev/nnn.py` & `machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/dev/nnn.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/joshuto.py` & `machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/joshuto.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/viu.py` & `machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/viu.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/xplr.py` & `machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/xplr.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_linux_installers/zellij.py` & `machineconfig-1.5/src/machineconfig/jobs/python_linux_installers/zellij.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/boxes.py` & `machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/boxes.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/dev/bypass_paywall.py` & `machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/dev/bypass_paywall.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/dev/obs_background_removal_plugin.py` & `machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/dev/obs_background_removal_plugin.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/fd.py` & `machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/fd.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/fzf.py` & `machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/fzf.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/python_windows_installers/zoomit.py` & `machineconfig-1.5/src/machineconfig/jobs/python_windows_installers/zoomit.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/windows/arhive/archive_pygraphviz.ps1` & `machineconfig-1.5/src/machineconfig/jobs/windows/arhive/archive_pygraphviz.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/jobs/windows/arhive/openssh-server_copy-ssh-id.ps1` & `machineconfig-1.5/src/machineconfig/jobs/windows/arhive/openssh-server_copy-ssh-id.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/profile/__pycache__/create.cpython-39.pyc` & `machineconfig-1.5/src/machineconfig/profile/__pycache__/create.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/profile/create.py` & `machineconfig-1.5/src/machineconfig/profile/create.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/profile/patches/linux/zzellij.sh` & `machineconfig-1.5/src/machineconfig/profile/patches/linux/zzellij.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/profile/records/linux/safe_cli_apps.json` & `machineconfig-1.5/src/machineconfig/profile/records/linux/safe_cli_apps.json`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/profile/records/windows/safe_cli_apps.json` & `machineconfig-1.5/src/machineconfig/profile/records/windows/safe_cli_apps.json`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/linux/activate_ve` & `machineconfig-1.5/src/machineconfig/scripts/linux/activate_ve`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/linux/cloud_mount` & `machineconfig-1.5/src/machineconfig/scripts/linux/cloud_mount`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/linux/cloud_sync` & `machineconfig-1.5/src/machineconfig/scripts/linux/cloud_sync`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/linux/fzf2g` & `machineconfig-1.5/src/machineconfig/scripts/linux/fzf2g`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/linux/fzfag` & `machineconfig-1.5/src/machineconfig/scripts/linux/fzfag`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/linux/fzffg` & `machineconfig-1.5/src/machineconfig/scripts/linux/fzffg`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/linux/fzfg` & `machineconfig-1.5/src/machineconfig/scripts/linux/fzfg`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/linux/mount_drive` & `machineconfig-1.5/src/machineconfig/scripts/linux/mount_drive`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-#!/usr/bin/env bash
-
-# Mount on linux
-# Lsblk
-
-lsblk
-# read device name from user input and choose default value of sdb1
-read -p "Enter device name (default: sdb1): " device
-# if user input is empty, set device to sdb1
-device=${device:-sdb1}
-read -p "Enter mount name (default: mymnt): " mnt_name
-mnt_name=${mnt_name:-mymnt}
-sudo mkdir -p /media/$mnt_name  # Make sure to create the mounting directory.
-
-# check if drive is bitlocker encrypted then print encryption type else print not encrypted
-if ! command -v dislocker &> /dev/null
-then
-    echo "dislocker could not be found"
-    echo "Installing dislocker"
-    sudo apt install dislocker
-fi
-
-
-# bitlocker_status=$(sudo bash -c "ls /sys/class/block/$(basename $device)/holders/ | grep -o bitlocker")
-bitlocker_status=$(lsblk -o FSTYPE "/dev/$device" | grep -o BitLocker)
-
-if [ "$bitlocker_status" = "BitLocker" ];  then
-    echo ">>>>>> Drive is bitlocker encrypted, therefore, bitlocker is needded"
-    # If drive is bitlocker , following: https://www.linuxuprising.com/2019/04/how-to-mount-bitlocker-encrypted.html
-
-    # check if password is stored here: $HOME/dotfiles/creds/data/bitlocker_pwd if so, read it.
-    # if not, prompt user for password and store it in the file.
-    if [ -f "$HOME/dotfiles/creds/data/bitlocker_pwd" ]; then
-        echo ">>>>>> Bitlocker Password file detected at default location $HOME/dotfiles/creds/data/bitlocker_pwd"
-        bitlocker_pwd=$(cat $HOME/dotfiles/creds/data/bitlocker_pwd)
-    else
-        echo ">>>>>> Password file does not exist"
-        read -p "Enter bitlocker password: " bitlocker_pwd
-        echo $bitlocker_pwd > $HOME/dotfiles/creds/data/bitlocker_pwd
-    fi
-
-
-    sudo mkdir -p /media/$mnt_name"_bitlocker"
-    sudo dislocker /dev/$device -u -- /media/$mnt_name"_bitlocker" # Will be prompted for password (-u)
-    # sudo mount -o loop /media/bitlocker/dislocker-file /media/bitlockermount
-    # Modified from here to fix permissions: https://askubuntu.com/questions/1045057/i-cant-write-only-read-on-usb-device-encrypted-with-bitlocker
-    sudo mount -o loop,rw,uid=1000,gid=1000 /media/$mnt_name"_bitlocker"/dislocker-file /media/$mnt_name
-else
-    echo "Drive is not encrypted"
-    sudo mount --source /dev/$device --target /media/$mnt_name
-fi
-
-# echo a success message if mount was successful (last command) else print error message
-if [ $? -eq 0 ]; then
-    echo "The drive has been successfully mounted at /media/$mnt_name"
-    echo "--------------------------------------"
-else
-    echo "There was an error while mounting the drive. Please check your input and try again."
-    exit 1
-fi
-
-# https://askubuntu.com/questions/1059228/how-to-mount-a-usb-drive-in-ubuntu-18-04
+#!/usr/bin/env bash
+
+# Mount on linux
+# Lsblk
+
+lsblk
+# read device name from user input and choose default value of sdb1
+read -p "Enter device name (default: sdb1): " device
+# if user input is empty, set device to sdb1
+device=${device:-sdb1}
+read -p "Enter mount name (default: mymnt): " mnt_name
+mnt_name=${mnt_name:-mymnt}
+sudo mkdir -p /media/$mnt_name  # Make sure to create the mounting directory.
+
+# check if drive is bitlocker encrypted then print encryption type else print not encrypted
+if ! command -v dislocker &> /dev/null
+then
+    echo "dislocker could not be found"
+    echo "Installing dislocker"
+    sudo apt install dislocker
+fi
+
+
+# bitlocker_status=$(sudo bash -c "ls /sys/class/block/$(basename $device)/holders/ | grep -o bitlocker")
+bitlocker_status=$(lsblk -o FSTYPE "/dev/$device" | grep -o BitLocker)
+
+if [ "$bitlocker_status" = "BitLocker" ];  then
+    echo ">>>>>> Drive is bitlocker encrypted, therefore, bitlocker is needded"
+    # If drive is bitlocker , following: https://www.linuxuprising.com/2019/04/how-to-mount-bitlocker-encrypted.html
+
+    # check if password is stored here: $HOME/dotfiles/creds/data/bitlocker_pwd if so, read it.
+    # if not, prompt user for password and store it in the file.
+    if [ -f "$HOME/dotfiles/creds/data/bitlocker_pwd" ]; then
+        echo ">>>>>> Bitlocker Password file detected at default location $HOME/dotfiles/creds/data/bitlocker_pwd"
+        bitlocker_pwd=$(cat $HOME/dotfiles/creds/data/bitlocker_pwd)
+    else
+        echo ">>>>>> Password file does not exist"
+        read -p "Enter bitlocker password: " bitlocker_pwd
+        echo $bitlocker_pwd > $HOME/dotfiles/creds/data/bitlocker_pwd
+    fi
+
+
+    sudo mkdir -p /media/$mnt_name"_bitlocker"
+    sudo dislocker /dev/$device -u -- /media/$mnt_name"_bitlocker" # Will be prompted for password (-u)
+    # sudo mount -o loop /media/bitlocker/dislocker-file /media/bitlockermount
+    # Modified from here to fix permissions: https://askubuntu.com/questions/1045057/i-cant-write-only-read-on-usb-device-encrypted-with-bitlocker
+    sudo mount -o loop,rw,uid=1000,gid=1000 /media/$mnt_name"_bitlocker"/dislocker-file /media/$mnt_name
+else
+    echo "Drive is not encrypted"
+    sudo mount --source /dev/$device --target /media/$mnt_name
+fi
+
+# echo a success message if mount was successful (last command) else print error message
+if [ $? -eq 0 ]; then
+    echo "The drive has been successfully mounted at /media/$mnt_name"
+    echo "--------------------------------------"
+else
+    echo "There was an error while mounting the drive. Please check your input and try again."
+    exit 1
+fi
+
+# https://askubuntu.com/questions/1059228/how-to-mount-a-usb-drive-in-ubuntu-18-04
```

### Comparing `machineconfig-1.4/src/machineconfig/scripts/linux/mount_nfs` & `machineconfig-1.5/src/machineconfig/scripts/linux/mount_nfs`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/linux/mount_nw_drive` & `machineconfig-1.5/src/machineconfig/scripts/linux/mount_nw_drive`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/linux/repos` & `machineconfig-1.5/src/machineconfig/scripts/linux/repos`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/linux/transfer.sh` & `machineconfig-1.5/src/machineconfig/scripts/linux/transfer.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/linux/z_ls` & `machineconfig-1.5/src/machineconfig/scripts/linux/z_ls`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/__pycache__/cloud_mount.cpython-39.pyc` & `machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/cloud_mount.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/__pycache__/cloud_rx.cpython-39.pyc` & `machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/cloud_rx.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/__pycache__/cloud_sx.cpython-39.pyc` & `machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/cloud_sx.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Mar  4 22:55:51 2023 UTC, .py size: 1980 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,108 +1,111 @@
-00000000: 610d 0d0a 0000 0000 77cc 0364 bc07 0000  a.......w..d....
+00000000: 610d 0d0a 0000 0000 2320 3264 dd07 0000  a.......# 2d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6401 6c03  d.l.m.Z...d.d.l.
-00000040: 5a03 6402 6403 8400 5a04 6505 6404 6b02  Z.d.d...Z.e.d.k.
-00000050: 722a 6504 8300 0100 6401 5300 2905 e900  r*e.....d.S.)...
-00000060: 0000 004e 6300 0000 0000 0000 0000 0000  ...Nc...........
-00000070: 0005 0000 000a 0000 0043 0000 0073 6c01  .........C...sl.
-00000080: 0000 7400 6a01 6401 6402 8d01 7d00 7c00  ..t.j.d.d...}.|.
-00000090: 6a02 6403 6404 6405 8d02 0100 7c00 6a02  j.d.d.d.....|.j.
-000000a0: 6406 6407 6408 6409 640a 8d04 0100 7c00  d.d.d.d.d.....|.
-000000b0: 6a02 640b 640c 640d 6409 640a 8d04 0100  j.d.d.d.d.d.....
-000000c0: 7c00 6a02 640e 640f 6410 6409 640a 8d04  |.j.d.d.d.d.d...
-000000d0: 0100 7c00 6a02 6411 6412 6413 6409 640a  ..|.j.d.d.d.d.d.
-000000e0: 8d04 0100 7c00 6a02 6414 6415 6416 6409  ....|.j.d.d.d.d.
-000000f0: 640a 8d04 0100 7c00 6a02 6417 6418 6419  d.....|.j.d.d.d.
-00000100: 6400 641a 8d04 0100 7c00 6a02 641b 641c  d.d.....|.j.d.d.
-00000110: 641d 641e 641a 8d04 0100 7c00 6a02 641f  d.d.d.....|.j.d.
-00000120: 6420 6421 6400 641a 8d04 0100 7c00 6a02  d d!d.d.....|.j.
-00000130: 6422 6423 6424 6400 641a 8d04 0100 7c00  d"d#d$d.d.....|.
-00000140: a003 a100 7d01 7c01 6a04 6400 7500 9001  ....}.|.j.d.u...
-00000150: 721e 7405 6a06 a007 a100 a008 6425 a101  r.t.j.......d%..
-00000160: 7d02 7a14 7c02 a009 a100 a00a 6426 641e  }.z.|.......d&d.
-00000170: a102 7d03 5700 6e26 0400 740b 9001 791a  ..}.W.n&..t...y.
-00000180: 0100 0100 0100 740c 6427 7c02 9b00 6428  ......t.d'|...d(
-00000190: 9d03 8301 0100 5900 641e 5300 3000 6e06  ......Y.d.S.0.n.
-000001a0: 7c01 6a04 7d03 7405 a006 7c01 6a0d a101  |.j.}.t...|.j...
-000001b0: 6a0e 7c03 7c01 6a0f 7c01 6a10 7c01 6a11  j.|.|.j.|.j.|.j.
-000001c0: 7c01 6a12 7c01 6a13 7c01 6a14 7c01 6a15  |.j.|.j.|.j.|.j.
-000001d0: 6429 8d08 7d04 7c01 6a11 9001 7268 740c  d)..}.|.j...rht.
-000001e0: 7c04 a016 a100 8301 0100 6400 5300 292a  |.........d.S.)*
-000001f0: 4e7a 1543 6c6f 7564 204d 616e 6167 656d  Nz.Cloud Managem
-00000200: 656e 7420 434c 492e 2901 5a0b 6465 7363  ent CLI.).Z.desc
-00000210: 7269 7074 696f 6eda 0466 696c 657a 1166  ription..filez.f
-00000220: 696c 652f 666f 6c64 6572 2070 6174 682e  ile/folder path.
-00000230: 2901 da04 6865 6c70 7a05 2d2d 7a69 707a  )...helpz.--zipz
-00000240: 022d 7a7a 135a 6970 2062 6566 6f72 6520  .-zz.Zip before 
-00000250: 7365 6e64 696e 672e 5a0a 7374 6f72 655f  sending.Z.store_
-00000260: 7472 7565 2902 7203 0000 00da 0661 6374  true).r......act
-00000270: 696f 6e7a 092d 2d65 6e63 7279 7074 7a02  ionz.--encryptz.
-00000280: 2d65 7a17 456e 6372 7970 7420 6265 666f  -ez.Encrypt befo
-00000290: 7265 2073 656e 6469 6e67 2e7a 122d 2d72  re sending.z.--r
-000002a0: 656c 6174 6976 655f 746f 5f68 6f6d 657a  elative_to_homez
-000002b0: 022d 727a 2c73 6574 2072 656d 6f74 6520  .-rz,set remote 
-000002c0: 7061 7468 2061 7320 686f 6d65 2072 656c  path as home rel
-000002d0: 6174 6976 6520 6c6f 6361 6c20 7061 7468  ative local path
-000002e0: 2e7a 0d2d 2d6f 735f 7370 6563 6966 6963  .z.--os_specific
-000002f0: 7a02 2d6f 7a45 4f53 2073 7065 6369 6669  z.-ozEOS specifi
-00000300: 6320 7061 7468 2028 7265 6c65 7661 6e74  c path (relevant
-00000310: 206f 6e6c 7920 7768 656e 2072 656c 6174   only when relat
-00000320: 6976 6520 666c 6167 2069 7320 7261 6973  ive flag is rais
-00000330: 6564 2061 7320 7765 6c6c 2e7a 072d 2d73  ed as well.z.--s
-00000340: 6861 7265 7a02 2d73 7a0b 5368 6172 6520  harez.-sz.Share 
-00000350: 6669 6c65 2e7a 072d 2d63 6c6f 7564 7a02  file.z.--cloudz.
-00000360: 2d63 7a1a 7263 6c6f 6e65 2063 6c6f 7564  -cz.rclone cloud
-00000370: 2070 726f 6669 6c65 206e 616d 652e 2902   profile name.).
-00000380: 7203 0000 00da 0764 6566 6175 6c74 7a0c  r......defaultz.
-00000390: 2d2d 7265 6d6f 7465 5f64 6972 7a02 2d64  --remote_dirz.-d
-000003a0: 7a1c 5265 6d6f 7465 2064 6972 6563 746f  z.Remote directo
-000003b0: 7279 2074 6f20 7365 6e64 2074 6f2e da00  ry to send to...
-000003c0: 7a05 2d2d 6b65 797a 022d 6b7a 124b 6579  z.--keyz.-kz.Key
-000003d0: 2066 6f72 2065 6e63 7279 7074 696f 6e7a   for encryptionz
-000003e0: 052d 2d70 7764 7a02 2d70 7a17 5061 7373  .--pwdz.-pz.Pass
-000003f0: 776f 7264 2066 6f72 2065 6e63 7279 7074  word for encrypt
-00000400: 696f 6e7a 2364 6f74 6669 6c65 732f 636f  ionz#dotfiles/co
-00000410: 6e66 6967 2f73 6574 7570 2f72 636c 6f6e  nfig/setup/rclon
-00000420: 655f 7265 6d6f 7465 da01 0a7a 194e 6f20  e_remote...z.No 
-00000430: 636c 6f75 6420 7072 6f66 696c 6520 666f  cloud profile fo
-00000440: 756e 6420 4020 7a38 2c20 706c 6561 7365  und @ z8, please
-00000450: 2073 6574 206f 6e65 2075 7020 6f72 2070   set one up or p
-00000460: 726f 7669 6465 206f 6e65 2076 6961 2074  rovide one via t
-00000470: 6865 202d 2d63 6c6f 7564 2066 6c61 672e  he --cloud flag.
-00000480: 2908 da05 636c 6f75 64da 037a 6970 5a08  )...cloud..zipZ.
-00000490: 7265 6c32 686f 6d65 da05 7368 6172 65da  rel2home..share.
-000004a0: 036b 6579 da03 7077 64da 0765 6e63 7279  .key..pwd..encry
-000004b0: 7074 da0b 6f73 5f73 7065 6369 6669 6329  pt..os_specific)
-000004c0: 17da 0861 7267 7061 7273 655a 0e41 7267  ...argparseZ.Arg
-000004d0: 756d 656e 7450 6172 7365 725a 0c61 6464  umentParserZ.add
-000004e0: 5f61 7267 756d 656e 745a 0a70 6172 7365  _argumentZ.parse
-000004f0: 5f61 7267 7372 0800 0000 da02 7462 da01  _argsr......tb..
-00000500: 50da 0468 6f6d 65da 086a 6f69 6e70 6174  P..home..joinpat
-00000510: 68da 0972 6561 645f 7465 7874 da07 7265  h..read_text..re
-00000520: 706c 6163 65da 1146 696c 654e 6f74 466f  place..FileNotFo
-00000530: 756e 6445 7272 6f72 da05 7072 696e 7472  undError..printr
-00000540: 0200 0000 5a08 746f 5f63 6c6f 7564 7209  ....Z.to_cloudr.
-00000550: 0000 005a 1072 656c 6174 6976 655f 746f  ...Z.relative_to
-00000560: 5f68 6f6d 6572 0a00 0000 720b 0000 0072  _homer....r....r
-00000570: 0c00 0000 720d 0000 0072 0e00 0000 5a0a  ....r....r....Z.
-00000580: 6173 5f75 726c 5f73 7472 2905 5a06 7061  as_url_str).Z.pa
-00000590: 7273 6572 da04 6172 6773 da05 5f70 6174  rser..args.._pat
-000005a0: 6872 0800 0000 da03 7265 73a9 0072 1b00  hr......res..r..
-000005b0: 0000 fa4d 633a 5c75 7365 7273 5c61 6c65  ...Mc:\users\ale
-000005c0: 785c 636f 6465 5c6d 6163 6869 6e65 636f  x\code\machineco
-000005d0: 6e66 6967 5c73 7263 5c6d 6163 6869 6e65  nfig\src\machine
-000005e0: 636f 6e66 6967 5c73 6372 6970 7473 5c70  config\scripts\p
-000005f0: 7974 686f 6e5c 636c 6f75 645f 7378 2e70  ython\cloud_sx.p
-00000600: 79da 0b61 7267 735f 7061 7273 6572 0700  y..args_parser..
-00000610: 0000 732e 0000 0000 010c 030e 0212 0112  ..s.............
-00000620: 0112 0112 0112 0212 0112 0112 0112 0208  ................
-00000630: 020c 0110 0116 010e 0110 010a 0106 0216  ................
-00000640: 0114 ff06 0272 1d00 0000 da08 5f5f 6d61  .....r......__ma
-00000650: 696e 5f5f 2906 5a11 6372 6f63 6f64 696c  in__).Z.crocodil
-00000660: 652e 746f 6f6c 626f 785a 0774 6f6f 6c62  e.toolboxZ.toolb
-00000670: 6f78 7210 0000 0072 0f00 0000 721d 0000  oxr....r....r...
-00000680: 00da 085f 5f6e 616d 655f 5f72 1b00 0000  ...__name__r....
-00000690: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
-000006a0: 083c 6d6f 6475 6c65 3e02 0000 0073 0800  .<module>....s..
-000006b0: 0000 0c01 0804 0820 0801                 ....... ..
+00000040: 5a03 6400 6402 6c04 6d05 5a05 0100 6505  Z.d.d.l.m.Z...e.
+00000050: 6403 6404 8400 8301 5a06 6507 6405 6b02  d.d.....Z.e.d.k.
+00000060: 723a 6506 8300 0100 6401 5300 2906 e900  r:e.....d.S.)...
+00000070: 0000 004e 2901 da05 476f 6f65 7963 0000  ...N)...Gooeyc..
+00000080: 0000 0000 0000 0000 0000 0500 0000 0a00  ................
+00000090: 0000 4300 0000 736c 0100 0074 006a 0164  ..C...sl...t.j.d
+000000a0: 0164 028d 017d 007c 006a 0264 0364 0464  .d...}.|.j.d.d.d
+000000b0: 058d 0201 007c 006a 0264 0664 0764 0864  .....|.j.d.d.d.d
+000000c0: 0964 0a8d 0401 007c 006a 0264 0b64 0c64  .d.....|.j.d.d.d
+000000d0: 0d64 0964 0a8d 0401 007c 006a 0264 0e64  .d.d.....|.j.d.d
+000000e0: 0f64 1064 0964 0a8d 0401 007c 006a 0264  .d.d.d.....|.j.d
+000000f0: 1164 1264 1364 0964 0a8d 0401 007c 006a  .d.d.d.d.....|.j
+00000100: 0264 1464 1564 1664 0964 0a8d 0401 007c  .d.d.d.d.d.....|
+00000110: 006a 0264 1764 1864 1964 0064 1a8d 0401  .j.d.d.d.d.d....
+00000120: 007c 006a 0264 1b64 1c64 1d64 1e64 1a8d  .|.j.d.d.d.d.d..
+00000130: 0401 007c 006a 0264 1f64 2064 2164 0064  ...|.j.d.d d!d.d
+00000140: 1a8d 0401 007c 006a 0264 2264 2364 2464  .....|.j.d"d#d$d
+00000150: 0064 1a8d 0401 007c 00a0 03a1 007d 017c  .d.....|.....}.|
+00000160: 016a 0464 0075 0090 0172 1e74 056a 06a0  .j.d.u...r.t.j..
+00000170: 07a1 00a0 0864 25a1 017d 027a 147c 02a0  .....d%..}.z.|..
+00000180: 09a1 00a0 0a64 2664 1ea1 027d 0357 006e  .....d&d...}.W.n
+00000190: 2604 0074 0b90 0179 1a01 0001 0001 0074  &..t...y.......t
+000001a0: 0c64 277c 029b 0064 289d 0383 0101 0059  .d'|...d(......Y
+000001b0: 0064 1e53 0030 006e 067c 016a 047d 0374  .d.S.0.n.|.j.}.t
+000001c0: 05a0 067c 016a 0da1 016a 0e7c 037c 016a  ...|.j...j.|.|.j
+000001d0: 0f7c 016a 107c 016a 117c 016a 127c 016a  .|.j.|.j.|.j.|.j
+000001e0: 137c 016a 147c 016a 1564 298d 087d 047c  .|.j.|.j.d)..}.|
+000001f0: 016a 1190 0172 6874 0c7c 04a0 16a1 0083  .j...rht.|......
+00000200: 0101 0064 0053 0029 2a4e 7a15 436c 6f75  ...d.S.)*Nz.Clou
+00000210: 6420 4d61 6e61 6765 6d65 6e74 2043 4c49  d Management CLI
+00000220: 2e29 015a 0b64 6573 6372 6970 7469 6f6e  .).Z.description
+00000230: da04 6669 6c65 7a11 6669 6c65 2f66 6f6c  ..filez.file/fol
+00000240: 6465 7220 7061 7468 2e29 01da 0468 656c  der path.)...hel
+00000250: 707a 052d 2d7a 6970 7a02 2d7a 7a13 5a69  pz.--zipz.-zz.Zi
+00000260: 7020 6265 666f 7265 2073 656e 6469 6e67  p before sending
+00000270: 2e5a 0a73 746f 7265 5f74 7275 6529 0272  .Z.store_true).r
+00000280: 0400 0000 da06 6163 7469 6f6e 7a09 2d2d  ......actionz.--
+00000290: 656e 6372 7970 747a 022d 657a 1745 6e63  encryptz.-ez.Enc
+000002a0: 7279 7074 2062 6566 6f72 6520 7365 6e64  rypt before send
+000002b0: 696e 672e 7a12 2d2d 7265 6c61 7469 7665  ing.z.--relative
+000002c0: 5f74 6f5f 686f 6d65 7a02 2d72 7a2c 7365  _to_homez.-rz,se
+000002d0: 7420 7265 6d6f 7465 2070 6174 6820 6173  t remote path as
+000002e0: 2068 6f6d 6520 7265 6c61 7469 7665 206c   home relative l
+000002f0: 6f63 616c 2070 6174 682e 7a0d 2d2d 6f73  ocal path.z.--os
+00000300: 5f73 7065 6369 6669 637a 022d 6f7a 454f  _specificz.-ozEO
+00000310: 5320 7370 6563 6966 6963 2070 6174 6820  S specific path 
+00000320: 2872 656c 6576 616e 7420 6f6e 6c79 2077  (relevant only w
+00000330: 6865 6e20 7265 6c61 7469 7665 2066 6c61  hen relative fla
+00000340: 6720 6973 2072 6169 7365 6420 6173 2077  g is raised as w
+00000350: 656c 6c2e 7a07 2d2d 7368 6172 657a 022d  ell.z.--sharez.-
+00000360: 737a 0b53 6861 7265 2066 696c 652e 7a07  sz.Share file.z.
+00000370: 2d2d 636c 6f75 647a 022d 637a 1a72 636c  --cloudz.-cz.rcl
+00000380: 6f6e 6520 636c 6f75 6420 7072 6f66 696c  one cloud profil
+00000390: 6520 6e61 6d65 2e29 0272 0400 0000 da07  e name.).r......
+000003a0: 6465 6661 756c 747a 0c2d 2d72 656d 6f74  defaultz.--remot
+000003b0: 655f 6469 727a 022d 647a 1c52 656d 6f74  e_dirz.-dz.Remot
+000003c0: 6520 6469 7265 6374 6f72 7920 746f 2073  e directory to s
+000003d0: 656e 6420 746f 2eda 007a 052d 2d6b 6579  end to...z.--key
+000003e0: 7a02 2d6b 7a12 4b65 7920 666f 7220 656e  z.-kz.Key for en
+000003f0: 6372 7970 7469 6f6e 7a05 2d2d 7077 647a  cryptionz.--pwdz
+00000400: 022d 707a 1750 6173 7377 6f72 6420 666f  .-pz.Password fo
+00000410: 7220 656e 6372 7970 7469 6f6e 7a23 646f  r encryptionz#do
+00000420: 7466 696c 6573 2f63 6f6e 6669 672f 7365  tfiles/config/se
+00000430: 7475 702f 7263 6c6f 6e65 5f72 656d 6f74  tup/rclone_remot
+00000440: 65da 010a 7a19 4e6f 2063 6c6f 7564 2070  e...z.No cloud p
+00000450: 726f 6669 6c65 2066 6f75 6e64 2040 207a  rofile found @ z
+00000460: 382c 2070 6c65 6173 6520 7365 7420 6f6e  8, please set on
+00000470: 6520 7570 206f 7220 7072 6f76 6964 6520  e up or provide 
+00000480: 6f6e 6520 7669 6120 7468 6520 2d2d 636c  one via the --cl
+00000490: 6f75 6420 666c 6167 2e29 08da 0563 6c6f  oud flag.)...clo
+000004a0: 7564 da03 7a69 705a 0872 656c 3268 6f6d  ud..zipZ.rel2hom
+000004b0: 65da 0573 6861 7265 da03 6b65 79da 0370  e..share..key..p
+000004c0: 7764 da07 656e 6372 7970 74da 0b6f 735f  wd..encrypt..os_
+000004d0: 7370 6563 6966 6963 2917 da08 6172 6770  specific)...argp
+000004e0: 6172 7365 5a0e 4172 6775 6d65 6e74 5061  arseZ.ArgumentPa
+000004f0: 7273 6572 5a0c 6164 645f 6172 6775 6d65  rserZ.add_argume
+00000500: 6e74 5a0a 7061 7273 655f 6172 6773 7209  ntZ.parse_argsr.
+00000510: 0000 00da 0274 62da 0150 da04 686f 6d65  .....tb..P..home
+00000520: da08 6a6f 696e 7061 7468 da09 7265 6164  ..joinpath..read
+00000530: 5f74 6578 74da 0772 6570 6c61 6365 da11  _text..replace..
+00000540: 4669 6c65 4e6f 7446 6f75 6e64 4572 726f  FileNotFoundErro
+00000550: 72da 0570 7269 6e74 7203 0000 005a 0874  r..printr....Z.t
+00000560: 6f5f 636c 6f75 6472 0a00 0000 5a10 7265  o_cloudr....Z.re
+00000570: 6c61 7469 7665 5f74 6f5f 686f 6d65 720b  lative_to_homer.
+00000580: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000590: 0000 720f 0000 005a 0a61 735f 7572 6c5f  ..r....Z.as_url_
+000005a0: 7374 7229 055a 0670 6172 7365 72da 0461  str).Z.parser..a
+000005b0: 7267 73da 055f 7061 7468 7209 0000 00da  rgs.._pathr.....
+000005c0: 0372 6573 a900 721c 0000 00fa 4d63 3a5c  .res..r.....Mc:\
+000005d0: 7573 6572 735c 616c 6578 5c63 6f64 655c  users\alex\code\
+000005e0: 6d61 6368 696e 6563 6f6e 6669 675c 7372  machineconfig\sr
+000005f0: 635c 6d61 6368 696e 6563 6f6e 6669 675c  c\machineconfig\
+00000600: 7363 7269 7074 735c 7079 7468 6f6e 5c63  scripts\python\c
+00000610: 6c6f 7564 5f73 782e 7079 da0b 6172 6773  loud_sx.py..args
+00000620: 5f70 6172 7365 7208 0000 0073 2e00 0000  _parser....s....
+00000630: 0002 0c03 0e02 1201 1201 1201 1201 1202  ................
+00000640: 1201 1201 1201 1202 0802 0c01 1001 1601  ................
+00000650: 0e01 1001 0a01 0602 1601 14ff 0602 721e  ..............r.
+00000660: 0000 00da 085f 5f6d 6169 6e5f 5f29 085a  .....__main__).Z
+00000670: 1163 726f 636f 6469 6c65 2e74 6f6f 6c62  .crocodile.toolb
+00000680: 6f78 5a07 746f 6f6c 626f 7872 1100 0000  oxZ.toolboxr....
+00000690: 7210 0000 005a 0567 6f6f 6579 7202 0000  r....Z.gooeyr...
+000006a0: 0072 1e00 0000 da08 5f5f 6e61 6d65 5f5f  .r......__name__
+000006b0: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
+000006c0: 1d00 0000 da08 3c6d 6f64 756c 653e 0200  ......<module>..
+000006d0: 0000 730c 0000 000c 0108 030c 0202 010a  ..s.............
+000006e0: 2008 01                                   ..
```

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/__pycache__/devops_backup_retrieve.cpython-39.pyc` & `machineconfig-1.5/src/machineconfig/scripts/python/__pycache__/devops_backup_retrieve.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/archive/bu_gdrive_rx.py` & `machineconfig-1.5/src/machineconfig/scripts/python/cloud_rx.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 
-
-from crocodile.comms.gdrive import GDriveAPI
-# from crocodile.file_management import P
+import crocodile.toolbox as tb
 import argparse
 
 
-def main(google_account, project, file, unzip, relative_to_home, decrypt, key, pwd, local_dir):
-    api = GDriveAPI(account=google_account, project=project)
-
-    if "http" in file: path = api.download(furl=file, local_dir=local_dir, rel2home=relative_to_home)  # , recursive, zipFirst)
-    else:
-        file = file
-        path = api.download(fpath=file, local_dir=local_dir, rel2home=relative_to_home, decrypt=decrypt, unzip=unzip, key=key, pwd=pwd)  # , recursive, zipFirst)
-    print(path)
-
-
 def arg_parser():
-    parser = argparse.ArgumentParser(description='FTP client')
+    parser = argparse.ArgumentParser(description='Cloud Download CLI.')
 
     # positional argument
-    parser.add_argument("file", help="file/folder path.", default="")
+    parser.add_argument("file", help="file/folder path to be received.")
     # FLAGS
     # parser.add_argument("--recursive", "-r", help="Send recursively.", action="store_true")  # default is False
-    parser.add_argument("--relative_to_home", "-R", help="Download to a directory to make it relative to home.", action="store_true")  # default is False
-    parser.add_argument("--decrypt", "-e", help="decrypt file.", action="store_true")  # default is False
-    parser.add_argument("--unzip", "-z", help="unzip file.", action="store_true")  # default is False
+    parser.add_argument("--decrypt", "-e", help="Decrypt after receiving.", action="store_true")  # default is False
+    parser.add_argument("--unzip", "-z", help="unzip after receiving.", action="store_true")  # default is False
+    parser.add_argument("--overwrite", "-w", help="Overwrite existing file.", action="store_true")  # default is False
     # optional argument
-    parser.add_argument("--local_dir", "-d", help="Local directory to put the file in.", default="")
-    parser.add_argument("--google_account", "-a", help="Google Account.", default=None)
-    parser.add_argument("--project", "-P", help="Project Name", default=None)
-    parser.add_argument("--key", "-k", help="Key for decryption", default=None)
-    parser.add_argument("--pwd", "-p", help="Password for decryption", default=None)
+    parser.add_argument("--cloud", "-c", help="rclone cloud profile name.", default=None)
+    parser.add_argument("--localpath", "-l", help="Local path to save to.", default=None)
+    parser.add_argument("--remote_dir", "-d", help="Remote directory to send to.", default="")
+    parser.add_argument("--relative_to_home", "-r", help="Relative to `myhome` folder", action="store_true")  # default is False
+    parser.add_argument("--os_specific", "-o", help="OS specific path (relevant only when relative flag is raised as well.", action="store_true")
+    parser.add_argument("--key", "-k", help="Key for encryption", default=None)
+    parser.add_argument("--pwd", "-p", help="Password for encryption", default=None)
 
     args = parser.parse_args()
-    main(google_account=args.google_account, project=args.project, file=args.file,
-         unzip=args.unzip, relative_to_home=args.relative_to_home, decrypt=args.decrypt, key=args.key, pwd=args.pwd, local_dir=args.local_dir)
+
+    if args.cloud is None:
+        _path = tb.P.home().joinpath("dotfiles/config/setup/rclone_remote")
+        try: cloud = _path.read_text().replace("\n", "")
+        except FileNotFoundError:
+            print(f"No cloud profile found @ {_path}, please set one up or provide one via the --cloud flag.")
+            return ""
+    else: cloud = args.cloud
+
+    tb.P(args.file).from_cloud(cloud=cloud, localpath=args.localpath,
+                               unzip=args.unzip, decrypt=args.decrypt, overwrite=args.overwrite,
+                               pwd=args.pwd, key=args.key,
+                               rel2home=args.relative_to_home, os_specific=args.os_specific,)
 
 
 if __name__ == "__main__":
     arg_parser()
```

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/archive/bu_gdrive_sx.py` & `machineconfig-1.5/src/machineconfig/scripts/python/cloud_sx.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 
-from crocodile.comms.gdrive import GDriveAPI
-# from crocodile.file_management import P
+import crocodile.toolbox as tb
 import argparse
-
-
-def main(google_account, project, file, encrypt_first, z, relative_to_home, remote_dir, share, key, pwd):
-    api = GDriveAPI(account=google_account, project=project)
-
-    if share: res = api.upload_and_share(local_path=file, rel2home=relative_to_home,
-                                         zip_first=z, encrypt_first=encrypt_first, key=key, pwd=pwd)
-    else: res = api.upload(local_path=file, remote_dir=remote_dir, rel2home=relative_to_home,
-                           zip_first=z, encrypt_first=encrypt_first, key=key, pwd=pwd)  # , recursive, zipFirst)
-    print(res)
+# import subprocess
 
 
 def args_parser():
-    parser = argparse.ArgumentParser(description='FTP client')
+    parser = argparse.ArgumentParser(description='Cloud Management CLI.')
 
     # positional argument
-    parser.add_argument("file", help="file/folder path.", default="")
+    parser.add_argument("file", help="file/folder path.")
     # FLAGS
-    # parser.add_argument("--recursive", "-r", help="Send recursively.", action="store_true")  # default is False
-    parser.add_argument("--zip_first", "-z", help="Zip before sending.", action="store_true")  # default is False
-    parser.add_argument("--encrypt_first", "-e", help="Encrypt before sending.", action="store_true")  # default is False
-    parser.add_argument("--relative_to_home", "-R", help="Zip before sending.", action="store_true")  # default is False
+    parser.add_argument("--zip", "-z", help="Zip before sending.", action="store_true")  # default is False
+    parser.add_argument("--encrypt", "-e", help="Encrypt before sending.", action="store_true")  # default is False
+    parser.add_argument("--relative_to_home", "-r", help="set remote path as home relative local path.", action="store_true")  # default is False
+    parser.add_argument("--os_specific", "-o", help="OS specific path (relevant only when relative flag is raised as well.", action="store_true")
     parser.add_argument("--share", "-s", help="Share file.", action="store_true")
     # optional argument
+    parser.add_argument("--cloud", "-c", help="rclone cloud profile name.", default=None)
     parser.add_argument("--remote_dir", "-d", help="Remote directory to send to.", default="")
-    parser.add_argument("--google_account", "-a", help="Google Account.", default=None)
-    parser.add_argument("--project", "-P", help="Project Name", default=None)
     parser.add_argument("--key", "-k", help="Key for encryption", default=None)
     parser.add_argument("--pwd", "-p", help="Password for encryption", default=None)
 
     args = parser.parse_args()
-    main(google_account=args.google_account, project=args.project, file=args.file, z=args.zip_first, relative_to_home=args.relative_to_home, remote_dir=args.remote_dir, share=args.share, key=args.key, pwd=args.pwd, encrypt_first=args.encrypt_first)
+
+    if args.cloud is None:
+        _path = tb.P.home().joinpath("dotfiles/config/setup/rclone_remote")
+        try: cloud = _path.read_text().replace("\n", "")
+        except FileNotFoundError:
+            print(f"No cloud profile found @ {_path}, please set one up or provide one via the --cloud flag.")
+            return ""
+    else: cloud = args.cloud
+
+    res = tb.P(args.file).to_cloud(cloud=cloud, zip=args.zip, rel2home=args.relative_to_home,
+                                   share=args.share, key=args.key, pwd=args.pwd, encrypt=args.encrypt, os_specific=args.os_specific,)
+    if args.share: print(res.as_url_str())
 
 
 if __name__ == "__main__":
     args_parser()
```

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/choose_ohmybash_theme.py` & `machineconfig-1.5/src/machineconfig/scripts/python/choose_ohmybash_theme.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/choose_ohmyposh_theme.py` & `machineconfig-1.5/src/machineconfig/scripts/python/choose_ohmyposh_theme.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/cloud_mount.py` & `machineconfig-1.5/src/machineconfig/scripts/python/cloud_mount.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/cloud_sync.py` & `machineconfig-1.5/src/machineconfig/scripts/python/cloud_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,211 +6,211 @@
 00000050: 696d 706f 7274 2050 524f 4752 414d 5f50  import PROGRAM_P
 00000060: 4154 480d 0a66 726f 6d20 6d61 6368 696e  ATH..from machin
 00000070: 6563 6f6e 6669 672e 7363 7269 7074 732e  econfig.scripts.
 00000080: 7079 7468 6f6e 2e63 6c6f 7564 5f6d 6f75  python.cloud_mou
 00000090: 6e74 2069 6d70 6f72 7420 6765 745f 6d70  nt import get_mp
 000000a0: 726f 6373 5f6d 6f75 6e74 5f74 7874 0d0a  rocs_mount_txt..
 000000b0: 696d 706f 7274 2061 7267 7061 7273 650d  import argparse.
-000000c0: 0a0d 0a22 2222 0d0a 0d0a 2222 220d 0a23  ..."""...."""..#
-000000d0: 2054 4f44 4f20 6164 6420 202d 2d76 6673   TODO add  --vfs
-000000e0: 2d63 6163 6865 2d6d 6f64 6520 6675 6c6c  -cache-mode full
-000000f0: 0d0a 0d0a 0d0a 6465 6620 6172 6773 5f70  ......def args_p
-00000100: 6172 7365 7228 293a 0d0a 2020 2020 7061  arser():..    pa
-00000110: 7273 6572 203d 2061 7267 7061 7273 652e  rser = argparse.
-00000120: 4172 6775 6d65 6e74 5061 7273 6572 2864  ArgumentParser(d
-00000130: 6573 6372 6970 7469 6f6e 3d22 2222 4120  escription="""A 
-00000140: 7772 6170 7065 7220 666f 7220 7263 6c6f  wrapper for rclo
-00000150: 6e65 2073 796e 6320 616e 6420 7263 6c6f  ne sync and rclo
-00000160: 6e65 2062 6973 796e 632c 2077 6974 6820  ne bisync, with 
-00000170: 736f 6d65 2065 7874 7261 2066 6561 7475  some extra featu
-00000180: 7265 732e 2222 2229 0d0a 0d0a 2020 2020  res.""")....    
-00000190: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
-000001a0: 656e 7428 2273 6f75 7263 6522 2c20 6865  ent("source", he
-000001b0: 6c70 3d22 736f 7572 6365 222c 2064 6566  lp="source", def
-000001c0: 6175 6c74 3d4e 6f6e 6529 0d0a 2020 2020  ault=None)..    
-000001d0: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
-000001e0: 656e 7428 2274 6172 6765 7422 2c20 6865  ent("target", he
-000001f0: 6c70 3d22 7461 7267 6574 222c 2064 6566  lp="target", def
-00000200: 6175 6c74 3d4e 6f6e 6529 0d0a 0d0a 2020  ault=None)....  
-00000210: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-00000220: 756d 656e 7428 222d 2d74 7261 6e73 6665  ument("--transfe
-00000230: 7273 222c 2022 2d74 222c 2068 656c 703d  rs", "-t", help=
-00000240: 224e 756d 6265 7220 6f66 2074 6872 6561  "Number of threa
-00000250: 6473 2069 6e20 7379 6e63 696e 672e 222c  ds in syncing.",
-00000260: 2064 6566 6175 6c74 3d31 3029 2020 2320   default=10)  # 
-00000270: 6465 6661 756c 7420 6973 2046 616c 7365  default is False
-00000280: 0d0a 2020 2020 2320 7061 7273 6572 2e61  ..    # parser.a
-00000290: 6464 5f61 7267 756d 656e 7428 222d 2d6b  dd_argument("--k
-000002a0: 6579 222c 2022 2d6b 222c 2068 656c 703d  ey", "-k", help=
-000002b0: 224b 6579 2066 6f72 2065 6e63 7279 7074  "Key for encrypt
-000002c0: 696f 6e22 2c20 6465 6661 756c 743d 4e6f  ion", default=No
-000002d0: 6e65 290d 0a20 2020 2023 2070 6172 7365  ne)..    # parse
-000002e0: 722e 6164 645f 6172 6775 6d65 6e74 2822  r.add_argument("
-000002f0: 2d2d 7077 6422 2c20 222d 5022 2c20 6865  --pwd", "-P", he
-00000300: 6c70 3d22 5061 7373 776f 7264 2066 6f72  lp="Password for
-00000310: 2065 6e63 7279 7074 696f 6e22 2c20 6465   encryption", de
-00000320: 6661 756c 743d 4e6f 6e65 290d 0a20 2020  fault=None)..   
-00000330: 2070 6172 7365 722e 6164 645f 6172 6775   parser.add_argu
-00000340: 6d65 6e74 2822 2d2d 6269 7379 6e63 222c  ment("--bisync",
-00000350: 2022 2d62 222c 2068 656c 703d 2242 6964   "-b", help="Bid
-00000360: 6972 6563 7469 6f6e 616c 2073 796e 632e  irectional sync.
-00000370: 222c 2061 6374 696f 6e3d 2273 746f 7265  ", action="store
-00000380: 5f74 7275 6522 2920 2023 2064 6566 6175  _true")  # defau
-00000390: 6c74 2069 7320 4661 6c73 650d 0a20 2020  lt is False..   
-000003a0: 2070 6172 7365 722e 6164 645f 6172 6775   parser.add_argu
-000003b0: 6d65 6e74 2822 2d2d 6465 6c65 7465 222c  ment("--delete",
-000003c0: 2022 2d44 222c 2068 656c 703d 2244 656c   "-D", help="Del
-000003d0: 6574 6520 6669 6c65 7320 696e 2072 656d  ete files in rem
-000003e0: 6f74 6520 7468 6174 2061 7265 206e 6f74  ote that are not
-000003f0: 2069 6e20 6c6f 6361 6c2e 222c 2061 6374   in local.", act
-00000400: 696f 6e3d 2273 746f 7265 5f74 7275 6522  ion="store_true"
-00000410: 2920 2023 2064 6566 6175 6c74 2069 7320  )  # default is 
-00000420: 4661 6c73 650d 0a0d 0a20 2020 2070 6172  False....    par
-00000430: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
-00000440: 2822 2d2d 7665 7262 6f73 6522 2c20 222d  ("--verbose", "-
-00000450: 7622 2c20 6865 6c70 3d22 5665 7262 6f73  v", help="Verbos
-00000460: 6974 7920 6f66 206d 7072 6f63 7320 746f  ity of mprocs to
-00000470: 2073 686f 7720 6465 7461 696c 7320 6f66   show details of
-00000480: 2073 796e 6369 6e67 2e22 2c20 6163 7469   syncing.", acti
-00000490: 6f6e 3d22 7374 6f72 655f 7472 7565 2229  on="store_true")
-000004a0: 2020 2320 6465 6661 756c 7420 6973 2046    # default is F
-000004b0: 616c 7365 0d0a 0d0a 2020 2020 6172 6773  alse....    args
-000004c0: 203d 2070 6172 7365 722e 7061 7273 655f   = parser.parse_
-000004d0: 6172 6773 2829 0d0a 0d0a 2020 2020 6966  args()....    if
-000004e0: 2022 3a22 2069 6e20 6172 6773 2e73 6f75   ":" in args.sou
-000004f0: 7263 653a 0d0a 2020 2020 2020 2020 736f  rce:..        so
-00000500: 7572 6365 203d 2061 7267 732e 736f 7572  urce = args.sour
-00000510: 6365 0d0a 2020 2020 2020 2020 7461 7267  ce..        targ
-00000520: 6574 203d 2050 2861 7267 732e 7461 7267  et = P(args.targ
-00000530: 6574 292e 6578 7061 6e64 7573 6572 2829  et).expanduser()
-00000540: 2e61 6273 6f6c 7574 6528 290d 0a20 2020  .absolute()..   
-00000550: 2020 2020 2063 6c6f 7564 203d 2073 6f75       cloud = sou
-00000560: 7263 652e 7370 6c69 7428 223a 2229 5b30  rce.split(":")[0
-00000570: 5d0d 0a20 2020 2020 2020 206c 6f63 616c  ]..        local
-00000580: 7061 7468 203d 2074 6172 6765 740d 0a20  path = target.. 
-00000590: 2020 2065 6c69 6620 223a 2220 696e 2061     elif ":" in a
-000005a0: 7267 732e 7461 7267 6574 3a0d 0a20 2020  rgs.target:..   
-000005b0: 2020 2020 2073 6f75 7263 6520 3d20 6172       source = ar
-000005c0: 6773 2e74 6172 6765 7420 2023 2075 6e63  gs.target  # unc
-000005d0: 6861 6e67 6564 0d0a 2020 2020 2020 2020  hanged..        
-000005e0: 7461 7267 6574 203d 2050 2861 7267 732e  target = P(args.
-000005f0: 736f 7572 6365 292e 6578 7061 6e64 7573  source).expandus
-00000600: 6572 2829 2e61 6273 6f6c 7574 6528 290d  er().absolute().
-00000610: 0a20 2020 2020 2020 2063 6c6f 7564 203d  .        cloud =
-00000620: 2073 6f75 7263 652e 7370 6c69 7428 223a   source.split(":
-00000630: 2229 5b30 5d0d 0a20 2020 2020 2020 206c  ")[0]..        l
-00000640: 6f63 616c 7061 7468 203d 2074 6172 6765  ocalpath = targe
-00000650: 740d 0a20 2020 2065 6c73 653a 2020 2320  t..    else:  # 
-00000660: 7573 6572 2064 6964 206e 6f74 2073 7065  user did not spe
-00000670: 6369 6679 2072 656d 6f74 6570 6174 682c  cify remotepath,
-00000680: 2073 6f20 6974 2077 696c 6c20 6265 2069   so it will be i
-00000690: 6e66 6572 7265 6420 6865 7265 0d0a 2020  nferred here..  
-000006a0: 2020 2020 2020 2320 6275 7420 6669 7273        # but firs
-000006b0: 7420 7765 206e 6565 6420 746f 206b 6e6f  t we need to kno
-000006c0: 7720 7768 6574 6865 7220 7468 6520 636c  w whether the cl
-000006d0: 6f75 6420 6973 2073 6f75 7263 6520 6f72  oud is source or
-000006e0: 2074 6172 6765 740d 0a20 2020 2020 2020   target..       
-000006f0: 2072 656d 6f74 6573 203d 2052 6561 642e   remotes = Read.
-00000700: 696e 6928 502e 686f 6d65 2829 2e6a 6f69  ini(P.home().joi
-00000710: 6e70 6174 6828 222e 636f 6e66 6967 2f72  npath(".config/r
-00000720: 636c 6f6e 652f 7263 6c6f 6e65 2e63 6f6e  clone/rclone.con
-00000730: 6622 2929 2e73 6563 7469 6f6e 7328 290d  f")).sections().
-00000740: 0a20 2020 2020 2020 2066 6f72 2061 5f72  .        for a_r
-00000750: 656d 6f74 6520 696e 2072 656d 6f74 6573  emote in remotes
-00000760: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00000770: 6620 6172 6773 2e73 6f75 7263 6520 3d3d  f args.source ==
-00000780: 2061 5f72 656d 6f74 653a 0d0a 2020 2020   a_remote:..    
-00000790: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-000007a0: 6574 203d 2050 2861 7267 732e 7461 7267  et = P(args.targ
-000007b0: 6574 292e 6578 7061 6e64 7573 6572 2829  et).expanduser()
-000007c0: 2e61 6273 6f6c 7574 6528 290d 0a20 2020  .absolute()..   
-000007d0: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
-000007e0: 7263 6520 3d20 6622 7b61 7267 732e 736f  rce = f"{args.so
-000007f0: 7572 6365 7d3a 7b27 6d79 686f 6d65 2f67  urce}:{'myhome/g
-00000800: 656e 6572 6963 5f6f 7327 202f 2074 6172  eneric_os' / tar
-00000810: 6765 742e 7265 6c32 686f 6d65 2829 7d22  get.rel2home()}"
-00000820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000830: 2020 636c 6f75 6420 3d20 6172 6773 2e73    cloud = args.s
-00000840: 6f75 7263 650d 0a20 2020 2020 2020 2020  ource..         
-00000850: 2020 2020 2020 206c 6f63 616c 7061 7468         localpath
-00000860: 203d 2074 6172 6765 740d 0a20 2020 2020   = target..     
-00000870: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00000880: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00000890: 2061 7267 732e 7461 7267 6574 203d 3d20   args.target == 
-000008a0: 615f 7265 6d6f 7465 3a0d 0a20 2020 2020  a_remote:..     
-000008b0: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
-000008c0: 6520 3d20 5028 6172 6773 2e73 6f75 7263  e = P(args.sourc
-000008d0: 6529 2e65 7870 616e 6475 7365 7228 292e  e).expanduser().
-000008e0: 6162 736f 6c75 7465 2829 0d0a 2020 2020  absolute()..    
-000008f0: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-00000900: 6574 203d 2066 227b 6172 6773 2e74 6172  et = f"{args.tar
-00000910: 6765 747d 3a7b 276d 7968 6f6d 652f 6765  get}:{'myhome/ge
-00000920: 6e65 7269 635f 6f73 2720 2f20 736f 7572  neric_os' / sour
-00000930: 6365 2e72 656c 3268 6f6d 6528 297d 220d  ce.rel2home()}".
-00000940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000950: 2063 6c6f 7564 203d 2061 7267 732e 7461   cloud = args.ta
-00000960: 7267 6574 0d0a 2020 2020 2020 2020 2020  rget..          
-00000970: 2020 2020 2020 6c6f 6361 6c70 6174 6820        localpath 
-00000980: 3d20 736f 7572 6365 0d0a 2020 2020 2020  = source..      
-00000990: 2020 2020 2020 2020 2020 6272 6561 6b0d            break.
-000009a0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-000009b0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000009c0: 7428 6622 436f 756c 6420 6e6f 7420 6669  t(f"Could not fi
-000009d0: 6e64 2061 2072 656d 6f74 6520 696e 207b  nd a remote in {
-000009e0: 7265 6d6f 7465 737d 2074 6861 7420 6d61  remotes} that ma
-000009f0: 7463 6865 7320 7b61 7267 732e 736f 7572  tches {args.sour
-00000a00: 6365 7d20 6f72 207b 6172 6773 2e74 6172  ce} or {args.tar
-00000a10: 6765 747d 2e22 290d 0a20 2020 2020 2020  get}.")..       
-00000a20: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00000a30: 4572 726f 720d 0a0d 0a20 2020 2023 206d  Error....    # m
-00000a40: 6170 2073 686f 7274 2066 6c61 6773 2074  ap short flags t
-00000a50: 6f20 6c6f 6e67 2066 6c61 6773 2028 2d75  o long flags (-u
-00000a60: 202d 3e20 2d2d 7570 6c6f 6164 292c 2066   -> --upload), f
-00000a70: 6f72 2065 6173 6965 7220 7573 6520 696e  or easier use in
-00000a80: 2074 6865 2073 6372 6970 740d 0a20 2020   the script..   
-00000a90: 2069 6620 6172 6773 2e62 6973 796e 633a   if args.bisync:
-00000aa0: 2070 7269 6e74 2866 2253 796e 6369 6e67   print(f"Syncing
-00000ab0: 207b 736f 7572 6365 7d20 7b27 3c3e 2720   {source} {'<>' 
-00000ac0: 2a20 377d 207b 7461 7267 6574 7d60 2229  * 7} {target}`")
-00000ad0: 0d0a 2020 2020 656c 7365 3a20 7072 696e  ..    else: prin
-00000ae0: 7428 6622 5379 6e63 696e 6720 7b73 6f75  t(f"Syncing {sou
-00000af0: 7263 657d 207b 273e 2720 2a20 3135 7d20  rce} {'>' * 15} 
-00000b00: 7b74 6172 6765 747d 6022 290d 0a0d 0a20  {target}`").... 
-00000b10: 2020 2069 6620 6172 6773 2e62 6973 796e     if args.bisyn
-00000b20: 633a 2072 636c 6f6e 655f 636d 6420 3d20  c: rclone_cmd = 
-00000b30: 6622 2222 7263 6c6f 6e65 2062 6973 796e  f"""rclone bisyn
-00000b40: 6320 7b73 6f75 7263 657d 207b 7461 7267  c {source} {targ
-00000b50: 6574 7d22 2222 0d0a 2020 2020 656c 7365  et}"""..    else
-00000b60: 3a20 7263 6c6f 6e65 5f63 6d64 203d 2066  : rclone_cmd = f
-00000b70: 2222 2272 636c 6f6e 6520 7379 6e63 207b  """rclone sync {
-00000b80: 736f 7572 6365 7d20 7b74 6172 6765 747d  source} {target}
-00000b90: 2222 220d 0a0d 0a20 2020 2072 636c 6f6e  """....    rclon
-00000ba0: 655f 636d 6420 2b3d 2066 2220 2d2d 7072  e_cmd += f" --pr
-00000bb0: 6f67 7265 7373 202d 2d74 7261 6e73 6665  ogress --transfe
-00000bc0: 7273 3d7b 6172 6773 2e74 7261 6e73 6665  rs={args.transfe
-00000bd0: 7273 7d20 2d2d 7665 7262 6f73 6522 0d0a  rs} --verbose"..
-00000be0: 2020 2020 6966 2061 7267 732e 6269 7379      if args.bisy
-00000bf0: 6e63 3a20 7263 6c6f 6e65 5f63 6d64 202b  nc: rclone_cmd +
-00000c00: 3d20 2220 2d2d 7265 7379 6e63 220d 0a20  = " --resync".. 
-00000c10: 2020 2069 6620 6172 6773 2e64 656c 6574     if args.delet
-00000c20: 653a 2072 636c 6f6e 655f 636d 6420 2b3d  e: rclone_cmd +=
-00000c30: 2022 202d 2d64 656c 6574 652d 6475 7269   " --delete-duri
-00000c40: 6e67 220d 0a0d 0a20 2020 2069 6620 6172  ng"....    if ar
-00000c50: 6773 2e76 6572 626f 7365 3a20 7478 7420  gs.verbose: txt 
-00000c60: 3d20 6765 745f 6d70 726f 6373 5f6d 6f75  = get_mprocs_mou
-00000c70: 6e74 5f74 7874 2863 6c6f 7564 3d63 6c6f  nt_txt(cloud=clo
-00000c80: 7564 2c20 7263 6c6f 6e65 5f63 6d64 3d72  ud, rclone_cmd=r
-00000c90: 636c 6f6e 655f 636d 642c 206c 6f63 616c  clone_cmd, local
-00000ca0: 7061 7468 3d6c 6f63 616c 7061 7468 290d  path=localpath).
-00000cb0: 0a20 2020 2065 6c73 653a 2074 7874 203d  .    else: txt =
-00000cc0: 2066 2222 2263 6420 7e5c 6e7b 7263 6c6f   f"""cd ~\n{rclo
-00000cd0: 6e65 5f63 6d64 7d22 2222 0d0a 2020 2020  ne_cmd}"""..    
-00000ce0: 7072 696e 7428 7227 7275 6e6e 696e 6720  print(r'running 
-00000cf0: 636f 6d6d 616e 6427 2e63 656e 7465 7228  command'.center(
-00000d00: 3130 302c 2027 2d27 2929 0d0a 2020 2020  100, '-'))..    
-00000d10: 7072 696e 7428 7478 7429 0d0a 2020 2020  print(txt)..    
-00000d20: 5052 4f47 5241 4d5f 5041 5448 2e77 7269  PROGRAM_PATH.wri
-00000d30: 7465 5f74 6578 7428 7478 7429 0d0a 0d0a  te_text(txt)....
-00000d40: 0d0a 6966 205f 5f6e 616d 655f 5f20 3d3d  ..if __name__ ==
-00000d50: 2027 5f5f 6d61 696e 5f5f 273a 0d0a 2020   '__main__':..  
-00000d60: 2020 6172 6773 5f70 6172 7365 7228 290d    args_parser().
-00000d70: 0a                                       .
+000000c0: 0a0d 0a22 2222 0d0a 0d0a 2222 220d 0a0d  ..."""...."""...
+000000d0: 0a23 2054 4f44 4f20 6164 6420 202d 2d76  .# TODO add  --v
+000000e0: 6673 2d63 6163 6865 2d6d 6f64 6520 6675  fs-cache-mode fu
+000000f0: 6c6c 0d0a 0d0a 0d0a 6465 6620 6172 6773  ll......def args
+00000100: 5f70 6172 7365 7228 293a 0d0a 2020 2020  _parser():..    
+00000110: 7061 7273 6572 203d 2061 7267 7061 7273  parser = argpars
+00000120: 652e 4172 6775 6d65 6e74 5061 7273 6572  e.ArgumentParser
+00000130: 2864 6573 6372 6970 7469 6f6e 3d22 2222  (description="""
+00000140: 4120 7772 6170 7065 7220 666f 7220 7263  A wrapper for rc
+00000150: 6c6f 6e65 2073 796e 6320 616e 6420 7263  lone sync and rc
+00000160: 6c6f 6e65 2062 6973 796e 632c 2077 6974  lone bisync, wit
+00000170: 6820 736f 6d65 2065 7874 7261 2066 6561  h some extra fea
+00000180: 7475 7265 732e 2222 2229 0d0a 0d0a 2020  tures.""")....  
+00000190: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
+000001a0: 756d 656e 7428 2273 6f75 7263 6522 2c20  ument("source", 
+000001b0: 6865 6c70 3d22 736f 7572 6365 222c 2064  help="source", d
+000001c0: 6566 6175 6c74 3d4e 6f6e 6529 0d0a 2020  efault=None)..  
+000001d0: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
+000001e0: 756d 656e 7428 2274 6172 6765 7422 2c20  ument("target", 
+000001f0: 6865 6c70 3d22 7461 7267 6574 222c 2064  help="target", d
+00000200: 6566 6175 6c74 3d4e 6f6e 6529 0d0a 0d0a  efault=None)....
+00000210: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
+00000220: 7267 756d 656e 7428 222d 2d74 7261 6e73  rgument("--trans
+00000230: 6665 7273 222c 2022 2d74 222c 2068 656c  fers", "-t", hel
+00000240: 703d 224e 756d 6265 7220 6f66 2074 6872  p="Number of thr
+00000250: 6561 6473 2069 6e20 7379 6e63 696e 672e  eads in syncing.
+00000260: 222c 2064 6566 6175 6c74 3d31 3029 2020  ", default=10)  
+00000270: 2320 6465 6661 756c 7420 6973 2046 616c  # default is Fal
+00000280: 7365 0d0a 2020 2020 2320 7061 7273 6572  se..    # parser
+00000290: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
+000002a0: 2d6b 6579 222c 2022 2d6b 222c 2068 656c  -key", "-k", hel
+000002b0: 703d 224b 6579 2066 6f72 2065 6e63 7279  p="Key for encry
+000002c0: 7074 696f 6e22 2c20 6465 6661 756c 743d  ption", default=
+000002d0: 4e6f 6e65 290d 0a20 2020 2023 2070 6172  None)..    # par
+000002e0: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
+000002f0: 2822 2d2d 7077 6422 2c20 222d 5022 2c20  ("--pwd", "-P", 
+00000300: 6865 6c70 3d22 5061 7373 776f 7264 2066  help="Password f
+00000310: 6f72 2065 6e63 7279 7074 696f 6e22 2c20  or encryption", 
+00000320: 6465 6661 756c 743d 4e6f 6e65 290d 0a20  default=None).. 
+00000330: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
+00000340: 6775 6d65 6e74 2822 2d2d 6269 7379 6e63  gument("--bisync
+00000350: 222c 2022 2d62 222c 2068 656c 703d 2242  ", "-b", help="B
+00000360: 6964 6972 6563 7469 6f6e 616c 2073 796e  idirectional syn
+00000370: 632e 222c 2061 6374 696f 6e3d 2273 746f  c.", action="sto
+00000380: 7265 5f74 7275 6522 2920 2023 2064 6566  re_true")  # def
+00000390: 6175 6c74 2069 7320 4661 6c73 650d 0a20  ault is False.. 
+000003a0: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
+000003b0: 6775 6d65 6e74 2822 2d2d 6465 6c65 7465  gument("--delete
+000003c0: 222c 2022 2d44 222c 2068 656c 703d 2244  ", "-D", help="D
+000003d0: 656c 6574 6520 6669 6c65 7320 696e 2072  elete files in r
+000003e0: 656d 6f74 6520 7468 6174 2061 7265 206e  emote that are n
+000003f0: 6f74 2069 6e20 6c6f 6361 6c2e 222c 2061  ot in local.", a
+00000400: 6374 696f 6e3d 2273 746f 7265 5f74 7275  ction="store_tru
+00000410: 6522 2920 2023 2064 6566 6175 6c74 2069  e")  # default i
+00000420: 7320 4661 6c73 650d 0a0d 0a20 2020 2070  s False....    p
+00000430: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+00000440: 6e74 2822 2d2d 7665 7262 6f73 6522 2c20  nt("--verbose", 
+00000450: 222d 7622 2c20 6865 6c70 3d22 5665 7262  "-v", help="Verb
+00000460: 6f73 6974 7920 6f66 206d 7072 6f63 7320  osity of mprocs 
+00000470: 746f 2073 686f 7720 6465 7461 696c 7320  to show details 
+00000480: 6f66 2073 796e 6369 6e67 2e22 2c20 6163  of syncing.", ac
+00000490: 7469 6f6e 3d22 7374 6f72 655f 7472 7565  tion="store_true
+000004a0: 2229 2020 2320 6465 6661 756c 7420 6973  ")  # default is
+000004b0: 2046 616c 7365 0d0a 0d0a 2020 2020 6172   False....    ar
+000004c0: 6773 203d 2070 6172 7365 722e 7061 7273  gs = parser.pars
+000004d0: 655f 6172 6773 2829 0d0a 0d0a 2020 2020  e_args()....    
+000004e0: 6966 2022 3a22 2069 6e20 6172 6773 2e73  if ":" in args.s
+000004f0: 6f75 7263 653a 0d0a 2020 2020 2020 2020  ource:..        
+00000500: 736f 7572 6365 203d 2061 7267 732e 736f  source = args.so
+00000510: 7572 6365 0d0a 2020 2020 2020 2020 7461  urce..        ta
+00000520: 7267 6574 203d 2050 2861 7267 732e 7461  rget = P(args.ta
+00000530: 7267 6574 292e 6578 7061 6e64 7573 6572  rget).expanduser
+00000540: 2829 2e61 6273 6f6c 7574 6528 290d 0a20  ().absolute().. 
+00000550: 2020 2020 2020 2063 6c6f 7564 203d 2073         cloud = s
+00000560: 6f75 7263 652e 7370 6c69 7428 223a 2229  ource.split(":")
+00000570: 5b30 5d0d 0a20 2020 2020 2020 206c 6f63  [0]..        loc
+00000580: 616c 7061 7468 203d 2074 6172 6765 740d  alpath = target.
+00000590: 0a20 2020 2065 6c69 6620 223a 2220 696e  .    elif ":" in
+000005a0: 2061 7267 732e 7461 7267 6574 3a0d 0a20   args.target:.. 
+000005b0: 2020 2020 2020 2073 6f75 7263 6520 3d20         source = 
+000005c0: 6172 6773 2e74 6172 6765 7420 2023 2075  args.target  # u
+000005d0: 6e63 6861 6e67 6564 0d0a 2020 2020 2020  nchanged..      
+000005e0: 2020 7461 7267 6574 203d 2050 2861 7267    target = P(arg
+000005f0: 732e 736f 7572 6365 292e 6578 7061 6e64  s.source).expand
+00000600: 7573 6572 2829 2e61 6273 6f6c 7574 6528  user().absolute(
+00000610: 290d 0a20 2020 2020 2020 2063 6c6f 7564  )..        cloud
+00000620: 203d 2073 6f75 7263 652e 7370 6c69 7428   = source.split(
+00000630: 223a 2229 5b30 5d0d 0a20 2020 2020 2020  ":")[0]..       
+00000640: 206c 6f63 616c 7061 7468 203d 2074 6172   localpath = tar
+00000650: 6765 740d 0a20 2020 2065 6c73 653a 2020  get..    else:  
+00000660: 2320 7573 6572 2064 6964 206e 6f74 2073  # user did not s
+00000670: 7065 6369 6679 2072 656d 6f74 6570 6174  pecify remotepat
+00000680: 682c 2073 6f20 6974 2077 696c 6c20 6265  h, so it will be
+00000690: 2069 6e66 6572 7265 6420 6865 7265 0d0a   inferred here..
+000006a0: 2020 2020 2020 2020 2320 6275 7420 6669          # but fi
+000006b0: 7273 7420 7765 206e 6565 6420 746f 206b  rst we need to k
+000006c0: 6e6f 7720 7768 6574 6865 7220 7468 6520  now whether the 
+000006d0: 636c 6f75 6420 6973 2073 6f75 7263 6520  cloud is source 
+000006e0: 6f72 2074 6172 6765 740d 0a20 2020 2020  or target..     
+000006f0: 2020 2072 656d 6f74 6573 203d 2052 6561     remotes = Rea
+00000700: 642e 696e 6928 502e 686f 6d65 2829 2e6a  d.ini(P.home().j
+00000710: 6f69 6e70 6174 6828 222e 636f 6e66 6967  oinpath(".config
+00000720: 2f72 636c 6f6e 652f 7263 6c6f 6e65 2e63  /rclone/rclone.c
+00000730: 6f6e 6622 2929 2e73 6563 7469 6f6e 7328  onf")).sections(
+00000740: 290d 0a20 2020 2020 2020 2066 6f72 2061  )..        for a
+00000750: 5f72 656d 6f74 6520 696e 2072 656d 6f74  _remote in remot
+00000760: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
+00000770: 2069 6620 6172 6773 2e73 6f75 7263 6520   if args.source 
+00000780: 3d3d 2061 5f72 656d 6f74 653a 0d0a 2020  == a_remote:..  
+00000790: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+000007a0: 7267 6574 203d 2050 2861 7267 732e 7461  rget = P(args.ta
+000007b0: 7267 6574 292e 6578 7061 6e64 7573 6572  rget).expanduser
+000007c0: 2829 2e61 6273 6f6c 7574 6528 290d 0a20  ().absolute().. 
+000007d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000007e0: 6f75 7263 6520 3d20 6622 7b61 7267 732e  ource = f"{args.
+000007f0: 736f 7572 6365 7d3a 7b27 6d79 686f 6d65  source}:{'myhome
+00000800: 2f67 656e 6572 6963 5f6f 7327 202f 2074  /generic_os' / t
+00000810: 6172 6765 742e 7265 6c32 686f 6d65 2829  arget.rel2home()
+00000820: 7d22 0d0a 2020 2020 2020 2020 2020 2020  }"..            
+00000830: 2020 2020 636c 6f75 6420 3d20 6172 6773      cloud = args
+00000840: 2e73 6f75 7263 650d 0a20 2020 2020 2020  .source..       
+00000850: 2020 2020 2020 2020 206c 6f63 616c 7061           localpa
+00000860: 7468 203d 2074 6172 6765 740d 0a20 2020  th = target..   
+00000870: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00000880: 616b 0d0a 2020 2020 2020 2020 2020 2020  ak..            
+00000890: 6966 2061 7267 732e 7461 7267 6574 203d  if args.target =
+000008a0: 3d20 615f 7265 6d6f 7465 3a0d 0a20 2020  = a_remote:..   
+000008b0: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
+000008c0: 7263 6520 3d20 5028 6172 6773 2e73 6f75  rce = P(args.sou
+000008d0: 7263 6529 2e65 7870 616e 6475 7365 7228  rce).expanduser(
+000008e0: 292e 6162 736f 6c75 7465 2829 0d0a 2020  ).absolute()..  
+000008f0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+00000900: 7267 6574 203d 2066 227b 6172 6773 2e74  rget = f"{args.t
+00000910: 6172 6765 747d 3a7b 276d 7968 6f6d 652f  arget}:{'myhome/
+00000920: 6765 6e65 7269 635f 6f73 2720 2f20 736f  generic_os' / so
+00000930: 7572 6365 2e72 656c 3268 6f6d 6528 297d  urce.rel2home()}
+00000940: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00000950: 2020 2063 6c6f 7564 203d 2061 7267 732e     cloud = args.
+00000960: 7461 7267 6574 0d0a 2020 2020 2020 2020  target..        
+00000970: 2020 2020 2020 2020 6c6f 6361 6c70 6174          localpat
+00000980: 6820 3d20 736f 7572 6365 0d0a 2020 2020  h = source..    
+00000990: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+000009a0: 6b0d 0a20 2020 2020 2020 2065 6c73 653a  k..        else:
+000009b0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+000009c0: 696e 7428 6622 436f 756c 6420 6e6f 7420  int(f"Could not 
+000009d0: 6669 6e64 2061 2072 656d 6f74 6520 696e  find a remote in
+000009e0: 207b 7265 6d6f 7465 737d 2074 6861 7420   {remotes} that 
+000009f0: 6d61 7463 6865 7320 7b61 7267 732e 736f  matches {args.so
+00000a00: 7572 6365 7d20 6f72 207b 6172 6773 2e74  urce} or {args.t
+00000a10: 6172 6765 747d 2e22 290d 0a20 2020 2020  arget}.")..     
+00000a20: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00000a30: 7565 4572 726f 720d 0a0d 0a20 2020 2023  ueError....    #
+00000a40: 206d 6170 2073 686f 7274 2066 6c61 6773   map short flags
+00000a50: 2074 6f20 6c6f 6e67 2066 6c61 6773 2028   to long flags (
+00000a60: 2d75 202d 3e20 2d2d 7570 6c6f 6164 292c  -u -> --upload),
+00000a70: 2066 6f72 2065 6173 6965 7220 7573 6520   for easier use 
+00000a80: 696e 2074 6865 2073 6372 6970 740d 0a20  in the script.. 
+00000a90: 2020 2069 6620 6172 6773 2e62 6973 796e     if args.bisyn
+00000aa0: 633a 2070 7269 6e74 2866 2253 796e 6369  c: print(f"Synci
+00000ab0: 6e67 207b 736f 7572 6365 7d20 7b27 3c3e  ng {source} {'<>
+00000ac0: 2720 2a20 377d 207b 7461 7267 6574 7d60  ' * 7} {target}`
+00000ad0: 2229 0d0a 2020 2020 656c 7365 3a20 7072  ")..    else: pr
+00000ae0: 696e 7428 6622 5379 6e63 696e 6720 7b73  int(f"Syncing {s
+00000af0: 6f75 7263 657d 207b 273e 2720 2a20 3135  ource} {'>' * 15
+00000b00: 7d20 7b74 6172 6765 747d 6022 290d 0a0d  } {target}`")...
+00000b10: 0a20 2020 2069 6620 6172 6773 2e62 6973  .    if args.bis
+00000b20: 796e 633a 2072 636c 6f6e 655f 636d 6420  ync: rclone_cmd 
+00000b30: 3d20 6622 2222 7263 6c6f 6e65 2062 6973  = f"""rclone bis
+00000b40: 796e 6320 7b73 6f75 7263 657d 207b 7461  ync {source} {ta
+00000b50: 7267 6574 7d22 2222 0d0a 2020 2020 656c  rget}"""..    el
+00000b60: 7365 3a20 7263 6c6f 6e65 5f63 6d64 203d  se: rclone_cmd =
+00000b70: 2066 2222 2272 636c 6f6e 6520 7379 6e63   f"""rclone sync
+00000b80: 207b 736f 7572 6365 7d20 7b74 6172 6765   {source} {targe
+00000b90: 747d 2222 220d 0a0d 0a20 2020 2072 636c  t}"""....    rcl
+00000ba0: 6f6e 655f 636d 6420 2b3d 2066 2220 2d2d  one_cmd += f" --
+00000bb0: 7072 6f67 7265 7373 202d 2d74 7261 6e73  progress --trans
+00000bc0: 6665 7273 3d7b 6172 6773 2e74 7261 6e73  fers={args.trans
+00000bd0: 6665 7273 7d20 2d2d 7665 7262 6f73 6522  fers} --verbose"
+00000be0: 0d0a 2020 2020 6966 2061 7267 732e 6269  ..    if args.bi
+00000bf0: 7379 6e63 3a20 7263 6c6f 6e65 5f63 6d64  sync: rclone_cmd
+00000c00: 202b 3d20 2220 2d2d 7265 7379 6e63 220d   += " --resync".
+00000c10: 0a20 2020 2069 6620 6172 6773 2e64 656c  .    if args.del
+00000c20: 6574 653a 2072 636c 6f6e 655f 636d 6420  ete: rclone_cmd 
+00000c30: 2b3d 2022 202d 2d64 656c 6574 652d 6475  += " --delete-du
+00000c40: 7269 6e67 220d 0a0d 0a20 2020 2069 6620  ring"....    if 
+00000c50: 6172 6773 2e76 6572 626f 7365 3a20 7478  args.verbose: tx
+00000c60: 7420 3d20 6765 745f 6d70 726f 6373 5f6d  t = get_mprocs_m
+00000c70: 6f75 6e74 5f74 7874 2863 6c6f 7564 3d63  ount_txt(cloud=c
+00000c80: 6c6f 7564 2c20 7263 6c6f 6e65 5f63 6d64  loud, rclone_cmd
+00000c90: 3d72 636c 6f6e 655f 636d 642c 206c 6f63  =rclone_cmd, loc
+00000ca0: 616c 7061 7468 3d6c 6f63 616c 7061 7468  alpath=localpath
+00000cb0: 290d 0a20 2020 2065 6c73 653a 2074 7874  )..    else: txt
+00000cc0: 203d 2066 2222 2263 6420 7e5c 6e7b 7263   = f"""cd ~\n{rc
+00000cd0: 6c6f 6e65 5f63 6d64 7d22 2222 0d0a 2020  lone_cmd}"""..  
+00000ce0: 2020 7072 696e 7428 7227 7275 6e6e 696e    print(r'runnin
+00000cf0: 6720 636f 6d6d 616e 6427 2e63 656e 7465  g command'.cente
+00000d00: 7228 3130 302c 2027 2d27 2929 0d0a 2020  r(100, '-'))..  
+00000d10: 2020 7072 696e 7428 7478 7429 0d0a 2020    print(txt)..  
+00000d20: 2020 5052 4f47 5241 4d5f 5041 5448 2e77    PROGRAM_PATH.w
+00000d30: 7269 7465 5f74 6578 7428 7478 7429 0d0a  rite_text(txt)..
+00000d40: 0d0a 0d0a 6966 205f 5f6e 616d 655f 5f20  ....if __name__ 
+00000d50: 3d3d 2027 5f5f 6d61 696e 5f5f 273a 0d0a  == '__main__':..
+00000d60: 2020 2020 6172 6773 5f70 6172 7365 7228      args_parser(
+00000d70: 290d 0a                                  )..
```

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/devops.py` & `machineconfig-1.5/src/machineconfig/scripts/python/devops.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,83 +2,86 @@
 from platform import system
 # import subprocess
 # import crocodile.toolbox as tb
 from machineconfig.utils.utils import display_options, PROGRAM_PATH, write_shell_script
 from enum import Enum
 
 
-# needs to be synced with devops.sh and devops.ps1
-
-
 class Options(Enum):
     update         = 'UPDATE essential repos'
     devaps         = 'DEVAPPS install'
     ve             = 'VE install'
     sym_path_shell = 'SYMLINKS, PATH & SHELL PROFILE'
     sym_new        = 'SYMLINKS new'
     ssh_add_pubkey = 'SSH add pub key to this machine'
     ssh_add_id     = 'SSH add identity (private key) to this machine'
     ssh_use_pair   = 'SSH use key pair to connect two machines'
     ssh_setup      = 'SSH setup'
     ssh_setup_wsl  = 'SSH setup wsl'
-    # repos_pull     = 'REPOS pull all'
-    # repos_commit   = 'REPOS commit all'
-    # repos_push     = 'REPOS push all'
     backup         = 'BACKUP & RETRIEVE'
 
 
-def main():
+def args_parser():
+    import argparse
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-w", "--which", help="which option to run", type=str, default=None)  # , choices=[op.value for op in Options]
+    args = parser.parse_args()
+    main(which=args.which)
+
+
+def main(which=None):
     PROGRAM_PATH.delete(sure=True, verbose=False)
     options = [op.value for op in Options]
-    choice_key = display_options(msg="", options=options, header="DEVOPS", default=options[0])
+    if which is None: choice_key = display_options(msg="", options=options, header="DEVOPS", default=options[0])
+    else: choice_key = Options[which].value
 
     if choice_key == Options.update.value:
         import machineconfig.scripts.python.devops_update_repos as helper
         program = helper.main()
 
     elif choice_key == Options.ve.value:
-        from machineconfig.jobs.python.python_ve_installer import main
-        program = main()
+        import machineconfig.jobs.python.python_ve_installer as helper
+        program = helper.main()
 
     elif choice_key == Options.devaps.value:
-        from machineconfig.scripts.python.devops_devapps_install import main
-        program = main()
+        import machineconfig.scripts.python.devops_devapps_install as helper
+        program = helper.main()
 
     elif choice_key == Options.sym_new.value:
-        from machineconfig.jobs.python.python_ve_symlink import main
-        program = main()
+        import machineconfig.jobs.python.python_ve_symlink as helper
+        program = helper.main()
 
     elif choice_key == Options.sym_path_shell.value:
-        from machineconfig.profile.create import main
-        main()
+        import machineconfig.profile.create as helper
+        helper.main()
         program = "echo 'done with symlinks'"
 
     elif choice_key == Options.ssh_add_pubkey.value:
-        from machineconfig.scripts.python.devops_add_ssh_key import main
-        program = main()
+        import machineconfig.scripts.python.devops_add_ssh_key as helper
+        program = helper.main()
 
     elif choice_key == Options.ssh_use_pair.value:
         raise NotImplementedError
 
     elif choice_key == Options.ssh_add_id.value:  # so that you can SSH directly withuot pointing to identity key.
-        from machineconfig.scripts.python.devops_add_identity import main
-        program = main()
+        import machineconfig.scripts.python.devops_add_identity as helper
+        program = helper.main()
 
     elif choice_key == Options.ssh_setup.value:
         program_windows = f"""Invoke-WebRequest https://raw.githubusercontent.com/thisismygitrepo/machineconfig/main/src/machineconfig/setup_windows/openssh_all.ps1 | Invoke-Expression  # https://github.com/thisismygitrepo.keys"""
         program_linux = f"""curl https://raw.githubusercontent.com/thisismygitrepo/machineconfig/main/src/machineconfig/setup_linux/openssh_all.sh | sudo bash  # https://github.com/thisismygitrepo.keys"""
         program = program_linux if system() == "Linux" else program_windows
 
     elif choice_key == Options.ssh_setup_wsl.value:
         program = f"""curl https://raw.githubusercontent.com/thisismygitrepo/machineconfig/main/src/machineconfig/setup_linux/openssh_wsl.sh | sudo bash"""
 
     elif choice_key == Options.backup.value:
         from machineconfig.scripts.python.devops_backup_retrieve import main
         program = main()
 
     else: raise ValueError(f"Unimplemented choice: {choice_key}")
-    if program: write_shell_script(program,)
+    if program: write_shell_script(program, display=True, preserve_cwd=True, desc="Shell script prepared by Python.", execute=True if which is not None else False)
     else: write_shell_script("echo 'Done.'", display=False, )  # Python did not return any script to run.
 
 
 if __name__ == "__main__":
-    main()
+    args_parser()
```

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/devops_add_identity.py` & `machineconfig-1.5/src/machineconfig/scripts/python/devops_add_identity.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/devops_add_ssh_key.py` & `machineconfig-1.5/src/machineconfig/scripts/python/devops_add_ssh_key.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/devops_backup_retrieve.py` & `machineconfig-1.5/src/machineconfig/scripts/python/devops_backup_retrieve.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/devops_devapps_install.py` & `machineconfig-1.5/src/machineconfig/scripts/python/devops_devapps_install.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,53 +2,71 @@
 
 from platform import system
 # import subprocess
 import crocodile.toolbox as tb
 from machineconfig.utils.utils import LIBRARY_ROOT, display_options
 
 
+if system() == "Windows": from machineconfig.jobs.python.python_windows_installers_all import get_cli_py_installers
+elif system() == "Linux": from machineconfig.jobs.python.python_linux_installers_all import get_cli_py_installers
+else: raise NotImplementedError(f"System {system()} not supported")
+
+
 def main(program_name=None):
-    if system() == "Windows": from machineconfig.jobs.python.python_windows_installers_all import get_cli_py_installers
-    elif system() == "Linux": from machineconfig.jobs.python.python_linux_installers_all import get_cli_py_installers
-    else: raise NotImplementedError(f"System {system()} not supported")
     installers = get_cli_py_installers()
     default = tb.P("all")
     installers.list.insert(0, default)
     installers.list.insert(0, tb.P("System Installers"))
     installers.list.insert(0, tb.P("Other dev apps"))
     options = list(installers.apply(lambda x: x.stem + ((' -- ' + str(x.readit().__doc__)) if x.exists() else '')))
     # options.sort()  # throws off sync between installers and options
 
     if program_name is None:
-        program_name = display_options(msg="", options=options, header="CHOOSE DEV APP", default=str(default), fzf=True)
+        program_names = display_options(msg="", options=options, header="CHOOSE DEV APP", default=str(default), fzf=True, multi=True)
+        total_program = ""
+        for program_name in program_names:
+            total_program += "\n" + get_program(program_name, options, installers)
+    else:
+        total_program = get_program(program_name, options, installers)
+    return total_program
 
+
+def get_program(program_name, options, installers):
     if program_name == "all":
         if system() == "Linux": from machineconfig.jobs.python.python_linux_installers_all import main
         elif system() == "Windows": from machineconfig.jobs.python.python_windows_installers_all import main
         else: raise NotImplementedError(f"System {system()} not supported")
         main()
         # program_linux = f"source {LIBRARY_ROOT}/setup_linux/devapps.sh"
         # program_windows = f"{LIBRARY_ROOT}/setup_windows/devapps.ps1"
         program = ""
     elif program_name == "System Installers":
         if system() == "Windows": options_more = parse_apps_installer_windows(LIBRARY_ROOT.joinpath("setup_windows/apps.ps1").read_text())
         elif system() == "Linux": options_more = parse_apps_installer_linux(LIBRARY_ROOT.joinpath("setup_linux/apps.sh").read_text())
         else: raise NotImplementedError(f"System {system()} not supported")
-        program_name = display_options(msg="", options=list(options_more.keys()), header="CHOOSE DEV APP", fzf=True)
-        program = options_more[program_name]
-        if program.startswith("#"): program = program[1:]
-        print(f"Running:\n{program}")
+        program_names = display_options(msg="", options=sorted(list(options_more.keys())), header="CHOOSE DEV APP", fzf=True, multi=True)
+        program = ""
+        for name in program_names:
+            sub_program = options_more[name]
+            if sub_program.startswith("#winget"): sub_program = sub_program[1:]
+            program += "\n" + sub_program
     elif program_name == "Other dev apps":
         installers = get_cli_py_installers(dev=True)
         options = list(installers.apply(lambda x: x.stem + ((' -- ' + str(x.readit().__doc__)) if x.exists() else '')))
-        options.sort()
-        program_name = display_options(msg="", options=options, header="CHOOSE DEV APP", fzf=True)
-        idx = options.index(program_name)
-        program = installers[idx].readit()['main']()  # finish the task
-        if program is None: program = "echo 'Finished Installation'"  # write an empty program
+        program_names = display_options(msg="", options=sorted(options), header="CHOOSE DEV APP", fzf=True, multi=True)
+        program = ""
+        for name in program_names:
+            idx = options.index(name)
+            try:
+                sub_program = installers[idx].readit()['main']()  # finish the task
+            except KeyError:
+                print(f"KeyError: could not find 'main' in {installers[idx]}")
+                raise KeyError
+            if sub_program is None: sub_program = "echo 'Finished Installation'"  # write an empty program
+            program += "\n" + sub_program
     else:
         idx = options.index(program_name)
         print(installers[idx])
         program = installers[idx].readit()['main']()  # finish the task
         if program is None: program = "echo 'Finished Installation'"  # write an empty program
     return program
```

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/devops_update_repos.py` & `machineconfig-1.5/src/machineconfig/scripts/python/devops_update_repos.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
 from platform import system
 import crocodile.toolbox as tb
-from machineconfig.utils.utils import write_shell_script
-
+# from machineconfig.utils.utils import write_shell_script
 
 sep = "\n"
 
 
 def main(verbose=True) -> str:
     _ = verbose
     repos = tb.P.home().joinpath("dotfiles/config/reposXXX.ini")
@@ -39,24 +38,31 @@
 """
                 additions.append(an_addition)
             else:
                 # if a_repo.is_dirty() and input(f"Repository {a_repo} is not clean, hard-reset it? y/[n]"): a_repo.git.reset('--hard')
                 additions.append(f"""
 echo "{("Pulling " + str(a_repo.working_dir)).center(80, "-")}"
 cd "{a_repo.working_dir}"
-{sep.join([f'git pull {remote.name}' for remote in a_repo.remotes])}
+{sep.join([f'git pull {remote.name} {a_repo.active_branch.name}' for remote in a_repo.remotes])}
 """)
         program = "\n".join(additions)
 
     elif system() == "Windows":
         program = "\n".join([f"""
 echo "{("Pulling " + str(a_repo.working_dir)).center(80, "-")}"
 cd "{a_repo.working_dir}"
-{sep.join([f'git pull {remote.name}' for remote in a_repo.remotes])}
+{sep.join([f'git pull {remote.name} {a_repo.active_branch.name}' for remote in a_repo.remotes])}
 """ for a_repo in repos_objs])
     else: raise NotImplementedError(f"System {system()} not supported")
-    write_shell_script(program, desc="Script to update repos")
-    return ""
+    # write_shell_script(program, desc="Script to update repos")
+    # return ""
+    return program
+
+
+# def get_pulls(remote):
+#     if len(remote.branches) == 0: return ""
+#     elif len(remote.branches) == 1: return f'git pull {remote.name} {remote.branches[0].name}'
+#     else: return f'git pull {remote.name} {remote.active_branch.name}'
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/dotfile.py` & `machineconfig-1.5/src/machineconfig/scripts/python/dotfile.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/ftprx.py` & `machineconfig-1.5/src/machineconfig/scripts/python/ftprx.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/ftpsx.py` & `machineconfig-1.5/src/machineconfig/scripts/python/ftpsx.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/im2text.py` & `machineconfig-1.5/src/machineconfig/scripts/python/im2text.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/onetimeshare.py` & `machineconfig-1.5/src/machineconfig/scripts/python/onetimeshare.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/pomodoro.py` & `machineconfig-1.5/src/machineconfig/scripts/python/pomodoro.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/repos.py` & `machineconfig-1.5/src/machineconfig/scripts/python/repos.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         if mess is None: mess = "auto_commit_" + tb.randstr()
         program += f'''
 git add .; git commit -am "{mess}"
 '''
     if action == GitAction.push or action == GitAction.pull:
         # remotes = tm.run(f"cd {path}; git remote", shell="powershell").op.split("\n")
         action_name = "pull" if action == GitAction.pull else "push"
-        cmds = [f'echo "pulling from {remote.url}" ; git {action_name} {remote.name}' for remote in repo.remotes]
+        cmds = [f'echo "pulling from {remote.url}" ; git {action_name} {remote.name} {repo.active_branch.name}' for remote in repo.remotes]
         program += '\n' + '\n'.join(cmds) + '\n'
     program = program + f'''
 echo ""; echo ""
 '''
     return program
```

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/snapshot.py` & `machineconfig-1.5/src/machineconfig/scripts/python/snapshot.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/tmate_conn.py` & `machineconfig-1.5/src/machineconfig/scripts/python/tmate_conn.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/tmate_start.py` & `machineconfig-1.5/src/machineconfig/scripts/python/tmate_start.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/transfer_wsl_win.py` & `machineconfig-1.5/src/machineconfig/scripts/python/transfer_wsl_win.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/python/wifi_conn.py` & `machineconfig-1.5/src/machineconfig/scripts/python/wifi_conn.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,52 +4,52 @@
 import configparser
 from pathlib import Path
 # import random
 # import string
 import os
 
 
-def createNewConnection(name, SSID, password):
+def create_new_connection(name, ssid, password):
     config = """<?xml version=\"1.0\"?>
 <WLANProfile xmlns="http://www.microsoft.com/networking/WLAN/profile/v1">
-    <name>"""+name+"""</name>
+    <name>""" + name + """</name>
     <SSIDConfig>
         <SSID>
-            <name>"""+SSID+"""</name>
+            <name>""" + ssid + """</name>
         </SSID>
     </SSIDConfig>
     <connectionType>ESS</connectionType>
     <connectionMode>auto</connectionMode>
     <MSM>
         <security>
             <authEncryption>
                 <authentication>WPA2PSK</authentication>
                 <encryption>AES</encryption>
                 <useOneX>false</useOneX>
             </authEncryption>
             <sharedKey>
                 <keyType>passPhrase</keyType>
                 <protected>false</protected>
-                <keyMaterial>"""+password+"""</keyMaterial>
+                <keyMaterial>""" + password + """</keyMaterial>
             </sharedKey>
         </security>
     </MSM>
 </WLANProfile>"""
     command = "netsh wlan add profile filename=\""+name+".xml\""+" interface=Wi-Fi"
     with open(name+".xml", 'w') as file:
         file.write(config)
     os.system(command)
 
 
-def connect(name, SSID):
-    command = "netsh wlan connect name=\""+name+"\" ssid=\""+SSID+"\" interface=Wi-Fi"
+def connect(name, ssid):
+    command = "netsh wlan connect name=\"" + name + "\" ssid=\""+ssid+"\" interface=Wi-Fi"
     os.system(command)
 
 
-def displayAvailableNetworks():
+def display_available_networks():
     command = "netsh wlan show networks interface=Wi-Fi"
     os.system(command)
 
 
 def main():
     creds = configparser.ConfigParser()
     creds.read(Path.home().joinpath('dotfiles/creds/msc/wifi.ini'))
```

### Comparing `machineconfig-1.4/src/machineconfig/scripts/windows/activate_ve.ps1` & `machineconfig-1.5/src/machineconfig/scripts/windows/activate_ve.ps1`

 * *Files 4% similar despite different names*

```diff
@@ -54,47 +54,54 @@
 00000350: 7669 7274 7561 6c20 656e 7669 726f 6e6d  virtual environm
 00000360: 656e 7420 2465 6e76 3a56 4952 5455 414c  ent $env:VIRTUAL
 00000370: 5f45 4e56 2220 7d0d 0a0d 0a7d 0d0a 0d0a  _ENV" }....}....
 00000380: 656c 7365 207b 0d0a 0d0a 2020 2020 2320  else {....    # 
 00000390: 6966 2024 6172 6773 5b30 5d20 6973 2070  if $args[0] is p
 000003a0: 6173 7365 642c 2069 7427 7320 6120 6e65  assed, it's a ne
 000003b0: 7720 7665 2074 6f20 6163 7469 7661 7465  w ve to activate
-000003c0: 0d0a 2020 2020 6966 2028 2461 7267 735b  ..    if ($args[
-000003d0: 305d 2920 7b0d 0a20 2020 2020 2020 2065  0]) {..        e
-000003e0: 6368 6f20 2244 6561 6374 6976 6174 696e  cho "Deactivatin
-000003f0: 6720 7669 7274 7561 6c20 656e 7669 726f  g virtual enviro
-00000400: 6e6d 656e 7420 2465 6e76 3a56 4952 5455  nment $env:VIRTU
-00000410: 414c 5f45 4e56 220d 0a20 2020 2020 2020  AL_ENV"..       
-00000420: 2064 6561 6374 6976 6174 6520 2d45 7272   deactivate -Err
-00000430: 6f72 4163 7469 6f6e 2053 696c 656e 746c  orAction Silentl
-00000440: 7943 6f6e 7469 6e75 650d 0a20 2020 2020  yContinue..     
-00000450: 2020 2024 6e61 6d65 203d 2024 6172 6773     $name = $args
-00000460: 5b30 5d0d 0a20 2020 2020 2020 2026 2022  [0]..        & "
-00000470: 2465 6e76 3a55 5345 5250 524f 4649 4c45  $env:USERPROFILE
-00000480: 2f76 656e 7673 2f24 6e61 6d65 2f53 6372  /venvs/$name/Scr
-00000490: 6970 7473 2f41 6374 6976 6174 652e 7073  ipts/Activate.ps
-000004a0: 3122 0d0a 2020 2020 2020 2020 6966 2028  1"..        if (
-000004b0: 243f 2920 7b20 5772 6974 652d 486f 7374  $?) { Write-Host
-000004c0: 2022 2060 757b 3237 3035 7d20 4163 7469   " `u{2705} Acti
-000004d0: 7661 7465 6420 7669 7274 7561 6c20 656e  vated virtual en
-000004e0: 7669 726f 6e6d 656e 7420 2465 6e76 3a56  vironment $env:V
-000004f0: 4952 5455 414c 5f45 4e56 2022 207d 0d0a  IRTUAL_ENV " }..
-00000500: 2020 2020 7d0d 0a20 2020 2065 6c73 6520      }..    else 
-00000510: 7b0d 0a20 2020 2020 2020 2057 7269 7465  {..        Write
-00000520: 2d48 6f73 7420 2220 5669 7274 7561 6c20  -Host " Virtual 
-00000530: 656e 7669 726f 6e6d 656e 7420 2724 656e  environment '$en
-00000540: 763a 5649 5254 5541 4c5f 454e 5627 2069  v:VIRTUAL_ENV' i
-00000550: 7320 616c 7265 6164 7920 6163 7469 7661  s already activa
-00000560: 7465 6420 220d 0a20 2020 207d 0d0a 0d0a  ted "..    }....
-00000570: 2020 2020 6966 2028 2128 5465 7374 2d50      if (!(Test-P
-00000580: 6174 6820 2443 4f4e 4649 475f 5041 5448  ath $CONFIG_PATH
-00000590: 2929 207b 0d0a 2020 2020 2020 2020 4e65  )) {..        Ne
-000005a0: 772d 4974 656d 202d 4974 656d 5479 7065  w-Item -ItemType
-000005b0: 2044 6972 6563 746f 7279 202d 5061 7468   Directory -Path
-000005c0: 2024 656e 763a 5553 4552 5052 4f46 494c   $env:USERPROFIL
-000005d0: 452f 2e63 6f6e 6669 672f 6d61 6368 696e  E/.config/machin
-000005e0: 6563 6f6e 6669 6720 2d45 7272 6f72 4163  econfig -ErrorAc
-000005f0: 7469 6f6e 2053 696c 656e 746c 7943 6f6e  tion SilentlyCon
-00000600: 7469 6e75 650d 0a20 2020 2020 2020 2024  tinue..        $
-00000610: 656e 763a 5649 5254 5541 4c5f 454e 5620  env:VIRTUAL_ENV 
-00000620: 3e20 2443 4f4e 4649 475f 5041 5448 0d0a  > $CONFIG_PATH..
-00000630: 2020 2020 7d0d 0a7d 0d0a 0d0a                }..}....
+000003c0: 0d0a 2020 2020 2320 6563 686f 2022 2465  ..    # echo "$e
+000003d0: 6e76 3a55 5345 5250 524f 4649 4c45 5c76  nv:USERPROFILE\v
+000003e0: 656e 7673 5c24 6172 6773 220d 0a20 2020  envs\$args"..   
+000003f0: 200d 0a20 2020 2069 6620 2824 6172 6773   ..    if ($args
+00000400: 5b30 5d20 2d61 6e64 2022 2465 6e76 3a56  [0] -and "$env:V
+00000410: 4952 5455 414c 5f45 4e56 2220 2d6e 6520  IRTUAL_ENV" -ne 
+00000420: 2224 656e 763a 5553 4552 5052 4f46 494c  "$env:USERPROFIL
+00000430: 455c 7665 6e76 735c 2461 7267 7322 2920  E\venvs\$args") 
+00000440: 7b0d 0a20 2020 2020 2020 2065 6368 6f20  {..        echo 
+00000450: 2244 6561 6374 6976 6174 696e 6720 7669  "Deactivating vi
+00000460: 7274 7561 6c20 656e 7669 726f 6e6d 656e  rtual environmen
+00000470: 7420 2465 6e76 3a56 4952 5455 414c 5f45  t $env:VIRTUAL_E
+00000480: 4e56 220d 0a20 2020 2020 2020 2064 6561  NV"..        dea
+00000490: 6374 6976 6174 6520 2d45 7272 6f72 4163  ctivate -ErrorAc
+000004a0: 7469 6f6e 2053 696c 656e 746c 7943 6f6e  tion SilentlyCon
+000004b0: 7469 6e75 650d 0a20 2020 2020 2020 2024  tinue..        $
+000004c0: 6e61 6d65 203d 2024 6172 6773 5b30 5d0d  name = $args[0].
+000004d0: 0a20 2020 2020 2020 2026 2022 2465 6e76  .        & "$env
+000004e0: 3a55 5345 5250 524f 4649 4c45 2f76 656e  :USERPROFILE/ven
+000004f0: 7673 2f24 6e61 6d65 2f53 6372 6970 7473  vs/$name/Scripts
+00000500: 2f41 6374 6976 6174 652e 7073 3122 0d0a  /Activate.ps1"..
+00000510: 2020 2020 2020 2020 6966 2028 243f 2920          if ($?) 
+00000520: 7b20 5772 6974 652d 486f 7374 2022 2060  { Write-Host " `
+00000530: 757b 3237 3035 7d20 4163 7469 7661 7465  u{2705} Activate
+00000540: 6420 7669 7274 7561 6c20 656e 7669 726f  d virtual enviro
+00000550: 6e6d 656e 7420 2465 6e76 3a56 4952 5455  nment $env:VIRTU
+00000560: 414c 5f45 4e56 2022 207d 0d0a 2020 2020  AL_ENV " }..    
+00000570: 7d0d 0a20 2020 2065 6c73 6520 7b0d 0a20  }..    else {.. 
+00000580: 2020 2020 2020 2057 7269 7465 2d48 6f73         Write-Hos
+00000590: 7420 2220 5669 7274 7561 6c20 656e 7669  t " Virtual envi
+000005a0: 726f 6e6d 656e 7420 2724 656e 763a 5649  ronment '$env:VI
+000005b0: 5254 5541 4c5f 454e 5627 2069 7320 616c  RTUAL_ENV' is al
+000005c0: 7265 6164 7920 6163 7469 7661 7465 6420  ready activated 
+000005d0: 220d 0a20 2020 207d 0d0a 0d0a 2020 2020  "..    }....    
+000005e0: 6966 2028 2128 5465 7374 2d50 6174 6820  if (!(Test-Path 
+000005f0: 2443 4f4e 4649 475f 5041 5448 2929 207b  $CONFIG_PATH)) {
+00000600: 0d0a 2020 2020 2020 2020 4e65 772d 4974  ..        New-It
+00000610: 656d 202d 4974 656d 5479 7065 2044 6972  em -ItemType Dir
+00000620: 6563 746f 7279 202d 5061 7468 2024 656e  ectory -Path $en
+00000630: 763a 5553 4552 5052 4f46 494c 452f 2e63  v:USERPROFILE/.c
+00000640: 6f6e 6669 672f 6d61 6368 696e 6563 6f6e  onfig/machinecon
+00000650: 6669 6720 2d45 7272 6f72 4163 7469 6f6e  fig -ErrorAction
+00000660: 2053 696c 656e 746c 7943 6f6e 7469 6e75   SilentlyContinu
+00000670: 650d 0a20 2020 2020 2020 2024 656e 763a  e..        $env:
+00000680: 5649 5254 5541 4c5f 454e 5620 3e20 2443  VIRTUAL_ENV > $C
+00000690: 4f4e 4649 475f 5041 5448 0d0a 2020 2020  ONFIG_PATH..    
+000006a0: 7d0d 0a7d 0d0a 0d0a                      }..}....
```

### Comparing `machineconfig-1.4/src/machineconfig/scripts/windows/archive/secure_pull.ps1` & `machineconfig-1.5/src/machineconfig/scripts/windows/archive/secure_pull.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/windows/archive/secure_push.ps1` & `machineconfig-1.5/src/machineconfig/scripts/windows/archive/secure_push.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/windows/cloud_mount.ps1` & `machineconfig-1.5/src/machineconfig/scripts/windows/cloud_mount.ps1`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 if ( $script_root -eq $null) {  # this does happen if a virtual enviroment is activated before running this script (don't know why)
 $script_root = $PSScriptRoot
 }
 
 python -m fire $script_root/../python/cloud_mount.py main   $args
 . $op_script
 
-deactivate -ErrorAction SilentlyContinue
+deactivate -ErrorAction SilentlyContinue
```

### Comparing `machineconfig-1.4/src/machineconfig/scripts/windows/croshell.ps1` & `machineconfig-1.5/src/machineconfig/scripts/windows/croshell.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/windows/im2text.ps1` & `machineconfig-1.5/src/machineconfig/scripts/windows/im2text.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/windows/mount_nfs.ps1` & `machineconfig-1.5/src/machineconfig/scripts/windows/mount_nfs.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/windows/repos.ps1` & `machineconfig-1.5/src/machineconfig/scripts/windows/repos.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/windows/transfer_sh.cmd` & `machineconfig-1.5/src/machineconfig/scripts/windows/transfer_sh.cmd`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/windows/wsl_rdp_windows_port_forwarding.ps1` & `machineconfig-1.5/src/machineconfig/scripts/windows/wsl_rdp_windows_port_forwarding.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/scripts/windows/wsl_ssh_windows_port_forwarding.ps1` & `machineconfig-1.5/src/machineconfig/scripts/windows/wsl_ssh_windows_port_forwarding.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/broot/br.sh` & `machineconfig-1.5/src/machineconfig/settings/broot/br.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/broot/brootcd.ps1` & `machineconfig-1.5/src/machineconfig/settings/broot/brootcd.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/lf/linux/colors` & `machineconfig-1.5/src/machineconfig/settings/lf/windows/colors`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,50 @@
 # vim:ft=dircolors
 # (This is not a dircolors file but it helps to highlight colors and comments)
 
 # default values from dircolors
 # (entries with a leading # are not implemented in lf)
-# #no     00              # NORMAL
-# fi      00              # FILE
-# #rs     0               # RESET
-# di      01;34           # DIR
-# ln      01;36           # LINK
-# #mh     00              # MULTIHARDLINK
-# pi      40;33           # FIFO
-# so      01;35           # SOCK
-# #do     01;35           # DOOR
-# bd      40;33;01        # BLK
-# cd      40;33;01        # CHR
-# or      40;31;01        # ORPHAN
-# #mi     00              # MISSING
-# su      37;41           # SETUID
-# sg      30;43           # SETGID
-# #ca     30;41           # CAPABILITY
-# tw      30;42           # STICKY_OTHER_WRITABLE
-# ow      34;42           # OTHER_WRITABLE
-# st      37;44           # STICKY
-# ex      01;32           # EXEC
+#no     00              # NORMAL
+fi      00;37;40              # FILE
+#rs     0               # RESET
+di      01;31;42           # DIR
+ln      02;32;45           # LINK
+#mh     00              # MULTIHARDLINK
+pi      03;33;40           # FIFO
+so      04;34;43           # SOCK
+#do     01;35           # DOOR
+bd      05;35;44        # BLK
+cd      06;36;45        # CHR
+or      07;37;46        # ORPHAN
+#mi     00              # MISSING
+su      08;31;47           # SETUID
+sg      09;32;40           # SETGID
+#ca     30;41           # CAPABILITY
+tw      01;33;41           # STICKY_OTHER_WRITABLE
+ow      02;36;40           # OTHER_WRITABLE
+st      03;35;43           # STICKY
+ex      04;36;44           # EXEC
 
-# default values from lf (with matching order)
+
+# file types (with matching order)
 # ln      01;36   # LINK
 # or      31;01   # ORPHAN
-# tw      01;34   # STICKY_OTHER_WRITABLE
-# ow      01;34   # OTHER_WRITABLE
+# tw      34      # STICKY_OTHER_WRITABLE
+# ow      34      # OTHER_WRITABLE
 # st      01;34   # STICKY
 # di      01;34   # DIR
 # pi      33      # FIFO
 # so      01;35   # SOCK
 # bd      33;01   # BLK
 # cd      33;01   # CHR
 # su      01;32   # SETUID
 # sg      01;32   # SETGID
 # ex      01;32   # EXEC
 # fi      00      # FILE
 
-# file types (with matching order)
-ln      01;36   # LINK
-or      31;01   # ORPHAN
-tw      34      # STICKY_OTHER_WRITABLE
-ow      34      # OTHER_WRITABLE
-st      01;34   # STICKY
-di      01;34   # DIR
-pi      33      # FIFO
-so      01;35   # SOCK
-bd      33;01   # BLK
-cd      33;01   # CHR
-su      01;32   # SETUID
-sg      01;32   # SETGID
-ex      01;32   # EXEC
-fi      00      # FILE
-
 # archives or compressed (dircolors defaults)
 *.tar   01;31
 *.tgz   01;31
 *.arc   01;31
 *.arj   01;31
 *.taz   01;31
 *.lha   01;31
```

### Comparing `machineconfig-1.4/src/machineconfig/settings/lf/linux/exe/lfcd.sh` & `machineconfig-1.5/src/machineconfig/settings/lf/linux/exe/lfcd.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/lf/linux/icons` & `machineconfig-1.5/src/machineconfig/settings/lf/linux/icons`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/lf/linux/lfrc` & `machineconfig-1.5/src/machineconfig/settings/lf/linux/lfrc`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/lf/windows/icons` & `machineconfig-1.5/src/machineconfig/settings/lf/windows/icons`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/lf/windows/lfcd.ps1` & `machineconfig-1.5/src/machineconfig/settings/lf/windows/lfcd.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/lf/windows/lfrc` & `machineconfig-1.5/src/machineconfig/settings/lf/windows/lfrc`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/lvim/generic/plugins_config/.flake8` & `machineconfig-1.5/src/machineconfig/settings/lvim/generic/plugins_config/.flake8`

 * *Files 2% similar despite different names*

```diff
@@ -6,10 +6,8 @@
 # H301: one import per line
 # H306: imports not in alphabetical order (time, os)
 # H401: docstring should not start with a space
 # H403: multi line docstrings should end on a new line
 # H404: multi line docstring should start without a leading new line
 # H405: multi line docstring summary not separated with an empty line
 # H501: Do not use self.__dict__ for string formatting
-extend-ignore = E301,E302,E501,E701,E702
-
-
+extend-ignore = E301,E302,E501,E701,E702,E225
```

### Comparing `machineconfig-1.4/src/machineconfig/settings/lvim/windows/archive/config_additional.lua` & `machineconfig-1.5/src/machineconfig/settings/lvim/windows/archive/config_additional.lua`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/mprocs/windows/mprocs.yaml` & `machineconfig-1.5/src/machineconfig/settings/mprocs/windows/mprocs.yaml`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/shells/nushell/config.nu` & `machineconfig-1.5/src/machineconfig/settings/shells/nushell/config.nu`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/shells/nushell/env.nu` & `machineconfig-1.5/src/machineconfig/settings/shells/nushell/env.nu`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/shells/pwsh/init.ps1` & `machineconfig-1.5/src/machineconfig/settings/shells/pwsh/init.ps1`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # Set-PSReadlineOption -PredictionViewStyle History
 # see how to get dynamic help with prerelease
 
 
 # PATH extension =====================================================
 $env:Path += ";~\code\machineconfig\src\machineconfig\scripts\windows;~\dotfiles\scripts\windows;C:\Program Files (x86)\GnuWin32\bin;C:\Program Files\CodeBlocks\MinGW\bin;C:\Program Files\nu\bin;C:\Program Files\Graphviz\bin"
 # $machineconfig_path = (python -c "print(__import__('machineconfig').__file__[:-12])")
+#C:\Program Files\Git\bin
+
 
 # sources  ================================================================
 . ~/code/machineconfig/src/machineconfig/settings/broot/brootcd.ps1
 . ~/code/machineconfig/src/machineconfig/settings/lf/windows/lfcd.ps1
 . ~/code/machineconfig/src/machineconfig/settings/tere/terecd.ps1
```

### Comparing `machineconfig-1.4/src/machineconfig/settings/svim/linux/init.toml` & `machineconfig-1.5/src/machineconfig/settings/svim/linux/init.toml`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/svim/windows/init.toml` & `machineconfig-1.5/src/machineconfig/settings/svim/windows/init.toml`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/wsl/.wslconfig` & `machineconfig-1.5/src/machineconfig/settings/wsl/.wslconfig`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # default file from https://learn.microsoft.com/en-us/windows/wsl/wsl-config#wslconfig
 
 # Settings apply across all Linux distros running on WSL 2
 [wsl2]
 
 # Limits VM memory to use no more than 4 GB, this can be set as whole numbers using GB or MB
-memory=8GB
+memory=16GB
 
 # Sets the VM to use two virtual processors
 # processors=2
 
 # Specify a custom Linux kernel to use with your installed distros. The default kernel used can be found at https://github.com/microsoft/WSL2-Linux-Kernel
 # kernel=C:\\temp\\myCustomKernel
```

### Comparing `machineconfig-1.4/src/machineconfig/settings/zellij/config.kdl` & `machineconfig-1.5/src/machineconfig/settings/zellij/config.kdl`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/settings/zellij/config.orig.kdl` & `machineconfig-1.5/src/machineconfig/settings/zellij/config.orig.kdl`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/setup_linux/nix/cli_installation.sh` & `machineconfig-1.5/src/machineconfig/setup_linux/nix/cli_installation.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/setup_linux/web_shortcuts/all.sh` & `machineconfig-1.5/src/machineconfig/setup_linux/web_shortcuts/all.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/setup_linux/web_shortcuts/ascii_art.sh` & `machineconfig-1.5/src/machineconfig/setup_linux/web_shortcuts/ascii_art.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/setup_linux/web_shortcuts/croshell.sh` & `machineconfig-1.5/src/machineconfig/setup_linux/web_shortcuts/croshell.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/setup_linux/web_shortcuts/ssh.sh` & `machineconfig-1.5/src/machineconfig/setup_linux/web_shortcuts/ssh.sh`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/setup_windows/web_shortcuts/all.ps1` & `machineconfig-1.5/src/machineconfig/setup_windows/web_shortcuts/all.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/setup_windows/web_shortcuts/ascii_art.ps1` & `machineconfig-1.5/src/machineconfig/setup_windows/web_shortcuts/ascii_art.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/setup_windows/web_shortcuts/croshell.ps1` & `machineconfig-1.5/src/machineconfig/setup_windows/web_shortcuts/croshell.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/setup_windows/wt_and_pwsh/install_fonts.ps1` & `machineconfig-1.5/src/machineconfig/setup_windows/wt_and_pwsh/install_fonts.ps1`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/setup_windows/wt_and_pwsh/set_pwsh_theme.py` & `machineconfig-1.5/src/machineconfig/setup_windows/wt_and_pwsh/set_pwsh_theme.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/setup_windows/wt_and_pwsh/set_wt_settings.py` & `machineconfig-1.5/src/machineconfig/setup_windows/wt_and_pwsh/set_wt_settings.py`

 * *Files identical despite different names*

### Comparing `machineconfig-1.4/src/machineconfig/utils/utils.py` & `machineconfig-1.5/src/machineconfig/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,642 +44,725 @@
 000002b0: 7028 666f 6c64 6572 3d22 746d 705f 696e  p(folder="tmp_in
 000002c0: 7374 616c 6c65 7273 2229 0d0a 0d0a 0d0a  stallers")......
 000002d0: 6465 6620 6469 7370 6c61 795f 6f70 7469  def display_opti
 000002e0: 6f6e 7328 6d73 672c 206f 7074 696f 6e73  ons(msg, options
 000002f0: 3a20 6c69 7374 2c20 6865 6164 6572 3d22  : list, header="
 00000300: 222c 2074 6169 6c3d 2222 2c20 7072 6f6d  ", tail="", prom
 00000310: 7074 3d22 222c 2064 6566 6175 6c74 3d4e  pt="", default=N
-00000320: 6f6e 652c 2066 7a66 3d46 616c 7365 293a  one, fzf=False):
-00000330: 0d0a 2020 2020 746f 6f6c 5f6e 616d 6520  ..    tool_name 
-00000340: 3d20 2266 7a66 220d 0a20 2020 2069 6620  = "fzf"..    if 
-00000350: 667a 6620 616e 6420 6368 6563 6b5f 746f  fzf and check_to
-00000360: 6f6c 5f65 7869 7374 7328 746f 6f6c 5f6e  ol_exists(tool_n
-00000370: 616d 6529 3a0d 0a20 2020 2020 2020 2069  ame):..        i
-00000380: 6e73 7461 6c6c 5f6e 5f69 6d70 6f72 7428  nstall_n_import(
-00000390: 2270 7966 7a66 2229 0d0a 2020 2020 2020  "pyfzf")..      
-000003a0: 2020 6672 6f6d 2070 7966 7a66 2e70 7966    from pyfzf.pyf
-000003b0: 7a66 2069 6d70 6f72 7420 467a 6650 726f  zf import FzfPro
-000003c0: 6d70 740d 0a20 2020 2020 2020 2066 7a66  mpt..        fzf
-000003d0: 203d 2046 7a66 5072 6f6d 7074 2829 0d0a   = FzfPrompt()..
-000003e0: 2020 2020 2020 2020 6368 6f69 6365 5f69          choice_i
-000003f0: 6478 203d 2066 7a66 2e70 726f 6d70 7428  dx = fzf.prompt(
-00000400: 6f70 7469 6f6e 7329 0d0a 2020 2020 2020  options)..      
-00000410: 2020 6966 2074 7970 6528 6368 6f69 6365    if type(choice
-00000420: 5f69 6478 2920 6973 206c 6973 7420 616e  _idx) is list an
-00000430: 6420 6c65 6e28 6368 6f69 6365 5f69 6478  d len(choice_idx
-00000440: 2920 3d3d 2031 3a20 6368 6f69 6365 5f69  ) == 1: choice_i
-00000450: 6478 203d 2063 686f 6963 655f 6964 785b  dx = choice_idx[
-00000460: 305d 0d0a 2020 2020 656c 7365 3a0d 0a20  0]..    else:.. 
-00000470: 2020 2020 2020 2063 6f6e 736f 6c65 203d         console =
-00000480: 2043 6f6e 736f 6c65 2829 0d0a 2020 2020   Console()..    
-00000490: 2020 2020 6966 2064 6566 6175 6c74 2069      if default i
-000004a0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-000004b0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-000004c0: 6465 6661 756c 7420 696e 206f 7074 696f  default in optio
-000004d0: 6e73 2c20 6622 4465 6661 756c 7420 607b  ns, f"Default `{
-000004e0: 6465 6661 756c 747d 6020 6f70 7469 6f6e  default}` option
-000004f0: 206e 6f74 2069 6e20 6f70 7469 6f6e 7320   not in options 
-00000500: 607b 6c69 7374 286f 7074 696f 6e73 297d  `{list(options)}
-00000510: 6022 0d0a 2020 2020 2020 2020 2020 2020  `"..            
-00000520: 6465 6661 756c 745f 6d73 6720 3d20 5465  default_msg = Te
-00000530: 7874 2866 2220 3c3c 3c3c 2d2d 2d2d 2d2d  xt(f" <<<<------
-00000540: 2d2d 2044 4546 4155 4c54 222c 2073 7479  -- DEFAULT", sty
-00000550: 6c65 3d22 626f 6c64 2072 6564 2229 0d0a  le="bold red")..
-00000560: 2020 2020 2020 2020 656c 7365 3a20 6465          else: de
-00000570: 6661 756c 745f 6d73 6720 3d20 2222 0d0a  fault_msg = ""..
-00000580: 2020 2020 2020 2020 7478 7420 3d20 5465          txt = Te
-00000590: 7874 2822 5c6e 2220 2b20 6d73 6720 2b20  xt("\n" + msg + 
-000005a0: 225c 6e22 290d 0a20 2020 2020 2020 2066  "\n")..        f
-000005b0: 6f72 2069 6478 2c20 6b65 7920 696e 2065  or idx, key in e
-000005c0: 6e75 6d65 7261 7465 286f 7074 696f 6e73  numerate(options
-000005d0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000005e0: 7478 7420 3d20 7478 7420 2b20 5465 7874  txt = txt + Text
-000005f0: 2866 227b 6964 783a 3264 7d20 222c 2073  (f"{idx:2d} ", s
-00000600: 7479 6c65 3d22 626f 6c64 2062 6c75 6522  tyle="bold blue"
-00000610: 2920 2b20 7374 7228 6b65 7929 202b 2028  ) + str(key) + (
-00000620: 6465 6661 756c 745f 6d73 6720 6966 2064  default_msg if d
-00000630: 6566 6175 6c74 2069 7320 6e6f 7420 4e6f  efault is not No
-00000640: 6e65 2061 6e64 2064 6566 6175 6c74 203d  ne and default =
-00000650: 3d20 6b65 7920 656c 7365 2022 2229 202b  = key else "") +
-00000660: 2022 5c6e 220d 0a20 2020 2020 2020 2074   "\n"..        t
-00000670: 7874 203d 2050 616e 656c 2874 7874 2c20  xt = Panel(txt, 
-00000680: 7469 746c 653d 6865 6164 6572 2c20 7375  title=header, su
-00000690: 6274 6974 6c65 3d74 6169 6c2c 2062 6f72  btitle=tail, bor
-000006a0: 6465 725f 7374 796c 653d 2262 6f6c 6420  der_style="bold 
-000006b0: 7265 6422 290d 0a20 2020 2020 2020 2063  red")..        c
-000006c0: 6f6e 736f 6c65 2e70 7269 6e74 2874 7874  onsole.print(txt
-000006d0: 290d 0a20 2020 2020 2020 2063 686f 6963  )..        choic
-000006e0: 655f 6964 7820 3d20 696e 7075 7428 6622  e_idx = input(f"
-000006f0: 7b70 726f 6d70 747d 5c6e 456e 7465 7220  {prompt}\nEnter 
-00000700: 6f70 7469 6f6e 202a 6e75 6d62 6572 2a20  option *number* 
-00000710: 286f 7220 6f70 7469 6f6e 206e 616d 6520  (or option name 
-00000720: 7374 6172 7469 6e67 2077 6974 6820 7370  starting with sp
-00000730: 6163 6529 3a20 2229 0d0a 0d0a 2020 2020  ace): ")....    
-00000740: 6966 2063 686f 6963 655f 6964 782e 7374  if choice_idx.st
-00000750: 6172 7473 7769 7468 2822 2022 293a 0d0a  artswith(" "):..
-00000760: 2020 2020 2020 2020 6368 6f69 6365 5f6b          choice_k
-00000770: 6579 203d 2063 686f 6963 655f 6964 782e  ey = choice_idx.
-00000780: 7374 7269 7028 290d 0a20 2020 2020 2020  strip()..       
-00000790: 2061 7373 6572 7420 6368 6f69 6365 5f6b   assert choice_k
-000007a0: 6579 2069 6e20 6f70 7469 6f6e 732c 2066  ey in options, f
-000007b0: 2243 686f 6963 6520 607b 6368 6f69 6365  "Choice `{choice
-000007c0: 5f6b 6579 7d60 206e 6f74 2069 6e20 6f70  _key}` not in op
-000007d0: 7469 6f6e 7320 607b 6f70 7469 6f6e 737d  tions `{options}
-000007e0: 6022 0d0a 2020 2020 2020 2020 6368 6f69  `"..        choi
-000007f0: 6365 5f69 6478 203d 206f 7074 696f 6e73  ce_idx = options
-00000800: 2e69 6e64 6578 2863 686f 6963 655f 6b65  .index(choice_ke
-00000810: 7929 0d0a 2020 2020 656c 7365 3a0d 0a20  y)..    else:.. 
-00000820: 2020 2020 2020 2069 6620 6368 6f69 6365         if choice
-00000830: 5f69 6478 203d 3d20 2222 3a0d 0a20 2020  _idx == "":..   
-00000840: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00000850: 6465 6661 756c 7420 6973 206e 6f74 204e  default is not N
-00000860: 6f6e 652c 2066 2244 6566 6175 6c74 206f  one, f"Default o
-00000870: 7074 696f 6e20 6e6f 7420 6176 6169 6c61  ption not availa
-00000880: 626c 6521 220d 0a20 2020 2020 2020 2020  ble!"..         
-00000890: 2020 2063 686f 6963 655f 6964 7820 3d20     choice_idx = 
-000008a0: 6f70 7469 6f6e 732e 696e 6465 7828 6465  options.index(de
-000008b0: 6661 756c 7429 0d0a 2020 2020 2020 2020  fault)..        
-000008c0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-000008d0: 2020 7472 793a 2063 686f 6963 655f 6964    try: choice_id
-000008e0: 7820 3d20 696e 7428 6368 6f69 6365 5f69  x = int(choice_i
-000008f0: 6478 290d 0a20 2020 2020 2020 2020 2020  dx)..           
-00000900: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
-00000910: 6f72 3a20 2023 2070 6172 7369 6e67 2065  or:  # parsing e
-00000920: 7272 6f72 0d0a 2020 2020 2020 2020 2020  rror..          
-00000930: 2020 2020 2020 7261 6973 6520 496e 6465        raise Inde
-00000940: 7845 7272 6f72 0d0a 2020 2020 2020 2020  xError..        
-00000950: 2020 2020 6368 6f69 6365 5f6b 6579 203d      choice_key =
-00000960: 206f 7074 696f 6e73 5b63 686f 6963 655f   options[choice_
-00000970: 6964 785d 0d0a 2020 2020 2020 2020 6578  idx]..        ex
-00000980: 6365 7074 2049 6e64 6578 4572 726f 723a  cept IndexError:
-00000990: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000009a0: 6d61 6e79 2062 6520 7573 6572 2066 6f72  many be user for
-000009b0: 676f 7474 656e 2074 6f20 7374 6172 7420  gotten to start 
-000009c0: 7769 7468 2061 2064 6173 680d 0a20 2020  with a dash..   
-000009d0: 2020 2020 2020 2020 2069 6620 6368 6f69           if choi
-000009e0: 6365 5f69 6478 2069 6e20 6f70 7469 6f6e  ce_idx in option
-000009f0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00000a00: 2020 2020 6368 6f69 6365 5f6b 6579 203d      choice_key =
-00000a10: 2063 686f 6963 655f 6964 780d 0a20 2020   choice_idx..   
-00000a20: 2020 2020 2020 2020 2020 2020 2063 686f               cho
-00000a30: 6963 655f 6964 7820 3d20 6f70 7469 6f6e  ice_idx = option
-00000a40: 732e 696e 6465 7828 6368 6f69 6365 5f69  s.index(choice_i
-00000a50: 6478 290d 0a20 2020 2020 2020 2020 2020  dx)..           
-00000a60: 2065 6c73 653a 2072 6169 7365 2056 616c   else: raise Val
-00000a70: 7565 4572 726f 7228 6622 556e 6b6e 6f77  ueError(f"Unknow
-00000a80: 6e20 6368 6f69 6365 2e20 7b63 686f 6963  n choice. {choic
-00000a90: 655f 6964 787d 2229 0d0a 2020 2020 7072  e_idx}")..    pr
-00000aa0: 696e 7428 6622 7b63 686f 6963 655f 6964  int(f"{choice_id
-00000ab0: 787d 3a20 7b63 686f 6963 655f 6b65 797d  x}: {choice_key}
-00000ac0: 222c 2066 223c 3c3c 3c2d 2d2d 2d2d 2d2d  ", f"<<<<-------
-00000ad0: 2d20 4348 4f49 4345 204d 4144 4522 290d  - CHOICE MADE").
-00000ae0: 0a20 2020 2072 6574 7572 6e20 6368 6f69  .    return choi
-00000af0: 6365 5f6b 6579 0d0a 0d0a 0d0a 6465 6620  ce_key......def 
-00000b00: 7379 6d6c 696e 6b28 7468 6973 3a20 502c  symlink(this: P,
-00000b10: 2074 6f5f 7468 6973 3a20 502c 2070 7269   to_this: P, pri
-00000b20: 6f72 6974 697a 655f 746f 5f74 6869 733d  oritize_to_this=
-00000b30: 5472 7565 293a 0d0a 2020 2020 2222 2268  True):..    """h
-00000b40: 656c 7065 7220 6675 6e63 7469 6f6e 2e20  elper function. 
-00000b50: 6372 6561 7465 7320 6120 7379 6d6c 696e  creates a symlin
-00000b60: 6b20 6672 6f6d 2060 7468 6973 6020 746f  k from `this` to
-00000b70: 2060 746f 5f74 6869 7360 2e0d 0a20 2020   `to_this`...   
-00000b80: 2057 6861 7420 6361 6e20 676f 2077 726f   What can go wro
-00000b90: 6e67 3f0d 0a20 2020 2064 6570 656e 6469  ng?..    dependi
-00000ba0: 6e67 206f 6e20 7468 6973 2061 6e64 2074  ng on this and t
-00000bb0: 6f5f 7468 6973 2065 7869 7374 656e 6365  o_this existence
-00000bc0: 2c20 6f6e 6520 7769 6c6c 2062 6520 7072  , one will be pr
-00000bd0: 696f 7265 7469 7a65 6420 6465 7065 6e64  ioretized depend
-00000be0: 696e 6720 6f6e 206f 7665 7277 7269 7465  ing on overwrite
-00000bf0: 2076 616c 7565 2e0d 0a20 2020 2054 7275   value...    Tru
-00000c00: 6520 6d65 616e 7320 7468 6973 2077 696c  e means this wil
-00000c10: 6c20 706f 7465 6e74 6961 6c6c 7920 6265  l potentially be
-00000c20: 206f 7665 7277 7269 7474 656e 2028 6465   overwritten (de
-00000c30: 7065 6e64 696e 6720 6f6e 2077 6865 7468  pending on wheth
-00000c40: 6572 2074 6f5f 7468 6973 2065 7869 7374  er to_this exist
-00000c50: 7320 6f72 206e 6f74 290d 0a20 2020 2046  s or not)..    F
-00000c60: 616c 7365 206d 6561 6e73 2074 6f5f 7468  alse means to_th
-00000c70: 6973 2077 696c 6c20 706f 7465 6e74 6961  is will potentia
-00000c80: 6c6c 7920 6265 206f 7665 7277 6974 7474  lly be overwittt
-00000c90: 656e 2e22 2222 0d0a 2020 2020 7468 6973  en."""..    this
-00000ca0: 203d 2050 2874 6869 7329 2e65 7870 616e   = P(this).expan
-00000cb0: 6475 7365 7228 292e 6162 736f 6c75 7465  duser().absolute
-00000cc0: 2829 0d0a 2020 2020 746f 5f74 6869 7320  ()..    to_this 
-00000cd0: 3d20 5028 746f 5f74 6869 7329 2e65 7870  = P(to_this).exp
-00000ce0: 616e 6475 7365 7228 292e 6162 736f 6c75  anduser().absolu
-00000cf0: 7465 2829 0d0a 2020 2020 6966 2074 6869  te()..    if thi
-00000d00: 732e 6973 5f73 796d 6c69 6e6b 2829 3a20  s.is_symlink(): 
-00000d10: 7468 6973 2e64 656c 6574 6528 7375 7265  this.delete(sure
-00000d20: 3d54 7275 6529 2020 2320 6465 6c65 7465  =True)  # delete
-00000d30: 2069 6620 6974 2065 7869 7374 7320 6173   if it exists as
-00000d40: 2073 796d 626c 6963 206c 696e 6b2c 206e   symblic link, n
-00000d50: 6f74 2061 2063 6f6e 6372 6574 6520 7061  ot a concrete pa
-00000d60: 7468 2e0d 0a20 2020 2069 6620 7468 6973  th...    if this
-00000d70: 2e65 7869 7374 7328 293a 2020 2320 7468  .exists():  # th
-00000d80: 6973 2069 7320 6120 7072 6f62 6c65 6d2e  is is a problem.
-00000d90: 2049 7420 7769 6c6c 2062 6520 7265 736f   It will be reso
-00000da0: 6c76 6564 2076 6961 2060 6f76 6572 7772  lved via `overwr
-00000db0: 6974 6560 0d0a 2020 2020 2020 2020 6966  ite`..        if
-00000dc0: 2070 7269 6f72 6974 697a 655f 746f 5f74   prioritize_to_t
-00000dd0: 6869 7320 6973 2054 7275 653a 2020 2320  his is True:  # 
-00000de0: 6974 202a 6361 6e2a 2062 6520 6465 6c65  it *can* be dele
-00000df0: 7465 642c 2062 7574 206c 6574 2773 206c  ted, but let's l
-00000e00: 6f6f 6b20 6174 2074 6172 6765 7420 6669  ook at target fi
-00000e10: 7273 742e 0d0a 2020 2020 2020 2020 2020  rst...          
-00000e20: 2020 6966 2074 6f5f 7468 6973 2e65 7869    if to_this.exi
-00000e30: 7374 7328 293a 2020 2320 7468 6973 2065  sts():  # this e
-00000e40: 7869 7374 732c 2074 6f5f 7468 6973 2061  xists, to_this a
-00000e50: 7320 7765 6c6c 2e20 746f 5f74 6869 7320  s well. to_this 
-00000e60: 6973 2070 7269 6f72 6974 697a 6564 2e0d  is prioritized..
-00000e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e80: 2074 6869 732e 6170 7065 6e64 2866 222e   this.append(f".
-00000e90: 6f72 6967 5f7b 7261 6e64 7374 7228 297d  orig_{randstr()}
-00000ea0: 222c 2069 6e70 6c61 6365 3d54 7275 6529  ", inplace=True)
-00000eb0: 2020 2320 7265 6e61 6d65 2069 7320 6265    # rename is be
-00000ec0: 7474 6572 2074 6861 6e20 6465 6c65 7469  tter than deleti
-00000ed0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-00000ee0: 656c 7365 3a20 7468 6973 2e6d 6f76 6528  else: this.move(
-00000ef0: 7061 7468 3d74 6f5f 7468 6973 2920 2023  path=to_this)  #
-00000f00: 2074 6869 7320 6578 6973 7473 2c20 746f   this exists, to
-00000f10: 5f74 6869 7320 646f 6573 6e27 742e 2074  _this doesn't. t
-00000f20: 6f5f 7468 6973 2069 7320 7072 696f 7269  o_this is priori
-00000f30: 7469 7a65 642e 0d0a 2020 2020 2020 2020  tized...        
-00000f40: 656c 6966 2070 7269 6f72 6974 697a 655f  elif prioritize_
-00000f50: 746f 5f74 6869 7320 6973 2046 616c 7365  to_this is False
-00000f60: 3a20 2023 2064 6f6e 2774 2073 6163 7265  :  # don't sacre
-00000f70: 6669 6365 2074 6869 732c 2073 6163 7265  fice this, sacre
-00000f80: 6669 6365 2074 6f5f 7468 6973 2e0d 0a20  fice to_this... 
-00000f90: 2020 2020 2020 2020 2020 2069 6620 746f             if to
-00000fa0: 5f74 6869 732e 6578 6973 7473 2829 3a20  _this.exists(): 
-00000fb0: 7468 6973 2e6d 6f76 6528 7061 7468 3d74  this.move(path=t
-00000fc0: 6f5f 7468 6973 2c20 6f76 6572 7772 6974  o_this, overwrit
-00000fd0: 653d 5472 7565 2920 2023 2074 6869 7320  e=True)  # this 
-00000fe0: 6578 6973 7473 2c20 746f 5f74 6869 7320  exists, to_this 
-00000ff0: 6173 2077 656c 6c2c 2074 6869 7320 6973  as well, this is
-00001000: 2070 7269 6f72 6974 697a 6564 2e20 2020   prioritized.   
-00001010: 2320 6e6f 7720 7765 2061 7265 2072 6561  # now we are rea
-00001020: 646c 7920 746f 206d 616b 6520 7468 6520  dly to make the 
-00001030: 6c69 6e6b 0d0a 2020 2020 2020 2020 2020  link..          
-00001040: 2020 656c 7365 3a20 7468 6973 2e6d 6f76    else: this.mov
-00001050: 6528 7061 7468 3d74 6f5f 7468 6973 2920  e(path=to_this) 
-00001060: 2023 2074 6869 7320 6578 6973 7473 2c20   # this exists, 
-00001070: 746f 5f74 6869 7320 646f 6573 6e27 742c  to_this doesn't,
-00001080: 2074 6869 7320 6973 2070 7269 6f72 6974   this is priorit
-00001090: 697a 6564 2e0d 0a20 2020 2065 6c73 653a  ized...    else:
-000010a0: 2020 2320 7468 6973 2064 6f65 736e 2774    # this doesn't
-000010b0: 2065 7869 7374 2e0d 0a20 2020 2020 2020   exist...       
-000010c0: 2069 6620 6e6f 7420 746f 5f74 6869 732e   if not to_this.
-000010d0: 6578 6973 7473 2829 3a20 746f 5f74 6869  exists(): to_thi
-000010e0: 732e 746f 7563 6828 2920 2023 2077 6520  s.touch()  # we 
-000010f0: 6861 7665 2074 6f20 746f 7563 6820 6974  have to touch it
-00001100: 2028 6669 6c65 2920 6f72 2063 7265 6174   (file) or creat
-00001110: 6520 6974 2028 666f 6c64 6572 290d 0a20  e it (folder).. 
-00001120: 2020 2069 6620 706c 6174 666f 726d 2e73     if platform.s
-00001130: 7973 7465 6d28 2920 3d3d 2022 5769 6e64  ystem() == "Wind
-00001140: 6f77 7322 3a20 5f20 3d20 696e 7374 616c  ows": _ = instal
-00001150: 6c5f 6e5f 696d 706f 7274 2822 7769 6e33  l_n_import("win3
-00001160: 3261 7069 222c 2022 7079 7769 6e33 3222  2api", "pywin32"
-00001170: 2920 2023 2074 6869 7320 6973 2063 7275  )  # this is cru
-00001180: 6369 616c 2066 6f72 2077 696e 646f 7773  cial for windows
-00001190: 2074 6f20 706f 7020 7570 2074 6865 2063   to pop up the c
-000011a0: 6f6e 6365 6e74 2077 696e 646f 7720 696e  oncent window in
-000011b0: 2063 6173 6520 7079 7468 6f6e 2077 6173   case python was
-000011c0: 206e 6f74 2072 756e 2061 7320 6164 6d69   not run as admi
-000011d0: 6e2e 0d0a 2020 2020 7472 793a 0d0a 2020  n...    try:..  
-000011e0: 2020 2020 2020 5028 7468 6973 292e 7379        P(this).sy
-000011f0: 6d6c 696e 6b5f 746f 2874 6f5f 7468 6973  mlink_to(to_this
-00001200: 2c20 7665 7262 6f73 653d 5472 7565 2c20  , verbose=True, 
-00001210: 6f76 6572 7772 6974 653d 5472 7565 290d  overwrite=True).
-00001220: 0a20 2020 2065 7863 6570 7420 4578 6365  .    except Exce
-00001230: 7074 696f 6e20 6173 2065 783a 2070 7269  ption as ex: pri
-00001240: 6e74 2866 2246 6169 6c65 6420 6174 206c  nt(f"Failed at l
-00001250: 696e 6b69 6e67 207b 7468 6973 7d20 3d3d  inking {this} ==
-00001260: 3e20 7b74 6f5f 7468 6973 7d2e 5c6e 5265  > {to_this}.\nRe
-00001270: 6173 6f6e 3a20 7b65 787d 2229 0d0a 0d0a  ason: {ex}")....
-00001280: 0d0a 6465 6620 6669 6e64 5f6d 6f76 655f  ..def find_move_
-00001290: 6465 6c65 7465 5f77 696e 646f 7773 2864  delete_windows(d
-000012a0: 6f77 6e6c 6f61 6465 642c 2074 6f6f 6c5f  ownloaded, tool_
-000012b0: 6e61 6d65 3d4e 6f6e 652c 2064 656c 6574  name=None, delet
-000012c0: 653d 5472 7565 293a 0d0a 2020 2020 6966  e=True):..    if
-000012d0: 2074 6f6f 6c5f 6e61 6d65 2069 7320 6e6f   tool_name is no
-000012e0: 7420 4e6f 6e65 2061 6e64 2022 2e65 7865  t None and ".exe
-000012f0: 2220 696e 2074 6f6f 6c5f 6e61 6d65 3a20  " in tool_name: 
-00001300: 746f 6f6c 5f6e 616d 6520 3d20 746f 6f6c  tool_name = tool
-00001310: 5f6e 616d 652e 7265 706c 6163 6528 222e  _name.replace(".
-00001320: 6578 6522 2c20 2222 290d 0a20 2020 2069  exe", "")..    i
-00001330: 6620 646f 776e 6c6f 6164 6564 2e69 735f  f downloaded.is_
-00001340: 6669 6c65 2829 3a0d 0a20 2020 2020 2020  file():..       
-00001350: 2065 7865 203d 2064 6f77 6e6c 6f61 6465   exe = downloade
-00001360: 640d 0a20 2020 2065 6c73 653a 0d0a 2020  d..    else:..  
-00001370: 2020 2020 2020 6966 2074 6f6f 6c5f 6e61        if tool_na
-00001380: 6d65 2069 7320 4e6f 6e65 3a20 6578 6520  me is None: exe 
-00001390: 3d20 646f 776e 6c6f 6164 6564 2e73 6561  = downloaded.sea
-000013a0: 7263 6828 222a 2e65 7865 222c 2072 3d54  rch("*.exe", r=T
-000013b0: 7275 6529 5b30 5d0d 0a20 2020 2020 2020  rue)[0]..       
-000013c0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-000013d0: 2020 2020 746d 7020 3d20 646f 776e 6c6f      tmp = downlo
-000013e0: 6164 6564 2e73 6561 7263 6828 6622 7b74  aded.search(f"{t
-000013f0: 6f6f 6c5f 6e61 6d65 7d2e 6578 6522 2c20  ool_name}.exe", 
-00001400: 723d 5472 7565 290d 0a20 2020 2020 2020  r=True)..       
-00001410: 2020 2020 2069 6620 6c65 6e28 746d 7029       if len(tmp)
-00001420: 203d 3d20 313a 2065 7865 203d 2074 6d70   == 1: exe = tmp
-00001430: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
-00001440: 2065 6c73 653a 2065 7865 203d 2064 6f77   else: exe = dow
-00001450: 6e6c 6f61 6465 642e 7365 6172 6368 2822  nloaded.search("
-00001460: 2a2e 6578 6522 2c20 723d 5472 7565 295b  *.exe", r=True)[
-00001470: 305d 0d0a 2020 2020 6578 652e 6d6f 7665  0]..    exe.move
-00001480: 2866 6f6c 6465 723d 502e 6765 745f 656e  (folder=P.get_en
-00001490: 7628 292e 5769 6e64 6f77 7341 7070 732c  v().WindowsApps,
-000014a0: 206f 7665 7277 7269 7465 3d54 7275 6529   overwrite=True)
-000014b0: 2020 2320 6c61 7465 7374 2076 6572 7369    # latest versi
-000014c0: 6f6e 206f 7665 7277 7269 7465 7320 6f6c  on overwrites ol
-000014d0: 6465 7220 696e 7374 616c 6c61 7469 6f6e  der installation
-000014e0: 2e0d 0a20 2020 2069 6620 6465 6c65 7465  ...    if delete
-000014f0: 3a20 646f 776e 6c6f 6164 6564 2e64 656c  : downloaded.del
-00001500: 6574 6528 7375 7265 3d54 7275 6529 0d0a  ete(sure=True)..
-00001510: 2020 2020 7265 7475 726e 2065 7865 0d0a      return exe..
-00001520: 0d0a 0d0a 6465 6620 6669 6e64 5f6d 6f76  ....def find_mov
-00001530: 655f 6465 6c65 7465 5f6c 696e 7578 2864  e_delete_linux(d
-00001540: 6f77 6e6c 6f61 6465 642c 2074 6f6f 6c5f  ownloaded, tool_
-00001550: 6e61 6d65 2c20 6465 6c65 7465 3d54 7275  name, delete=Tru
-00001560: 6529 3a0d 0a20 2020 2069 6620 646f 776e  e):..    if down
-00001570: 6c6f 6164 6564 2e69 735f 6669 6c65 2829  loaded.is_file()
-00001580: 3a0d 0a20 2020 2020 2020 2065 7865 203d  :..        exe =
-00001590: 2064 6f77 6e6c 6f61 6465 640d 0a20 2020   downloaded..   
-000015a0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-000015b0: 7265 7320 3d20 646f 776e 6c6f 6164 6564  res = downloaded
-000015c0: 2e73 6561 7263 6828 6622 2a7b 746f 6f6c  .search(f"*{tool
-000015d0: 5f6e 616d 657d 2a22 2c20 666f 6c64 6572  _name}*", folder
-000015e0: 733d 4661 6c73 652c 2072 3d54 7275 6529  s=False, r=True)
-000015f0: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
-00001600: 2872 6573 2920 3d3d 2031 3a20 6578 6520  (res) == 1: exe 
-00001610: 3d20 7265 735b 305d 0d0a 2020 2020 2020  = res[0]..      
-00001620: 2020 656c 7365 3a20 6578 6520 3d20 646f    else: exe = do
-00001630: 776e 6c6f 6164 6564 2e73 6561 7263 6828  wnloaded.search(
-00001640: 746f 6f6c 5f6e 616d 652c 2066 6f6c 6465  tool_name, folde
-00001650: 7273 3d46 616c 7365 2c20 723d 5472 7565  rs=False, r=True
-00001660: 295b 305d 0d0a 2020 2020 7072 696e 7428  )[0]..    print(
-00001670: 6622 4d4f 5649 4e47 2066 696c 6520 607b  f"MOVING file `{
-00001680: 7265 7072 2865 7865 297d 6020 746f 2027  repr(exe)}` to '
-00001690: 2f75 7372 2f6c 6f63 616c 2f62 696e 2722  /usr/local/bin'"
-000016a0: 290d 0a20 2020 2065 7865 2e63 686d 6f64  )..    exe.chmod
-000016b0: 2830 6f37 3737 290d 0a20 2020 2023 2065  (0o777)..    # e
-000016c0: 7865 2e6d 6f76 6528 666f 6c64 6572 3d72  xe.move(folder=r
-000016d0: 222f 7573 722f 6c6f 6361 6c2f 6269 6e22  "/usr/local/bin"
-000016e0: 2c20 6f76 6572 7772 6974 653d 4661 6c73  , overwrite=Fals
-000016f0: 6529 0d0a 2020 2020 5465 726d 696e 616c  e)..    Terminal
-00001700: 2829 2e72 756e 2866 2273 7564 6f20 6d76  ().run(f"sudo mv
-00001710: 207b 6578 657d 202f 7573 722f 6c6f 6361   {exe} /usr/loca
-00001720: 6c2f 6269 6e2f 2229 2e70 7269 6e74 5f69  l/bin/").print_i
-00001730: 665f 756e 7375 6363 6573 7366 756c 2864  f_unsuccessful(d
-00001740: 6573 633d 224d 4f56 494e 4720 6578 6563  esc="MOVING exec
-00001750: 7574 6162 6c65 2074 6f20 2f75 7372 2f6c  utable to /usr/l
-00001760: 6f63 616c 2f62 696e 222c 2073 7472 6963  ocal/bin", stric
-00001770: 745f 6572 723d 5472 7565 2c20 7374 7269  t_err=True, stri
-00001780: 6374 5f72 6574 7572 6e63 6f64 653d 5472  ct_returncode=Tr
-00001790: 7565 290d 0a20 2020 2069 6620 6465 6c65  ue)..    if dele
-000017a0: 7465 3a20 646f 776e 6c6f 6164 6564 2e64  te: downloaded.d
-000017b0: 656c 6574 6528 7375 7265 3d54 7275 6529  elete(sure=True)
-000017c0: 0d0a 2020 2020 7265 7475 726e 204e 6f6e  ..    return Non
-000017d0: 650d 0a0d 0a0d 0a64 6566 2067 6574 5f6c  e......def get_l
-000017e0: 6174 6573 745f 7265 6c65 6173 6528 7265  atest_release(re
-000017f0: 706f 5f75 726c 2c20 646f 776e 6c6f 6164  po_url, download
-00001800: 5f6e 5f65 7874 7261 6374 3d46 616c 7365  _n_extract=False
-00001810: 2c20 7375 6666 6978 3d22 7838 365f 3634  , suffix="x86_64
-00001820: 2d70 632d 7769 6e64 6f77 732d 6d73 7663  -pc-windows-msvc
-00001830: 222c 2066 696c 655f 6e61 6d65 3d4e 6f6e  ", file_name=Non
-00001840: 652c 2074 6f6f 6c5f 6e61 6d65 3d4e 6f6e  e, tool_name=Non
-00001850: 652c 2065 7865 5f6e 616d 653d 4e6f 6e65  e, exe_name=None
-00001860: 2c20 6465 6c65 7465 3d54 7275 652c 2073  , delete=True, s
-00001870: 7472 6970 5f76 3d46 616c 7365 2c20 6c69  trip_v=False, li
-00001880: 6e75 783d 4661 6c73 652c 2063 6f6d 7072  nux=False, compr
-00001890: 6573 7369 6f6e 3d4e 6f6e 652c 2073 6570  ession=None, sep
-000018a0: 3d22 2d22 2c20 7665 7273 696f 6e3d 4e6f  ="-", version=No
-000018b0: 6e65 293a 0d0a 2020 2020 636f 6e73 6f6c  ne):..    consol
-000018c0: 6520 3d20 436f 6e73 6f6c 6528 290d 0a20  e = Console().. 
-000018d0: 2020 2070 7269 6e74 2822 5c6e 5c6e 5c6e     print("\n\n\n
-000018e0: 2229 0d0a 2020 2020 7072 696e 7428 6622  ")..    print(f"
-000018f0: 496e 7370 6563 7469 6e67 206c 6174 6573  Inspecting lates
-00001900: 7420 7265 6c65 6173 6520 4020 7b72 6570  t release @ {rep
-00001910: 6f5f 7572 6c7d 2020 202e 2e2e 2229 0d0a  o_url}   ...")..
-00001920: 2020 2020 2320 7769 7468 2063 6f6e 736f      # with conso
-00001930: 6c65 2e73 7461 7475 7328 2249 6e73 7461  le.status("Insta
-00001940: 6c6c 696e 672e 2e2e 2229 3a20 2023 206d  lling..."):  # m
-00001950: 616b 6573 2074 726f 7562 6c65 7320 6f6e  akes troubles on
-00001960: 206c 696e 7578 2077 6865 6e20 7072 6f6d   linux when prom
-00001970: 7074 2061 736b 7320 666f 7220 7061 7373  pt asks for pass
-00001980: 776f 7264 2074 6f20 6d6f 7665 2066 696c  word to move fil
-00001990: 6520 746f 202f 7573 722f 6269 6e0d 0a0d  e to /usr/bin...
-000019a0: 0a20 2020 2069 6620 7665 7273 696f 6e20  .    if version 
-000019b0: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-000019c0: 2020 696d 706f 7274 2072 6571 7565 7374    import request
-000019d0: 7320 2023 2068 7474 7073 3a2f 2f64 6f63  s  # https://doc
-000019e0: 732e 6769 7468 7562 2e63 6f6d 2f65 6e2f  s.github.com/en/
-000019f0: 7265 706f 7369 746f 7269 6573 2f72 656c  repositories/rel
-00001a00: 6561 7369 6e67 2d70 726f 6a65 6374 732d  easing-projects-
-00001a10: 6f6e 2d67 6974 6875 622f 6c69 6e6b 696e  on-github/linkin
-00001a20: 672d 746f 2d72 656c 6561 7365 730d 0a20  g-to-releases.. 
-00001a30: 2020 2020 2020 206c 6174 6573 745f 7665         latest_ve
-00001a40: 7273 696f 6e20 3d20 7265 7175 6573 7473  rsion = requests
-00001a50: 2e67 6574 2873 7472 2872 6570 6f5f 7572  .get(str(repo_ur
-00001a60: 6c29 202b 2022 2f72 656c 6561 7365 732f  l) + "/releases/
-00001a70: 6c61 7465 7374 2229 2e75 726c 2e73 706c  latest").url.spl
-00001a80: 6974 2822 2f22 295b 2d31 5d20 2023 2074  it("/")[-1]  # t
-00001a90: 6869 7320 6973 2074 6f20 7265 736f 6c76  his is to resolv
-00001aa0: 6520 7468 6520 7265 6469 7265 6374 696f  e the redirectio
-00001ab0: 6e20 7468 6174 206f 6363 7572 6573 3a20  n that occures: 
-00001ac0: 6874 7470 733a 2f2f 7374 6163 6b6f 7665  https://stackove
-00001ad0: 7266 6c6f 772e 636f 6d2f 7175 6573 7469  rflow.com/questi
-00001ae0: 6f6e 732f 3336 3037 3038 3231 2f68 6f77  ons/36070821/how
-00001af0: 2d74 6f2d 6765 742d 7265 6469 7265 6374  -to-get-redirect
-00001b00: 2d75 726c 2d75 7369 6e67 2d70 7974 686f  -url-using-pytho
-00001b10: 6e2d 7265 7175 6573 7473 0d0a 2020 2020  n-requests..    
-00001b20: 656c 7365 3a20 6c61 7465 7374 5f76 6572  else: latest_ver
-00001b30: 7369 6f6e 203d 2076 6572 7369 6f6e 0d0a  sion = version..
-00001b40: 0d0a 2020 2020 646f 776e 6c6f 6164 5f6c  ..    download_l
-00001b50: 696e 6b20 3d20 5028 7265 706f 5f75 726c  ink = P(repo_url
-00001b60: 202b 2022 2f72 656c 6561 7365 732f 646f   + "/releases/do
-00001b70: 776e 6c6f 6164 2f22 202b 206c 6174 6573  wnload/" + lates
-00001b80: 745f 7665 7273 696f 6e29 0d0a 2020 2020  t_version)..    
-00001b90: 636f 6d70 7265 7373 696f 6e20 3d20 636f  compression = co
-00001ba0: 6d70 7265 7373 696f 6e20 6f72 2028 227a  mpression or ("z
-00001bb0: 6970 2220 6966 206e 6f74 206c 696e 7578  ip" if not linux
-00001bc0: 2065 6c73 6520 2274 6172 2e67 7a22 290d   else "tar.gz").
-00001bd0: 0a20 2020 2076 6572 7369 6f6e 203d 2064  .    version = d
-00001be0: 6f77 6e6c 6f61 645f 6c69 6e6b 5b2d 315d  ownload_link[-1]
-00001bf0: 0d0a 2020 2020 7665 7273 696f 6e20 3d20  ..    version = 
-00001c00: 7374 7228 7665 7273 696f 6e29 2e72 6570  str(version).rep
-00001c10: 6c61 6365 2822 7622 2c20 2222 2920 6966  lace("v", "") if
-00001c20: 2073 7472 6970 5f76 2065 6c73 6520 7374   strip_v else st
-00001c30: 7228 7665 7273 696f 6e29 0d0a 2020 2020  r(version)..    
-00001c40: 746f 6f6c 5f6e 616d 6520 3d20 746f 6f6c  tool_name = tool
-00001c50: 5f6e 616d 6520 6f72 2050 2872 6570 6f5f  _name or P(repo_
-00001c60: 7572 6c29 5b2d 315d 0d0a 2020 2020 502e  url)[-1]..    P.
-00001c70: 686f 6d65 2829 2e6a 6f69 6e70 6174 6828  home().joinpath(
-00001c80: 6622 746d 705f 7265 7375 6c74 732f 636c  f"tmp_results/cl
-00001c90: 695f 746f 6f6c 735f 696e 7374 616c 6c65  i_tools_installe
-00001ca0: 7273 2f76 6572 7369 6f6e 732f 7b74 6f6f  rs/versions/{too
-00001cb0: 6c5f 6e61 6d65 7d22 292e 6372 6561 7465  l_name}").create
-00001cc0: 2870 6172 656e 7473 5f6f 6e6c 793d 5472  (parents_only=Tr
-00001cd0: 7565 292e 7772 6974 655f 7465 7874 2876  ue).write_text(v
-00001ce0: 6572 7369 6f6e 290d 0a0d 0a20 2020 2069  ersion)....    i
-00001cf0: 6620 6e6f 7420 646f 776e 6c6f 6164 5f6e  f not download_n
-00001d00: 5f65 7874 7261 6374 3a20 7265 7475 726e  _extract: return
-00001d10: 2064 6f77 6e6c 6f61 645f 6c69 6e6b 0d0a   download_link..
-00001d20: 2020 2020 636f 6e73 6f6c 652e 7275 6c65      console.rule
-00001d30: 2866 2249 6e73 7461 6c6c 696e 6720 7b74  (f"Installing {t
-00001d40: 6f6f 6c5f 6e61 6d65 7d20 7665 7273 696f  ool_name} versio
-00001d50: 6e20 7b76 6572 7369 6f6e 7d22 290d 0a20  n {version}").. 
-00001d60: 2020 2069 6620 6669 6c65 5f6e 616d 6520     if file_name 
-00001d70: 6973 204e 6f6e 653a 2020 2320 6974 2069  is None:  # it i
-00001d80: 7320 6e6f 7420 636f 6e73 7461 6e74 2c20  s not constant, 
-00001d90: 736f 2077 6520 636f 6d70 696c 6520 6974  so we compile it
-00001da0: 2066 726f 6d20 7061 7274 7320 6173 2066   from parts as f
-00001db0: 6f6c 6c6f 7773 3a0d 0a20 2020 2020 2020  ollows:..       
-00001dc0: 2066 696c 655f 6e61 6d65 203d 2066 277b   file_name = f'{
-00001dd0: 746f 6f6c 5f6e 616d 657d 7b73 6570 7d7b  tool_name}{sep}{
-00001de0: 7665 7273 696f 6e7d 7b73 6570 7d7b 7375  version}{sep}{su
-00001df0: 6666 6978 7d2e 7b63 6f6d 7072 6573 7369  ffix}.{compressi
-00001e00: 6f6e 7d27 0d0a 2020 2020 646f 776e 6c6f  on}'..    downlo
-00001e10: 6164 5f6c 696e 6b20 3d20 646f 776e 6c6f  ad_link = downlo
-00001e20: 6164 5f6c 696e 6b2e 6a6f 696e 7061 7468  ad_link.joinpath
-00001e30: 2866 696c 655f 6e61 6d65 290d 0a20 2020  (file_name)..   
-00001e40: 2070 7269 6e74 2822 446f 776e 6c6f 6164   print("Download
-00001e50: 696e 6722 2c20 646f 776e 6c6f 6164 5f6c  ing", download_l
-00001e60: 696e 6b2e 6173 5f75 726c 5f73 7472 2829  ink.as_url_str()
-00001e70: 290d 0a20 2020 2064 6f77 6e6c 6f61 6465  )..    downloade
-00001e80: 6420 3d20 646f 776e 6c6f 6164 5f6c 696e  d = download_lin
-00001e90: 6b2e 646f 776e 6c6f 6164 2866 6f6c 6465  k.download(folde
-00001ea0: 723d 746d 705f 696e 7374 616c 6c5f 6469  r=tmp_install_di
-00001eb0: 7229 0d0a 0d0a 2020 2020 6966 2022 7461  r)....    if "ta
-00001ec0: 722e 677a 2220 696e 2064 6f77 6e6c 6f61  r.gz" in downloa
-00001ed0: 645f 6c69 6e6b 3a20 646f 776e 6c6f 6164  d_link: download
-00001ee0: 6564 203d 2064 6f77 6e6c 6f61 6465 642e  ed = downloaded.
-00001ef0: 756e 677a 5f75 6e74 6172 2869 6e70 6c61  ungz_untar(inpla
-00001f00: 6365 3d54 7275 6529 0d0a 2020 2020 656c  ce=True)..    el
-00001f10: 6966 2022 7a69 7022 2069 6e20 646f 776e  if "zip" in down
-00001f20: 6c6f 6164 5f6c 696e 6b3a 2064 6f77 6e6c  load_link: downl
-00001f30: 6f61 6465 6420 3d20 646f 776e 6c6f 6164  oaded = download
-00001f40: 6564 2e75 6e7a 6970 2869 6e70 6c61 6365  ed.unzip(inplace
-00001f50: 3d54 7275 652c 206f 7665 7277 7269 7465  =True, overwrite
-00001f60: 3d54 7275 6529 0d0a 2020 2020 656c 6966  =True)..    elif
-00001f70: 2022 7461 722e 787a 2220 696e 2064 6f77   "tar.xz" in dow
-00001f80: 6e6c 6f61 645f 6c69 6e6b 3a20 646f 776e  nload_link: down
-00001f90: 6c6f 6164 6564 203d 2064 6f77 6e6c 6f61  loaded = downloa
-00001fa0: 6465 642e 756e 787a 5f75 6e74 6172 2869  ded.unxz_untar(i
-00001fb0: 6e70 6c61 6365 3d54 7275 6529 0d0a 2020  nplace=True)..  
-00001fc0: 2020 656c 7365 3a20 7061 7373 2020 2320    else: pass  # 
-00001fd0: 6e6f 2063 6f6d 7072 6573 7369 6f6e 2e0d  no compression..
-00001fe0: 0a0d 0a20 2020 2069 6620 646f 776e 6c6f  ...    if downlo
-00001ff0: 6164 5f6e 5f65 7874 7261 6374 2061 6e64  ad_n_extract and
-00002000: 206e 6f74 206c 696e 7578 3a20 7265 7475   not linux: retu
-00002010: 726e 2066 696e 645f 6d6f 7665 5f64 656c  rn find_move_del
-00002020: 6574 655f 7769 6e64 6f77 7328 646f 776e  ete_windows(down
-00002030: 6c6f 6164 6564 2c20 6578 655f 6e61 6d65  loaded, exe_name
-00002040: 206f 7220 746f 6f6c 5f6e 616d 652c 2064   or tool_name, d
-00002050: 656c 6574 6529 0d0a 2020 2020 656c 6966  elete)..    elif
-00002060: 2064 6f77 6e6c 6f61 645f 6e5f 6578 7472   download_n_extr
-00002070: 6163 7420 616e 6420 6c69 6e75 783a 2072  act and linux: r
-00002080: 6574 7572 6e20 6669 6e64 5f6d 6f76 655f  eturn find_move_
-00002090: 6465 6c65 7465 5f6c 696e 7578 2864 6f77  delete_linux(dow
-000020a0: 6e6c 6f61 6465 642c 2065 7865 5f6e 616d  nloaded, exe_nam
-000020b0: 6520 6f72 2074 6f6f 6c5f 6e61 6d65 2c20  e or tool_name, 
-000020c0: 6465 6c65 7465 290d 0a0d 0a20 2020 2023  delete)....    #
-000020d0: 2063 6f6e 736f 6c65 2e72 756c 6528 6622   console.rule(f"
-000020e0: 436f 6d70 6c65 7465 6420 496e 7374 616c  Completed Instal
-000020f0: 6c61 7469 6f6e 2229 0d0a 2020 2020 2320  lation")..    # 
-00002100: 7265 7475 726e 2072 6573 0d0a 0d0a 0d0a  return res......
-00002110: 6465 6620 6765 745f 7368 656c 6c5f 7363  def get_shell_sc
-00002120: 7269 7074 5f65 7865 6375 7469 6e67 5f70  ript_executing_p
-00002130: 7973 6372 6970 7428 7079 7468 6f6e 5f66  yscript(python_f
-00002140: 696c 652c 2066 756e 633d 4e6f 6e65 2c20  ile, func=None, 
-00002150: 7379 7374 656d 3d4e 6f6e 652c 2076 655f  system=None, ve_
-00002160: 6e61 6d65 3d22 7665 2229 3a0d 0a20 2020  name="ve"):..   
-00002170: 2069 6620 6675 6e63 2069 7320 4e6f 6e65   if func is None
-00002180: 3a20 6578 6563 5f6c 696e 6520 3d20 6622  : exec_line = f"
-00002190: 2222 7079 7468 6f6e 207b 7079 7468 6f6e  ""python {python
-000021a0: 5f66 696c 657d 2222 220d 0a20 2020 2065  _file}"""..    e
-000021b0: 6c73 653a 2065 7865 635f 6c69 6e65 203d  lse: exec_line =
-000021c0: 2066 2222 2270 7974 686f 6e20 2d6d 2066   f"""python -m f
-000021d0: 6972 6520 7b70 7974 686f 6e5f 6669 6c65  ire {python_file
-000021e0: 7d20 7b66 756e 637d 2222 220d 0a20 2020  } {func}"""..   
-000021f0: 2072 6574 7572 6e20 6622 2222 0d0a 2e20   return f"""... 
-00002200: 7e2f 7363 7269 7074 732f 6163 7469 7661  ~/scripts/activa
-00002210: 7465 5f76 6520 7b76 655f 6e61 6d65 7d0d  te_ve {ve_name}.
-00002220: 0a7b 6578 6563 5f6c 696e 657d 0d0a 6465  .{exec_line}..de
-00002230: 6163 7469 7661 7465 0d0a 2222 220d 0a0d  activate.."""...
-00002240: 0a0d 0a64 6566 2077 7269 7465 5f73 6865  ...def write_she
-00002250: 6c6c 5f73 6372 6970 7428 7072 6f67 7261  ll_script(progra
-00002260: 6d2c 2064 6573 633d 2222 2c20 7072 6573  m, desc="", pres
-00002270: 6572 7665 5f63 7764 3d54 7275 652c 2064  erve_cwd=True, d
-00002280: 6973 706c 6179 3d54 7275 6529 3a0d 0a20  isplay=True):.. 
-00002290: 2020 2069 6620 7072 6573 6572 7665 5f63     if preserve_c
-000022a0: 7764 3a0d 0a20 2020 2020 2020 2069 6620  wd:..        if 
-000022b0: 706c 6174 666f 726d 2e73 7973 7465 6d28  platform.system(
-000022c0: 2920 3d3d 2022 5769 6e64 6f77 7322 3a0d  ) == "Windows":.
-000022d0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-000022e0: 6772 616d 203d 2022 246f 7269 675f 7061  gram = "$orig_pa
-000022f0: 7468 203d 2024 7077 645c 6e22 202b 2070  th = $pwd\n" + p
-00002300: 726f 6772 616d 202b 2022 5c6e 6364 2024  rogram + "\ncd $
-00002310: 6f72 6967 5f70 6174 6822 0d0a 2020 2020  orig_path"..    
-00002320: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00002330: 2020 2020 2020 2070 726f 6772 616d 203d         program =
-00002340: 2027 6f72 6967 5f70 6174 683d 2428 6364   'orig_path=$(cd
-00002350: 202d 2d20 222e 2220 2626 2070 7764 295c   -- "." && pwd)\
-00002360: 6e27 202b 2070 726f 6772 616d 202b 2027  n' + program + '
-00002370: 5c6e 6364 2022 246f 7269 675f 7061 7468  \ncd "$orig_path
-00002380: 2220 7c7c 2065 7869 7427 0d0a 2020 2020  " || exit'..    
-00002390: 6966 2064 6973 706c 6179 3a0d 0a20 2020  if display:..   
-000023a0: 2020 2020 2070 7269 6e74 2866 2245 7865       print(f"Exe
-000023b0: 6375 7469 6e67 207b 5052 4f47 5241 4d5f  cuting {PROGRAM_
-000023c0: 5041 5448 7d22 290d 0a20 2020 2020 2020  PATH}")..       
-000023d0: 2070 7269 6e74 5f70 726f 6772 616d 6d69   print_programmi
-000023e0: 6e67 5f73 6372 6970 7428 7072 6f67 7261  ng_script(progra
-000023f0: 6d3d 7072 6f67 7261 6d2c 206c 6578 6572  m=program, lexer
-00002400: 3d22 7368 656c 6c22 2c20 6465 7363 3d64  ="shell", desc=d
-00002410: 6573 6329 0d0a 2020 2020 6966 2070 6c61  esc)..    if pla
-00002420: 7466 6f72 6d2e 7379 7374 656d 2829 203d  tform.system() =
-00002430: 3d20 2757 696e 646f 7773 273a 2050 524f  = 'Windows': PRO
-00002440: 4752 414d 5f50 4154 482e 6372 6561 7465  GRAM_PATH.create
-00002450: 2870 6172 656e 7473 5f6f 6e6c 793d 5472  (parents_only=Tr
-00002460: 7565 292e 7772 6974 655f 7465 7874 2870  ue).write_text(p
-00002470: 726f 6772 616d 290d 0a20 2020 2065 6c73  rogram)..    els
-00002480: 653a 2050 524f 4752 414d 5f50 4154 482e  e: PROGRAM_PATH.
-00002490: 6372 6561 7465 2870 6172 656e 7473 5f6f  create(parents_o
-000024a0: 6e6c 793d 5472 7565 292e 7772 6974 655f  nly=True).write_
-000024b0: 7465 7874 2866 227b 7072 6f67 7261 6d7d  text(f"{program}
-000024c0: 2229 0d0a 2020 2020 7265 7475 726e 204e  ")..    return N
-000024d0: 6f6e 650d 0a0d 0a0d 0a64 6566 2070 7269  one......def pri
-000024e0: 6e74 5f70 726f 6772 616d 6d69 6e67 5f73  nt_programming_s
-000024f0: 6372 6970 7428 7072 6f67 7261 6d3a 2073  cript(program: s
-00002500: 7472 2c20 6c65 7865 723a 2073 7472 2c20  tr, lexer: str, 
-00002510: 6465 7363 3d22 2229 3a0d 0a20 2020 2069  desc=""):..    i
-00002520: 6620 6c65 7865 7220 3d3d 2022 7368 656c  f lexer == "shel
-00002530: 6c22 3a0d 0a20 2020 2020 2020 2069 6620  l":..        if 
-00002540: 706c 6174 666f 726d 2e73 7973 7465 6d28  platform.system(
-00002550: 2920 3d3d 2022 5769 6e64 6f77 7322 3a20  ) == "Windows": 
-00002560: 6c65 7865 7220 3d20 2270 6f77 6572 7368  lexer = "powersh
-00002570: 656c 6c22 0d0a 2020 2020 2020 2020 656c  ell"..        el
-00002580: 6966 2070 6c61 7466 6f72 6d2e 7379 7374  if platform.syst
-00002590: 656d 2829 203d 3d20 224c 696e 7578 223a  em() == "Linux":
-000025a0: 206c 6578 6572 203d 2022 7368 220d 0a20   lexer = "sh".. 
-000025b0: 2020 2020 2020 2065 6c73 653a 2072 6169         else: rai
-000025c0: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-000025d0: 6445 7272 6f72 2866 226c 6578 6572 207b  dError(f"lexer {
-000025e0: 6c65 7865 727d 206e 6f74 2069 6d70 6c65  lexer} not imple
-000025f0: 6d65 6e74 6564 2066 6f72 2073 7973 7465  mented for syste
-00002600: 6d20 7b70 6c61 7466 6f72 6d2e 7379 7374  m {platform.syst
-00002610: 656d 2829 7d22 290d 0a20 2020 2063 6f6e  em()}")..    con
-00002620: 736f 6c65 203d 2043 6f6e 736f 6c65 2829  sole = Console()
-00002630: 0d0a 2020 2020 636f 6e73 6f6c 652e 7072  ..    console.pr
-00002640: 696e 7428 5061 6e65 6c28 5379 6e74 6178  int(Panel(Syntax
-00002650: 2870 726f 6772 616d 2c20 6c65 7865 723d  (program, lexer=
-00002660: 6c65 7865 7229 2c20 7469 746c 653d 6465  lexer), title=de
-00002670: 7363 292c 2073 7479 6c65 3d22 626f 6c64  sc), style="bold
-00002680: 2072 6564 2229 0d0a 0d0a 0d0a 6465 6620   red")......def 
-00002690: 6765 745f 6c61 7465 7374 5f76 6572 7369  get_latest_versi
-000026a0: 6f6e 2875 726c 293a 0d0a 2020 2020 2320  on(url):..    # 
-000026b0: 6e6f 7420 7965 7420 7573 6564 2c20 636f  not yet used, co
-000026c0: 6e73 6964 6572 2c20 7573 696e 6720 6974  nsider, using it
-000026d0: 2e0d 0a20 2020 2069 6d70 6f72 7420 7265  ...    import re
-000026e0: 7175 6573 7473 0d0a 2020 2020 696d 706f  quests..    impo
-000026f0: 7274 206a 736f 6e0d 0a20 2020 2075 726c  rt json..    url
-00002700: 203d 2066 2268 7474 7073 3a2f 2f61 7069   = f"https://api
-00002710: 2e67 6974 6875 622e 636f 6d2f 7265 706f  .github.com/repo
-00002720: 732f 7b75 726c 2e73 706c 6974 2827 6769  s/{url.split('gi
-00002730: 7468 7562 2e63 6f6d 2f27 295b 315d 7d2f  thub.com/')[1]}/
-00002740: 7265 6c65 6173 6573 2f6c 6174 6573 7422  releases/latest"
-00002750: 0d0a 2020 2020 2320 5265 706c 6163 6520  ..    # Replace 
-00002760: 7b6f 776e 6572 7d20 616e 6420 7b72 6570  {owner} and {rep
-00002770: 6f7d 2077 6974 6820 7468 6520 6163 7475  o} with the actu
-00002780: 616c 206f 776e 6572 2061 6e64 2072 6570  al owner and rep
-00002790: 6f73 6974 6f72 7920 6e61 6d65 0d0a 2020  ository name..  
-000027a0: 2020 7265 7370 6f6e 7365 203d 2072 6571    response = req
-000027b0: 7565 7374 732e 6765 7428 7572 6c29 0d0a  uests.get(url)..
-000027c0: 2020 2020 6966 2072 6573 706f 6e73 652e      if response.
-000027d0: 7374 6174 7573 5f63 6f64 6520 3d3d 2032  status_code == 2
-000027e0: 3030 3a0d 0a20 2020 2020 2020 2064 6174  00:..        dat
-000027f0: 6120 3d20 6a73 6f6e 2e6c 6f61 6473 2872  a = json.loads(r
-00002800: 6573 706f 6e73 652e 7465 7874 290d 0a20  esponse.text).. 
-00002810: 2020 2020 2020 206c 6174 6573 745f 7665         latest_ve
-00002820: 7273 696f 6e20 3d20 6461 7461 5b22 7461  rsion = data["ta
-00002830: 675f 6e61 6d65 225d 0d0a 2020 2020 2020  g_name"]..      
-00002840: 2020 7072 696e 7428 224c 6174 6573 7420    print("Latest 
-00002850: 7265 6c65 6173 6520 7665 7273 696f 6e3a  release version:
-00002860: 222c 206c 6174 6573 745f 7665 7273 696f  ", latest_versio
-00002870: 6e29 0d0a 2020 2020 656c 7365 3a20 7072  n)..    else: pr
-00002880: 696e 7428 2245 7272 6f72 3a22 2c20 7265  int("Error:", re
-00002890: 7370 6f6e 7365 2e73 7461 7475 735f 636f  sponse.status_co
-000028a0: 6465 290d 0a0d 0a0d 0a64 6566 2063 6865  de)......def che
-000028b0: 636b 5f74 6f6f 6c5f 6578 6973 7473 2874  ck_tool_exists(t
-000028c0: 6f6f 6c5f 6e61 6d65 293a 0d0a 2020 2020  ool_name):..    
-000028d0: 6966 2070 6c61 7466 6f72 6d2e 7379 7374  if platform.syst
-000028e0: 656d 2829 203d 3d20 2257 696e 646f 7773  em() == "Windows
-000028f0: 223a 2074 6f6f 6c5f 6e61 6d65 203d 2074  ": tool_name = t
-00002900: 6f6f 6c5f 6e61 6d65 202b 2022 2e65 7865  ool_name + ".exe
-00002910: 220d 0a20 2020 2069 6620 706c 6174 666f  "..    if platfo
-00002920: 726d 2e73 7973 7465 6d28 2920 3d3d 2022  rm.system() == "
-00002930: 5769 6e64 6f77 7322 3a20 636d 6420 3d20  Windows": cmd = 
-00002940: 2277 6865 7265 2e65 7865 220d 0a20 2020  "where.exe"..   
-00002950: 2065 6c69 6620 706c 6174 666f 726d 2e73   elif platform.s
-00002960: 7973 7465 6d28 2920 3d3d 2022 4c69 6e75  ystem() == "Linu
-00002970: 7822 3a20 636d 6420 3d20 2277 6869 6368  x": cmd = "which
-00002980: 220d 0a20 2020 2065 6c73 653a 2072 6169  "..    else: rai
-00002990: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-000029a0: 6445 7272 6f72 2866 2270 6c61 7466 6f72  dError(f"platfor
-000029b0: 6d20 7b70 6c61 7466 6f72 6d2e 7379 7374  m {platform.syst
-000029c0: 656d 2829 7d20 6e6f 7420 696d 706c 656d  em()} not implem
-000029d0: 656e 7465 6422 290d 0a20 2020 2069 6d70  ented")..    imp
-000029e0: 6f72 7420 7375 6270 726f 6365 7373 0d0a  ort subprocess..
-000029f0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-00002a00: 2020 7375 6270 726f 6365 7373 2e63 6865    subprocess.che
-00002a10: 636b 5f6f 7574 7075 7428 5b63 6d64 2c20  ck_output([cmd, 
-00002a20: 746f 6f6c 5f6e 616d 655d 290d 0a20 2020  tool_name])..   
-00002a30: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00002a40: 0d0a 2020 2020 6578 6365 7074 2028 7375  ..    except (su
-00002a50: 6270 726f 6365 7373 2e43 616c 6c65 6450  bprocess.CalledP
-00002a60: 726f 6365 7373 4572 726f 722c 2046 696c  rocessError, Fil
-00002a70: 654e 6f74 466f 756e 6445 7272 6f72 293a  eNotFoundError):
-00002a80: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00002a90: 2046 616c 7365 0d0a 0d0a 0d0a 6966 205f   False......if _
-00002aa0: 5f6e 616d 655f 5f20 3d3d 2027 5f5f 6d61  _name__ == '__ma
-00002ab0: 696e 5f5f 273a 0d0a 2020 2020 7061 7373  in__':..    pass
-00002ac0: 0d0a                                     ..
+00000320: 6f6e 652c 2066 7a66 3d46 616c 7365 2c20  one, fzf=False, 
+00000330: 6d75 6c74 693d 4661 6c73 6529 202d 3e20  multi=False) -> 
+00000340: 7374 7220 6f72 206c 6973 743a 0d0a 2020  str or list:..  
+00000350: 2020 746f 6f6c 5f6e 616d 6520 3d20 2266    tool_name = "f
+00000360: 7a66 220d 0a20 2020 2069 6620 667a 6620  zf"..    if fzf 
+00000370: 616e 6420 6368 6563 6b5f 746f 6f6c 5f65  and check_tool_e
+00000380: 7869 7374 7328 746f 6f6c 5f6e 616d 6529  xists(tool_name)
+00000390: 3a0d 0a20 2020 2020 2020 2069 6e73 7461  :..        insta
+000003a0: 6c6c 5f6e 5f69 6d70 6f72 7428 2270 7966  ll_n_import("pyf
+000003b0: 7a66 2229 0d0a 2020 2020 2020 2020 6672  zf")..        fr
+000003c0: 6f6d 2070 7966 7a66 2e70 7966 7a66 2069  om pyfzf.pyfzf i
+000003d0: 6d70 6f72 7420 467a 6650 726f 6d70 740d  mport FzfPrompt.
+000003e0: 0a20 2020 2020 2020 2066 7a66 203d 2046  .        fzf = F
+000003f0: 7a66 5072 6f6d 7074 2829 0d0a 2020 2020  zfPrompt()..    
+00000400: 2020 2020 6e6c 203d 2022 5c6e 220d 0a20      nl = "\n".. 
+00000410: 2020 2020 2020 2063 686f 6963 655f 6964         choice_id
+00000420: 7820 3d20 667a 662e 7072 6f6d 7074 286f  x = fzf.prompt(o
+00000430: 7074 696f 6e73 2c20 667a 665f 6f70 7469  ptions, fzf_opti
+00000440: 6f6e 733d 2822 2d2d 6d75 6c74 6922 2069  ons=("--multi" i
+00000450: 6620 6d75 6c74 6920 656c 7365 2022 2229  f multi else "")
+00000460: 202b 2066 2220 2d2d 7072 6f6d 7074 3d7b   + f" --prompt={
+00000470: 7072 6f6d 7074 2e72 6570 6c61 6365 286e  prompt.replace(n
+00000480: 6c2c 2027 2027 297d 202d 2d62 6f72 6465  l, ' ')} --borde
+00000490: 723d 726f 756e 6465 6422 2920 2320 2d2d  r=rounded") # --
+000004a0: 626f 7264 6572 2d6c 6162 656c 3d7b 6d73  border-label={ms
+000004b0: 672e 7265 706c 6163 6528 6e6c 2c20 2720  g.replace(nl, ' 
+000004c0: 2729 7d22 290d 0a20 2020 2065 6c73 653a  ')}")..    else:
+000004d0: 0d0a 2020 2020 2020 2020 636f 6e73 6f6c  ..        consol
+000004e0: 6520 3d20 436f 6e73 6f6c 6528 290d 0a20  e = Console().. 
+000004f0: 2020 2020 2020 2069 6620 6465 6661 756c         if defaul
+00000500: 7420 6973 206e 6f74 204e 6f6e 653a 0d0a  t is not None:..
+00000510: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00000520: 7274 2064 6566 6175 6c74 2069 6e20 6f70  rt default in op
+00000530: 7469 6f6e 732c 2066 2244 6566 6175 6c74  tions, f"Default
+00000540: 2060 7b64 6566 6175 6c74 7d60 206f 7074   `{default}` opt
+00000550: 696f 6e20 6e6f 7420 696e 206f 7074 696f  ion not in optio
+00000560: 6e73 2060 7b6c 6973 7428 6f70 7469 6f6e  ns `{list(option
+00000570: 7329 7d60 220d 0a20 2020 2020 2020 2020  s)}`"..         
+00000580: 2020 2064 6566 6175 6c74 5f6d 7367 203d     default_msg =
+00000590: 2054 6578 7428 6622 203c 3c3c 3c2d 2d2d   Text(f" <<<<---
+000005a0: 2d2d 2d2d 2d20 4445 4641 554c 5422 2c20  ----- DEFAULT", 
+000005b0: 7374 796c 653d 2262 6f6c 6420 7265 6422  style="bold red"
+000005c0: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
+000005d0: 2064 6566 6175 6c74 5f6d 7367 203d 2022   default_msg = "
+000005e0: 220d 0a20 2020 2020 2020 2074 7874 203d  "..        txt =
+000005f0: 2054 6578 7428 225c 6e22 202b 206d 7367   Text("\n" + msg
+00000600: 202b 2022 5c6e 2229 0d0a 2020 2020 2020   + "\n")..      
+00000610: 2020 666f 7220 6964 782c 206b 6579 2069    for idx, key i
+00000620: 6e20 656e 756d 6572 6174 6528 6f70 7469  n enumerate(opti
+00000630: 6f6e 7329 3a0d 0a20 2020 2020 2020 2020  ons):..         
+00000640: 2020 2074 7874 203d 2074 7874 202b 2054     txt = txt + T
+00000650: 6578 7428 6622 7b69 6478 3a32 647d 2022  ext(f"{idx:2d} "
+00000660: 2c20 7374 796c 653d 2262 6f6c 6420 626c  , style="bold bl
+00000670: 7565 2229 202b 2073 7472 286b 6579 2920  ue") + str(key) 
+00000680: 2b20 2864 6566 6175 6c74 5f6d 7367 2069  + (default_msg i
+00000690: 6620 6465 6661 756c 7420 6973 206e 6f74  f default is not
+000006a0: 204e 6f6e 6520 616e 6420 6465 6661 756c   None and defaul
+000006b0: 7420 3d3d 206b 6579 2065 6c73 6520 2222  t == key else ""
+000006c0: 2920 2b20 225c 6e22 0d0a 2020 2020 2020  ) + "\n"..      
+000006d0: 2020 7478 7420 3d20 5061 6e65 6c28 7478    txt = Panel(tx
+000006e0: 742c 2074 6974 6c65 3d68 6561 6465 722c  t, title=header,
+000006f0: 2073 7562 7469 746c 653d 7461 696c 2c20   subtitle=tail, 
+00000700: 626f 7264 6572 5f73 7479 6c65 3d22 626f  border_style="bo
+00000710: 6c64 2072 6564 2229 0d0a 2020 2020 2020  ld red")..      
+00000720: 2020 636f 6e73 6f6c 652e 7072 696e 7428    console.print(
+00000730: 7478 7429 0d0a 2020 2020 2020 2020 6368  txt)..        ch
+00000740: 6f69 6365 5f69 6478 203d 2069 6e70 7574  oice_idx = input
+00000750: 2866 227b 7072 6f6d 7074 7d5c 6e45 6e74  (f"{prompt}\nEnt
+00000760: 6572 206f 7074 696f 6e20 2a6e 756d 6265  er option *numbe
+00000770: 722a 2028 6f72 206f 7074 696f 6e20 6e61  r* (or option na
+00000780: 6d65 2073 7461 7274 696e 6720 7769 7468  me starting with
+00000790: 2073 7061 6365 293a 2022 290d 0a0d 0a20   space): ").... 
+000007a0: 2020 2069 6620 6e6f 7420 667a 663a 0d0a     if not fzf:..
+000007b0: 2020 2020 2020 2020 6966 2063 686f 6963          if choic
+000007c0: 655f 6964 782e 7374 6172 7473 7769 7468  e_idx.startswith
+000007d0: 2822 2022 293a 0d0a 2020 2020 2020 2020  (" "):..        
+000007e0: 2020 2020 6368 6f69 6365 5f6b 6579 203d      choice_key =
+000007f0: 2063 686f 6963 655f 6964 782e 7374 7269   choice_idx.stri
+00000800: 7028 290d 0a20 2020 2020 2020 2020 2020  p()..           
+00000810: 2061 7373 6572 7420 6368 6f69 6365 5f6b   assert choice_k
+00000820: 6579 2069 6e20 6f70 7469 6f6e 732c 2066  ey in options, f
+00000830: 2243 686f 6963 6520 607b 6368 6f69 6365  "Choice `{choice
+00000840: 5f6b 6579 7d60 206e 6f74 2069 6e20 6f70  _key}` not in op
+00000850: 7469 6f6e 7320 607b 6f70 7469 6f6e 737d  tions `{options}
+00000860: 6022 0d0a 2020 2020 2020 2020 2020 2020  `"..            
+00000870: 6368 6f69 6365 5f69 6478 203d 206f 7074  choice_idx = opt
+00000880: 696f 6e73 2e69 6e64 6578 2863 686f 6963  ions.index(choic
+00000890: 655f 6b65 7929 0d0a 2020 2020 2020 2020  e_key)..        
+000008a0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000008b0: 2020 2069 6620 6368 6f69 6365 5f69 6478     if choice_idx
+000008c0: 203d 3d20 2222 3a0d 0a20 2020 2020 2020   == "":..       
+000008d0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+000008e0: 6465 6661 756c 7420 6973 206e 6f74 204e  default is not N
+000008f0: 6f6e 652c 2066 2244 6566 6175 6c74 206f  one, f"Default o
+00000900: 7074 696f 6e20 6e6f 7420 6176 6169 6c61  ption not availa
+00000910: 626c 6521 220d 0a20 2020 2020 2020 2020  ble!"..         
+00000920: 2020 2020 2020 2063 686f 6963 655f 6964         choice_id
+00000930: 7820 3d20 6f70 7469 6f6e 732e 696e 6465  x = options.inde
+00000940: 7828 6465 6661 756c 7429 0d0a 2020 2020  x(default)..    
+00000950: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00000960: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00000970: 793a 2063 686f 6963 655f 6964 7820 3d20  y: choice_idx = 
+00000980: 696e 7428 6368 6f69 6365 5f69 6478 290d  int(choice_idx).
+00000990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000009a0: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
+000009b0: 6f72 3a20 2023 2070 6172 7369 6e67 2065  or:  # parsing e
+000009c0: 7272 6f72 0d0a 2020 2020 2020 2020 2020  rror..          
+000009d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000009e0: 496e 6465 7845 7272 6f72 0d0a 2020 2020  IndexError..    
+000009f0: 2020 2020 2020 2020 2020 2020 6368 6f69              choi
+00000a00: 6365 5f6b 6579 203d 206f 7074 696f 6e73  ce_key = options
+00000a10: 5b63 686f 6963 655f 6964 785d 0d0a 2020  [choice_idx]..  
+00000a20: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00000a30: 2049 6e64 6578 4572 726f 723a 0d0a 2020   IndexError:..  
+00000a40: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00000a50: 6d61 6e79 2062 6520 7573 6572 2066 6f72  many be user for
+00000a60: 676f 7474 656e 2074 6f20 7374 6172 7420  gotten to start 
+00000a70: 7769 7468 2061 2064 6173 680d 0a20 2020  with a dash..   
+00000a80: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00000a90: 6368 6f69 6365 5f69 6478 2069 6e20 6f70  choice_idx in op
+00000aa0: 7469 6f6e 733a 0d0a 2020 2020 2020 2020  tions:..        
+00000ab0: 2020 2020 2020 2020 2020 2020 6368 6f69              choi
+00000ac0: 6365 5f6b 6579 203d 2063 686f 6963 655f  ce_key = choice_
+00000ad0: 6964 780d 0a20 2020 2020 2020 2020 2020  idx..           
+00000ae0: 2020 2020 2020 2020 2063 686f 6963 655f           choice_
+00000af0: 6964 7820 3d20 6f70 7469 6f6e 732e 696e  idx = options.in
+00000b00: 6465 7828 6368 6f69 6365 5f69 6478 290d  dex(choice_idx).
+00000b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000b20: 2065 6c73 653a 2072 6169 7365 2056 616c   else: raise Val
+00000b30: 7565 4572 726f 7228 6622 556e 6b6e 6f77  ueError(f"Unknow
+00000b40: 6e20 6368 6f69 6365 2e20 7b63 686f 6963  n choice. {choic
+00000b50: 655f 6964 787d 2229 0d0a 2020 2020 2020  e_idx}")..      
+00000b60: 2020 2020 2020 6578 6365 7074 2054 7970        except Typ
+00000b70: 6545 7272 6f72 3a0d 0a20 2020 2020 2020  eError:..       
+00000b80: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+00000b90: 7970 6545 7272 6f72 2866 2255 6e6b 6e6f  ypeError(f"Unkno
+00000ba0: 776e 2063 686f 6963 652e 207b 6368 6f69  wn choice. {choi
+00000bb0: 6365 5f69 6478 7d22 290d 0a20 2020 2020  ce_idx}")..     
+00000bc0: 2020 2020 2020 2020 2020 2023 2070 6173             # pas
+00000bd0: 730d 0a20 2020 2020 2020 2070 7269 6e74  s..        print
+00000be0: 2866 227b 6368 6f69 6365 5f69 6478 7d3a  (f"{choice_idx}:
+00000bf0: 207b 6368 6f69 6365 5f6b 6579 7d22 2c20   {choice_key}", 
+00000c00: 6622 3c3c 3c3c 2d2d 2d2d 2d2d 2d2d 2043  f"<<<<-------- C
+00000c10: 484f 4943 4520 4d41 4445 2229 0d0a 2020  HOICE MADE")..  
+00000c20: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00000c30: 2069 6620 6e6f 7420 6d75 6c74 6920 616e   if not multi an
+00000c40: 6420 7479 7065 2863 686f 6963 655f 6964  d type(choice_id
+00000c50: 7829 2069 7320 6c69 7374 2061 6e64 206c  x) is list and l
+00000c60: 656e 2863 686f 6963 655f 6964 7829 203d  en(choice_idx) =
+00000c70: 3d20 313a 2063 686f 6963 655f 6964 7820  = 1: choice_idx 
+00000c80: 3d20 6368 6f69 6365 5f69 6478 5b30 5d0d  = choice_idx[0].
+00000c90: 0a20 2020 2020 2020 2063 686f 6963 655f  .        choice_
+00000ca0: 6b65 7920 3d20 6368 6f69 6365 5f69 6478  key = choice_idx
+00000cb0: 0d0a 2020 2020 7265 7475 726e 2063 686f  ..    return cho
+00000cc0: 6963 655f 6b65 790d 0a0d 0a0d 0a64 6566  ice_key......def
+00000cd0: 2073 796d 6c69 6e6b 2874 6869 733a 2050   symlink(this: P
+00000ce0: 2c20 746f 5f74 6869 733a 2050 2c20 7072  , to_this: P, pr
+00000cf0: 696f 7269 7469 7a65 5f74 6f5f 7468 6973  ioritize_to_this
+00000d00: 3d54 7275 6529 3a0d 0a20 2020 2022 2222  =True):..    """
+00000d10: 6865 6c70 6572 2066 756e 6374 696f 6e2e  helper function.
+00000d20: 2063 7265 6174 6573 2061 2073 796d 6c69   creates a symli
+00000d30: 6e6b 2066 726f 6d20 6074 6869 7360 2074  nk from `this` t
+00000d40: 6f20 6074 6f5f 7468 6973 602e 0d0a 2020  o `to_this`...  
+00000d50: 2020 5768 6174 2063 616e 2067 6f20 7772    What can go wr
+00000d60: 6f6e 673f 0d0a 2020 2020 6465 7065 6e64  ong?..    depend
+00000d70: 696e 6720 6f6e 2074 6869 7320 616e 6420  ing on this and 
+00000d80: 746f 5f74 6869 7320 6578 6973 7465 6e63  to_this existenc
+00000d90: 652c 206f 6e65 2077 696c 6c20 6265 2070  e, one will be p
+00000da0: 7269 6f72 6574 697a 6564 2064 6570 656e  rioretized depen
+00000db0: 6469 6e67 206f 6e20 6f76 6572 7772 6974  ding on overwrit
+00000dc0: 6520 7661 6c75 652e 0d0a 2020 2020 5472  e value...    Tr
+00000dd0: 7565 206d 6561 6e73 2074 6869 7320 7769  ue means this wi
+00000de0: 6c6c 2070 6f74 656e 7469 616c 6c79 2062  ll potentially b
+00000df0: 6520 6f76 6572 7772 6974 7465 6e20 2864  e overwritten (d
+00000e00: 6570 656e 6469 6e67 206f 6e20 7768 6574  epending on whet
+00000e10: 6865 7220 746f 5f74 6869 7320 6578 6973  her to_this exis
+00000e20: 7473 206f 7220 6e6f 7429 0d0a 2020 2020  ts or not)..    
+00000e30: 4661 6c73 6520 6d65 616e 7320 746f 5f74  False means to_t
+00000e40: 6869 7320 7769 6c6c 2070 6f74 656e 7469  his will potenti
+00000e50: 616c 6c79 2062 6520 6f76 6572 7769 7474  ally be overwitt
+00000e60: 7465 6e2e 2222 220d 0a20 2020 2074 6869  ten."""..    thi
+00000e70: 7320 3d20 5028 7468 6973 292e 6578 7061  s = P(this).expa
+00000e80: 6e64 7573 6572 2829 2e61 6273 6f6c 7574  nduser().absolut
+00000e90: 6528 290d 0a20 2020 2074 6f5f 7468 6973  e()..    to_this
+00000ea0: 203d 2050 2874 6f5f 7468 6973 292e 6578   = P(to_this).ex
+00000eb0: 7061 6e64 7573 6572 2829 2e61 6273 6f6c  panduser().absol
+00000ec0: 7574 6528 290d 0a20 2020 2069 6620 7468  ute()..    if th
+00000ed0: 6973 2e69 735f 7379 6d6c 696e 6b28 293a  is.is_symlink():
+00000ee0: 2074 6869 732e 6465 6c65 7465 2873 7572   this.delete(sur
+00000ef0: 653d 5472 7565 2920 2023 2064 656c 6574  e=True)  # delet
+00000f00: 6520 6966 2069 7420 6578 6973 7473 2061  e if it exists a
+00000f10: 7320 7379 6d62 6c69 6320 6c69 6e6b 2c20  s symblic link, 
+00000f20: 6e6f 7420 6120 636f 6e63 7265 7465 2070  not a concrete p
+00000f30: 6174 682e 0d0a 2020 2020 6966 2074 6869  ath...    if thi
+00000f40: 732e 6578 6973 7473 2829 3a20 2023 2074  s.exists():  # t
+00000f50: 6869 7320 6973 2061 2070 726f 626c 656d  his is a problem
+00000f60: 2e20 4974 2077 696c 6c20 6265 2072 6573  . It will be res
+00000f70: 6f6c 7665 6420 7669 6120 606f 7665 7277  olved via `overw
+00000f80: 7269 7465 600d 0a20 2020 2020 2020 2069  rite`..        i
+00000f90: 6620 7072 696f 7269 7469 7a65 5f74 6f5f  f prioritize_to_
+00000fa0: 7468 6973 2069 7320 5472 7565 3a20 2023  this is True:  #
+00000fb0: 2069 7420 2a63 616e 2a20 6265 2064 656c   it *can* be del
+00000fc0: 6574 6564 2c20 6275 7420 6c65 7427 7320  eted, but let's 
+00000fd0: 6c6f 6f6b 2061 7420 7461 7267 6574 2066  look at target f
+00000fe0: 6972 7374 2e0d 0a20 2020 2020 2020 2020  irst...         
+00000ff0: 2020 2069 6620 746f 5f74 6869 732e 6578     if to_this.ex
+00001000: 6973 7473 2829 3a20 2023 2074 6869 7320  ists():  # this 
+00001010: 6578 6973 7473 2c20 746f 5f74 6869 7320  exists, to_this 
+00001020: 6173 2077 656c 6c2e 2074 6f5f 7468 6973  as well. to_this
+00001030: 2069 7320 7072 696f 7269 7469 7a65 642e   is prioritized.
+00001040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001050: 2020 7468 6973 2e61 7070 656e 6428 6622    this.append(f"
+00001060: 2e6f 7269 675f 7b72 616e 6473 7472 2829  .orig_{randstr()
+00001070: 7d22 2c20 696e 706c 6163 653d 5472 7565  }", inplace=True
+00001080: 2920 2023 2072 656e 616d 6520 6973 2062  )  # rename is b
+00001090: 6574 7465 7220 7468 616e 2064 656c 6574  etter than delet
+000010a0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+000010b0: 2065 6c73 653a 2074 6869 732e 6d6f 7665   else: this.move
+000010c0: 2870 6174 683d 746f 5f74 6869 7329 2020  (path=to_this)  
+000010d0: 2320 7468 6973 2065 7869 7374 732c 2074  # this exists, t
+000010e0: 6f5f 7468 6973 2064 6f65 736e 2774 2e20  o_this doesn't. 
+000010f0: 746f 5f74 6869 7320 6973 2070 7269 6f72  to_this is prior
+00001100: 6974 697a 6564 2e0d 0a20 2020 2020 2020  itized...       
+00001110: 2065 6c69 6620 7072 696f 7269 7469 7a65   elif prioritize
+00001120: 5f74 6f5f 7468 6973 2069 7320 4661 6c73  _to_this is Fals
+00001130: 653a 2020 2320 646f 6e27 7420 7361 6372  e:  # don't sacr
+00001140: 6566 6963 6520 7468 6973 2c20 7361 6372  efice this, sacr
+00001150: 6566 6963 6520 746f 5f74 6869 732e 0d0a  efice to_this...
+00001160: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00001170: 6f5f 7468 6973 2e65 7869 7374 7328 293a  o_this.exists():
+00001180: 2074 6869 732e 6d6f 7665 2870 6174 683d   this.move(path=
+00001190: 746f 5f74 6869 732c 206f 7665 7277 7269  to_this, overwri
+000011a0: 7465 3d54 7275 6529 2020 2320 7468 6973  te=True)  # this
+000011b0: 2065 7869 7374 732c 2074 6f5f 7468 6973   exists, to_this
+000011c0: 2061 7320 7765 6c6c 2c20 7468 6973 2069   as well, this i
+000011d0: 7320 7072 696f 7269 7469 7a65 642e 2020  s prioritized.  
+000011e0: 2023 206e 6f77 2077 6520 6172 6520 7265   # now we are re
+000011f0: 6164 6c79 2074 6f20 6d61 6b65 2074 6865  adly to make the
+00001200: 206c 696e 6b0d 0a20 2020 2020 2020 2020   link..         
+00001210: 2020 2065 6c73 653a 2074 6869 732e 6d6f     else: this.mo
+00001220: 7665 2870 6174 683d 746f 5f74 6869 7329  ve(path=to_this)
+00001230: 2020 2320 7468 6973 2065 7869 7374 732c    # this exists,
+00001240: 2074 6f5f 7468 6973 2064 6f65 736e 2774   to_this doesn't
+00001250: 2c20 7468 6973 2069 7320 7072 696f 7269  , this is priori
+00001260: 7469 7a65 642e 0d0a 2020 2020 656c 7365  tized...    else
+00001270: 3a20 2023 2074 6869 7320 646f 6573 6e27  :  # this doesn'
+00001280: 7420 6578 6973 742e 0d0a 2020 2020 2020  t exist...      
+00001290: 2020 6966 206e 6f74 2074 6f5f 7468 6973    if not to_this
+000012a0: 2e65 7869 7374 7328 293a 2074 6f5f 7468  .exists(): to_th
+000012b0: 6973 2e74 6f75 6368 2829 2020 2320 7765  is.touch()  # we
+000012c0: 2068 6176 6520 746f 2074 6f75 6368 2069   have to touch i
+000012d0: 7420 2866 696c 6529 206f 7220 6372 6561  t (file) or crea
+000012e0: 7465 2069 7420 2866 6f6c 6465 7229 0d0a  te it (folder)..
+000012f0: 2020 2020 6966 2070 6c61 7466 6f72 6d2e      if platform.
+00001300: 7379 7374 656d 2829 203d 3d20 2257 696e  system() == "Win
+00001310: 646f 7773 223a 205f 203d 2069 6e73 7461  dows": _ = insta
+00001320: 6c6c 5f6e 5f69 6d70 6f72 7428 2277 696e  ll_n_import("win
+00001330: 3332 6170 6922 2c20 2270 7977 696e 3332  32api", "pywin32
+00001340: 2229 2020 2320 7468 6973 2069 7320 6372  ")  # this is cr
+00001350: 7563 6961 6c20 666f 7220 7769 6e64 6f77  ucial for window
+00001360: 7320 746f 2070 6f70 2075 7020 7468 6520  s to pop up the 
+00001370: 636f 6e63 656e 7420 7769 6e64 6f77 2069  concent window i
+00001380: 6e20 6361 7365 2070 7974 686f 6e20 7761  n case python wa
+00001390: 7320 6e6f 7420 7275 6e20 6173 2061 646d  s not run as adm
+000013a0: 696e 2e0d 0a20 2020 2074 7279 3a0d 0a20  in...    try:.. 
+000013b0: 2020 2020 2020 2050 2874 6869 7329 2e73         P(this).s
+000013c0: 796d 6c69 6e6b 5f74 6f28 746f 5f74 6869  ymlink_to(to_thi
+000013d0: 732c 2076 6572 626f 7365 3d54 7275 652c  s, verbose=True,
+000013e0: 206f 7665 7277 7269 7465 3d54 7275 6529   overwrite=True)
+000013f0: 0d0a 2020 2020 6578 6365 7074 2045 7863  ..    except Exc
+00001400: 6570 7469 6f6e 2061 7320 6578 3a20 7072  eption as ex: pr
+00001410: 696e 7428 6622 4661 696c 6564 2061 7420  int(f"Failed at 
+00001420: 6c69 6e6b 696e 6720 7b74 6869 737d 203d  linking {this} =
+00001430: 3d3e 207b 746f 5f74 6869 737d 2e5c 6e52  => {to_this}.\nR
+00001440: 6561 736f 6e3a 207b 6578 7d22 290d 0a0d  eason: {ex}")...
+00001450: 0a0d 0a64 6566 2066 696e 645f 6d6f 7665  ...def find_move
+00001460: 5f64 656c 6574 655f 7769 6e64 6f77 7328  _delete_windows(
+00001470: 646f 776e 6c6f 6164 6564 2c20 746f 6f6c  downloaded, tool
+00001480: 5f6e 616d 653d 4e6f 6e65 2c20 6465 6c65  _name=None, dele
+00001490: 7465 3d54 7275 6529 3a0d 0a20 2020 2069  te=True):..    i
+000014a0: 6620 746f 6f6c 5f6e 616d 6520 6973 206e  f tool_name is n
+000014b0: 6f74 204e 6f6e 6520 616e 6420 222e 6578  ot None and ".ex
+000014c0: 6522 2069 6e20 746f 6f6c 5f6e 616d 653a  e" in tool_name:
+000014d0: 2074 6f6f 6c5f 6e61 6d65 203d 2074 6f6f   tool_name = too
+000014e0: 6c5f 6e61 6d65 2e72 6570 6c61 6365 2822  l_name.replace("
+000014f0: 2e65 7865 222c 2022 2229 0d0a 2020 2020  .exe", "")..    
+00001500: 6966 2064 6f77 6e6c 6f61 6465 642e 6973  if downloaded.is
+00001510: 5f66 696c 6528 293a 0d0a 2020 2020 2020  _file():..      
+00001520: 2020 6578 6520 3d20 646f 776e 6c6f 6164    exe = download
+00001530: 6564 0d0a 2020 2020 656c 7365 3a0d 0a20  ed..    else:.. 
+00001540: 2020 2020 2020 2069 6620 746f 6f6c 5f6e         if tool_n
+00001550: 616d 6520 6973 204e 6f6e 653a 2065 7865  ame is None: exe
+00001560: 203d 2064 6f77 6e6c 6f61 6465 642e 7365   = downloaded.se
+00001570: 6172 6368 2822 2a2e 6578 6522 2c20 723d  arch("*.exe", r=
+00001580: 5472 7565 295b 305d 0d0a 2020 2020 2020  True)[0]..      
+00001590: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+000015a0: 2020 2020 2074 6d70 203d 2064 6f77 6e6c       tmp = downl
+000015b0: 6f61 6465 642e 7365 6172 6368 2866 227b  oaded.search(f"{
+000015c0: 746f 6f6c 5f6e 616d 657d 2e65 7865 222c  tool_name}.exe",
+000015d0: 2072 3d54 7275 6529 0d0a 2020 2020 2020   r=True)..      
+000015e0: 2020 2020 2020 6966 206c 656e 2874 6d70        if len(tmp
+000015f0: 2920 3d3d 2031 3a20 6578 6520 3d20 746d  ) == 1: exe = tm
+00001600: 705b 305d 0d0a 2020 2020 2020 2020 2020  p[0]..          
+00001610: 2020 656c 7365 3a20 6578 6520 3d20 646f    else: exe = do
+00001620: 776e 6c6f 6164 6564 2e73 6561 7263 6828  wnloaded.search(
+00001630: 222a 2e65 7865 222c 2072 3d54 7275 6529  "*.exe", r=True)
+00001640: 5b30 5d0d 0a20 2020 2065 7865 2e6d 6f76  [0]..    exe.mov
+00001650: 6528 666f 6c64 6572 3d50 2e67 6574 5f65  e(folder=P.get_e
+00001660: 6e76 2829 2e57 696e 646f 7773 4170 7073  nv().WindowsApps
+00001670: 2c20 6f76 6572 7772 6974 653d 5472 7565  , overwrite=True
+00001680: 2920 2023 206c 6174 6573 7420 7665 7273  )  # latest vers
+00001690: 696f 6e20 6f76 6572 7772 6974 6573 206f  ion overwrites o
+000016a0: 6c64 6572 2069 6e73 7461 6c6c 6174 696f  lder installatio
+000016b0: 6e2e 0d0a 2020 2020 6966 2064 656c 6574  n...    if delet
+000016c0: 653a 2064 6f77 6e6c 6f61 6465 642e 6465  e: downloaded.de
+000016d0: 6c65 7465 2873 7572 653d 5472 7565 290d  lete(sure=True).
+000016e0: 0a20 2020 2072 6574 7572 6e20 6578 650d  .    return exe.
+000016f0: 0a0d 0a0d 0a64 6566 2066 696e 645f 6d6f  .....def find_mo
+00001700: 7665 5f64 656c 6574 655f 6c69 6e75 7828  ve_delete_linux(
+00001710: 646f 776e 6c6f 6164 6564 2c20 746f 6f6c  downloaded, tool
+00001720: 5f6e 616d 652c 2064 656c 6574 653d 5472  _name, delete=Tr
+00001730: 7565 293a 0d0a 2020 2020 6966 2064 6f77  ue):..    if dow
+00001740: 6e6c 6f61 6465 642e 6973 5f66 696c 6528  nloaded.is_file(
+00001750: 293a 0d0a 2020 2020 2020 2020 6578 6520  ):..        exe 
+00001760: 3d20 646f 776e 6c6f 6164 6564 0d0a 2020  = downloaded..  
+00001770: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00001780: 2072 6573 203d 2064 6f77 6e6c 6f61 6465   res = downloade
+00001790: 642e 7365 6172 6368 2866 222a 7b74 6f6f  d.search(f"*{too
+000017a0: 6c5f 6e61 6d65 7d2a 222c 2066 6f6c 6465  l_name}*", folde
+000017b0: 7273 3d46 616c 7365 2c20 723d 5472 7565  rs=False, r=True
+000017c0: 290d 0a20 2020 2020 2020 2069 6620 6c65  )..        if le
+000017d0: 6e28 7265 7329 203d 3d20 313a 2065 7865  n(res) == 1: exe
+000017e0: 203d 2072 6573 5b30 5d0d 0a20 2020 2020   = res[0]..     
+000017f0: 2020 2065 6c73 653a 2065 7865 203d 2064     else: exe = d
+00001800: 6f77 6e6c 6f61 6465 642e 7365 6172 6368  ownloaded.search
+00001810: 2874 6f6f 6c5f 6e61 6d65 2c20 666f 6c64  (tool_name, fold
+00001820: 6572 733d 4661 6c73 652c 2072 3d54 7275  ers=False, r=Tru
+00001830: 6529 5b30 5d0d 0a20 2020 2070 7269 6e74  e)[0]..    print
+00001840: 2866 224d 4f56 494e 4720 6669 6c65 2060  (f"MOVING file `
+00001850: 7b72 6570 7228 6578 6529 7d60 2074 6f20  {repr(exe)}` to 
+00001860: 272f 7573 722f 6c6f 6361 6c2f 6269 6e27  '/usr/local/bin'
+00001870: 2229 0d0a 2020 2020 6578 652e 6368 6d6f  ")..    exe.chmo
+00001880: 6428 306f 3737 3729 0d0a 2020 2020 2320  d(0o777)..    # 
+00001890: 6578 652e 6d6f 7665 2866 6f6c 6465 723d  exe.move(folder=
+000018a0: 7222 2f75 7372 2f6c 6f63 616c 2f62 696e  r"/usr/local/bin
+000018b0: 222c 206f 7665 7277 7269 7465 3d46 616c  ", overwrite=Fal
+000018c0: 7365 290d 0a20 2020 2054 6572 6d69 6e61  se)..    Termina
+000018d0: 6c28 292e 7275 6e28 6622 7375 646f 206d  l().run(f"sudo m
+000018e0: 7620 7b65 7865 7d20 2f75 7372 2f6c 6f63  v {exe} /usr/loc
+000018f0: 616c 2f62 696e 2f22 292e 7072 696e 745f  al/bin/").print_
+00001900: 6966 5f75 6e73 7563 6365 7373 6675 6c28  if_unsuccessful(
+00001910: 6465 7363 3d22 4d4f 5649 4e47 2065 7865  desc="MOVING exe
+00001920: 6375 7461 626c 6520 746f 202f 7573 722f  cutable to /usr/
+00001930: 6c6f 6361 6c2f 6269 6e22 2c20 7374 7269  local/bin", stri
+00001940: 6374 5f65 7272 3d54 7275 652c 2073 7472  ct_err=True, str
+00001950: 6963 745f 7265 7475 726e 636f 6465 3d54  ict_returncode=T
+00001960: 7275 6529 0d0a 2020 2020 6966 2064 656c  rue)..    if del
+00001970: 6574 653a 2064 6f77 6e6c 6f61 6465 642e  ete: downloaded.
+00001980: 6465 6c65 7465 2873 7572 653d 5472 7565  delete(sure=True
+00001990: 290d 0a20 2020 2072 6574 7572 6e20 4e6f  )..    return No
+000019a0: 6e65 0d0a 0d0a 0d0a 6465 6620 6765 745f  ne......def get_
+000019b0: 6c61 7465 7374 5f72 656c 6561 7365 2872  latest_release(r
+000019c0: 6570 6f5f 7572 6c2c 2064 6f77 6e6c 6f61  epo_url, downloa
+000019d0: 645f 6e5f 6578 7472 6163 743d 4661 6c73  d_n_extract=Fals
+000019e0: 652c 2073 7566 6669 783d 2278 3836 5f36  e, suffix="x86_6
+000019f0: 342d 7063 2d77 696e 646f 7773 2d6d 7376  4-pc-windows-msv
+00001a00: 6322 2c20 6669 6c65 5f6e 616d 653d 4e6f  c", file_name=No
+00001a10: 6e65 2c20 746f 6f6c 5f6e 616d 653d 4e6f  ne, tool_name=No
+00001a20: 6e65 2c20 6578 655f 6e61 6d65 3d4e 6f6e  ne, exe_name=Non
+00001a30: 652c 2064 656c 6574 653d 5472 7565 2c20  e, delete=True, 
+00001a40: 7374 7269 705f 763d 4661 6c73 652c 206c  strip_v=False, l
+00001a50: 696e 7578 3d46 616c 7365 2c20 636f 6d70  inux=False, comp
+00001a60: 7265 7373 696f 6e3d 4e6f 6e65 2c20 7365  ression=None, se
+00001a70: 703d 222d 222c 2076 6572 7369 6f6e 3d4e  p="-", version=N
+00001a80: 6f6e 6529 3a0d 0a20 2020 2063 6f6e 736f  one):..    conso
+00001a90: 6c65 203d 2043 6f6e 736f 6c65 2829 0d0a  le = Console()..
+00001aa0: 2020 2020 7072 696e 7428 225c 6e5c 6e5c      print("\n\n\
+00001ab0: 6e22 290d 0a20 2020 2070 7269 6e74 2866  n")..    print(f
+00001ac0: 2249 6e73 7065 6374 696e 6720 6c61 7465  "Inspecting late
+00001ad0: 7374 2072 656c 6561 7365 2040 207b 7265  st release @ {re
+00001ae0: 706f 5f75 726c 7d20 2020 2e2e 2e22 290d  po_url}   ...").
+00001af0: 0a20 2020 2023 2077 6974 6820 636f 6e73  .    # with cons
+00001b00: 6f6c 652e 7374 6174 7573 2822 496e 7374  ole.status("Inst
+00001b10: 616c 6c69 6e67 2e2e 2e22 293a 2020 2320  alling..."):  # 
+00001b20: 6d61 6b65 7320 7472 6f75 626c 6573 206f  makes troubles o
+00001b30: 6e20 6c69 6e75 7820 7768 656e 2070 726f  n linux when pro
+00001b40: 6d70 7420 6173 6b73 2066 6f72 2070 6173  mpt asks for pas
+00001b50: 7377 6f72 6420 746f 206d 6f76 6520 6669  sword to move fi
+00001b60: 6c65 2074 6f20 2f75 7372 2f62 696e 0d0a  le to /usr/bin..
+00001b70: 0d0a 2020 2020 6966 2076 6572 7369 6f6e  ..    if version
+00001b80: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00001b90: 2020 2069 6d70 6f72 7420 7265 7175 6573     import reques
+00001ba0: 7473 2020 2320 6874 7470 733a 2f2f 646f  ts  # https://do
+00001bb0: 6373 2e67 6974 6875 622e 636f 6d2f 656e  cs.github.com/en
+00001bc0: 2f72 6570 6f73 6974 6f72 6965 732f 7265  /repositories/re
+00001bd0: 6c65 6173 696e 672d 7072 6f6a 6563 7473  leasing-projects
+00001be0: 2d6f 6e2d 6769 7468 7562 2f6c 696e 6b69  -on-github/linki
+00001bf0: 6e67 2d74 6f2d 7265 6c65 6173 6573 0d0a  ng-to-releases..
+00001c00: 2020 2020 2020 2020 6c61 7465 7374 5f76          latest_v
+00001c10: 6572 7369 6f6e 203d 2072 6571 7565 7374  ersion = request
+00001c20: 732e 6765 7428 7374 7228 7265 706f 5f75  s.get(str(repo_u
+00001c30: 726c 2920 2b20 222f 7265 6c65 6173 6573  rl) + "/releases
+00001c40: 2f6c 6174 6573 7422 292e 7572 6c2e 7370  /latest").url.sp
+00001c50: 6c69 7428 222f 2229 5b2d 315d 2020 2320  lit("/")[-1]  # 
+00001c60: 7468 6973 2069 7320 746f 2072 6573 6f6c  this is to resol
+00001c70: 7665 2074 6865 2072 6564 6972 6563 7469  ve the redirecti
+00001c80: 6f6e 2074 6861 7420 6f63 6375 7265 733a  on that occures:
+00001c90: 2068 7474 7073 3a2f 2f73 7461 636b 6f76   https://stackov
+00001ca0: 6572 666c 6f77 2e63 6f6d 2f71 7565 7374  erflow.com/quest
+00001cb0: 696f 6e73 2f33 3630 3730 3832 312f 686f  ions/36070821/ho
+00001cc0: 772d 746f 2d67 6574 2d72 6564 6972 6563  w-to-get-redirec
+00001cd0: 742d 7572 6c2d 7573 696e 672d 7079 7468  t-url-using-pyth
+00001ce0: 6f6e 2d72 6571 7565 7374 730d 0a20 2020  on-requests..   
+00001cf0: 2065 6c73 653a 206c 6174 6573 745f 7665   else: latest_ve
+00001d00: 7273 696f 6e20 3d20 7665 7273 696f 6e0d  rsion = version.
+00001d10: 0a0d 0a20 2020 2064 6f77 6e6c 6f61 645f  ...    download_
+00001d20: 6c69 6e6b 203d 2050 2872 6570 6f5f 7572  link = P(repo_ur
+00001d30: 6c20 2b20 222f 7265 6c65 6173 6573 2f64  l + "/releases/d
+00001d40: 6f77 6e6c 6f61 642f 2220 2b20 6c61 7465  ownload/" + late
+00001d50: 7374 5f76 6572 7369 6f6e 290d 0a20 2020  st_version)..   
+00001d60: 2063 6f6d 7072 6573 7369 6f6e 203d 2063   compression = c
+00001d70: 6f6d 7072 6573 7369 6f6e 206f 7220 2822  ompression or ("
+00001d80: 7a69 7022 2069 6620 6e6f 7420 6c69 6e75  zip" if not linu
+00001d90: 7820 656c 7365 2022 7461 722e 677a 2229  x else "tar.gz")
+00001da0: 0d0a 2020 2020 7665 7273 696f 6e20 3d20  ..    version = 
+00001db0: 646f 776e 6c6f 6164 5f6c 696e 6b5b 2d31  download_link[-1
+00001dc0: 5d0d 0a20 2020 2076 6572 7369 6f6e 203d  ]..    version =
+00001dd0: 2073 7472 2876 6572 7369 6f6e 292e 7265   str(version).re
+00001de0: 706c 6163 6528 2276 222c 2022 2229 2069  place("v", "") i
+00001df0: 6620 7374 7269 705f 7620 656c 7365 2073  f strip_v else s
+00001e00: 7472 2876 6572 7369 6f6e 290d 0a20 2020  tr(version)..   
+00001e10: 2074 6f6f 6c5f 6e61 6d65 203d 2074 6f6f   tool_name = too
+00001e20: 6c5f 6e61 6d65 206f 7220 5028 7265 706f  l_name or P(repo
+00001e30: 5f75 726c 295b 2d31 5d0d 0a20 2020 2050  _url)[-1]..    P
+00001e40: 2e68 6f6d 6528 292e 6a6f 696e 7061 7468  .home().joinpath
+00001e50: 2866 2274 6d70 5f72 6573 756c 7473 2f63  (f"tmp_results/c
+00001e60: 6c69 5f74 6f6f 6c73 5f69 6e73 7461 6c6c  li_tools_install
+00001e70: 6572 732f 7665 7273 696f 6e73 2f7b 746f  ers/versions/{to
+00001e80: 6f6c 5f6e 616d 657d 2229 2e63 7265 6174  ol_name}").creat
+00001e90: 6528 7061 7265 6e74 735f 6f6e 6c79 3d54  e(parents_only=T
+00001ea0: 7275 6529 2e77 7269 7465 5f74 6578 7428  rue).write_text(
+00001eb0: 7665 7273 696f 6e29 0d0a 0d0a 2020 2020  version)....    
+00001ec0: 6966 206e 6f74 2064 6f77 6e6c 6f61 645f  if not download_
+00001ed0: 6e5f 6578 7472 6163 743a 2072 6574 7572  n_extract: retur
+00001ee0: 6e20 646f 776e 6c6f 6164 5f6c 696e 6b0d  n download_link.
+00001ef0: 0a20 2020 2063 6f6e 736f 6c65 2e72 756c  .    console.rul
+00001f00: 6528 6622 496e 7374 616c 6c69 6e67 207b  e(f"Installing {
+00001f10: 746f 6f6c 5f6e 616d 657d 2076 6572 7369  tool_name} versi
+00001f20: 6f6e 207b 7665 7273 696f 6e7d 2229 0d0a  on {version}")..
+00001f30: 2020 2020 6966 2066 696c 655f 6e61 6d65      if file_name
+00001f40: 2069 7320 4e6f 6e65 3a20 2023 2069 7420   is None:  # it 
+00001f50: 6973 206e 6f74 2063 6f6e 7374 616e 742c  is not constant,
+00001f60: 2073 6f20 7765 2063 6f6d 7069 6c65 2069   so we compile i
+00001f70: 7420 6672 6f6d 2070 6172 7473 2061 7320  t from parts as 
+00001f80: 666f 6c6c 6f77 733a 0d0a 2020 2020 2020  follows:..      
+00001f90: 2020 6669 6c65 5f6e 616d 6520 3d20 6627    file_name = f'
+00001fa0: 7b74 6f6f 6c5f 6e61 6d65 7d7b 7365 707d  {tool_name}{sep}
+00001fb0: 7b76 6572 7369 6f6e 7d7b 7365 707d 7b73  {version}{sep}{s
+00001fc0: 7566 6669 787d 2e7b 636f 6d70 7265 7373  uffix}.{compress
+00001fd0: 696f 6e7d 270d 0a20 2020 2064 6f77 6e6c  ion}'..    downl
+00001fe0: 6f61 645f 6c69 6e6b 203d 2064 6f77 6e6c  oad_link = downl
+00001ff0: 6f61 645f 6c69 6e6b 2e6a 6f69 6e70 6174  oad_link.joinpat
+00002000: 6828 6669 6c65 5f6e 616d 6529 0d0a 2020  h(file_name)..  
+00002010: 2020 7072 696e 7428 2244 6f77 6e6c 6f61    print("Downloa
+00002020: 6469 6e67 222c 2064 6f77 6e6c 6f61 645f  ding", download_
+00002030: 6c69 6e6b 2e61 735f 7572 6c5f 7374 7228  link.as_url_str(
+00002040: 2929 0d0a 2020 2020 646f 776e 6c6f 6164  ))..    download
+00002050: 6564 203d 2064 6f77 6e6c 6f61 645f 6c69  ed = download_li
+00002060: 6e6b 2e64 6f77 6e6c 6f61 6428 666f 6c64  nk.download(fold
+00002070: 6572 3d74 6d70 5f69 6e73 7461 6c6c 5f64  er=tmp_install_d
+00002080: 6972 290d 0a0d 0a20 2020 2069 6620 2274  ir)....    if "t
+00002090: 6172 2e67 7a22 2069 6e20 646f 776e 6c6f  ar.gz" in downlo
+000020a0: 6164 5f6c 696e 6b3a 2064 6f77 6e6c 6f61  ad_link: downloa
+000020b0: 6465 6420 3d20 646f 776e 6c6f 6164 6564  ded = downloaded
+000020c0: 2e75 6e67 7a5f 756e 7461 7228 696e 706c  .ungz_untar(inpl
+000020d0: 6163 653d 5472 7565 290d 0a20 2020 2065  ace=True)..    e
+000020e0: 6c69 6620 227a 6970 2220 696e 2064 6f77  lif "zip" in dow
+000020f0: 6e6c 6f61 645f 6c69 6e6b 3a20 646f 776e  nload_link: down
+00002100: 6c6f 6164 6564 203d 2064 6f77 6e6c 6f61  loaded = downloa
+00002110: 6465 642e 756e 7a69 7028 696e 706c 6163  ded.unzip(inplac
+00002120: 653d 5472 7565 2c20 6f76 6572 7772 6974  e=True, overwrit
+00002130: 653d 5472 7565 290d 0a20 2020 2065 6c69  e=True)..    eli
+00002140: 6620 2274 6172 2e78 7a22 2069 6e20 646f  f "tar.xz" in do
+00002150: 776e 6c6f 6164 5f6c 696e 6b3a 2064 6f77  wnload_link: dow
+00002160: 6e6c 6f61 6465 6420 3d20 646f 776e 6c6f  nloaded = downlo
+00002170: 6164 6564 2e75 6e78 7a5f 756e 7461 7228  aded.unxz_untar(
+00002180: 696e 706c 6163 653d 5472 7565 290d 0a20  inplace=True).. 
+00002190: 2020 2065 6c73 653a 2070 6173 7320 2023     else: pass  #
+000021a0: 206e 6f20 636f 6d70 7265 7373 696f 6e2e   no compression.
+000021b0: 0d0a 0d0a 2020 2020 6966 2064 6f77 6e6c  ....    if downl
+000021c0: 6f61 645f 6e5f 6578 7472 6163 7420 616e  oad_n_extract an
+000021d0: 6420 6e6f 7420 6c69 6e75 783a 2072 6574  d not linux: ret
+000021e0: 7572 6e20 6669 6e64 5f6d 6f76 655f 6465  urn find_move_de
+000021f0: 6c65 7465 5f77 696e 646f 7773 2864 6f77  lete_windows(dow
+00002200: 6e6c 6f61 6465 642c 2065 7865 5f6e 616d  nloaded, exe_nam
+00002210: 6520 6f72 2074 6f6f 6c5f 6e61 6d65 2c20  e or tool_name, 
+00002220: 6465 6c65 7465 290d 0a20 2020 2065 6c69  delete)..    eli
+00002230: 6620 646f 776e 6c6f 6164 5f6e 5f65 7874  f download_n_ext
+00002240: 7261 6374 2061 6e64 206c 696e 7578 3a20  ract and linux: 
+00002250: 7265 7475 726e 2066 696e 645f 6d6f 7665  return find_move
+00002260: 5f64 656c 6574 655f 6c69 6e75 7828 646f  _delete_linux(do
+00002270: 776e 6c6f 6164 6564 2c20 6578 655f 6e61  wnloaded, exe_na
+00002280: 6d65 206f 7220 746f 6f6c 5f6e 616d 652c  me or tool_name,
+00002290: 2064 656c 6574 6529 0d0a 0d0a 2020 2020   delete)....    
+000022a0: 2320 636f 6e73 6f6c 652e 7275 6c65 2866  # console.rule(f
+000022b0: 2243 6f6d 706c 6574 6564 2049 6e73 7461  "Completed Insta
+000022c0: 6c6c 6174 696f 6e22 290d 0a20 2020 2023  llation")..    #
+000022d0: 2072 6574 7572 6e20 7265 730d 0a0d 0a0d   return res.....
+000022e0: 0a64 6566 2067 6574 5f73 6865 6c6c 5f73  .def get_shell_s
+000022f0: 6372 6970 745f 6578 6563 7574 696e 675f  cript_executing_
+00002300: 7079 7363 7269 7074 2870 7974 686f 6e5f  pyscript(python_
+00002310: 6669 6c65 2c20 6675 6e63 3d4e 6f6e 652c  file, func=None,
+00002320: 2073 7973 7465 6d3d 4e6f 6e65 2c20 7665   system=None, ve
+00002330: 5f6e 616d 653d 2276 6522 293a 0d0a 2020  _name="ve"):..  
+00002340: 2020 6966 2066 756e 6320 6973 204e 6f6e    if func is Non
+00002350: 653a 2065 7865 635f 6c69 6e65 203d 2066  e: exec_line = f
+00002360: 2222 2270 7974 686f 6e20 7b70 7974 686f  """python {pytho
+00002370: 6e5f 6669 6c65 7d22 2222 0d0a 2020 2020  n_file}"""..    
+00002380: 656c 7365 3a20 6578 6563 5f6c 696e 6520  else: exec_line 
+00002390: 3d20 6622 2222 7079 7468 6f6e 202d 6d20  = f"""python -m 
+000023a0: 6669 7265 207b 7079 7468 6f6e 5f66 696c  fire {python_fil
+000023b0: 657d 207b 6675 6e63 7d22 2222 0d0a 2020  e} {func}"""..  
+000023c0: 2020 7265 7475 726e 2066 2222 220d 0a2e    return f"""...
+000023d0: 207e 2f73 6372 6970 7473 2f61 6374 6976   ~/scripts/activ
+000023e0: 6174 655f 7665 207b 7665 5f6e 616d 657d  ate_ve {ve_name}
+000023f0: 0d0a 7b65 7865 635f 6c69 6e65 7d0d 0a64  ..{exec_line}..d
+00002400: 6561 6374 6976 6174 650d 0a22 2222 0d0a  eactivate.."""..
+00002410: 0d0a 0d0a 6465 6620 7772 6974 655f 7368  ....def write_sh
+00002420: 656c 6c5f 7363 7269 7074 2870 726f 6772  ell_script(progr
+00002430: 616d 2c20 6465 7363 3d22 222c 2070 7265  am, desc="", pre
+00002440: 7365 7276 655f 6377 643d 5472 7565 2c20  serve_cwd=True, 
+00002450: 6469 7370 6c61 793d 5472 7565 2c20 6578  display=True, ex
+00002460: 6563 7574 653d 4661 6c73 6529 3a0d 0a20  ecute=False):.. 
+00002470: 2020 2069 6620 7072 6573 6572 7665 5f63     if preserve_c
+00002480: 7764 3a0d 0a20 2020 2020 2020 2069 6620  wd:..        if 
+00002490: 706c 6174 666f 726d 2e73 7973 7465 6d28  platform.system(
+000024a0: 2920 3d3d 2022 5769 6e64 6f77 7322 3a0d  ) == "Windows":.
+000024b0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+000024c0: 6772 616d 203d 2022 246f 7269 675f 7061  gram = "$orig_pa
+000024d0: 7468 203d 2024 7077 645c 6e22 202b 2070  th = $pwd\n" + p
+000024e0: 726f 6772 616d 202b 2022 5c6e 6364 2024  rogram + "\ncd $
+000024f0: 6f72 6967 5f70 6174 6822 0d0a 2020 2020  orig_path"..    
+00002500: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00002510: 2020 2020 2020 2070 726f 6772 616d 203d         program =
+00002520: 2027 6f72 6967 5f70 6174 683d 2428 6364   'orig_path=$(cd
+00002530: 202d 2d20 222e 2220 2626 2070 7764 295c   -- "." && pwd)\
+00002540: 6e27 202b 2070 726f 6772 616d 202b 2027  n' + program + '
+00002550: 5c6e 6364 2022 246f 7269 675f 7061 7468  \ncd "$orig_path
+00002560: 2220 7c7c 2065 7869 7427 0d0a 2020 2020  " || exit'..    
+00002570: 6966 2064 6973 706c 6179 3a0d 0a20 2020  if display:..   
+00002580: 2020 2020 2070 7269 6e74 2866 2245 7865       print(f"Exe
+00002590: 6375 7469 6e67 207b 5052 4f47 5241 4d5f  cuting {PROGRAM_
+000025a0: 5041 5448 7d22 290d 0a20 2020 2020 2020  PATH}")..       
+000025b0: 2070 7269 6e74 5f70 726f 6772 616d 6d69   print_programmi
+000025c0: 6e67 5f73 6372 6970 7428 7072 6f67 7261  ng_script(progra
+000025d0: 6d3d 7072 6f67 7261 6d2c 206c 6578 6572  m=program, lexer
+000025e0: 3d22 7368 656c 6c22 2c20 6465 7363 3d64  ="shell", desc=d
+000025f0: 6573 6329 0d0a 2020 2020 6966 2070 6c61  esc)..    if pla
+00002600: 7466 6f72 6d2e 7379 7374 656d 2829 203d  tform.system() =
+00002610: 3d20 2757 696e 646f 7773 273a 2050 524f  = 'Windows': PRO
+00002620: 4752 414d 5f50 4154 482e 6372 6561 7465  GRAM_PATH.create
+00002630: 2870 6172 656e 7473 5f6f 6e6c 793d 5472  (parents_only=Tr
+00002640: 7565 292e 7772 6974 655f 7465 7874 2870  ue).write_text(p
+00002650: 726f 6772 616d 290d 0a20 2020 2065 6c73  rogram)..    els
+00002660: 653a 2050 524f 4752 414d 5f50 4154 482e  e: PROGRAM_PATH.
+00002670: 6372 6561 7465 2870 6172 656e 7473 5f6f  create(parents_o
+00002680: 6e6c 793d 5472 7565 292e 7772 6974 655f  nly=True).write_
+00002690: 7465 7874 2866 227b 7072 6f67 7261 6d7d  text(f"{program}
+000026a0: 2229 0d0a 0d0a 2020 2020 6966 2065 7865  ")....    if exe
+000026b0: 6375 7465 3a20 5465 726d 696e 616c 2829  cute: Terminal()
+000026c0: 2e72 756e 2866 222e 207b 5052 4f47 5241  .run(f". {PROGRA
+000026d0: 4d5f 5041 5448 7d22 2c20 7368 656c 6c3d  M_PATH}", shell=
+000026e0: 2270 6f77 6572 7368 656c 6c22 292e 7072  "powershell").pr
+000026f0: 696e 745f 6966 5f75 6e73 7563 6365 7373  int_if_unsuccess
+00002700: 6675 6c28 6465 7363 3d22 4578 6563 7574  ful(desc="Execut
+00002710: 696e 6720 7368 656c 6c20 7363 7269 7074  ing shell script
+00002720: 222c 2073 7472 6963 745f 6572 723d 5472  ", strict_err=Tr
+00002730: 7565 2c20 7374 7269 6374 5f72 6574 7572  ue, strict_retur
+00002740: 6e63 6f64 653d 5472 7565 290d 0a20 2020  ncode=True)..   
+00002750: 2072 6574 7572 6e20 4e6f 6e65 0d0a 0d0a   return None....
+00002760: 0d0a 6465 6620 7072 696e 745f 7072 6f67  ..def print_prog
+00002770: 7261 6d6d 696e 675f 7363 7269 7074 2870  ramming_script(p
+00002780: 726f 6772 616d 3a20 7374 722c 206c 6578  rogram: str, lex
+00002790: 6572 3a20 7374 722c 2064 6573 633d 2222  er: str, desc=""
+000027a0: 293a 0d0a 2020 2020 6966 206c 6578 6572  ):..    if lexer
+000027b0: 203d 3d20 2273 6865 6c6c 223a 0d0a 2020   == "shell":..  
+000027c0: 2020 2020 2020 6966 2070 6c61 7466 6f72        if platfor
+000027d0: 6d2e 7379 7374 656d 2829 203d 3d20 2257  m.system() == "W
+000027e0: 696e 646f 7773 223a 206c 6578 6572 203d  indows": lexer =
+000027f0: 2022 706f 7765 7273 6865 6c6c 220d 0a20   "powershell".. 
+00002800: 2020 2020 2020 2065 6c69 6620 706c 6174         elif plat
+00002810: 666f 726d 2e73 7973 7465 6d28 2920 3d3d  form.system() ==
+00002820: 2022 4c69 6e75 7822 3a20 6c65 7865 7220   "Linux": lexer 
+00002830: 3d20 2273 6822 0d0a 2020 2020 2020 2020  = "sh"..        
+00002840: 656c 7365 3a20 7261 6973 6520 4e6f 7449  else: raise NotI
+00002850: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
+00002860: 6622 6c65 7865 7220 7b6c 6578 6572 7d20  f"lexer {lexer} 
+00002870: 6e6f 7420 696d 706c 656d 656e 7465 6420  not implemented 
+00002880: 666f 7220 7379 7374 656d 207b 706c 6174  for system {plat
+00002890: 666f 726d 2e73 7973 7465 6d28 297d 2229  form.system()}")
+000028a0: 0d0a 2020 2020 636f 6e73 6f6c 6520 3d20  ..    console = 
+000028b0: 436f 6e73 6f6c 6528 290d 0a20 2020 2063  Console()..    c
+000028c0: 6f6e 736f 6c65 2e70 7269 6e74 2850 616e  onsole.print(Pan
+000028d0: 656c 2853 796e 7461 7828 7072 6f67 7261  el(Syntax(progra
+000028e0: 6d2c 206c 6578 6572 3d6c 6578 6572 292c  m, lexer=lexer),
+000028f0: 2074 6974 6c65 3d64 6573 6329 2c20 7374   title=desc), st
+00002900: 796c 653d 2262 6f6c 6420 7265 6422 290d  yle="bold red").
+00002910: 0a0d 0a0d 0a64 6566 2067 6574 5f6c 6174  .....def get_lat
+00002920: 6573 745f 7665 7273 696f 6e28 7572 6c29  est_version(url)
+00002930: 3a0d 0a20 2020 2023 206e 6f74 2079 6574  :..    # not yet
+00002940: 2075 7365 642c 2063 6f6e 7369 6465 722c   used, consider,
+00002950: 2075 7369 6e67 2069 742e 0d0a 2020 2020   using it...    
+00002960: 696d 706f 7274 2072 6571 7565 7374 730d  import requests.
+00002970: 0a20 2020 2069 6d70 6f72 7420 6a73 6f6e  .    import json
+00002980: 0d0a 2020 2020 7572 6c20 3d20 6622 6874  ..    url = f"ht
+00002990: 7470 733a 2f2f 6170 692e 6769 7468 7562  tps://api.github
+000029a0: 2e63 6f6d 2f72 6570 6f73 2f7b 7572 6c2e  .com/repos/{url.
+000029b0: 7370 6c69 7428 2767 6974 6875 622e 636f  split('github.co
+000029c0: 6d2f 2729 5b31 5d7d 2f72 656c 6561 7365  m/')[1]}/release
+000029d0: 732f 6c61 7465 7374 220d 0a20 2020 2023  s/latest"..    #
+000029e0: 2052 6570 6c61 6365 207b 6f77 6e65 727d   Replace {owner}
+000029f0: 2061 6e64 207b 7265 706f 7d20 7769 7468   and {repo} with
+00002a00: 2074 6865 2061 6374 7561 6c20 6f77 6e65   the actual owne
+00002a10: 7220 616e 6420 7265 706f 7369 746f 7279  r and repository
+00002a20: 206e 616d 650d 0a20 2020 2072 6573 706f   name..    respo
+00002a30: 6e73 6520 3d20 7265 7175 6573 7473 2e67  nse = requests.g
+00002a40: 6574 2875 726c 290d 0a20 2020 2069 6620  et(url)..    if 
+00002a50: 7265 7370 6f6e 7365 2e73 7461 7475 735f  response.status_
+00002a60: 636f 6465 203d 3d20 3230 303a 0d0a 2020  code == 200:..  
+00002a70: 2020 2020 2020 6461 7461 203d 206a 736f        data = jso
+00002a80: 6e2e 6c6f 6164 7328 7265 7370 6f6e 7365  n.loads(response
+00002a90: 2e74 6578 7429 0d0a 2020 2020 2020 2020  .text)..        
+00002aa0: 6c61 7465 7374 5f76 6572 7369 6f6e 203d  latest_version =
+00002ab0: 2064 6174 615b 2274 6167 5f6e 616d 6522   data["tag_name"
+00002ac0: 5d0d 0a20 2020 2020 2020 2070 7269 6e74  ]..        print
+00002ad0: 2822 4c61 7465 7374 2072 656c 6561 7365  ("Latest release
+00002ae0: 2076 6572 7369 6f6e 3a22 2c20 6c61 7465   version:", late
+00002af0: 7374 5f76 6572 7369 6f6e 290d 0a20 2020  st_version)..   
+00002b00: 2065 6c73 653a 2070 7269 6e74 2822 4572   else: print("Er
+00002b10: 726f 723a 222c 2072 6573 706f 6e73 652e  ror:", response.
+00002b20: 7374 6174 7573 5f63 6f64 6529 0d0a 0d0a  status_code)....
+00002b30: 0d0a 6465 6620 6368 6563 6b5f 746f 6f6c  ..def check_tool
+00002b40: 5f65 7869 7374 7328 746f 6f6c 5f6e 616d  _exists(tool_nam
+00002b50: 6529 3a0d 0a20 2020 2069 6620 706c 6174  e):..    if plat
+00002b60: 666f 726d 2e73 7973 7465 6d28 2920 3d3d  form.system() ==
+00002b70: 2022 5769 6e64 6f77 7322 3a20 746f 6f6c   "Windows": tool
+00002b80: 5f6e 616d 6520 3d20 746f 6f6c 5f6e 616d  _name = tool_nam
+00002b90: 6520 2b20 222e 6578 6522 0d0a 2020 2020  e + ".exe"..    
+00002ba0: 6966 2070 6c61 7466 6f72 6d2e 7379 7374  if platform.syst
+00002bb0: 656d 2829 203d 3d20 2257 696e 646f 7773  em() == "Windows
+00002bc0: 223a 2063 6d64 203d 2022 7768 6572 652e  ": cmd = "where.
+00002bd0: 6578 6522 0d0a 2020 2020 656c 6966 2070  exe"..    elif p
+00002be0: 6c61 7466 6f72 6d2e 7379 7374 656d 2829  latform.system()
+00002bf0: 203d 3d20 224c 696e 7578 223a 2063 6d64   == "Linux": cmd
+00002c00: 203d 2022 7768 6963 6822 0d0a 2020 2020   = "which"..    
+00002c10: 656c 7365 3a20 7261 6973 6520 4e6f 7449  else: raise NotI
+00002c20: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
+00002c30: 6622 706c 6174 666f 726d 207b 706c 6174  f"platform {plat
+00002c40: 666f 726d 2e73 7973 7465 6d28 297d 206e  form.system()} n
+00002c50: 6f74 2069 6d70 6c65 6d65 6e74 6564 2229  ot implemented")
+00002c60: 0d0a 2020 2020 696d 706f 7274 2073 7562  ..    import sub
+00002c70: 7072 6f63 6573 730d 0a20 2020 2074 7279  process..    try
+00002c80: 3a0d 0a20 2020 2020 2020 2073 7562 7072  :..        subpr
+00002c90: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
+00002ca0: 7574 285b 636d 642c 2074 6f6f 6c5f 6e61  ut([cmd, tool_na
+00002cb0: 6d65 5d29 0d0a 2020 2020 2020 2020 7265  me])..        re
+00002cc0: 7475 726e 2054 7275 650d 0a20 2020 2065  turn True..    e
+00002cd0: 7863 6570 7420 2873 7562 7072 6f63 6573  xcept (subproces
+00002ce0: 732e 4361 6c6c 6564 5072 6f63 6573 7345  s.CalledProcessE
+00002cf0: 7272 6f72 2c20 4669 6c65 4e6f 7446 6f75  rror, FileNotFou
+00002d00: 6e64 4572 726f 7229 3a0d 0a20 2020 2020  ndError):..     
+00002d10: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
+00002d20: 0a0d 0a0d 0a64 6566 2067 6574 5f63 7572  .....def get_cur
+00002d30: 7265 6e74 5f76 6528 293a 0d0a 2020 2020  rent_ve():..    
+00002d40: 696d 706f 7274 2073 7973 0d0a 2020 2020  import sys..    
+00002d50: 7061 7468 203d 2050 2873 7973 2e65 7865  path = P(sys.exe
+00002d60: 6375 7461 626c 6529 2020 2320 736f 6d65  cutable)  # some
+00002d70: 7468 696e 6720 6c69 6b65 207e 5c5c 7665  thing like ~\\ve
+00002d80: 6e76 735c 5c76 655c 5c53 6372 6970 7473  nvs\\ve\\Scripts
+00002d90: 5c5c 7079 7468 6f6e 2e65 7865 270d 0a20  \\python.exe'.. 
+00002da0: 2020 2069 6620 502e 686f 6d65 2829 2e6a     if P.home().j
+00002db0: 6f69 6e70 6174 6828 2276 6522 2920 696e  oinpath("ve") in
+00002dc0: 2070 6174 683a 0d0a 2020 2020 2020 2020   path:..        
+00002dd0: 7265 7475 726e 2070 6174 682e 7061 7265  return path.pare
+00002de0: 6e74 2e70 6172 656e 742e 7374 656d 0d0a  nt.parent.stem..
+00002df0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00002e00: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
+00002e10: 656d 656e 7465 6445 7272 6f72 2822 4e6f  ementedError("No
+00002e20: 7420 6120 6b69 6e64 206f 6620 7669 7274  t a kind of virt
+00002e30: 7561 6c20 656e 7669 726f 6d65 6e74 2074  ual enviroment t
+00002e40: 6861 7420 4920 6578 7065 6374 6564 2e22  hat I expected."
+00002e50: 290d 0a20 2020 2020 2020 2023 2072 6574  )..        # ret
+00002e60: 7572 6e20 7061 7468 2e70 6172 656e 742e  urn path.parent.
+00002e70: 7061 7265 6e74 2e73 7465 6d0d 0a0d 0a0d  parent.stem.....
+00002e80: 0a64 6566 2063 686f 6f73 655f 7373 685f  .def choose_ssh_
+00002e90: 686f 7374 286d 756c 7469 3d54 7275 6529  host(multi=True)
+00002ea0: 3a0d 0a20 2020 2066 726f 6d20 7061 7261  :..    from para
+00002eb0: 6d69 6b6f 2069 6d70 6f72 7420 5353 4843  miko import SSHC
+00002ec0: 6f6e 6669 670d 0a20 2020 2063 203d 2053  onfig..    c = S
+00002ed0: 5348 436f 6e66 6967 2829 0d0a 2020 2020  SHConfig()..    
+00002ee0: 632e 7061 7273 6528 6f70 656e 2850 2e68  c.parse(open(P.h
+00002ef0: 6f6d 6528 292e 6a6f 696e 7061 7468 2822  ome().joinpath("
+00002f00: 2e73 7368 2f63 6f6e 6669 6722 292e 7374  .ssh/config").st
+00002f10: 7229 290d 0a20 2020 2063 686f 6963 6573  r))..    choices
+00002f20: 203d 206c 6973 7428 632e 6765 745f 686f   = list(c.get_ho
+00002f30: 7374 6e61 6d65 7328 2929 0d0a 2020 2020  stnames())..    
+00002f40: 686f 7374 7320 3d20 6469 7370 6c61 795f  hosts = display_
+00002f50: 6f70 7469 6f6e 7328 6d73 673d 2222 2c20  options(msg="", 
+00002f60: 6f70 7469 6f6e 733d 6368 6f69 6365 732c  options=choices,
+00002f70: 206d 756c 7469 3d6d 756c 7469 2c20 667a   multi=multi, fz
+00002f80: 663d 5472 7565 290d 0a20 2020 2072 6574  f=True)..    ret
+00002f90: 7572 6e20 686f 7374 730d 0a0d 0a0d 0a69  urn hosts......i
+00002fa0: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 275f  f __name__ == '_
+00002fb0: 5f6d 6169 6e5f 5f27 3a0d 0a20 2020 2023  _main__':..    #
+00002fc0: 2069 6d70 6f72 7420 7479 7065 720d 0a20   import typer.. 
+00002fd0: 2020 2023 2074 7970 6572 2e72 756e 2863     # typer.run(c
+00002fe0: 6865 636b 5f74 6f6f 6c5f 6578 6973 7473  heck_tool_exists
+00002ff0: 290d 0a20 2020 2070 6173 730d 0a         )..    pass..
```

### Comparing `machineconfig-1.4/src/machineconfig.egg-info/PKG-INFO` & `machineconfig-1.5/src/machineconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineconfig
-Version: 1.4
+Version: 1.5
 Summary: Dotfiles management package
 Home-page: https://github.com/thisismygitrepo/machineconfig
 Author: Alex Al-Saffar
 Author-email: programmer@usa.com
 Project-URL: Bug Tracker, https://github.com/thisismygitrepo/machineconfig/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `machineconfig-1.4/src/machineconfig.egg-info/SOURCES.txt` & `machineconfig-1.5/src/machineconfig.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,26 +16,29 @@
 src/machineconfig/jobs/linux/archive/install_nu.sh
 src/machineconfig/jobs/linux/archive/install_zellij.sh
 src/machineconfig/jobs/linux/archive/lf.sh
 src/machineconfig/jobs/linux/archive/quirks.sh
 src/machineconfig/jobs/python/__init__.py
 src/machineconfig/jobs/python/check_installations.py
 src/machineconfig/jobs/python/create_bootable_media.py
+src/machineconfig/jobs/python/create_zellij_template.py
 src/machineconfig/jobs/python/python_cargo_build_share.py
 src/machineconfig/jobs/python/python_linux_installers_all.py
 src/machineconfig/jobs/python/python_ve_installer.py
 src/machineconfig/jobs/python/python_ve_symlink.py
 src/machineconfig/jobs/python/python_windows_installers_all.py
 src/machineconfig/jobs/python/__pycache__/__init__.cpython-39.pyc
 src/machineconfig/jobs/python/__pycache__/python_linux_installers_all.cpython-39.pyc
 src/machineconfig/jobs/python/__pycache__/python_ve_symlink.cpython-39.pyc
 src/machineconfig/jobs/python/__pycache__/python_windows_installers_all.cpython-39.pyc
 src/machineconfig/jobs/python/archive/python_tools.txt
 src/machineconfig/jobs/python_generic_installers/__init__.py
 src/machineconfig/jobs/python_generic_installers/broot.py
+src/machineconfig/jobs/python_generic_installers/browsh.py
+src/machineconfig/jobs/python_generic_installers/chatgpt.py
 src/machineconfig/jobs/python_generic_installers/cpufetch.py
 src/machineconfig/jobs/python_generic_installers/delta.py
 src/machineconfig/jobs/python_generic_installers/diskonaut.py
 src/machineconfig/jobs/python_generic_installers/dua.py
 src/machineconfig/jobs/python_generic_installers/gitui.py
 src/machineconfig/jobs/python_generic_installers/gopass.py
 src/machineconfig/jobs/python_generic_installers/helix.py
@@ -44,25 +47,27 @@
 src/machineconfig/jobs/python_generic_installers/navi.py
 src/machineconfig/jobs/python_generic_installers/ots.py
 src/machineconfig/jobs/python_generic_installers/ouch.py
 src/machineconfig/jobs/python_generic_installers/pomodoro.py
 src/machineconfig/jobs/python_generic_installers/procs.py
 src/machineconfig/jobs/python_generic_installers/rclone.py
 src/machineconfig/jobs/python_generic_installers/tere.py
+src/machineconfig/jobs/python_generic_installers/vtm.py
 src/machineconfig/jobs/python_generic_installers/watchexec.py
 src/machineconfig/jobs/python_generic_installers/__pycache__/__init__.cpython-39.pyc
 src/machineconfig/jobs/python_generic_installers/archive/__init__.py
 src/machineconfig/jobs/python_generic_installers/archive/nvim.py
 src/machineconfig/jobs/python_generic_installers/archive/strongbox.py
-src/machineconfig/jobs/python_generic_installers/archive/vtm.py
 src/machineconfig/jobs/python_generic_installers/dev/__init__.py
+src/machineconfig/jobs/python_generic_installers/dev/autogpt.py
 src/machineconfig/jobs/python_generic_installers/dev/bw.py
 src/machineconfig/jobs/python_generic_installers/dev/evcxr.py
 src/machineconfig/jobs/python_generic_installers/dev/kondo.py
 src/machineconfig/jobs/python_generic_installers/dev/lvim.py
+src/machineconfig/jobs/python_generic_installers/dev/ngrok.py
 src/machineconfig/jobs/python_generic_installers/dev/opencommit.py
 src/machineconfig/jobs/python_generic_installers/dev/qrcp.py
 src/machineconfig/jobs/python_generic_installers/dev/qrscan.py
 src/machineconfig/jobs/python_generic_installers/dev/rust-analyzer.py
 src/machineconfig/jobs/python_generic_installers/dev/termscp.py
 src/machineconfig/jobs/python_generic_installers/dev/tldr.py
 src/machineconfig/jobs/python_generic_installers/dev/tokei.py
@@ -128,76 +133,75 @@
 src/machineconfig/scripts/linux/cloud_mount
 src/machineconfig/scripts/linux/cloud_repo_sync
 src/machineconfig/scripts/linux/cloud_rx
 src/machineconfig/scripts/linux/cloud_sx
 src/machineconfig/scripts/linux/cloud_sync
 src/machineconfig/scripts/linux/croshell
 src/machineconfig/scripts/linux/devops
-src/machineconfig/scripts/linux/fresh_lvim_installation
+src/machineconfig/scripts/linux/fire
 src/machineconfig/scripts/linux/ftprx
 src/machineconfig/scripts/linux/ftpsx
 src/machineconfig/scripts/linux/fzf2g
 src/machineconfig/scripts/linux/fzfag
 src/machineconfig/scripts/linux/fzffg
 src/machineconfig/scripts/linux/fzfg
+src/machineconfig/scripts/linux/launch_multiple_machines
 src/machineconfig/scripts/linux/mount_drive
 src/machineconfig/scripts/linux/mount_nfs
 src/machineconfig/scripts/linux/mount_nw_drive
 src/machineconfig/scripts/linux/repos
 src/machineconfig/scripts/linux/sk_rg
 src/machineconfig/scripts/linux/tmate_conn
 src/machineconfig/scripts/linux/tmate_start
 src/machineconfig/scripts/linux/transfer.sh
 src/machineconfig/scripts/linux/transfer_wsl_win
 src/machineconfig/scripts/linux/z_ls
-src/machineconfig/scripts/linux/archive/dotfiles_pull
-src/machineconfig/scripts/linux/archive/dotfiles_push
-src/machineconfig/scripts/linux/archive/secure_pull
-src/machineconfig/scripts/linux/archive/secure_push
 src/machineconfig/scripts/python/__init__.py
+src/machineconfig/scripts/python/chatgpt.py
 src/machineconfig/scripts/python/choose_ohmybash_theme.py
 src/machineconfig/scripts/python/choose_ohmyposh_theme.py
 src/machineconfig/scripts/python/cloud_mount.py
 src/machineconfig/scripts/python/cloud_repo_sync.py
 src/machineconfig/scripts/python/cloud_rx.py
 src/machineconfig/scripts/python/cloud_sx.py
 src/machineconfig/scripts/python/cloud_sync.py
 src/machineconfig/scripts/python/devops.py
 src/machineconfig/scripts/python/devops_add_identity.py
 src/machineconfig/scripts/python/devops_add_ssh_key.py
 src/machineconfig/scripts/python/devops_backup_retrieve.py
 src/machineconfig/scripts/python/devops_devapps_install.py
 src/machineconfig/scripts/python/devops_update_repos.py
 src/machineconfig/scripts/python/dotfile.py
+src/machineconfig/scripts/python/fire_jobs.py
 src/machineconfig/scripts/python/ftprx.py
 src/machineconfig/scripts/python/ftpsx.py
 src/machineconfig/scripts/python/im2text.py
 src/machineconfig/scripts/python/mount_nfs.py
 src/machineconfig/scripts/python/mount_ssh.py
 src/machineconfig/scripts/python/onetimeshare.py
 src/machineconfig/scripts/python/pomodoro.py
 src/machineconfig/scripts/python/repos.py
 src/machineconfig/scripts/python/snapshot.py
 src/machineconfig/scripts/python/tmate_conn.py
 src/machineconfig/scripts/python/tmate_start.py
 src/machineconfig/scripts/python/transfer_wsl_win.py
 src/machineconfig/scripts/python/wifi_conn.py
 src/machineconfig/scripts/python/__pycache__/__init__.cpython-39.pyc
+src/machineconfig/scripts/python/__pycache__/chatgpt.cpython-39.pyc
 src/machineconfig/scripts/python/__pycache__/cloud_mount.cpython-39.pyc
 src/machineconfig/scripts/python/__pycache__/cloud_rx.cpython-39.pyc
 src/machineconfig/scripts/python/__pycache__/cloud_sx.cpython-39.pyc
+src/machineconfig/scripts/python/__pycache__/devops.cpython-39.pyc
 src/machineconfig/scripts/python/__pycache__/devops_backup_retrieve.cpython-39.pyc
 src/machineconfig/scripts/python/__pycache__/devops_devapps_install.cpython-39.pyc
 src/machineconfig/scripts/python/__pycache__/devops_update_repos.cpython-39.pyc
-src/machineconfig/scripts/python/archive/__init__.py
-src/machineconfig/scripts/python/archive/bu_gdrive_rx.py
-src/machineconfig/scripts/python/archive/bu_gdrive_sx.py
-src/machineconfig/scripts/python/archive/bu_onedrive_rx.py
-src/machineconfig/scripts/python/archive/bu_onedrive_sx.py
+src/machineconfig/scripts/python/__pycache__/fire_jobs.cpython-39.pyc
+src/machineconfig/scripts/python/__pycache__/pomodoro.cpython-39.pyc
 src/machineconfig/scripts/windows/activate_ve.ps1
+src/machineconfig/scripts/windows/chatgpt.ps1
 src/machineconfig/scripts/windows/choose_shell_theme.ps1
 src/machineconfig/scripts/windows/cloud_mount.ps1
 src/machineconfig/scripts/windows/cloud_repo_sync.ps1
 src/machineconfig/scripts/windows/cloud_rx.ps1
 src/machineconfig/scripts/windows/cloud_sx.ps1
 src/machineconfig/scripts/windows/cloud_sync.ps1
 src/machineconfig/scripts/windows/croshell.ps1
@@ -207,14 +211,15 @@
 src/machineconfig/scripts/windows/fix_rclone_link.ps1
 src/machineconfig/scripts/windows/ftprx.ps1
 src/machineconfig/scripts/windows/ftpsx.ps1
 src/machineconfig/scripts/windows/fzfb.ps1
 src/machineconfig/scripts/windows/fzfg.ps1
 src/machineconfig/scripts/windows/grep.ps1
 src/machineconfig/scripts/windows/im2text.ps1
+src/machineconfig/scripts/windows/kill_process.ps1
 src/machineconfig/scripts/windows/mount_nfs.ps1
 src/machineconfig/scripts/windows/nano.ps1
 src/machineconfig/scripts/windows/neofetch.ps1
 src/machineconfig/scripts/windows/pomodoro.ps1
 src/machineconfig/scripts/windows/py2exe.ps1
 src/machineconfig/scripts/windows/reload_path.ps1
 src/machineconfig/scripts/windows/repos.ps1
@@ -222,18 +227,19 @@
 src/machineconfig/scripts/windows/tmate_conn.ps1
 src/machineconfig/scripts/windows/transfer_sh.cmd
 src/machineconfig/scripts/windows/unlock_bitlocker.ps1
 src/machineconfig/scripts/windows/wifi_conn.ps1
 src/machineconfig/scripts/windows/wsl_rdp_windows_port_forwarding.ps1
 src/machineconfig/scripts/windows/wsl_ssh_windows_port_forwarding.ps1
 src/machineconfig/scripts/windows/wsl_windows_transfer.ps1
+src/machineconfig/scripts/windows/wts.ps1
 src/machineconfig/scripts/windows/archive/gource2vid.ps1
-src/machineconfig/scripts/windows/archive/lvim_fresh_installation.ps1
 src/machineconfig/scripts/windows/archive/secure_pull.ps1
 src/machineconfig/scripts/windows/archive/secure_push.ps1
+src/machineconfig/scripts/windows/utils/op_script_delete.ps1
 src/machineconfig/settings/broot/br.sh
 src/machineconfig/settings/broot/brootcd.ps1
 src/machineconfig/settings/helix/config.toml
 src/machineconfig/settings/helix/languages.toml
 src/machineconfig/settings/lf/linux/colors
 src/machineconfig/settings/lf/linux/icons
 src/machineconfig/settings/lf/linux/lfrc
@@ -272,24 +278,26 @@
 src/machineconfig/settings/lvim/windows/archive/config_additional.lua
 src/machineconfig/settings/lvim/windows/lua/user/custom_config.lua
 src/machineconfig/settings/mprocs/windows/mprocs.yaml
 src/machineconfig/settings/shells/bash/init.sh
 src/machineconfig/settings/shells/nushell/config.nu
 src/machineconfig/settings/shells/nushell/env.nu
 src/machineconfig/settings/shells/pwsh/init.ps1
+src/machineconfig/settings/shells/vtm/settings.xml
 src/machineconfig/settings/shells/wt/settings.json
 src/machineconfig/settings/svim/linux/init.toml
 src/machineconfig/settings/svim/windows/init.toml
 src/machineconfig/settings/tere/terecd.ps1
 src/machineconfig/settings/tere/terecd.sh
 src/machineconfig/settings/tmux/.tmate.conf
 src/machineconfig/settings/tmux/.tmux.conf
 src/machineconfig/settings/wsl/.wslconfig
 src/machineconfig/settings/zellij/config.kdl
 src/machineconfig/settings/zellij/config.orig.kdl
+src/machineconfig/settings/zellij/layouts/hist
 src/machineconfig/settings/zellij/layouts/st.kdl
 src/machineconfig/settings/zellij/themes/mytheme.kdl
 src/machineconfig/setup_linux/nix/cli_installation.sh
 src/machineconfig/setup_linux/others/archive
 src/machineconfig/setup_linux/others/chrome.sh
 src/machineconfig/setup_linux/others/openssh-server_add_pub_key.sh
 src/machineconfig/setup_linux/web_shortcuts/all.sh
@@ -305,9 +313,10 @@
 src/machineconfig/setup_windows/web_shortcuts/croshell.ps1
 src/machineconfig/setup_windows/web_shortcuts/ssh.ps1
 src/machineconfig/setup_windows/wt_and_pwsh/__init__.py
 src/machineconfig/setup_windows/wt_and_pwsh/install_fonts.ps1
 src/machineconfig/setup_windows/wt_and_pwsh/set_pwsh_theme.py
 src/machineconfig/setup_windows/wt_and_pwsh/set_wt_settings.py
 src/machineconfig/utils/__init__.py
+src/machineconfig/utils/procs.py
 src/machineconfig/utils/to_exe.py
 src/machineconfig/utils/utils.py
```

