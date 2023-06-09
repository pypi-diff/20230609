# Comparing `tmp/baguette_verse-1.0.6.tar.gz` & `tmp/baguette_verse-1.0.6.1.tar.gz`

## Comparing `baguette_verse-1.0.6.tar` & `baguette_verse-1.0.6.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/__init__.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/baguette.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/logger.py
--rw-r--r--   0        0        0    16694 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/rack.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/__init__.py
--rw-r--r--   0        0        0    23828 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/bake.py
--rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/compiler.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/__init__.py
--rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/build.py
--rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/colors.py
--rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/config.py
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/event.py
--rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/filters.py
--rw-r--r--   0        0        0    34141 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/graph.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/record.py
--rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/utils.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/__init__.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/utils.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/data/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/data/__proc__.py
--rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/data/entities.py
--rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/data/integration.py
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/data/relations.py
--rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/data/utils.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/execution/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/execution/__proc__.py
--rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/execution/entities.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/execution/integration.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/execution/relations.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/execution/utils.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/__proc__.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/entities.py
--rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/integration.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/relations.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/imports/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/imports/__proc__.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/imports/entities.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/imports/integration.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/imports/relations.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/network/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/network/__proc__.py
--rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/network/entities.py
--rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/network/integration.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/network/relations.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/registry/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/registry/__proc__.py
--rw-r--r--   0        0        0    11045 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/registry/entities.py
--rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/registry/integration.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/registry/relations.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/__init__.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/extractor.py
--rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/toast.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/metalib/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/metalib/interact.py
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/metalib/utils.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/source/__init__.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/source/evaluator.py
--rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/source/metagraph.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/source/utils.py
--rw-r--r--   0        0        0  9439185 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/tutorial/data.zip
--rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/tutorial/scripts.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/tutorial/state.txt
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/tutorial/utils.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/.gitignore
--rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/LICENSE
--rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/README.md
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    48795 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/__init__.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/baguette.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/logger.py
+-rw-r--r--   0        0        0    16694 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/rack.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/__init__.py
+-rw-r--r--   0        0        0    23828 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/bake.py
+-rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/compiler.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/__init__.py
+-rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/build.py
+-rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/colors.py
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/config.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/event.py
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/filters.py
+-rw-r--r--   0        0        0    34141 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/graph.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/record.py
+-rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/utils.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/__init__.py
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/utils.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/data/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/data/__proc__.py
+-rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/data/entities.py
+-rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/data/integration.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/data/relations.py
+-rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/data/utils.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/__proc__.py
+-rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/entities.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/integration.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/relations.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/utils.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/__proc__.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/entities.py
+-rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/integration.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/relations.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/__proc__.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/entities.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/integration.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/relations.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/network/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/network/__proc__.py
+-rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/network/entities.py
+-rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/network/integration.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/network/relations.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/__proc__.py
+-rw-r--r--   0        0        0    11045 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/entities.py
+-rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/integration.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/relations.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/__init__.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/extractor.py
+-rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/toast.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/metalib/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/metalib/interact.py
+-rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/metalib/utils.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/source/__init__.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/source/evaluator.py
+-rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/source/metagraph.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/source/utils.py
+-rw-r--r--   0        0        0  9439185 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/tutorial/data.zip
+-rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/tutorial/scripts.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/tutorial/state.txt
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/tutorial/utils.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/.gitignore
+-rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/LICENSE
+-rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/README.md
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    48841 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/PKG-INFO
```

### Comparing `baguette_verse-1.0.6/baguette/baguette.py` & `baguette_verse-1.0.6.1/baguette/baguette.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/logger.py` & `baguette_verse-1.0.6.1/baguette/logger.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/rack.py` & `baguette_verse-1.0.6.1/baguette/rack.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/bake.py` & `baguette_verse-1.0.6.1/baguette/bakery/bake.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/compiler.py` & `baguette_verse-1.0.6.1/baguette/bakery/compiler.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/build.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/build.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/colors.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/colors.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/config.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/config.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/event.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/event.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/filters.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/filters.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/graph.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/graph.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/record.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/record.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/utils.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/__init__.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/__init__.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/utils.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -90,27 +90,37 @@
     return index
 
 
 
 
 
 @cache
