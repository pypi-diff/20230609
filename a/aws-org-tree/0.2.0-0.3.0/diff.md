# Comparing `tmp/aws-org-tree-0.2.0.tar.gz` & `tmp/aws_org_tree-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-org-tree-0.2.0.tar", max compression
+gzip compressed data, was "aws_org_tree-0.3.0.tar", max compression
```

## Comparing `aws-org-tree-0.2.0.tar` & `aws_org_tree-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4463 2021-10-29 01:23:10.632150 aws-org-tree-0.2.0/aws_org_tree.py
--rw-r--r--   0        0        0      484 2021-10-29 01:23:10.632150 aws-org-tree-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      734 2021-11-01 13:09:49.201584 aws-org-tree-0.2.0/setup.py
--rw-r--r--   0        0        0      575 2021-11-01 13:09:49.201806 aws-org-tree-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1272 2023-06-09 15:25:58.611128 aws_org_tree-0.3.0/README.md
+-rw-r--r--   0        0        0     7305 2023-06-09 15:09:48.414050 aws_org_tree-0.3.0/aws_org_tree.py
+-rw-r--r--   0        0        0     1368 2023-06-09 15:31:21.718985 aws_org_tree-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2185 1970-01-01 00:00:00.000000 aws_org_tree-0.3.0/PKG-INFO
```

