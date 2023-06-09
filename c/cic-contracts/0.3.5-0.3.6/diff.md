# Comparing `tmp/cic-contracts-0.3.5.tar.gz` & `tmp/cic-contracts-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cic-contracts-0.3.5.tar", last modified: Thu Jun  8 15:06:18 2023, max compression
+gzip compressed data, was "dist/cic-contracts-0.3.6.tar", last modified: Thu Jun  8 15:56:26 2023, max compression
```

## Comparing `cic-contracts-0.3.5.tar` & `cic-contracts-0.3.6.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.363323 cic-contracts-0.3.5/
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-04-29 14:00:22.000000 cic-contracts-0.3.5/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       87 2023-06-08 08:11:27.000000 cic-contracts-0.3.5/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)    26461 2023-06-08 15:06:18.363323 cic-contracts-0.3.5/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)    25714 2023-06-08 07:22:38.000000 cic-contracts-0.3.5/README.md
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.353323 cic-contracts-0.3.5/cic_contracts/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-06-08 12:53:10.000000 cic-contracts-0.3.5/cic_contracts/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3542 2022-04-29 14:00:22.000000 cic-contracts-0.3.5/cic_contracts/accounts_index.py
--rw-r--r--   0 lash      (1000) lash      (1000)      671 2022-04-29 14:00:22.000000 cic-contracts-0.3.5/cic_contracts/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     9153 2022-04-29 14:00:22.000000 cic-contracts-0.3.5/cic_contracts/erc20.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3722 2022-04-29 14:00:22.000000 cic-contracts-0.3.5/cic_contracts/registry.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.356656 cic-contracts-0.3.5/cic_contracts/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)      303 2023-06-08 12:53:05.000000 cic-contracts-0.3.5/cic_contracts/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      617 2023-02-24 10:28:52.000000 cic-contracts-0.3.5/cic_contracts/unittest/owned.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.356656 cic-contracts-0.3.5/cic_contracts/unittest/solidity/
--rw-r--r--   0 lash      (1000) lash      (1000)     3592 2023-06-08 15:04:59.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/BurnerTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     1098 2023-06-06 16:40:27.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/BurnerTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     2048 2023-06-08 15:04:59.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/CappedTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      637 2023-06-06 12:47:42.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/CappedTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     2600 2023-06-08 15:05:00.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/ExpireTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      979 2023-06-08 14:58:25.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/ExpireTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     3302 2023-06-08 15:05:00.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/MinterTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      963 2023-06-06 13:56:23.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/MinterTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     1780 2023-06-08 15:05:00.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/SealTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      611 2023-06-08 07:04:28.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/SealTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     2548 2023-06-08 15:05:00.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/WriterTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      790 2023-06-06 17:14:40.000000 cic-contracts-0.3.5/cic_contracts/unittest/solidity/WriterTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)      595 2022-04-29 14:00:22.000000 cic-contracts-0.3.5/cic_contracts/writer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.356656 cic-contracts-0.3.5/cic_contracts.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)    26461 2023-06-08 15:06:18.000000 cic-contracts-0.3.5/cic_contracts.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1986 2023-06-08 15:06:18.000000 cic-contracts-0.3.5/cic_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-08 15:06:18.000000 cic-contracts-0.3.5/cic_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-08 15:06:18.000000 cic-contracts-0.3.5/cic_contracts.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       78 2023-06-08 15:06:18.000000 cic-contracts-0.3.5/cic_contracts.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.356656 cic-contracts-0.3.5/eth_burner/
--rw-r--r--   0 lash      (1000) lash      (1000)       28 2023-06-06 16:42:08.000000 cic-contracts-0.3.5/eth_burner/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1166 2023-06-06 16:42:28.000000 cic-contracts-0.3.5/eth_burner/burn.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.356656 cic-contracts-0.3.5/eth_burner/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 16:41:44.000000 cic-contracts-0.3.5/eth_burner/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1509 2023-06-08 12:58:24.000000 cic-contracts-0.3.5/eth_burner/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      613 2023-06-08 13:23:00.000000 cic-contracts-0.3.5/eth_burner/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_capped/
--rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:39:42.000000 cic-contracts-0.3.5/eth_capped/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      799 2023-06-06 08:39:35.000000 cic-contracts-0.3.5/eth_capped/capped.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_capped/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 12:09:11.000000 cic-contracts-0.3.5/eth_capped/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2091 2023-06-08 13:25:50.000000 cic-contracts-0.3.5/eth_capped/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1069 2023-06-08 13:32:19.000000 cic-contracts-0.3.5/eth_capped/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_expire/
--rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:31:55.000000 cic-contracts-0.3.5/eth_expire/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1309 2023-06-06 08:31:55.000000 cic-contracts-0.3.5/eth_expire/expire.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_expire/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 13:21:21.000000 cic-contracts-0.3.5/eth_expire/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2226 2023-06-08 14:46:09.000000 cic-contracts-0.3.5/eth_expire/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1005 2023-06-08 14:54:26.000000 cic-contracts-0.3.5/eth_expire/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_minter/
--rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 14:19:41.000000 cic-contracts-0.3.5/eth_minter/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      921 2023-06-06 14:24:42.000000 cic-contracts-0.3.5/eth_minter/minter.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_minter/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 14:19:49.000000 cic-contracts-0.3.5/eth_minter/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1555 2023-06-08 12:57:48.000000 cic-contracts-0.3.5/eth_minter/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      618 2023-06-06 14:26:59.000000 cic-contracts-0.3.5/eth_minter/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_seal/
--rw-r--r--   0 lash      (1000) lash      (1000)       26 2023-06-08 07:02:02.000000 cic-contracts-0.3.5/eth_seal/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1282 2023-06-08 06:50:18.000000 cic-contracts-0.3.5/eth_seal/seal.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_seal/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       44 2023-06-08 07:02:18.000000 cic-contracts-0.3.5/eth_seal/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2006 2023-06-08 12:57:46.000000 cic-contracts-0.3.5/eth_seal/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      502 2023-06-08 07:00:50.000000 cic-contracts-0.3.5/eth_seal/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.359989 cic-contracts-0.3.5/eth_writer/
--rw-r--r--   0 lash      (1000) lash      (1000)       25 2023-06-06 08:29:33.000000 cic-contracts-0.3.5/eth_writer/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1753 2023-06-06 08:29:33.000000 cic-contracts-0.3.5/eth_writer/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.363323 cic-contracts-0.3.5/eth_writer/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 17:01:25.000000 cic-contracts-0.3.5/eth_writer/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1908 2023-06-08 12:59:05.000000 cic-contracts-0.3.5/eth_writer/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1650 2023-06-06 17:11:14.000000 cic-contracts-0.3.5/eth_writer/unittest/interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-06 08:27:06.000000 cic-contracts-0.3.5/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      962 2023-06-08 15:06:18.363323 cic-contracts-0.3.5/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      650 2023-06-08 07:21:42.000000 cic-contracts-0.3.5/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       75 2023-06-06 13:03:05.000000 cic-contracts-0.3.5/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:06:18.363323 cic-contracts-0.3.5/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 16:41:18.000000 cic-contracts-0.3.5/tests/test_burner.py
--rw-r--r--   0 lash      (1000) lash      (1000)      770 2023-06-08 13:23:46.000000 cic-contracts-0.3.5/tests/test_capped.py
--rw-r--r--   0 lash      (1000) lash      (1000)      766 2023-06-08 14:56:41.000000 cic-contracts-0.3.5/tests/test_expire.py
--rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 14:12:58.000000 cic-contracts-0.3.5/tests/test_minter.py
--rw-r--r--   0 lash      (1000) lash      (1000)      740 2023-06-08 07:03:56.000000 cic-contracts-0.3.5/tests/test_seal.py
--rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 17:06:53.000000 cic-contracts-0.3.5/tests/test_writer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.783304 cic-contracts-0.3.6/
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-04-29 14:00:22.000000 cic-contracts-0.3.6/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       87 2023-06-08 08:11:27.000000 cic-contracts-0.3.6/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)    26461 2023-06-08 15:56:26.783304 cic-contracts-0.3.6/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)    25714 2023-06-08 07:22:38.000000 cic-contracts-0.3.6/README.md
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.773304 cic-contracts-0.3.6/cic_contracts/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-06-08 12:53:10.000000 cic-contracts-0.3.6/cic_contracts/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3542 2022-04-29 14:00:22.000000 cic-contracts-0.3.6/cic_contracts/accounts_index.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      671 2022-04-29 14:00:22.000000 cic-contracts-0.3.6/cic_contracts/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     9153 2022-04-29 14:00:22.000000 cic-contracts-0.3.6/cic_contracts/erc20.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3722 2022-04-29 14:00:22.000000 cic-contracts-0.3.6/cic_contracts/registry.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.776638 cic-contracts-0.3.6/cic_contracts/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)      303 2023-06-08 12:53:05.000000 cic-contracts-0.3.6/cic_contracts/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      617 2023-02-24 10:28:52.000000 cic-contracts-0.3.6/cic_contracts/unittest/owned.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.776638 cic-contracts-0.3.6/cic_contracts/unittest/solidity/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3592 2023-06-08 15:04:59.000000 cic-contracts-0.3.6/cic_contracts/unittest/solidity/BurnerTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1098 2023-06-06 16:40:27.000000 cic-contracts-0.3.6/cic_contracts/unittest/solidity/BurnerTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     2048 2023-06-08 15:04:59.000000 cic-contracts-0.3.6/cic_contracts/unittest/solidity/CappedTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      637 2023-06-06 12:47:42.000000 cic-contracts-0.3.6/cic_contracts/unittest/solidity/CappedTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     2600 2023-06-08 15:05:00.000000 cic-contracts-0.3.6/cic_contracts/unittest/solidity/ExpireTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      979 2023-06-08 14:58:25.000000 cic-contracts-0.3.6/cic_contracts/unittest/solidity/ExpireTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     3302 2023-06-08 15:05:00.000000 cic-contracts-0.3.6/cic_contracts/unittest/solidity/MinterTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      963 2023-06-06 13:56:23.000000 cic-contracts-0.3.6/cic_contracts/unittest/solidity/MinterTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     1780 2023-06-08 15:05:00.000000 cic-contracts-0.3.6/cic_contracts/unittest/solidity/SealTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      611 2023-06-08 07:04:28.000000 cic-contracts-0.3.6/cic_contracts/unittest/solidity/SealTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     2548 2023-06-08 15:05:00.000000 cic-contracts-0.3.6/cic_contracts/unittest/solidity/WriterTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      790 2023-06-06 17:14:40.000000 cic-contracts-0.3.6/cic_contracts/unittest/solidity/WriterTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)      595 2022-04-29 14:00:22.000000 cic-contracts-0.3.6/cic_contracts/writer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.773304 cic-contracts-0.3.6/cic_contracts.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)    26461 2023-06-08 15:56:26.000000 cic-contracts-0.3.6/cic_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1986 2023-06-08 15:56:26.000000 cic-contracts-0.3.6/cic_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-08 15:56:26.000000 cic-contracts-0.3.6/cic_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-08 15:56:26.000000 cic-contracts-0.3.6/cic_contracts.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       78 2023-06-08 15:56:26.000000 cic-contracts-0.3.6/cic_contracts.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.776638 cic-contracts-0.3.6/eth_burner/
+-rw-r--r--   0 lash      (1000) lash      (1000)       28 2023-06-06 16:42:08.000000 cic-contracts-0.3.6/eth_burner/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1166 2023-06-06 16:42:28.000000 cic-contracts-0.3.6/eth_burner/burn.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.776638 cic-contracts-0.3.6/eth_burner/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 16:41:44.000000 cic-contracts-0.3.6/eth_burner/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1509 2023-06-08 12:58:24.000000 cic-contracts-0.3.6/eth_burner/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      613 2023-06-08 13:23:00.000000 cic-contracts-0.3.6/eth_burner/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.776638 cic-contracts-0.3.6/eth_capped/
+-rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:39:42.000000 cic-contracts-0.3.6/eth_capped/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      799 2023-06-06 08:39:35.000000 cic-contracts-0.3.6/eth_capped/capped.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.776638 cic-contracts-0.3.6/eth_capped/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 12:09:11.000000 cic-contracts-0.3.6/eth_capped/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2091 2023-06-08 13:25:50.000000 cic-contracts-0.3.6/eth_capped/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1069 2023-06-08 13:32:19.000000 cic-contracts-0.3.6/eth_capped/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.779971 cic-contracts-0.3.6/eth_expire/
+-rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:31:55.000000 cic-contracts-0.3.6/eth_expire/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1309 2023-06-06 08:31:55.000000 cic-contracts-0.3.6/eth_expire/expire.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.779971 cic-contracts-0.3.6/eth_expire/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 13:21:21.000000 cic-contracts-0.3.6/eth_expire/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2226 2023-06-08 14:46:09.000000 cic-contracts-0.3.6/eth_expire/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1005 2023-06-08 14:54:26.000000 cic-contracts-0.3.6/eth_expire/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.779971 cic-contracts-0.3.6/eth_minter/
+-rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 14:19:41.000000 cic-contracts-0.3.6/eth_minter/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      921 2023-06-06 14:24:42.000000 cic-contracts-0.3.6/eth_minter/minter.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.779971 cic-contracts-0.3.6/eth_minter/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 14:19:49.000000 cic-contracts-0.3.6/eth_minter/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1555 2023-06-08 12:57:48.000000 cic-contracts-0.3.6/eth_minter/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      618 2023-06-06 14:26:59.000000 cic-contracts-0.3.6/eth_minter/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.779971 cic-contracts-0.3.6/eth_seal/
+-rw-r--r--   0 lash      (1000) lash      (1000)       26 2023-06-08 07:02:02.000000 cic-contracts-0.3.6/eth_seal/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1282 2023-06-08 06:50:18.000000 cic-contracts-0.3.6/eth_seal/seal.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.779971 cic-contracts-0.3.6/eth_seal/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       44 2023-06-08 07:02:18.000000 cic-contracts-0.3.6/eth_seal/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2006 2023-06-08 12:57:46.000000 cic-contracts-0.3.6/eth_seal/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1072 2023-06-08 15:41:19.000000 cic-contracts-0.3.6/eth_seal/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.779971 cic-contracts-0.3.6/eth_writer/
+-rw-r--r--   0 lash      (1000) lash      (1000)       25 2023-06-06 08:29:33.000000 cic-contracts-0.3.6/eth_writer/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1753 2023-06-06 08:29:33.000000 cic-contracts-0.3.6/eth_writer/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.779971 cic-contracts-0.3.6/eth_writer/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 17:01:25.000000 cic-contracts-0.3.6/eth_writer/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1908 2023-06-08 12:59:05.000000 cic-contracts-0.3.6/eth_writer/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1650 2023-06-06 17:11:14.000000 cic-contracts-0.3.6/eth_writer/unittest/interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-06 08:27:06.000000 cic-contracts-0.3.6/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      962 2023-06-08 15:56:26.783304 cic-contracts-0.3.6/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      650 2023-06-08 07:21:42.000000 cic-contracts-0.3.6/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       75 2023-06-06 13:03:05.000000 cic-contracts-0.3.6/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-08 15:56:26.783304 cic-contracts-0.3.6/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 16:41:18.000000 cic-contracts-0.3.6/tests/test_burner.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      770 2023-06-08 13:23:46.000000 cic-contracts-0.3.6/tests/test_capped.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      766 2023-06-08 14:56:41.000000 cic-contracts-0.3.6/tests/test_expire.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 14:12:58.000000 cic-contracts-0.3.6/tests/test_minter.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      740 2023-06-08 07:03:56.000000 cic-contracts-0.3.6/tests/test_seal.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 17:06:53.000000 cic-contracts-0.3.6/tests/test_writer.py
```

### Comparing `cic-contracts-0.3.5/LICENSE` & `cic-contracts-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/PKG-INFO` & `cic-contracts-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cic-contracts
-Version: 0.3.5
+Version: 0.3.6
 Summary: CIC network smart contract interfaces
 Home-page: https://gitlab.com/cicnet/cic-contracts
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPL3
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cic-contracts-0.3.5/README.md` & `cic-contracts-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/accounts_index.py` & `cic-contracts-0.3.6/cic_contracts/accounts_index.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/base.py` & `cic-contracts-0.3.6/cic_contracts/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/erc20.py` & `cic-contracts-0.3.6/cic_contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/registry.py` & `cic-contracts-0.3.6/cic_contracts/registry.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/unittest/owned.py` & `cic-contracts-0.3.6/cic_contracts/unittest/owned.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/unittest/solidity/BurnerTest.bin` & `cic-contracts-0.3.6/cic_contracts/unittest/solidity/BurnerTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/unittest/solidity/BurnerTest.sol` & `cic-contracts-0.3.6/cic_contracts/unittest/solidity/BurnerTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/unittest/solidity/CappedTest.bin` & `cic-contracts-0.3.6/cic_contracts/unittest/solidity/CappedTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/unittest/solidity/CappedTest.sol` & `cic-contracts-0.3.6/cic_contracts/unittest/solidity/CappedTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/unittest/solidity/ExpireTest.bin` & `cic-contracts-0.3.6/cic_contracts/unittest/solidity/ExpireTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/unittest/solidity/ExpireTest.sol` & `cic-contracts-0.3.6/cic_contracts/unittest/solidity/ExpireTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/unittest/solidity/MinterTest.bin` & `cic-contracts-0.3.6/cic_contracts/unittest/solidity/MinterTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/unittest/solidity/MinterTest.sol` & `cic-contracts-0.3.6/cic_contracts/unittest/solidity/MinterTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/unittest/solidity/SealTest.bin` & `cic-contracts-0.3.6/cic_contracts/unittest/solidity/SealTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/unittest/solidity/SealTest.sol` & `cic-contracts-0.3.6/cic_contracts/unittest/solidity/SealTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/unittest/solidity/WriterTest.bin` & `cic-contracts-0.3.6/cic_contracts/unittest/solidity/WriterTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/unittest/solidity/WriterTest.sol` & `cic-contracts-0.3.6/cic_contracts/unittest/solidity/WriterTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts/writer.py` & `cic-contracts-0.3.6/cic_contracts/writer.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/cic_contracts.egg-info/PKG-INFO` & `cic-contracts-0.3.6/cic_contracts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cic-contracts
-Version: 0.3.5
+Version: 0.3.6
 Summary: CIC network smart contract interfaces
 Home-page: https://gitlab.com/cicnet/cic-contracts
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPL3
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cic-contracts-0.3.5/cic_contracts.egg-info/SOURCES.txt` & `cic-contracts-0.3.6/cic_contracts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_burner/burn.py` & `cic-contracts-0.3.6/eth_burner/burn.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_burner/unittest/base.py` & `cic-contracts-0.3.6/eth_burner/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_burner/unittest/interface.py` & `cic-contracts-0.3.6/eth_burner/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_capped/capped.py` & `cic-contracts-0.3.6/eth_capped/capped.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_capped/unittest/base.py` & `cic-contracts-0.3.6/eth_capped/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_capped/unittest/interface.py` & `cic-contracts-0.3.6/eth_capped/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_expire/expire.py` & `cic-contracts-0.3.6/eth_expire/expire.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_expire/unittest/base.py` & `cic-contracts-0.3.6/eth_expire/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_expire/unittest/interface.py` & `cic-contracts-0.3.6/eth_expire/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_minter/minter.py` & `cic-contracts-0.3.6/eth_minter/minter.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_minter/unittest/base.py` & `cic-contracts-0.3.6/eth_minter/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_minter/unittest/interface.py` & `cic-contracts-0.3.6/eth_minter/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_seal/seal.py` & `cic-contracts-0.3.6/eth_seal/seal.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_seal/unittest/base.py` & `cic-contracts-0.3.6/eth_seal/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_writer/interface.py` & `cic-contracts-0.3.6/eth_writer/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_writer/unittest/base.py` & `cic-contracts-0.3.6/eth_writer/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/eth_writer/unittest/interface.py` & `cic-contracts-0.3.6/eth_writer/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/setup.cfg` & `cic-contracts-0.3.6/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cic-contracts
-version = 0.3.5
+version = 0.3.6
 description = CIC network smart contract interfaces
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://gitlab.com/cicnet/cic-contracts
 keywords = 
 	dlt
 	blockchain
```

### Comparing `cic-contracts-0.3.5/setup.py` & `cic-contracts-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/tests/test_burner.py` & `cic-contracts-0.3.6/tests/test_burner.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/tests/test_capped.py` & `cic-contracts-0.3.6/tests/test_capped.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/tests/test_expire.py` & `cic-contracts-0.3.6/tests/test_expire.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/tests/test_minter.py` & `cic-contracts-0.3.6/tests/test_minter.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/tests/test_seal.py` & `cic-contracts-0.3.6/tests/test_seal.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.5/tests/test_writer.py` & `cic-contracts-0.3.6/tests/test_writer.py`

 * *Files identical despite different names*