-def relation_types(edge_class : type[Edge]) -> tuple[type[Vertex], type[Vertex]]:
+def relation_types(edge_class : type[Edge]) -> tuple[tuple[type[Vertex]], tuple[type[Vertex]]]:
     """
     Given an Edge or Arrow subclass, gives the best type hints for the source and destination vertices.
     Defaults to (Vertex, Vertex) when no annotations exist.
     """
     from typing import get_type_hints
+    from types import UnionType
     from ..graph import Edge, Vertex
 
     if not isinstance(edge_class, type) or not issubclass(edge_class, Edge):
         raise TypeError("Expected Edge subclass, got " + repr(edge_class))
 
     hints = get_type_hints(edge_class)
-    return hints.get("source", Vertex), hints.get("destination", Vertex)
+    S, D = hints.get("source", Vertex), hints.get("destination", Vertex)
+    if isinstance(S, UnionType):
+        S = tuple(S.__args__)
+    else:
+        S = (S, )
+    if isinstance(D, UnionType):
+        D = tuple(D.__args__)
+    else:
+        D = (D, )
+    return S, D
 
 
 
 
 
 def baguette_structure():
     """
```

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/data/entities.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/data/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/data/integration.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/data/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/data/relations.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/data/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/data/utils.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/data/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/execution/entities.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/execution/integration.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/execution/relations.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/execution/utils.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/entities.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/integration.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/relations.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/imports/entities.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/imports/integration.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/imports/relations.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/network/entities.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/network/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/network/integration.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/network/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/network/relations.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/network/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/registry/entities.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/registry/integration.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/bakery/source/types/registry/relations.py` & `baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/croutons/extractor.py` & `baguette_verse-1.0.6.1/baguette/croutons/extractor.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/croutons/toast.py` & `baguette_verse-1.0.6.1/baguette/croutons/toast.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/croutons/metalib/__init__.py` & `baguette_verse-1.0.6.1/baguette/croutons/metalib/__init__.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/croutons/metalib/interact.py` & `baguette_verse-1.0.6.1/baguette/croutons/metalib/interact.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/croutons/metalib/utils.py` & `baguette_verse-1.0.6.1/baguette/croutons/metalib/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/croutons/source/evaluator.py` & `baguette_verse-1.0.6.1/baguette/croutons/source/evaluator.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/croutons/source/metagraph.py` & `baguette_verse-1.0.6.1/baguette/croutons/source/metagraph.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/croutons/source/utils.py` & `baguette_verse-1.0.6.1/baguette/croutons/source/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,54 +11,43 @@
 
 
 def baguette_structure() -> MetaGraph:
     """
     Returns the structure graph of BAGUETTE. It contains all the possible relations in BAGUETTE.
     """
     from itertools import permutations, product
-    from types import UnionType
     from typing import TypeVar
 
     from ...bakery.source.graph import Arrow, Edge, Vertex
     from ...bakery.source.types.utils import relation_types, relations, types
     from .metagraph import MetaArrow, MetaEdge, MetaGraph, MetaVertex
 
     types_list = list(types())
 
     R : type[Edge]
-    S : type[Vertex] | UnionType
-    D : type[Vertex] | UnionType
+    S : tuple[type[Vertex]]
+    D : tuple[type[Vertex]]
 
     mg = MetaGraph()
     
     involved_in_source : dict[type[Vertex], set[type[Edge]]] = {}
     involved_in_destination : dict[type[Vertex], set[type[Edge]]] = {}
 
     for T in types_list:
         involved_in_destination[T] = set()
         involved_in_source[T] = set()
 
         for R in relations():
             S, D = relation_types(R)
             
-            if isinstance(S, UnionType):
-                St = S.__args__
-            else:
-                St = (S, )
-            for Si in St:
-                if issubclass(T, Si):
-                    involved_in_source[T].add(R)
+            if issubclass(T, S):
+                involved_in_source[T].add(R)
             
-            if isinstance(D, UnionType):
-                Dt = D.__args__
-            else:
-                Dt = (D, )
-            for Di in Dt:
-                if issubclass(T, Di):
-                    involved_in_destination[T].add(R)
+            if issubclass(T, D):
+                involved_in_destination[T].add(R)
 
     vertex_merges : dict[type[Vertex], set[type[Vertex]]] = {}
 
     for Ti, Tj in permutations(types_list, 2):
             if involved_in_destination[Ti] == involved_in_destination[Tj] and involved_in_source[Ti] == involved_in_source[Ti]:
                 
                 if Ti in vertex_merges:
```

### Comparing `baguette_verse-1.0.6/baguette/tutorial/data.zip` & `baguette_verse-1.0.6.1/baguette/tutorial/data.zip`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/tutorial/scripts.py` & `baguette_verse-1.0.6.1/baguette/tutorial/scripts.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/baguette/tutorial/utils.py` & `baguette_verse-1.0.6.1/baguette/tutorial/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/.gitignore` & `baguette_verse-1.0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/LICENSE` & `baguette_verse-1.0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6/README.md` & `baguette_verse-1.0.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # BAGUETTE-VERSE
 
 This is the BAGUETTE framework. BAGUETTE stands for **Behavioral Analysis Graph Using Execution Traces Towards Explanability**.
 BAGUETTE is a **heterogeneous graph** data structure used to represent the **behavior of malware samples**.
 
 The BAGUETTE-VERSE is a framework to build and analyze BAGUETTE graphs.
 
-BAGUETTE requires Python >= 3.10 as well as three Python modules: viper_lib, python-magic and Levenshtein. You can install all these dependencies by hand, but the easiest way is just to use `pip` in the Python installation you want to use:
+BAGUETTE requires Python >= 3.10 as well as three Python modules: viper_lib, python-magic and Levenshtein. You can install all these dependencies by hand, but the easiest way is just to use [`pip`](https://pypi.org/project/baguette-verse/) in the Python installation you want to use:
 
 ```$ pip install baguette-verse```
 
 BAGUETTE is a pure Python project, meaning that a BAGUETTE graph is a Python data structure and for now can only be manipulated using the Python interface described below.
 
 If you want to learn BAGUETTE interactively, once installed, you can just run this command to start the tutorial:
```

### Comparing `baguette_verse-1.0.6/pyproject.toml` & `baguette_verse-1.0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baguette-verse"
-version = "1.0.6"
+version = "1.0.6.1"
 authors = [
   { name="Vincent Raulin", email="vincent.raulin@inria.fr" },
 ]
 description = "A malware behavioral analysis framework centered around BAGUETTE!"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

### Comparing `baguette_verse-1.0.6/PKG-INFO` & `baguette_verse-1.0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baguette-verse
-Version: 1.0.6
+Version: 1.0.6.1
 Summary: A malware behavioral analysis framework centered around BAGUETTE!
 Project-URL: Repository, https://gitlab.inria.fr/vraulin/baguette-verse
 Project-URL: Bug Tracker, https://gitlab.inria.fr/vraulin/baguette-verse/-/issues
 Author-email: Vincent Raulin <vincent.raulin@inria.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
@@ -680,15 +680,15 @@
 # BAGUETTE-VERSE
 
 This is the BAGUETTE framework. BAGUETTE stands for **Behavioral Analysis Graph Using Execution Traces Towards Explanability**.
 BAGUETTE is a **heterogeneous graph** data structure used to represent the **behavior of malware samples**.
 
 The BAGUETTE-VERSE is a framework to build and analyze BAGUETTE graphs.
 
-BAGUETTE requires Python >= 3.10 as well as three Python modules: viper_lib, python-magic and Levenshtein. You can install all these dependencies by hand, but the easiest way is just to use `pip` in the Python installation you want to use:
+BAGUETTE requires Python >= 3.10 as well as three Python modules: viper_lib, python-magic and Levenshtein. You can install all these dependencies by hand, but the easiest way is just to use [`pip`](https://pypi.org/project/baguette-verse/) in the Python installation you want to use:
 
 ```$ pip install baguette-verse```
 
 BAGUETTE is a pure Python project, meaning that a BAGUETTE graph is a Python data structure and for now can only be manipulated using the Python interface described below.
 
 If you want to learn BAGUETTE interactively, once installed, you can just run this command to start the tutorial:
```

