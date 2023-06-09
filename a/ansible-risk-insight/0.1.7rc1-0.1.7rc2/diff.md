# Comparing `tmp/ansible-risk-insight-0.1.7rc1.tar.gz` & `tmp/ansible-risk-insight-0.1.7rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-risk-insight-0.1.7rc1.tar", last modified: Fri May 19 04:27:07 2023, max compression
+gzip compressed data, was "ansible-risk-insight-0.1.7rc2.tar", last modified: Thu May 25 08:07:57 2023, max compression
```

## Comparing `ansible-risk-insight-0.1.7rc1.tar` & `ansible-risk-insight-0.1.7rc2.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.434586 ansible-risk-insight-0.1.7rc1/
--rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/.flake8
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.353750 ansible-risk-insight-0.1.7rc1/.github/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.361087 ansible-risk-insight-0.1.7rc1/.github/workflows/
--rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.7rc1/.github/workflows/lint.yml
--rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.7rc1/.github/workflows/test.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.7rc1/.gitignore
--rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.7rc1/.pre-commit-config.yaml
--rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/CONTRIBUTING.md
--rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/LICENSE
--rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.7rc1/Makefile
--rw-r--r--   0 hiro       (501) staff       (20)      275 2023-05-19 04:27:07.434394 ansible-risk-insight-0.1.7rc1/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.7rc1/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.376534 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/
--rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-05-19 01:44:19.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)      662 2023-05-19 04:27:02.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/_version.py
--rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/analyzer.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.385656 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/annotator_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.398935 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/
--rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py
--rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py
--rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/command.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py
--rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/file.py
--rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py
--rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/git.py
--rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
--rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py
--rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py
--rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py
--rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
--rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/script.py
--rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py
--rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/template.py
--rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
--rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py
--rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py
--rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible_builtin.py
--rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak
--rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/module_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/risk_annotator_base.py
--rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/sample_custom_annotator.py
--rw-r--r--   0 hiro       (501) staff       (20)     9222 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/variable_resolver.py
--rw-r--r--   0 hiro       (501) staff       (20)   846979 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/ansible_builtin_modules.json
--rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/ansible_variables.txt
--rw-r--r--   0 hiro       (501) staff       (20)     2964 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/awx_utils.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/batch.sh
--rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/builtin-modules.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.399162 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/
--rw-r--r--   0 hiro       (501) staff       (20)     7429 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.401846 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/
--rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-05-19 01:44:23.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/diff.py
--rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/generate.py
--rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/list.py
--rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/release.py
--rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/search.py
--rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/update.py
--rw-r--r--   0 hiro       (501) staff       (20)    31810 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/context.py
--rw-r--r--   0 hiro       (501) staff       (20)    46758 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/dependency_dir_preparator.py
--rw-r--r--   0 hiro       (501) staff       (20)     8612 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/dependency_finder.py
--rw-r--r--   0 hiro       (501) staff       (20)    11036 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/finder.py
--rw-r--r--   0 hiro       (501) staff       (20)     2508 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/findings.py
--rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/key_test.py
--rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/keyutil.py
--rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/loader.py
--rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/logger.py
--rw-r--r--   0 hiro       (501) staff       (20)    60903 2023-05-19 01:44:42.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/model_loader.py
--rw-r--r--   0 hiro       (501) staff       (20)    76012 2023-05-19 01:43:47.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/models.py
--rw-r--r--   0 hiro       (501) staff       (20)    24282 2023-05-19 01:44:34.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/parser.py
--rw-r--r--   0 hiro       (501) staff       (20)     5955 2023-05-19 01:44:28.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/ram_generator.py
--rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/requirements.txt
--rw-r--r--   0 hiro       (501) staff       (20)    44597 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/risk_assessment_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     8504 2023-05-19 00:55:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/risk_detector.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.418563 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     4076 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P001_module_name_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     6282 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     6322 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)     3036 2023-04-28 09:03:05.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P004_variable_validation.py
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R101_command_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R103_download_exec.py
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R105_outbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R106_inbound_transfer.py
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R108_privilege_escalation.py
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R109_key_config_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R110_non_builtin_use.py
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R114_file_change.py
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R115_file_deletion.py
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py
--rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R117_external_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py
--rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R202_unconditional_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R203_unused_override.py
--rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
--rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R301_non_fqcn_use.md
--rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py
--rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R302_role_without_metadata.py
--rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R303_task_without_name.py
--rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R304_unresolved_module.py
--rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R305_unresolved_role.py
--rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R306_undefined_variable.py
--rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py
--rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R404_show_variables.py
--rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py
--rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/__init__.py
--rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-21 02:09:38.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/rule_versions.json
--rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/safe_glob.py
--rw-r--r--   0 hiro       (501) staff       (20)    46832 2023-05-19 01:44:44.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/scanner.py
--rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/task_keywords.txt
--rw-r--r--   0 hiro       (501) staff       (20)    38319 2023-05-19 01:44:37.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/tree.py
--rw-r--r--   0 hiro       (501) staff       (20)    24619 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/utils.py
--rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/variable_manager.py
--rw-r--r--   0 hiro       (501) staff       (20)      971 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight/yaml.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.378393 ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)      275 2023-05-19 04:27:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     8097 2023-05-19 04:27:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-05-19 04:27:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       99 2023-05-19 04:27:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)       91 2023-05-19 04:27:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)       21 2023-05-19 04:27:07.000000 ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc1/data-struct.txt
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.354738 ansible-risk-insight-0.1.7rc1/doc/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.422724 ansible-risk-insight-0.1.7rc1/doc/images/
--rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.7rc1/doc/images/ari-apply-rules.png
--rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.7rc1/doc/images/ari-arch.png
--rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.7rc1/doc/images/ari-overview.png
--rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.7rc1/doc/images/ari-ram-list.png
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.425052 ansible-risk-insight-0.1.7rc1/docs/
--rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.7rc1/docs/annotation.md
--rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.7rc1/docs/customize_rules.md
--rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.7rc1/docs/index.md
--rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.7rc1/docs/installing.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.429698 ansible-risk-insight-0.1.7rc1/docs/rules/
--rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R101_command_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R102_command_instead_of_shell.md
--rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R103_download_exec.md
--rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R104_unauthorized_download_src.md
--rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R105_outbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R106_inbound_transfer.md
--rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R107_pkg_install_with_insecure_option.md
--rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R108_privilege_escalation.md
--rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R109_key_config_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R110_non_builtin_use.md
--rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R111_parameterized_import_role.md
--rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R112_parameterized_import_taskfile.md
--rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R113_parameterized_pkg_install.md
--rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R114_file_change.md
--rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R115_file_deletion.md
--rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R116_insecure_file_permission.md
--rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc1/docs/rules/R301_non_fqcn_use.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.430217 ansible-risk-insight-0.1.7rc1/example/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.430577 ansible-risk-insight-0.1.7rc1/example/playbooks/
--rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.7rc1/example/playbooks/sample_playbook.yml
--rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.7rc1/example/readme.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.430869 ansible-risk-insight-0.1.7rc1/example/rules/
--rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.7rc1/example/rules/sample_rule.py
--rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.7rc1/example/sample.py
--rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.7rc1/mkdocs.yml
--rw-r--r--   0 hiro       (501) staff       (20)      993 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc1/pyproject.toml
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-19 04:27:07.434650 ansible-risk-insight-0.1.7rc1/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.7rc1/setup.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.431234 ansible-risk-insight-0.1.7rc1/test/
--rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.7rc1/test/test_scanner.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.356301 ansible-risk-insight-0.1.7rc1/test/testdata/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.355609 ansible-risk-insight-0.1.7rc1/test/testdata/projects/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.432069 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/
--rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/MANIFEST.json
--rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/galaxy.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.355813 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.356139 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/sample-role-1/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.432447 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.432810 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.433149 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.356389 ansible-risk-insight-0.1.7rc1/test/testdata/roles/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.356761 ansible-risk-insight-0.1.7rc1/test/testdata/roles/test_role/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.433457 ansible-risk-insight-0.1.7rc1/test/testdata/roles/test_role/defaults/
--rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/roles/test_role/defaults/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.433727 ansible-risk-insight-0.1.7rc1/test/testdata/roles/test_role/meta/
--rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/roles/test_role/meta/main.yml
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-19 04:27:07.434037 ansible-risk-insight-0.1.7rc1/test/testdata/roles/test_role/tasks/
--rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc1/test/testdata/roles/test_role/tasks/main.yml
--rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.7rc1/tox.ini
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.429154 ansible-risk-insight-0.1.7rc2/
+-rw-r--r--   0 hiro       (501) staff       (20)       46 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc2/.flake8
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.366340 ansible-risk-insight-0.1.7rc2/.github/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.372346 ansible-risk-insight-0.1.7rc2/.github/workflows/
+-rw-r--r--   0 hiro       (501) staff       (20)      832 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.7rc2/.github/workflows/lint.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      749 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.7rc2/.github/workflows/test.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-03-23 07:29:42.000000 ansible-risk-insight-0.1.7rc2/.gitignore
+-rw-r--r--   0 hiro       (501) staff       (20)      436 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.7rc2/.pre-commit-config.yaml
+-rw-r--r--   0 hiro       (501) staff       (20)      990 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc2/CONTRIBUTING.md
+-rw-r--r--   0 hiro       (501) staff       (20)    11357 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc2/LICENSE
+-rw-r--r--   0 hiro       (501) staff       (20)      456 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.7rc2/Makefile
+-rw-r--r--   0 hiro       (501) staff       (20)      275 2023-05-25 08:07:57.429004 ansible-risk-insight-0.1.7rc2/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     4510 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.7rc2/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.384369 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/
+-rw-r--r--   0 hiro       (501) staff       (20)     1907 2023-05-19 01:44:19.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)      662 2023-05-25 08:07:44.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/_version.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3519 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/analyzer.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.387130 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1408 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/annotator_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.391673 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/
+-rw-r--r--   0 hiro       (501) staff       (20)     1393 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/apt.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1587 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/apt_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1446 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/assemble.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1460 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1388 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/command.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/dnf.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1447 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/expect.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/file.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1320 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/get_url.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1317 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/git.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1511 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1339 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/pip.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1380 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/raw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1448 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/replace.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1371 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1386 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/script.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1384 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1327 2023-02-01 01:54:20.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/subversion.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/template.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2221 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/unarchive.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1499 2023-02-09 05:39:40.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/uri.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1498 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/yum.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1230 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible_builtin.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46432 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible_builtin.py.bak
+-rw-r--r--   0 hiro       (501) staff       (20)     1113 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/module_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2846 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/risk_annotator_base.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2381 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/sample_custom_annotator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9222 2023-05-19 01:44:14.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/variable_resolver.py
+-rw-r--r--   0 hiro       (501) staff       (20)   846979 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/ansible_builtin_modules.json
+-rw-r--r--   0 hiro       (501) staff       (20)     2306 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/ansible_variables.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     3312 2023-05-25 06:38:28.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/awx_utils.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      678 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/batch.sh
+-rw-r--r--   0 hiro       (501) staff       (20)     1049 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/builtin-modules.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.391844 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/
+-rw-r--r--   0 hiro       (501) staff       (20)     7429 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.393701 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/ram/
+-rw-r--r--   0 hiro       (501) staff       (20)     2032 2023-05-19 01:44:23.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/ram/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1705 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/ram/diff.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3085 2023-04-04 07:22:15.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/ram/generate.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1486 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/ram/list.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1690 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/ram/release.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1720 2023-01-06 06:26:43.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/ram/search.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2033 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/ram/update.py
+-rw-r--r--   0 hiro       (501) staff       (20)    31842 2023-05-25 06:23:13.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/context.py
+-rw-r--r--   0 hiro       (501) staff       (20)    46758 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/dependency_dir_preparator.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8612 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/dependency_finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)    11036 2023-04-26 08:32:29.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/finder.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2508 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/findings.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1291 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/key_test.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8235 2023-03-30 02:27:00.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/keyutil.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8683 2023-04-13 09:29:16.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1615 2023-02-13 09:30:01.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/logger.py
+-rw-r--r--   0 hiro       (501) staff       (20)    60897 2023-05-25 06:38:29.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/model_loader.py
+-rw-r--r--   0 hiro       (501) staff       (20)    76012 2023-05-19 01:43:47.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/models.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24418 2023-05-25 05:08:02.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/parser.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5955 2023-05-19 01:44:28.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/ram_generator.py
+-rw-r--r--   0 hiro       (501) staff       (20)      105 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/requirements.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    44597 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/risk_assessment_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8504 2023-05-25 02:34:50.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/risk_detector.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.415711 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     4076 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/P001_module_name_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     6571 2023-05-25 06:38:28.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/P002_module_argument_key_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     6322 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/P003_module_argument_value_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3036 2023-04-28 09:03:05.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/P004_variable_validation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1801 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R101_command_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1684 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R102_command_instead_of_shell.py
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2703 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R103_download_exec.py
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2370 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R104_unauthorized_download_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1846 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R105_outbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1947 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R106_inbound_transfer.py
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2066 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1536 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R108_privilege_escalation.py
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1756 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R109_key_config_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1642 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R110_non_builtin_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1729 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R111_parameterized_import_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1952 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1875 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R113_parameterized_pkg_install.py
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)     2088 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R114_file_change.py
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1871 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R115_file_deletion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1649 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R116_insecure_file_permission.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1661 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R117_external_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1927 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R201_changed_data_dependence.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2123 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R202_unconditional_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2181 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R203_unused_override.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2180 2023-03-28 00:46:23.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R204_unnecessary_set_fact.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1707 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R205_unnecessary_include_vars.py
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R301_non_fqcn_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)     1827 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R301_non_fqcn_use.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1430 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R302_role_without_metadata.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1416 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R303_task_without_name.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1607 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R304_unresolved_module.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1712 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R305_unresolved_role.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1787 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R306_undefined_variable.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1925 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R401_list_all_inbound_src.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1609 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R402_list_all_used_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1939 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R404_show_variables.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1974 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R501_dependency_suggestion.py
+-rw-r--r--   0 hiro       (501) staff       (20)      636 2023-01-31 05:05:07.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/__init__.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5279 2023-04-21 02:09:38.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/rule_versions.json
+-rw-r--r--   0 hiro       (501) staff       (20)     1521 2023-05-19 01:44:11.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3261 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/safe_glob.py
+-rw-r--r--   0 hiro       (501) staff       (20)    47220 2023-05-25 06:38:29.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/scanner.py
+-rw-r--r--   0 hiro       (501) staff       (20)      394 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/task_keywords.txt
+-rw-r--r--   0 hiro       (501) staff       (20)    39915 2023-05-25 06:38:29.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/tree.py
+-rw-r--r--   0 hiro       (501) staff       (20)    24586 2023-05-23 00:15:29.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/utils.py
+-rw-r--r--   0 hiro       (501) staff       (20)      939 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/variable_manager.py
+-rw-r--r--   0 hiro       (501) staff       (20)      971 2023-03-23 08:17:01.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight/yaml.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.385345 ansible-risk-insight-0.1.7rc2/ansible_risk_insight.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)      275 2023-05-25 08:07:57.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     8097 2023-05-25 08:07:57.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-05-25 08:07:57.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       99 2023-05-25 08:07:57.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       91 2023-05-25 08:07:57.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       21 2023-05-25 08:07:57.000000 ansible-risk-insight-0.1.7rc2/ansible_risk_insight.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)     1473 2022-12-14 05:36:09.000000 ansible-risk-insight-0.1.7rc2/data-struct.txt
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.367140 ansible-risk-insight-0.1.7rc2/doc/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.419232 ansible-risk-insight-0.1.7rc2/doc/images/
+-rw-r--r--   0 hiro       (501) staff       (20)   169018 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.7rc2/doc/images/ari-apply-rules.png
+-rw-r--r--   0 hiro       (501) staff       (20)   403143 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.7rc2/doc/images/ari-arch.png
+-rw-r--r--   0 hiro       (501) staff       (20)   316218 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.7rc2/doc/images/ari-overview.png
+-rw-r--r--   0 hiro       (501) staff       (20)   473549 2023-02-27 07:18:31.000000 ansible-risk-insight-0.1.7rc2/doc/images/ari-ram-list.png
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.421495 ansible-risk-insight-0.1.7rc2/docs/
+-rw-r--r--   0 hiro       (501) staff       (20)     2179 2023-03-01 02:03:44.000000 ansible-risk-insight-0.1.7rc2/docs/annotation.md
+-rw-r--r--   0 hiro       (501) staff       (20)     6685 2023-02-27 08:35:40.000000 ansible-risk-insight-0.1.7rc2/docs/customize_rules.md
+-rw-r--r--   0 hiro       (501) staff       (20)      458 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.7rc2/docs/index.md
+-rw-r--r--   0 hiro       (501) staff       (20)      188 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.7rc2/docs/installing.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.425168 ansible-risk-insight-0.1.7rc2/docs/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)      309 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R101_command_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      453 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R102_command_instead_of_shell.md
+-rw-r--r--   0 hiro       (501) staff       (20)      633 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R103_download_exec.md
+-rw-r--r--   0 hiro       (501) staff       (20)      696 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R104_unauthorized_download_src.md
+-rw-r--r--   0 hiro       (501) staff       (20)      506 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R105_outbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      469 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R106_inbound_transfer.md
+-rw-r--r--   0 hiro       (501) staff       (20)      600 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R107_pkg_install_with_insecure_option.md
+-rw-r--r--   0 hiro       (501) staff       (20)      550 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R108_privilege_escalation.md
+-rw-r--r--   0 hiro       (501) staff       (20)      399 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R109_key_config_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      149 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R110_non_builtin_use.md
+-rw-r--r--   0 hiro       (501) staff       (20)      325 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R111_parameterized_import_role.md
+-rw-r--r--   0 hiro       (501) staff       (20)      410 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R112_parameterized_import_taskfile.md
+-rw-r--r--   0 hiro       (501) staff       (20)      490 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R113_parameterized_pkg_install.md
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R114_file_change.md
+-rw-r--r--   0 hiro       (501) staff       (20)      494 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R115_file_deletion.md
+-rw-r--r--   0 hiro       (501) staff       (20)      422 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R116_insecure_file_permission.md
+-rw-r--r--   0 hiro       (501) staff       (20)      403 2023-02-13 07:57:48.000000 ansible-risk-insight-0.1.7rc2/docs/rules/R301_non_fqcn_use.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.425732 ansible-risk-insight-0.1.7rc2/example/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.426022 ansible-risk-insight-0.1.7rc2/example/playbooks/
+-rw-r--r--   0 hiro       (501) staff       (20)      509 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.7rc2/example/playbooks/sample_playbook.yml
+-rw-r--r--   0 hiro       (501) staff       (20)     1106 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.7rc2/example/readme.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.426276 ansible-risk-insight-0.1.7rc2/example/rules/
+-rw-r--r--   0 hiro       (501) staff       (20)     1366 2023-03-06 00:24:15.000000 ansible-risk-insight-0.1.7rc2/example/rules/sample_rule.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1728 2023-03-23 08:17:04.000000 ansible-risk-insight-0.1.7rc2/example/sample.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1300 2023-02-07 04:27:33.000000 ansible-risk-insight-0.1.7rc2/mkdocs.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      993 2023-05-15 07:37:16.000000 ansible-risk-insight-0.1.7rc2/pyproject.toml
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-25 08:07:57.429204 ansible-risk-insight-0.1.7rc2/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2022-12-16 00:52:20.000000 ansible-risk-insight-0.1.7rc2/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.426647 ansible-risk-insight-0.1.7rc2/test/
+-rw-r--r--   0 hiro       (501) staff       (20)     2668 2023-03-30 11:42:56.000000 ansible-risk-insight-0.1.7rc2/test/test_scanner.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.368359 ansible-risk-insight-0.1.7rc2/test/testdata/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.367864 ansible-risk-insight-0.1.7rc2/test/testdata/projects/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.427216 ansible-risk-insight-0.1.7rc2/test/testdata/projects/my.collection/
+-rw-r--r--   0 hiro       (501) staff       (20)      845 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc2/test/testdata/projects/my.collection/MANIFEST.json
+-rw-r--r--   0 hiro       (501) staff       (20)      460 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc2/test/testdata/projects/my.collection/galaxy.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.368018 ansible-risk-insight-0.1.7rc2/test/testdata/projects/my.collection/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.368268 ansible-risk-insight-0.1.7rc2/test/testdata/projects/my.collection/roles/sample-role-1/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.427439 ansible-risk-insight-0.1.7rc2/test/testdata/projects/my.collection/roles/sample-role-1/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc2/test/testdata/projects/my.collection/roles/sample-role-1/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.427603 ansible-risk-insight-0.1.7rc2/test/testdata/projects/my.collection/roles/sample-role-1/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      418 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc2/test/testdata/projects/my.collection/roles/sample-role-1/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.427781 ansible-risk-insight-0.1.7rc2/test/testdata/projects/my.collection/roles/sample-role-1/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc2/test/testdata/projects/my.collection/roles/sample-role-1/tasks/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.368422 ansible-risk-insight-0.1.7rc2/test/testdata/roles/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.368686 ansible-risk-insight-0.1.7rc2/test/testdata/roles/test_role/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.427954 ansible-risk-insight-0.1.7rc2/test/testdata/roles/test_role/defaults/
+-rw-r--r--   0 hiro       (501) staff       (20)       43 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc2/test/testdata/roles/test_role/defaults/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.428172 ansible-risk-insight-0.1.7rc2/test/testdata/roles/test_role/meta/
+-rw-r--r--   0 hiro       (501) staff       (20)      414 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc2/test/testdata/roles/test_role/meta/main.yml
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-25 08:07:57.428433 ansible-risk-insight-0.1.7rc2/test/testdata/roles/test_role/tasks/
+-rw-r--r--   0 hiro       (501) staff       (20)      212 2022-12-15 06:16:53.000000 ansible-risk-insight-0.1.7rc2/test/testdata/roles/test_role/tasks/main.yml
+-rw-r--r--   0 hiro       (501) staff       (20)      589 2023-01-05 06:52:13.000000 ansible-risk-insight-0.1.7rc2/tox.ini
```

### Comparing `ansible-risk-insight-0.1.7rc1/.github/workflows/lint.yml` & `ansible-risk-insight-0.1.7rc2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/.github/workflows/test.yml` & `ansible-risk-insight-0.1.7rc2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/.gitignore` & `ansible-risk-insight-0.1.7rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/CONTRIBUTING.md` & `ansible-risk-insight-0.1.7rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/LICENSE` & `ansible-risk-insight-0.1.7rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/README.md` & `ansible-risk-insight-0.1.7rc2/README.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/__init__.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/_version.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.7rc1"
+__version__ = "0.1.7rc2"
```

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/analyzer.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/analyzer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/__init__.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/annotator_base.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/apt.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/apt.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/apt_key.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/apt_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/assemble.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/assemble.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/blockinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/command.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/command.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/dnf.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/dnf.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/expect.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/expect.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/file.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/file.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/get_url.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/get_url.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/git.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/git.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/lineinfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/pip.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/pip.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/raw.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/raw.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/replace.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/replace.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/rpm_key.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/script.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/script.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/shell.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/subversion.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/subversion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/template.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/template.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/unarchive.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/unarchive.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/uri.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/uri.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible.builtin/yum.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible.builtin/yum.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible_builtin.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible_builtin.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/ansible_builtin.py.bak` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/ansible_builtin.py.bak`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/module_annotator_base.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/module_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/risk_annotator_base.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/risk_annotator_base.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/sample_custom_annotator.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/sample_custom_annotator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/annotators/variable_resolver.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/annotators/variable_resolver.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/ansible_builtin_modules.json` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/ansible_builtin_modules.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/ansible_variables.txt` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/ansible_variables.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/awx_utils.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/awx_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,26 @@
                     matched = True
                     break
     except IOError:
         return False
     return matched
 
 
+def could_be_taskfile(fpath):
+    if could_be_playbook(fpath):
+        return False
+    with codecs.open(fpath, "r", encoding="utf-8", errors="ignore") as f:
+        for n, line in enumerate(f):
+            if "- name: " in line:
+                return True
+            if "ansible.builtin." in line:
+                return True
+    return False
+
+
 # this method is based on awx code
 # awx/main/models/projects.py#L206-L217 in ansible/awx
 def search_playbooks(root_path):
     results = []
     if root_path and os.path.exists(root_path):
         for dirpath, dirnames, filenames in os.walk(root_path, followlinks=False):
             if skip_directory(dirpath):
```

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/batch.sh` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/batch.sh`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/builtin-modules.txt` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/builtin-modules.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/__init__.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/__init__.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/diff.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/ram/diff.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/generate.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/ram/generate.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/list.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/ram/list.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/release.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/ram/release.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/search.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/ram/search.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/cli/ram/update.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/cli/ram/update.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/context.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -536,15 +536,16 @@
         elif isinstance(loop_values, dict):
             tmp_variables = {}
             for k, v in loop_values.items():
                 key = "{}.{}".format(loop_key, k)
                 tmp_variables.update({key: v})
             variables_in_loop.append(tmp_variables)
         else:
-            raise ValueError("loop_values of type {} is not supported yet".format(type(loop_values).__name__))
+            if loop_values:
+                raise ValueError("loop_values of type {} is not supported yet".format(type(loop_values).__name__))
 
     resolved_opts_in_loop = []
     mutable_vars_per_mo = {}
     for variables in variables_in_loop:
         resolved_opts = None
         if isinstance(taskcall.spec.module_options, dict):
             resolved_opts = {}
```

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/dependency_dir_preparator.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/dependency_dir_preparator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/dependency_finder.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/dependency_finder.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/finder.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/finder.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/findings.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/findings.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/key_test.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/key_test.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/keyutil.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/keyutil.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/loader.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/loader.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/logger.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/model_loader.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/model_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,21 +66,21 @@
     split_target_playbook_fullpath,
     split_target_taskfile_fullpath,
     get_module_specs_by_ansible_doc,
     get_documentation_in_module_file,
     get_class_by_arg_type,
     is_test_object,
 )
