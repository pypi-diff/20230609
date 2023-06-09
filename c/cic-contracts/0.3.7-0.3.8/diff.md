# Comparing `tmp/cic-contracts-0.3.7.tar.gz` & `tmp/cic-contracts-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cic-contracts-0.3.7.tar", last modified: Fri Jun  9 08:44:15 2023, max compression
+gzip compressed data, was "dist/cic-contracts-0.3.8.tar", last modified: Fri Jun  9 08:46:19 2023, max compression
```

## Comparing `cic-contracts-0.3.7.tar` & `cic-contracts-0.3.8.tar`

### file list

```diff
@@ -1,91 +1,157 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.156640 cic-contracts-0.3.7/
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-04-29 14:00:22.000000 cic-contracts-0.3.7/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       87 2023-06-08 08:11:27.000000 cic-contracts-0.3.7/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)    26467 2023-06-09 08:44:15.156640 cic-contracts-0.3.7/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)    25714 2023-06-08 07:22:38.000000 cic-contracts-0.3.7/README.md
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.146640 cic-contracts-0.3.7/cic_contracts/
--rw-r--r--   0 lash      (1000) lash      (1000)      160 2023-06-09 08:32:05.000000 cic-contracts-0.3.7/cic_contracts/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3542 2022-04-29 14:00:22.000000 cic-contracts-0.3.7/cic_contracts/accounts_index.py
--rw-r--r--   0 lash      (1000) lash      (1000)      671 2022-04-29 14:00:22.000000 cic-contracts-0.3.7/cic_contracts/base.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.149973 cic-contracts-0.3.7/cic_contracts/data/
--rw-r--r--   0 lash      (1000) lash      (1000)       85 2023-06-09 08:04:14.000000 cic-contracts-0.3.7/cic_contracts/data/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     9153 2022-04-29 14:00:22.000000 cic-contracts-0.3.7/cic_contracts/erc20.py
--rw-r--r--   0 lash      (1000) lash      (1000)      183 2023-06-09 07:58:31.000000 cic-contracts-0.3.7/cic_contracts/names.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3722 2022-04-29 14:00:22.000000 cic-contracts-0.3.7/cic_contracts/registry.py
--rw-r--r--   0 lash      (1000) lash      (1000)      350 2023-06-09 08:24:11.000000 cic-contracts-0.3.7/cic_contracts/search.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.149973 cic-contracts-0.3.7/cic_contracts/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)      380 2023-06-09 08:32:53.000000 cic-contracts-0.3.7/cic_contracts/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      617 2023-02-24 10:28:52.000000 cic-contracts-0.3.7/cic_contracts/unittest/owned.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.149973 cic-contracts-0.3.7/cic_contracts/unittest/solidity/
--rw-r--r--   0 lash      (1000) lash      (1000)     3592 2023-06-08 15:04:59.000000 cic-contracts-0.3.7/cic_contracts/unittest/solidity/BurnerTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     1098 2023-06-06 16:40:27.000000 cic-contracts-0.3.7/cic_contracts/unittest/solidity/BurnerTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     2048 2023-06-08 15:04:59.000000 cic-contracts-0.3.7/cic_contracts/unittest/solidity/CappedTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      637 2023-06-06 12:47:42.000000 cic-contracts-0.3.7/cic_contracts/unittest/solidity/CappedTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     2600 2023-06-08 15:05:00.000000 cic-contracts-0.3.7/cic_contracts/unittest/solidity/ExpireTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      979 2023-06-08 14:58:25.000000 cic-contracts-0.3.7/cic_contracts/unittest/solidity/ExpireTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     3302 2023-06-08 15:05:00.000000 cic-contracts-0.3.7/cic_contracts/unittest/solidity/MinterTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      963 2023-06-06 13:56:23.000000 cic-contracts-0.3.7/cic_contracts/unittest/solidity/MinterTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     1784 2023-06-09 08:41:43.000000 cic-contracts-0.3.7/cic_contracts/unittest/solidity/SealTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      615 2023-06-09 08:41:39.000000 cic-contracts-0.3.7/cic_contracts/unittest/solidity/SealTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)     2548 2023-06-08 15:05:00.000000 cic-contracts-0.3.7/cic_contracts/unittest/solidity/WriterTest.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      790 2023-06-06 17:14:40.000000 cic-contracts-0.3.7/cic_contracts/unittest/solidity/WriterTest.sol
--rw-r--r--   0 lash      (1000) lash      (1000)      595 2022-04-29 14:00:22.000000 cic-contracts-0.3.7/cic_contracts/writer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.149973 cic-contracts-0.3.7/cic_contracts.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)    26467 2023-06-09 08:44:15.000000 cic-contracts-0.3.7/cic_contracts.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     2064 2023-06-09 08:44:15.000000 cic-contracts-0.3.7/cic_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-09 08:44:15.000000 cic-contracts-0.3.7/cic_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-09 08:44:15.000000 cic-contracts-0.3.7/cic_contracts.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       78 2023-06-09 08:44:15.000000 cic-contracts-0.3.7/cic_contracts.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.149973 cic-contracts-0.3.7/eth_burner/
--rw-r--r--   0 lash      (1000) lash      (1000)       28 2023-06-06 16:42:08.000000 cic-contracts-0.3.7/eth_burner/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1166 2023-06-06 16:42:28.000000 cic-contracts-0.3.7/eth_burner/burn.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.149973 cic-contracts-0.3.7/eth_burner/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 16:41:44.000000 cic-contracts-0.3.7/eth_burner/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1543 2023-06-09 08:31:16.000000 cic-contracts-0.3.7/eth_burner/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      613 2023-06-08 13:23:00.000000 cic-contracts-0.3.7/eth_burner/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.149973 cic-contracts-0.3.7/eth_capped/
--rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:39:42.000000 cic-contracts-0.3.7/eth_capped/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      799 2023-06-06 08:39:35.000000 cic-contracts-0.3.7/eth_capped/capped.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.153307 cic-contracts-0.3.7/eth_capped/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 12:09:11.000000 cic-contracts-0.3.7/eth_capped/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2125 2023-06-09 08:31:15.000000 cic-contracts-0.3.7/eth_capped/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1069 2023-06-08 13:32:19.000000 cic-contracts-0.3.7/eth_capped/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.153307 cic-contracts-0.3.7/eth_expire/
--rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:31:55.000000 cic-contracts-0.3.7/eth_expire/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1309 2023-06-06 08:31:55.000000 cic-contracts-0.3.7/eth_expire/expire.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.153307 cic-contracts-0.3.7/eth_expire/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 13:21:21.000000 cic-contracts-0.3.7/eth_expire/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2260 2023-06-09 08:33:27.000000 cic-contracts-0.3.7/eth_expire/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1005 2023-06-08 14:54:26.000000 cic-contracts-0.3.7/eth_expire/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.153307 cic-contracts-0.3.7/eth_minter/
--rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 14:19:41.000000 cic-contracts-0.3.7/eth_minter/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      921 2023-06-06 14:24:42.000000 cic-contracts-0.3.7/eth_minter/minter.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.153307 cic-contracts-0.3.7/eth_minter/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 14:19:49.000000 cic-contracts-0.3.7/eth_minter/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1589 2023-06-09 08:34:35.000000 cic-contracts-0.3.7/eth_minter/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      618 2023-06-06 14:26:59.000000 cic-contracts-0.3.7/eth_minter/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.153307 cic-contracts-0.3.7/eth_seal/
--rw-r--r--   0 lash      (1000) lash      (1000)       26 2023-06-08 07:02:02.000000 cic-contracts-0.3.7/eth_seal/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1282 2023-06-08 06:50:18.000000 cic-contracts-0.3.7/eth_seal/seal.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.153307 cic-contracts-0.3.7/eth_seal/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       44 2023-06-08 07:02:18.000000 cic-contracts-0.3.7/eth_seal/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2086 2023-06-09 08:38:00.000000 cic-contracts-0.3.7/eth_seal/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1072 2023-06-08 15:41:19.000000 cic-contracts-0.3.7/eth_seal/unittest/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.153307 cic-contracts-0.3.7/eth_writer/
--rw-r--r--   0 lash      (1000) lash      (1000)       25 2023-06-06 08:29:33.000000 cic-contracts-0.3.7/eth_writer/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1753 2023-06-06 08:29:33.000000 cic-contracts-0.3.7/eth_writer/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.153307 cic-contracts-0.3.7/eth_writer/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 17:01:25.000000 cic-contracts-0.3.7/eth_writer/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1942 2023-06-09 08:34:01.000000 cic-contracts-0.3.7/eth_writer/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1650 2023-06-06 17:11:14.000000 cic-contracts-0.3.7/eth_writer/unittest/interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-06 08:27:06.000000 cic-contracts-0.3.7/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      987 2023-06-09 08:44:15.156640 cic-contracts-0.3.7/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      650 2023-06-08 07:21:42.000000 cic-contracts-0.3.7/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       75 2023-06-06 13:03:05.000000 cic-contracts-0.3.7/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:44:15.156640 cic-contracts-0.3.7/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 16:41:18.000000 cic-contracts-0.3.7/tests/test_burner.py
--rw-r--r--   0 lash      (1000) lash      (1000)      770 2023-06-08 13:23:46.000000 cic-contracts-0.3.7/tests/test_capped.py
--rw-r--r--   0 lash      (1000) lash      (1000)      766 2023-06-08 14:56:41.000000 cic-contracts-0.3.7/tests/test_expire.py
--rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 14:12:58.000000 cic-contracts-0.3.7/tests/test_minter.py
--rw-r--r--   0 lash      (1000) lash      (1000)      740 2023-06-08 07:03:56.000000 cic-contracts-0.3.7/tests/test_seal.py
--rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 17:06:53.000000 cic-contracts-0.3.7/tests/test_writer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.363306 cic-contracts-0.3.8/
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-04-29 14:00:22.000000 cic-contracts-0.3.8/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      108 2023-06-09 08:46:07.000000 cic-contracts-0.3.8/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)    26467 2023-06-09 08:46:19.363306 cic-contracts-0.3.8/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)    25714 2023-06-08 07:22:38.000000 cic-contracts-0.3.8/README.md
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.346639 cic-contracts-0.3.8/cic_contracts/
+-rw-r--r--   0 lash      (1000) lash      (1000)      160 2023-06-09 08:32:05.000000 cic-contracts-0.3.8/cic_contracts/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3542 2022-04-29 14:00:22.000000 cic-contracts-0.3.8/cic_contracts/accounts_index.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      671 2022-04-29 14:00:22.000000 cic-contracts-0.3.8/cic_contracts/base.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.356639 cic-contracts-0.3.8/cic_contracts/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/AccountsIndex.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)     1118 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/AccountsIndex.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/AccountsIndexMutable.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)     1137 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/AccountsIndexMutable.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Burner.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)     1119 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Burner.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Capped.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      362 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Capped.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Chrono.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      204 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Chrono.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Declarator.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)     2554 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Declarator.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Digest.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      822 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Digest.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC165.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      201 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC165.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC173.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      581 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC173.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC20.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)     2440 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC20.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC5007.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      396 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC5007.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC5192.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      475 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC5192.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC5679Ext20.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      528 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC5679Ext20.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC5679Ext721.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      524 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC5679Ext721.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC721.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)     3066 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC721.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC721Enumerable.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      621 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC721Enumerable.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC721Metadata.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      486 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC721Metadata.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC721Receiver.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      393 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/ERC721Receiver.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Expire.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      670 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Expire.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Faucet.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)     1706 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Faucet.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Locator.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      382 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Locator.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Minter.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)     1099 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Minter.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Msg.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      272 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Msg.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/MultiHash.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      992 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/MultiHash.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Offline.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      793 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Offline.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/OwnedAccepter.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      144 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/OwnedAccepter.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/OwnedTaker.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      349 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/OwnedTaker.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Registry.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      489 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Registry.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/RegistryClient.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      758 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/RegistryClient.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Seal.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      509 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Seal.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/TokenVend.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      713 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/TokenVend.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/TokenVote.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)     3011 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/TokenVote.json
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Writer.interface
+-rw-r--r--   0 lash      (1000) lash      (1000)      894 2023-06-09 08:27:37.000000 cic-contracts-0.3.8/cic_contracts/data/Writer.json
+-rw-r--r--   0 lash      (1000) lash      (1000)       85 2023-06-09 08:04:14.000000 cic-contracts-0.3.8/cic_contracts/data/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     9153 2022-04-29 14:00:22.000000 cic-contracts-0.3.8/cic_contracts/erc20.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      183 2023-06-09 07:58:31.000000 cic-contracts-0.3.8/cic_contracts/names.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3722 2022-04-29 14:00:22.000000 cic-contracts-0.3.8/cic_contracts/registry.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      350 2023-06-09 08:24:11.000000 cic-contracts-0.3.8/cic_contracts/search.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.356639 cic-contracts-0.3.8/cic_contracts/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)      380 2023-06-09 08:32:53.000000 cic-contracts-0.3.8/cic_contracts/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      617 2023-02-24 10:28:52.000000 cic-contracts-0.3.8/cic_contracts/unittest/owned.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.356639 cic-contracts-0.3.8/cic_contracts/unittest/solidity/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3592 2023-06-08 15:04:59.000000 cic-contracts-0.3.8/cic_contracts/unittest/solidity/BurnerTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1098 2023-06-06 16:40:27.000000 cic-contracts-0.3.8/cic_contracts/unittest/solidity/BurnerTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     2048 2023-06-08 15:04:59.000000 cic-contracts-0.3.8/cic_contracts/unittest/solidity/CappedTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      637 2023-06-06 12:47:42.000000 cic-contracts-0.3.8/cic_contracts/unittest/solidity/CappedTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     2600 2023-06-08 15:05:00.000000 cic-contracts-0.3.8/cic_contracts/unittest/solidity/ExpireTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      979 2023-06-08 14:58:25.000000 cic-contracts-0.3.8/cic_contracts/unittest/solidity/ExpireTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     3302 2023-06-08 15:05:00.000000 cic-contracts-0.3.8/cic_contracts/unittest/solidity/MinterTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      963 2023-06-06 13:56:23.000000 cic-contracts-0.3.8/cic_contracts/unittest/solidity/MinterTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     1784 2023-06-09 08:41:43.000000 cic-contracts-0.3.8/cic_contracts/unittest/solidity/SealTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      615 2023-06-09 08:41:39.000000 cic-contracts-0.3.8/cic_contracts/unittest/solidity/SealTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)     2548 2023-06-08 15:05:00.000000 cic-contracts-0.3.8/cic_contracts/unittest/solidity/WriterTest.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      790 2023-06-06 17:14:40.000000 cic-contracts-0.3.8/cic_contracts/unittest/solidity/WriterTest.sol
+-rw-r--r--   0 lash      (1000) lash      (1000)      595 2022-04-29 14:00:22.000000 cic-contracts-0.3.8/cic_contracts/writer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.346639 cic-contracts-0.3.8/cic_contracts.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)    26467 2023-06-09 08:46:19.000000 cic-contracts-0.3.8/cic_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     4459 2023-06-09 08:46:19.000000 cic-contracts-0.3.8/cic_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-09 08:46:19.000000 cic-contracts-0.3.8/cic_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-09 08:46:19.000000 cic-contracts-0.3.8/cic_contracts.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       78 2023-06-09 08:46:19.000000 cic-contracts-0.3.8/cic_contracts.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.356639 cic-contracts-0.3.8/eth_burner/
+-rw-r--r--   0 lash      (1000) lash      (1000)       28 2023-06-06 16:42:08.000000 cic-contracts-0.3.8/eth_burner/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1166 2023-06-06 16:42:28.000000 cic-contracts-0.3.8/eth_burner/burn.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.359972 cic-contracts-0.3.8/eth_burner/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 16:41:44.000000 cic-contracts-0.3.8/eth_burner/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1543 2023-06-09 08:31:16.000000 cic-contracts-0.3.8/eth_burner/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      613 2023-06-08 13:23:00.000000 cic-contracts-0.3.8/eth_burner/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.359972 cic-contracts-0.3.8/eth_capped/
+-rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:39:42.000000 cic-contracts-0.3.8/eth_capped/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      799 2023-06-06 08:39:35.000000 cic-contracts-0.3.8/eth_capped/capped.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.359972 cic-contracts-0.3.8/eth_capped/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 12:09:11.000000 cic-contracts-0.3.8/eth_capped/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2125 2023-06-09 08:31:15.000000 cic-contracts-0.3.8/eth_capped/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1069 2023-06-08 13:32:19.000000 cic-contracts-0.3.8/eth_capped/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.359972 cic-contracts-0.3.8/eth_expire/
+-rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 08:31:55.000000 cic-contracts-0.3.8/eth_expire/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1309 2023-06-06 08:31:55.000000 cic-contracts-0.3.8/eth_expire/expire.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.359972 cic-contracts-0.3.8/eth_expire/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 13:21:21.000000 cic-contracts-0.3.8/eth_expire/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2260 2023-06-09 08:33:27.000000 cic-contracts-0.3.8/eth_expire/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1005 2023-06-08 14:54:26.000000 cic-contracts-0.3.8/eth_expire/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.359972 cic-contracts-0.3.8/eth_minter/
+-rw-r--r--   0 lash      (1000) lash      (1000)       30 2023-06-06 14:19:41.000000 cic-contracts-0.3.8/eth_minter/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      921 2023-06-06 14:24:42.000000 cic-contracts-0.3.8/eth_minter/minter.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.359972 cic-contracts-0.3.8/eth_minter/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 14:19:49.000000 cic-contracts-0.3.8/eth_minter/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1589 2023-06-09 08:34:35.000000 cic-contracts-0.3.8/eth_minter/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      618 2023-06-06 14:26:59.000000 cic-contracts-0.3.8/eth_minter/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.359972 cic-contracts-0.3.8/eth_seal/
+-rw-r--r--   0 lash      (1000) lash      (1000)       26 2023-06-08 07:02:02.000000 cic-contracts-0.3.8/eth_seal/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1282 2023-06-08 06:50:18.000000 cic-contracts-0.3.8/eth_seal/seal.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.359972 cic-contracts-0.3.8/eth_seal/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       44 2023-06-08 07:02:18.000000 cic-contracts-0.3.8/eth_seal/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2086 2023-06-09 08:38:00.000000 cic-contracts-0.3.8/eth_seal/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1072 2023-06-08 15:41:19.000000 cic-contracts-0.3.8/eth_seal/unittest/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.359972 cic-contracts-0.3.8/eth_writer/
+-rw-r--r--   0 lash      (1000) lash      (1000)       25 2023-06-06 08:29:33.000000 cic-contracts-0.3.8/eth_writer/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1753 2023-06-06 08:29:33.000000 cic-contracts-0.3.8/eth_writer/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.363306 cic-contracts-0.3.8/eth_writer/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       46 2023-06-06 17:01:25.000000 cic-contracts-0.3.8/eth_writer/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1942 2023-06-09 08:34:01.000000 cic-contracts-0.3.8/eth_writer/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1650 2023-06-06 17:11:14.000000 cic-contracts-0.3.8/eth_writer/unittest/interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-06-06 08:27:06.000000 cic-contracts-0.3.8/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      987 2023-06-09 08:46:19.363306 cic-contracts-0.3.8/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      650 2023-06-08 07:21:42.000000 cic-contracts-0.3.8/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       75 2023-06-06 13:03:05.000000 cic-contracts-0.3.8/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 08:46:19.363306 cic-contracts-0.3.8/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 16:41:18.000000 cic-contracts-0.3.8/tests/test_burner.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      770 2023-06-08 13:23:46.000000 cic-contracts-0.3.8/tests/test_capped.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      766 2023-06-08 14:56:41.000000 cic-contracts-0.3.8/tests/test_expire.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 14:12:58.000000 cic-contracts-0.3.8/tests/test_minter.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      740 2023-06-08 07:03:56.000000 cic-contracts-0.3.8/tests/test_seal.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      724 2023-06-06 17:06:53.000000 cic-contracts-0.3.8/tests/test_writer.py
```

### Comparing `cic-contracts-0.3.7/LICENSE` & `cic-contracts-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/PKG-INFO` & `cic-contracts-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cic-contracts
-Version: 0.3.7
+Version: 0.3.8
 Summary: CIC network smart contract interfaces
 Home-page: https://gitlab.com/cicnet/cic-contracts
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPL3
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cic-contracts-0.3.7/README.md` & `cic-contracts-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/accounts_index.py` & `cic-contracts-0.3.8/cic_contracts/accounts_index.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/base.py` & `cic-contracts-0.3.8/cic_contracts/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/erc20.py` & `cic-contracts-0.3.8/cic_contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/registry.py` & `cic-contracts-0.3.8/cic_contracts/registry.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/unittest/owned.py` & `cic-contracts-0.3.8/cic_contracts/unittest/owned.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/unittest/solidity/BurnerTest.bin` & `cic-contracts-0.3.8/cic_contracts/unittest/solidity/BurnerTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/unittest/solidity/BurnerTest.sol` & `cic-contracts-0.3.8/cic_contracts/unittest/solidity/BurnerTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/unittest/solidity/CappedTest.bin` & `cic-contracts-0.3.8/cic_contracts/unittest/solidity/CappedTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/unittest/solidity/CappedTest.sol` & `cic-contracts-0.3.8/cic_contracts/unittest/solidity/CappedTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/unittest/solidity/ExpireTest.bin` & `cic-contracts-0.3.8/cic_contracts/unittest/solidity/ExpireTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/unittest/solidity/ExpireTest.sol` & `cic-contracts-0.3.8/cic_contracts/unittest/solidity/ExpireTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/unittest/solidity/MinterTest.bin` & `cic-contracts-0.3.8/cic_contracts/unittest/solidity/MinterTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/unittest/solidity/MinterTest.sol` & `cic-contracts-0.3.8/cic_contracts/unittest/solidity/MinterTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/unittest/solidity/SealTest.bin` & `cic-contracts-0.3.8/cic_contracts/unittest/solidity/SealTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/unittest/solidity/SealTest.sol` & `cic-contracts-0.3.8/cic_contracts/unittest/solidity/SealTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/unittest/solidity/WriterTest.bin` & `cic-contracts-0.3.8/cic_contracts/unittest/solidity/WriterTest.bin`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/unittest/solidity/WriterTest.sol` & `cic-contracts-0.3.8/cic_contracts/unittest/solidity/WriterTest.sol`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts/writer.py` & `cic-contracts-0.3.8/cic_contracts/writer.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/cic_contracts.egg-info/PKG-INFO` & `cic-contracts-0.3.8/cic_contracts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cic-contracts
-Version: 0.3.7
+Version: 0.3.8
 Summary: CIC network smart contract interfaces
 Home-page: https://gitlab.com/cicnet/cic-contracts
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPL3
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cic-contracts-0.3.7/eth_burner/burn.py` & `cic-contracts-0.3.8/eth_burner/burn.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_burner/unittest/base.py` & `cic-contracts-0.3.8/eth_burner/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_burner/unittest/interface.py` & `cic-contracts-0.3.8/eth_burner/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_capped/capped.py` & `cic-contracts-0.3.8/eth_capped/capped.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_capped/unittest/base.py` & `cic-contracts-0.3.8/eth_capped/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_capped/unittest/interface.py` & `cic-contracts-0.3.8/eth_capped/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_expire/expire.py` & `cic-contracts-0.3.8/eth_expire/expire.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_expire/unittest/base.py` & `cic-contracts-0.3.8/eth_expire/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_expire/unittest/interface.py` & `cic-contracts-0.3.8/eth_expire/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_minter/minter.py` & `cic-contracts-0.3.8/eth_minter/minter.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_minter/unittest/base.py` & `cic-contracts-0.3.8/eth_minter/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_minter/unittest/interface.py` & `cic-contracts-0.3.8/eth_minter/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_seal/seal.py` & `cic-contracts-0.3.8/eth_seal/seal.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_seal/unittest/base.py` & `cic-contracts-0.3.8/eth_seal/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_seal/unittest/interface.py` & `cic-contracts-0.3.8/eth_seal/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_writer/interface.py` & `cic-contracts-0.3.8/eth_writer/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_writer/unittest/base.py` & `cic-contracts-0.3.8/eth_writer/unittest/base.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/eth_writer/unittest/interface.py` & `cic-contracts-0.3.8/eth_writer/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/setup.cfg` & `cic-contracts-0.3.8/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cic-contracts
-version = 0.3.7
+version = 0.3.8
 description = CIC network smart contract interfaces
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://gitlab.com/cicnet/cic-contracts
 keywords = 
 	dlt
 	blockchain
```

### Comparing `cic-contracts-0.3.7/setup.py` & `cic-contracts-0.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/tests/test_burner.py` & `cic-contracts-0.3.8/tests/test_burner.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/tests/test_capped.py` & `cic-contracts-0.3.8/tests/test_capped.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/tests/test_expire.py` & `cic-contracts-0.3.8/tests/test_expire.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/tests/test_minter.py` & `cic-contracts-0.3.8/tests/test_minter.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/tests/test_seal.py` & `cic-contracts-0.3.8/tests/test_seal.py`

 * *Files identical despite different names*

### Comparing `cic-contracts-0.3.7/tests/test_writer.py` & `cic-contracts-0.3.8/tests/test_writer.py`

 * *Files identical despite different names*