-from .awx_utils import could_be_playbook
+from .awx_utils import could_be_playbook, could_be_taskfile
 
 # collection info direcotry can be something like
 #   "brightcomputing.bcm-9.1.11+41615.gitfab9053.info"
 collection_info_dir_re = re.compile(r"^[a-z0-9_]+\.[a-z0-9_]+-[0-9]+\.[0-9]+\.[0-9]+.*\.info$")
 
-string_module_options_re = re.compile(r"[a-z0-9]+=(?:[^ ]*{{ [^ ]+ }}[^ ]*|[^ ])+")
+string_module_options_re = re.compile(r"^([a-z0-9]+=(?:[^ ]*{{ [^ ]+ }}[^ ]*|[^ ])+\s?)+$")
 
 loop_task_option_names = [
     "loop",
     "with_list",
     "with_items",
     "with_dict",
     # TODO: support the following
@@ -604,22 +604,25 @@
     if path == "":
         return []
     patterns = [
         os.path.join(path, "/*.ya?ml"),
         os.path.join(path, "/playbooks/**/*.ya?ml"),
     ]
     if include_test_contents:
-        patterns.append(os.path.join(path, "tests/integration/**/*.ya?ml"))
+        patterns.append(os.path.join(path, "tests/**/*.ya?ml"))
         patterns.append(os.path.join(path, "molecule/**/*.ya?ml"))
     candidates = safe_glob(patterns, recursive=True)
     playbooks = []
     playbook_names = []
     for fpath in candidates:
         if could_be_playbook(fpath):
-            if "/roles/" in fpath:
+            relative_path = ""
+            if fpath.startswith(path):
+                relative_path = fpath[len(path) :]
+            if "/roles/" in relative_path:
                 continue
             p = None
             try:
                 p = load_playbook(
                     path=fpath,
                     basedir=basedir,
                     skip_playbook_format_error=skip_playbook_format_error,
@@ -650,35 +653,45 @@
     name="",
     collection_name="",
     module_dir_paths=[],
     basedir="",
     use_ansible_doc=True,
     skip_playbook_format_error=True,
     skip_task_format_error=True,
+    include_test_contents=False,
     load_children=True,
 ):
     roleObj = Role()
     fullpath = ""
     if os.path.exists(path) and path != "" and path != ".":
         fullpath = path
     if os.path.exists(os.path.join(basedir, path)):
         fullpath = os.path.normpath(os.path.join(basedir, path))
     if fullpath == "":
         raise ValueError(f"directory not found: {path}, {basedir}")
+    else:
+        # some roles can be found at "/path/to/role.name/role.name"
+        # especially when the role has dependency roles
+        # so we try it here
+        basename = os.path.basename(fullpath)
+        tmp_fullpath = os.path.join(fullpath, basename)
+        if os.path.exists(tmp_fullpath):
+            fullpath = tmp_fullpath
     meta_file_path = ""
     defaults_dir_path = ""
     vars_dir_path = ""
     tasks_dir_path = ""
     handlers_dir_path = ""
     includes_dir_path = ""
     if fullpath != "":
         meta_file_path = os.path.join(fullpath, "meta/main.yml")
         defaults_dir_path = os.path.join(fullpath, "defaults")
         vars_dir_path = os.path.join(fullpath, "vars")
         tasks_dir_path = os.path.join(fullpath, "tasks")
+        tests_dir_path = os.path.join(fullpath, "tests")
         handlers_dir_path = os.path.join(fullpath, "handlers")
         includes_dir_path = os.path.join(fullpath, "includes")
     if os.path.exists(meta_file_path):
         with open(meta_file_path, "r") as file:
             try:
                 roleObj.metadata = yaml.load(file, Loader=Loader)
             except Exception as e:
@@ -715,43 +728,23 @@
     if collection_name != "" and not is_test:
         collection = collection_name
         fqcn = "{}.{}".format(collection_name, role_name)
     roleObj.collection = collection
     roleObj.fqcn = fqcn
     roleObj.set_key()
 
-    if os.path.exists(os.path.join(fullpath, "playbooks")):
-        playbook_files = safe_glob(fullpath + "/playbooks/**/*.ya?ml", recursive=True)
-        playbooks = []
-        for f in playbook_files:
-            p = None
-            try:
-                p = load_playbook(
-                    f,
-                    role_name=role_name,
-                    collection_name=collection_name,
-                    basedir=basedir,
-                    skip_playbook_format_error=skip_playbook_format_error,
-                    skip_task_format_error=skip_task_format_error,
-                )
-            except PlaybookFormatError as e:
-                if skip_playbook_format_error:
-                    logger.debug("this file is not in a playbook format, maybe not a playbook file, skip this: {}".format(e.args[0]))
-                    continue
-                else:
-                    raise PlaybookFormatError(f"this file is not in a playbook format, maybe not a playbook file: {e.args[0]}")
-            except Exception:
-                logger.exception("error while loading the playbook at {}".format(f))
-            if load_children:
-                playbooks.append(p)
-            else:
-                playbooks.append(p.defined_in)
-        if not load_children:
-            playbooks = sorted(playbooks)
-        roleObj.playbooks = playbooks
+    playbooks = load_playbooks(
+        path=fullpath,
+        basedir=basedir,
+        skip_playbook_format_error=skip_playbook_format_error,
+        skip_task_format_error=skip_task_format_error,
+        include_test_contents=include_test_contents,
+        load_children=load_children,
+    )
+    roleObj.playbooks = playbooks
 
     if os.path.exists(defaults_dir_path):
         patterns = [
             defaults_dir_path + "/**/*.ya?ml",
         ]
         defaults_yaml_files = safe_glob(patterns, recursive=True)
         default_variables = {}
@@ -820,19 +813,23 @@
         modules = sorted(modules)
     roleObj.modules = modules
 
     patterns = [tasks_dir_path + "/**/*.ya?ml"]
     # ansible.network collection has this type of another taskfile directory
     if os.path.exists(includes_dir_path):
         patterns.extend([includes_dir_path + "/**/*.ya?ml"])
+    if include_test_contents:
+        patterns.extend([tests_dir_path + "/**/*.ya?ml"])
     task_yaml_files = safe_glob(patterns, recursive=True)
 
     taskfiles = []
     for task_yaml_path in task_yaml_files:
         tf = None
+        if not could_be_taskfile(task_yaml_path):
+            continue
         try:
             tf = load_taskfile(
                 task_yaml_path,
                 role_name=fqcn,
                 collection_name=collection_name,
                 basedir=basedir,
                 skip_task_format_error=skip_task_format_error,
@@ -938,14 +935,15 @@
         try:
             r = load_role(
                 path=role_dir,
                 basedir=basedir,
                 use_ansible_doc=use_ansible_doc,
                 skip_playbook_format_error=skip_playbook_format_error,
                 skip_task_format_error=skip_task_format_error,
+                include_test_contents=include_test_contents,
             )
         except Exception:
             logger.exception("error while loading the role at {}".format(role_dir))
         if load_children:
             roles.append(r)
         else:
             roles.append(r.defined_in)
@@ -1556,15 +1554,15 @@
 def load_object(loadObj):
     target_type = loadObj.target_type
     path = loadObj.path
     obj = None
     if target_type == LoadType.COLLECTION:
         obj = load_collection(collection_dir=path, basedir=path, include_test_contents=loadObj.include_test_contents, load_children=False)
     elif target_type == LoadType.ROLE:
-        obj = load_role(path=path, basedir=path, load_children=False)
+        obj = load_role(path=path, basedir=path, include_test_contents=loadObj.include_test_contents, load_children=False)
     elif target_type == LoadType.PLAYBOOK:
         basedir = ""
         target_playbook_path = ""
         if loadObj.playbook_yaml:
             target_playbook_path = path
         else:
             basedir, target_playbook_path = split_target_playbook_fullpath(path)
@@ -1588,14 +1586,19 @@
 
     if hasattr(obj, "roles"):
         loadObj.roles = obj.roles
     if hasattr(obj, "playbooks"):
         loadObj.playbooks = obj.playbooks
     if hasattr(obj, "taskfiles"):
         loadObj.taskfiles = obj.taskfiles
+    if hasattr(obj, "handlers"):
+        current = loadObj.taskfiles
+        if not current:
+            current = []
+        loadObj.taskfiles = current + obj.handlers
     if hasattr(obj, "modules"):
         loadObj.modules = obj.modules
 
     if target_type == LoadType.ROLE:
         loadObj.roles = [obj.defined_in]
     elif target_type == LoadType.PLAYBOOK and loadObj.playbook_only:
         loadObj.playbooks = [obj.defined_in]
```

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/models.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/models.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/parser.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
             try:
                 obj = load_role(
                     path=ld.path,
                     basedir=ld.path,
                     use_ansible_doc=self.use_ansible_doc,
                     skip_playbook_format_error=self.skip_playbook_format_error,
                     skip_task_format_error=self.skip_task_format_error,
+                    include_test_contents=ld.include_test_contents,
                     load_children=False,
                 )
             except PlaybookFormatError:
                 if not self.skip_playbook_format_error:
                     raise
             except TaskFormatError:
                 if not self.skip_task_format_error:
@@ -220,14 +221,15 @@
                 r = load_role(
                     path=role_path,
                     collection_name=collection_name,
                     basedir=basedir,
                     use_ansible_doc=self.use_ansible_doc,
                     skip_playbook_format_error=self.skip_playbook_format_error,
                     skip_task_format_error=self.skip_task_format_error,
+                    include_test_contents=ld.include_test_contents,
                 )
                 roles.append(r)
             except PlaybookFormatError:
                 if not self.skip_playbook_format_error:
                     raise
             except TaskFormatError:
                 if not self.skip_task_format_error:
```

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/ram_generator.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/ram_generator.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/risk_assessment_model.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/risk_assessment_model.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/risk_detector.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/risk_detector.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P001_module_name_validation.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/P001_module_name_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P002_module_argument_key_validation.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/P002_module_argument_key_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     Severity,
     RuleTag as Tag,
     ExecutableType,
     ActionGroupMetadata,
 )
 
 
+def is_set_fact(module_fqcn):
+    return module_fqcn == "ansible.builtin.set_fact"
+
+
 @dataclass
 class ModuleArgumentKeyValidationRule(Rule):
     rule_id: str = "P002"
     description: str = "Validate module argument keys and set annotations"
     enabled: bool = True
     name: str = "ModuleArgumentKeyValidation"
     version: str = "v0.0.1"
@@ -85,51 +89,56 @@
                             break
                     if found:
                         break
 
             used_keys = []
             if isinstance(mo, dict):
                 used_keys = list(mo.keys())
+
             available_keys = []
             required_keys = []
             alias_reverse_map = {}
             available_args = None
-            if task.module:
-                for arg in task.module.arguments:
-                    available_keys.extend(arg.available_keys())
-                    if arg.required:
-                        aliases = arg.aliases if arg.aliases else []
-                        req_k = {"key": arg.name, "aliases": aliases}
-                        required_keys.append(req_k)
-                    if arg.aliases:
-                        for al in arg.aliases:
-                            alias_reverse_map[al] = arg.name
-                available_args = task.module.arguments
-            wrong_keys = [key for key in used_keys if key not in available_keys]
+            wrong_keys = []
             missing_required_keys = []
-            for k in required_keys:
-                name = k.get("key", "")
-                aliases = k.get("aliases", [])
-                if name in used_keys:
-                    continue
-                if name in default_args:
-                    continue
-                if aliases:
-                    found = False
-                    for a_k in aliases:
-                        if a_k in used_keys:
-                            found = True
-                            break
-                        if a_k in default_args:
-                            found = True
-                            break
-                    if found:
+            if not is_set_fact(module_fqcn):
+                if task.module:
+                    for arg in task.module.arguments:
+                        available_keys.extend(arg.available_keys())
+                        if arg.required:
+                            aliases = arg.aliases if arg.aliases else []
+                            req_k = {"key": arg.name, "aliases": aliases}
+                            required_keys.append(req_k)
+                        if arg.aliases:
+                            for al in arg.aliases:
+                                alias_reverse_map[al] = arg.name
+                    available_args = task.module.arguments
+
+                wrong_keys = [key for key in used_keys if key not in available_keys]
+
+                for k in required_keys:
+                    name = k.get("key", "")
+                    aliases = k.get("aliases", [])
+                    if name in used_keys:
+                        continue
+                    if name in default_args:
                         continue
-                # here, the required key was not found
-                missing_required_keys.append(name)
+                    if aliases:
+                        found = False
+                        for a_k in aliases:
+                            if a_k in used_keys:
+                                found = True
+                                break
+                            if a_k in default_args:
+                                found = True
+                                break
+                        if found:
+                            continue
+                    # here, the required key was not found
+                    missing_required_keys.append(name)
 
             used_alias_and_real_keys = []
             for k in used_keys:
                 if k not in alias_reverse_map:
                     continue
                 real_name = alias_reverse_map[k]
                 used_alias_and_real_keys.append(
```

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P003_module_argument_value_validation.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/P003_module_argument_value_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/P004_variable_validation.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/P004_variable_validation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R101_command_exec.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R101_command_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R102_command_instead_of_shell.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R102_command_instead_of_shell.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R103_download_exec.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R103_download_exec.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R104_unauthorized_download_src.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R104_unauthorized_download_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R105_outbound_transfer.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R105_outbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R106_inbound_transfer.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R106_inbound_transfer.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R107_pkg_install_with_insecure_option.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R108_privilege_escalation.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R108_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R109_key_config_change.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R109_key_config_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R110_non_builtin_use.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R110_non_builtin_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R111_parameterized_import_role.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R111_parameterized_import_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R112_parameterized_import_taskfile.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R113_parameterized_pkg_install.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R113_parameterized_pkg_install.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R114_file_change.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R114_file_change.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R115_file_deletion.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R115_file_deletion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R116_insecure_file_permission.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R116_insecure_file_permission.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R117_external_role.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R117_external_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R201_changed_data_dependence.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R201_changed_data_dependence.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R202_unconditional_override.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R202_unconditional_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R203_unused_override.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R203_unused_override.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R204_unnecessary_set_fact.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R204_unnecessary_set_fact.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R205_unnecessary_include_vars.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R205_unnecessary_include_vars.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R301_non_fqcn_use.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R301_non_fqcn_use.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R302_role_without_metadata.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R302_role_without_metadata.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R303_task_without_name.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R303_task_without_name.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R304_unresolved_module.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R304_unresolved_module.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R305_unresolved_role.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R305_unresolved_role.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R306_undefined_variable.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R306_undefined_variable.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R401_list_all_inbound_src.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R401_list_all_inbound_src.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R402_list_all_used_variables.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R402_list_all_used_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R404_show_variables.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R404_show_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/R501_dependency_suggestion.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/R501_dependency_suggestion.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/__init__.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/rule_versions.json` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/rule_versions.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/rules/sample_rule.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/safe_glob.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/safe_glob.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/scanner.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,15 @@
     version: str = ""
     hash: str = ""
 
     source_repository: str = ""
     out_dir: str = ""
 
     include_test_contents: bool = False
+    load_all_taskfiles: bool = False
 
     extra_requirements: list = field(default_factory=list)
     resolve_failures: dict = field(default_factory=dict)
 
     findings: Findings = None
     result: ARIResult = None
 
@@ -545,15 +546,20 @@
                 if self.name in obj_path:
                     self.target_object = obj
                     break
         return
 
     def construct_trees(self, ram_client=None):
         trees, additional, extra_requirements, resolve_failures = tree(
-            self.root_definitions, self.ext_definitions, ram_client, self.target_playbook_name, self.target_taskfile_name
+            self.root_definitions,
+            self.ext_definitions,
+            ram_client,
+            self.target_playbook_name,
+            self.target_taskfile_name,
+            self.load_all_taskfiles,
         )
 
         # set annotation for spec mutations
         if self.spec_mutations_from_previous_scan:
             spec_mutations = self.spec_mutations_from_previous_scan
             for _tree in trees:
                 for callobj in _tree.items:
@@ -790,14 +796,15 @@
         source_repository: str = "",
         playbook_yaml: str = "",
         playbook_only: bool = False,
         taskfile_yaml: str = "",
         taskfile_only: bool = False,
         raw_yaml: str = "",
         include_test_contents: bool = False,
+        load_all_taskfiles: bool = False,
         objects: bool = False,
         out_dir: str = "",
         spec_mutations_from_previous_scan: dict = None,
     ):
         time_records = {}
         self.record_begin(time_records, "scandata_init")
 
@@ -828,14 +835,15 @@
             use_src_cache=use_src_cache,
             source_repository=source_repository,
             playbook_yaml=playbook_yaml,
             playbook_only=playbook_only,
             taskfile_yaml=taskfile_yaml,
             taskfile_only=taskfile_only,
             include_test_contents=include_test_contents,
+            load_all_taskfiles=load_all_taskfiles,
             out_dir=out_dir,
             root_dir=self.root_dir,
             rules_dir=self.rules_dir,
             rules=self.rules,
             rules_cache=self.rules_cache,
             persist_dependency_cache=self.persist_dependency_cache,
             spec_mutations_from_previous_scan=spec_mutations_from_previous_scan,
@@ -934,14 +942,15 @@
                             hash=ext_hash,
                             target_path=ext_target_path,
                             dependency_dir=scandata.dependency_dir,
                             install_dependencies=False,
                             skip_dependency=True,
                             source_repository=scandata.source_repository,
                             include_test_contents=include_test_contents,
+                            load_all_taskfiles=load_all_taskfiles,
                             load_only=True,
                         )
                         dep_scandata = dep_scanner.get_last_scandata()
                         scandata.ext_definitions[key] = dep_scandata.root_definitions
                         dep_loaded = True
 
             self.record_end(time_records, "dependency_load")
@@ -1089,14 +1098,15 @@
                     use_src_cache=use_src_cache,
                     source_repository=source_repository,
                     playbook_yaml=playbook_yaml,
                     playbook_only=playbook_only,
                     taskfile_yaml=taskfile_yaml,
                     taskfile_only=taskfile_only,
                     include_test_contents=include_test_contents,
+                    load_all_taskfiles=load_all_taskfiles,
                     objects=objects,
                     raw_yaml=raw_yaml,
                     out_dir=out_dir,
                     spec_mutations_from_previous_scan=scandata.spec_mutations,
                 )
 
         return scandata.findings.report.get("ari_result", None)
@@ -1165,16 +1175,16 @@
         end = datetime.datetime.utcnow()
         time_records[record_name]["end"] = end.isoformat()
         begin = datetime.datetime.fromisoformat(time_records[record_name]["begin"])
         elapsed = (end - begin).total_seconds()
         time_records[record_name]["elapsed"] = elapsed
 
 
-def tree(root_definitions, ext_definitions, ram_client=None, target_playbook_path=None, target_taskfile_path=None):
-    tl = TreeLoader(root_definitions, ext_definitions, ram_client, target_playbook_path, target_taskfile_path)
+def tree(root_definitions, ext_definitions, ram_client=None, target_playbook_path=None, target_taskfile_path=None, load_all_taskfiles=False):
+    tl = TreeLoader(root_definitions, ext_definitions, ram_client, target_playbook_path, target_taskfile_path, load_all_taskfiles)
     trees, additional = tl.run()
     if trees is None:
         raise ValueError("failed to get trees")
     # if node_objects is None:
     #     raise ValueError("failed to get node_objects")
     return (
         trees,
```

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/tree.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/tree.py`

 * *Files 11% similar despite different names*

```diff
@@ -400,29 +400,36 @@
 def init_builtin_modules():
     builtin_module_dict = load_builtin_modules()
     modules = list(builtin_module_dict.values())
     return modules
 
 
 class TreeLoader(object):
-    def __init__(self, root_definitions, ext_definitions, ram_client=None, target_playbook_path=None, target_taskfile_path=None):
+    def __init__(
+        self, root_definitions, ext_definitions, ram_client=None, target_playbook_path=None, target_taskfile_path=None, load_all_taskfiles=False
+    ):
         self.ram_client: RAMClient = ram_client
 
         # use mappings just to get tree tops (playbook/role)
         # we don't load any files by this mappings here
         self.load_and_mapping = root_definitions.get("mappings", None)
         self.playbook_mappings = self.load_and_mapping.playbooks
         self.role_mappings = self.load_and_mapping.roles
         self.taskfile_mappings = []
 
         if target_playbook_path:
             self.playbook_mappings = [p for p in self.playbook_mappings if p[0] == target_playbook_path]
             self.role_mappings = []
 
-        if target_taskfile_path:
+        # some taskfiles might not be included from `tasks/main.yml` of a role.
+        # ARI does not scan them by default, but it does when `load_all_taskfiles == True`
+        if load_all_taskfiles:
+            self.taskfile_mappings = self.load_and_mapping.taskfiles
+        # or, if the scan is for a single taskfile, ARI just scans it
+        elif target_taskfile_path:
             self.taskfile_mappings = self.load_and_mapping.taskfiles
             self.taskfile_mappings = [tf for tf in self.taskfile_mappings if tf[0] == target_taskfile_path]
             self.playbook_mappings = []
             self.role_mappings = []
 
         # TODO: dependency check, especially for
         # collection dependencies for role
@@ -437,14 +444,15 @@
         self.dicts = make_dicts(self.root_definitions, self.ext_definitions)
 
         self.module_redirects = load_module_redirects(self.root_definitions, self.ext_definitions, self.dicts["modules"])
 
         self.var_manager: VariableManager = VariableManager()
 
         self.target_playbook_path = target_playbook_path
+        self.load_all_taskfiles = load_all_taskfiles
 
         self.module_resolve_cache = {}
         self.role_resolve_cache = {}
         self.taskfile_resolve_cache = {}
 
         self.resolved_module_from_ram = {}
         self.resolved_role_from_ram = {}
@@ -464,27 +472,52 @@
 
     def run(self):
         additional_objects = ObjectList()
         if self.load_and_mapping.target_type == LoadType.PROJECT:
             p_defs = self.org_root_definitions.get("definitions", {}).get("projects", [])
             if len(p_defs) > 0:
                 additional_objects.add(p_defs[0])
+        covered_taskfiles = []
         for i, mapping in enumerate(self.playbook_mappings):
             logger.debug("[{}/{}] {}".format(i + 1, len(self.playbook_mappings), mapping[1]))
             playbook_key = mapping[1]
             tree_objects = self._recursive_get_calls(playbook_key)
             self.trees.append(tree_objects)
+
+            if self.load_all_taskfiles and tree_objects and tree_objects.items:
+                for call_obj in tree_objects.items:
+                    if not isinstance(call_obj, CallObject):
+                        continue
+                    spec_obj = call_obj.spec
+                    if isinstance(spec_obj, TaskFile):
+                        taskfile_key = spec_obj.key
+                        if taskfile_key not in covered_taskfiles:
+                            covered_taskfiles.append(taskfile_key)
+
         for i, mapping in enumerate(self.role_mappings):
             logger.debug("[{}/{}] {}".format(i + 1, len(self.role_mappings), mapping[1]))
             role_key = mapping[1]
             tree_objects = self._recursive_get_calls(role_key)
             self.trees.append(tree_objects)
+
+            if self.load_all_taskfiles and tree_objects and tree_objects.items:
+                for call_obj in tree_objects.items:
+                    if not isinstance(call_obj, CallObject):
+                        continue
+                    spec_obj = call_obj.spec
+                    if isinstance(spec_obj, TaskFile):
+                        taskfile_key = spec_obj.key
+                        if taskfile_key not in covered_taskfiles:
+                            covered_taskfiles.append(taskfile_key)
+
         for i, mapping in enumerate(self.taskfile_mappings):
             logger.debug("[{}/{}] {}".format(i + 1, len(self.taskfile_mappings), mapping[1]))
             taskfile_key = mapping[1]
+            if self.load_all_taskfiles and taskfile_key in covered_taskfiles:
+                continue
             tree_objects = self._recursive_get_calls(taskfile_key)
             self.trees.append(tree_objects)
         return self.trees, additional_objects
 
     def _recursive_get_calls(self, key, caller=None, handover={}, index=0, history=[]):
         obj_list = ObjectList()
         obj = self.get_object(key)
```

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/utils.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -724,16 +724,15 @@
         raise ValueError(f"only dict input is allowed, but got {type(src)}")
 
     if not isinstance(dst, dict):
         raise ValueError(f"only dict input is allowed, but got {type(dst)}")
 
     for k, sv in src.items():
         if isinstance(sv, dict):
-            if k not in dst:
-                dst[k] = {}
+            dst[k] = {}
             recursive_copy_dict(sv, dst[k])
         else:
             dst[k] = deepcopy(sv)
     return
 
 
 def is_test_object(path: str):
```

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/variable_manager.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/variable_manager.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight/yaml.py` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight/yaml.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/ansible_risk_insight.egg-info/SOURCES.txt` & `ansible-risk-insight-0.1.7rc2/ansible_risk_insight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/data-struct.txt` & `ansible-risk-insight-0.1.7rc2/data-struct.txt`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/doc/images/ari-apply-rules.png` & `ansible-risk-insight-0.1.7rc2/doc/images/ari-apply-rules.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/doc/images/ari-arch.png` & `ansible-risk-insight-0.1.7rc2/doc/images/ari-arch.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/doc/images/ari-overview.png` & `ansible-risk-insight-0.1.7rc2/doc/images/ari-overview.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/doc/images/ari-ram-list.png` & `ansible-risk-insight-0.1.7rc2/doc/images/ari-ram-list.png`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/docs/annotation.md` & `ansible-risk-insight-0.1.7rc2/docs/annotation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/docs/customize_rules.md` & `ansible-risk-insight-0.1.7rc2/docs/customize_rules.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/docs/rules/R103_download_exec.md` & `ansible-risk-insight-0.1.7rc2/docs/rules/R103_download_exec.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/docs/rules/R104_unauthorized_download_src.md` & `ansible-risk-insight-0.1.7rc2/docs/rules/R104_unauthorized_download_src.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/docs/rules/R107_pkg_install_with_insecure_option.md` & `ansible-risk-insight-0.1.7rc2/docs/rules/R107_pkg_install_with_insecure_option.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/docs/rules/R108_privilege_escalation.md` & `ansible-risk-insight-0.1.7rc2/docs/rules/R108_privilege_escalation.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/example/readme.md` & `ansible-risk-insight-0.1.7rc2/example/readme.md`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/example/rules/sample_rule.py` & `ansible-risk-insight-0.1.7rc2/example/rules/sample_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/example/sample.py` & `ansible-risk-insight-0.1.7rc2/example/sample.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/mkdocs.yml` & `ansible-risk-insight-0.1.7rc2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/pyproject.toml` & `ansible-risk-insight-0.1.7rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/test/test_scanner.py` & `ansible-risk-insight-0.1.7rc2/test/test_scanner.py`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/test/testdata/projects/my.collection/MANIFEST.json` & `ansible-risk-insight-0.1.7rc2/test/testdata/projects/my.collection/MANIFEST.json`

 * *Files identical despite different names*

### Comparing `ansible-risk-insight-0.1.7rc1/tox.ini` & `ansible-risk-insight-0.1.7rc2/tox.ini`

 * *Files identical despite different names*

