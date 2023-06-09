# Comparing `tmp/learnMSA-1.1.2.tar.gz` & `tmp/learnMSA-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learnMSA-1.1.2.tar", last modified: Thu Apr  6 07:59:57 2023, max compression
+gzip compressed data, was "learnMSA-1.2.0.tar", last modified: Fri Jun  9 07:25:13 2023, max compression
```

## Comparing `learnMSA-1.1.2.tar` & `learnMSA-1.2.0.tar`

### file list

```diff
@@ -1,291 +1,292 @@
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.279234 learnMSA-1.1.2/
--rw-r--r--   0 jovyan   (17731) root         (0)      242 2023-04-06 07:59:57.278904 learnMSA-1.1.2/PKG-INFO
--rw-r--r--   0 jovyan   (17731) root         (0)     2987 2023-04-06 07:56:29.000000 learnMSA-1.1.2/README.md
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:56.922365 learnMSA-1.1.2/learnMSA/
--rw-r--r--   0 jovyan   (17731) root         (0)       33 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/__init__.py
--rw-r--r--   0 jovyan   (17731) root         (0)       21 2023-04-06 07:57:56.000000 learnMSA-1.1.2/learnMSA/_version.py
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:56.950966 learnMSA-1.1.2/learnMSA/msa_hmm/
--rw-r--r--   0 jovyan   (17731) root         (0)    33748 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/Align.py
--rw-r--r--   0 jovyan   (17731) root         (0)    28583 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/AlignmentModel.py
--rw-r--r--   0 jovyan   (17731) root         (0)    25907 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/AncProbsLayer.py
--rw-r--r--   0 jovyan   (17731) root         (0)     3674 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/Configuration.py
--rw-r--r--   0 jovyan   (17731) root         (0)     7999 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/DirichletMixture.py
--rw-r--r--   0 jovyan   (17731) root         (0)     7173 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/Emitter.py
--rw-r--r--   0 jovyan   (17731) root         (0)    10866 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/Fasta.py
--rw-r--r--   0 jovyan   (17731) root         (0)     6065 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/Initializers.py
--rw-r--r--   0 jovyan   (17731) root         (0)     7835 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/MsaHmmCell.py
--rw-r--r--   0 jovyan   (17731) root         (0)     5289 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/MsaHmmLayer.py
--rw-r--r--   0 jovyan   (17731) root         (0)     9183 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/Priors.py
--rw-r--r--   0 jovyan   (17731) root         (0)     9872 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/Training.py
--rw-r--r--   0 jovyan   (17731) root         (0)    29732 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/Transitioner.py
--rw-r--r--   0 jovyan   (17731) root         (0)     1119 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/Utility.py
--rw-r--r--   0 jovyan   (17731) root         (0)    13806 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/Visualize.py
--rw-r--r--   0 jovyan   (17731) root         (0)     7844 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/Viterbi.py
--rw-r--r--   0 jovyan   (17731) root         (0)      839 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/__init__.py
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:56.903710 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:56.955975 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    53002 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1434 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:56.961699 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)   518353 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1444 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:56.967715 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    33749 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      818 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:56.972623 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    66005 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:56.977530 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    35917 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1627 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:56.982333 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    68449 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1644 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:56.987319 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    67114 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1444 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:56.992334 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1745 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:56.997180 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1997 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.002153 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     3913 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1598 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.007200 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     4441 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.012082 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     3106 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1412 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.017093 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    66005 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.022095 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)   130517 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.027179 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    68173 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1641 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.032376 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)   132961 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1644 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.037327 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)   131626 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1444 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.042249 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     9557 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.047126 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    17621 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.051986 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    11725 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.056955 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    20065 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1617 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.061797 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    18730 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1415 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.066709 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     2249 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.071599 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     3005 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.076414 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     4417 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1606 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.081247 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     5449 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.086187 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     4114 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1412 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.091542 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)   260305 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1444 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.096840 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    17621 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.101826 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    33749 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      812 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.106608 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    19789 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1610 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.111564 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    36193 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1624 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.116511 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    34858 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1425 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.121325 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     3761 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.126154 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     6029 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.131341 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     5929 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1606 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.136353 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     8473 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.140425 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     7138 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1412 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:56.917252 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.144655 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1413 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      789 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.148941 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1529 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.153527 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.158614 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.163781 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.169004 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1413 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      789 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.174120 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1529 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.179368 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.184731 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.189847 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.195004 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1601 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      792 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.200257 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1709 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.205407 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1673 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      794 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.210561 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1853 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      800 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.215789 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1437 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      789 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.220887 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1973 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      801 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.226276 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     2453 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.232624 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1541 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.239683 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1589 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.245362 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1589 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.251371 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1685 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.257331 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.263304 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1781 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.269052 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1733 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.274683 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1973 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      801 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:57.277564 learnMSA-1.1.2/learnMSA/run/
--rw-r--r--   0 jovyan   (17731) root         (0)       41 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/run/__init__.py
--rw-r--r--   0 jovyan   (17731) root         (0)     3837 2023-04-06 07:56:29.000000 learnMSA-1.1.2/learnMSA/run/console.py
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-04-06 07:59:56.929383 learnMSA-1.1.2/learnMSA.egg-info/
--rw-r--r--   0 jovyan   (17731) root         (0)      242 2023-04-06 07:59:56.000000 learnMSA-1.1.2/learnMSA.egg-info/PKG-INFO
--rw-r--r--   0 jovyan   (17731) root         (0)    15589 2023-04-06 07:59:56.000000 learnMSA-1.1.2/learnMSA.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan   (17731) root         (0)        1 2023-04-06 07:59:56.000000 learnMSA-1.1.2/learnMSA.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan   (17731) root         (0)       51 2023-04-06 07:59:56.000000 learnMSA-1.1.2/learnMSA.egg-info/entry_points.txt
--rw-r--r--   0 jovyan   (17731) root         (0)       45 2023-04-06 07:59:56.000000 learnMSA-1.1.2/learnMSA.egg-info/requires.txt
--rw-r--r--   0 jovyan   (17731) root         (0)        9 2023-04-06 07:59:56.000000 learnMSA-1.1.2/learnMSA.egg-info/top_level.txt
--rw-r--r--   0 jovyan   (17731) root         (0)       80 2023-04-06 07:56:29.000000 learnMSA-1.1.2/pyproject.toml
--rw-r--r--   0 jovyan   (17731) root         (0)       38 2023-04-06 07:59:57.279583 learnMSA-1.1.2/setup.cfg
--rw-r--r--   0 jovyan   (17731) root         (0)     1015 2023-04-06 07:56:29.000000 learnMSA-1.1.2/setup.py
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:13.445426 learnMSA-1.2.0/
+-rw-r--r--   0 jovyan   (17731) root         (0)      242 2023-06-09 07:25:13.445060 learnMSA-1.2.0/PKG-INFO
+-rw-r--r--   0 jovyan   (17731) root         (0)     3721 2023-06-07 06:46:13.000000 learnMSA-1.2.0/README.md
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:59.036971 learnMSA-1.2.0/learnMSA/
+-rw-r--r--   0 jovyan   (17731) root         (0)       33 2023-01-12 09:31:05.000000 learnMSA-1.2.0/learnMSA/__init__.py
+-rw-r--r--   0 jovyan   (17731) root         (0)       21 2023-06-09 07:21:50.000000 learnMSA-1.2.0/learnMSA/_version.py
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:59.109855 learnMSA-1.2.0/learnMSA/msa_hmm/
+-rw-r--r--   0 jovyan   (17731) root         (0)    34665 2023-06-08 09:14:32.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Align.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     6483 2023-06-09 07:19:53.000000 learnMSA-1.2.0/learnMSA/msa_hmm/AlignInsertions.py
+-rw-r--r--   0 jovyan   (17731) root         (0)    34673 2023-06-08 08:57:24.000000 learnMSA-1.2.0/learnMSA/msa_hmm/AlignmentModel.py
+-rw-r--r--   0 jovyan   (17731) root         (0)    25907 2023-04-17 07:14:46.000000 learnMSA-1.2.0/learnMSA/msa_hmm/AncProbsLayer.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     4510 2023-06-01 14:05:27.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Configuration.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     7999 2023-02-27 14:23:42.000000 learnMSA-1.2.0/learnMSA/msa_hmm/DirichletMixture.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     7519 2023-05-08 08:03:16.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Emitter.py
+-rw-r--r--   0 jovyan   (17731) root         (0)    11353 2023-06-01 11:47:09.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Fasta.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     6065 2023-04-18 09:17:14.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Initializers.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     7824 2023-05-08 09:04:58.000000 learnMSA-1.2.0/learnMSA/msa_hmm/MsaHmmCell.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     5645 2023-05-08 08:54:55.000000 learnMSA-1.2.0/learnMSA/msa_hmm/MsaHmmLayer.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     9183 2023-04-06 07:04:35.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Priors.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     9857 2023-04-18 10:52:29.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Training.py
+-rw-r--r--   0 jovyan   (17731) root         (0)    29732 2023-06-01 16:57:53.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Transitioner.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     1119 2023-01-12 09:37:48.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Utility.py
+-rw-r--r--   0 jovyan   (17731) root         (0)    13807 2023-04-18 10:55:32.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Visualize.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     7809 2023-05-08 08:18:25.000000 learnMSA-1.2.0/learnMSA/msa_hmm/Viterbi.py
+-rw-r--r--   0 jovyan   (17731) root         (0)      897 2023-06-01 11:39:37.000000 learnMSA-1.2.0/learnMSA/msa_hmm/__init__.py
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:58.836651 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:59.680225 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    53002 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1434 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:59.784145 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)   518353 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:59.865836 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    33749 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      818 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:00.320068 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    66005 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:00.405339 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    35917 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1627 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:00.543252 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    68449 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1644 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:00.898145 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    67114 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:01.110649 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1745 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:01.361744 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1997 2023-01-12 09:32:03.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:01.405701 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     3913 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1598 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:01.432407 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     4441 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:01.477464 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     3106 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1412 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:01.796052 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    66005 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:02.222098 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)   130517 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:02.393442 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    68173 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1641 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:02.523027 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)   132961 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1644 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:02.766075 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)   131626 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:03.329836 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     9557 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:03.658701 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    17621 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:03.816790 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    11725 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:04.610927 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    20065 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1617 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:04.725954 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    18730 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1415 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:04.791122 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     2249 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:04.842058 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     3005 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:04.931241 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     4417 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1606 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:04.993482 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     5449 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:05.430069 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     4114 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1412 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:05.685703 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)   260305 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:05.764712 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    17621 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:06.290222 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    33749 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      812 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:06.485418 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    19789 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1610 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:06.585254 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    36193 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1624 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:06.641727 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    34858 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1425 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:06.744603 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     3761 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:06.979308 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     6029 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:07.208000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     5929 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1606 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:07.271910 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     8473 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:07.375790 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     7138 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1412 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:58.851374 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:07.509855 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1413 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      789 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:07.563267 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1529 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:07.962507 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:08.022213 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:08.297885 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:08.524785 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1413 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      789 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:08.695837 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1529 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:08.735006 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:09.426033 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:09.483204 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:09.715189 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1601 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      792 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:09.787561 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1709 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:09.859043 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1673 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      794 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:09.936643 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1853 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      800 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:10.379364 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1437 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      789 2022-08-16 08:25:07.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:10.930956 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1973 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      801 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:11.550495 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     2453 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:11.639468 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1541 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:11.861770 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1589 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:11.909572 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1589 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:12.543145 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1685 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:12.634104 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:12.841160 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1781 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:12.932645 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1733 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:13.174985 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1973 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      801 2023-01-12 09:32:05.000000 learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:25:13.442221 learnMSA-1.2.0/learnMSA/run/
+-rw-r--r--   0 jovyan   (17731) root         (0)       41 2022-08-17 06:53:42.000000 learnMSA-1.2.0/learnMSA/run/__init__.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     7910 2023-06-08 09:43:01.000000 learnMSA-1.2.0/learnMSA/run/console.py
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-09 07:24:59.045022 learnMSA-1.2.0/learnMSA.egg-info/
+-rw-r--r--   0 jovyan   (17731) root         (0)      242 2023-06-09 07:24:58.000000 learnMSA-1.2.0/learnMSA.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan   (17731) root         (0)    15625 2023-06-09 07:24:58.000000 learnMSA-1.2.0/learnMSA.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan   (17731) root         (0)        1 2023-06-09 07:24:58.000000 learnMSA-1.2.0/learnMSA.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan   (17731) root         (0)       51 2023-06-09 07:24:58.000000 learnMSA-1.2.0/learnMSA.egg-info/entry_points.txt
+-rw-r--r--   0 jovyan   (17731) root         (0)       45 2023-06-09 07:24:58.000000 learnMSA-1.2.0/learnMSA.egg-info/requires.txt
+-rw-r--r--   0 jovyan   (17731) root         (0)        9 2023-06-09 07:24:58.000000 learnMSA-1.2.0/learnMSA.egg-info/top_level.txt
+-rw-r--r--   0 jovyan   (17731) root         (0)       80 2022-08-09 12:49:25.000000 learnMSA-1.2.0/pyproject.toml
+-rw-r--r--   0 jovyan   (17731) root         (0)       38 2023-06-09 07:25:13.445801 learnMSA-1.2.0/setup.cfg
+-rw-r--r--   0 jovyan   (17731) root         (0)     1015 2023-02-01 15:12:42.000000 learnMSA-1.2.0/setup.py
```

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/Align.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/Align.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 import sys
 import learnMSA.msa_hmm.Fasta as fasta
 import learnMSA.msa_hmm.Training as train
 import learnMSA.msa_hmm.Initializers as initializers
 from learnMSA.msa_hmm.AlignmentModel import AlignmentModel
 from learnMSA.msa_hmm.Configuration import as_str, assert_config
 from pathlib import Path
-
+from learnMSA.msa_hmm.AlignInsertions import make_aligned_insertions
 
 def get_initial_model_lengths(fasta_file, config, random=True):
     #initial model length
     model_length = np.quantile(fasta_file.seq_lens, q=config["length_init_quantile"])
     model_length *= config["len_mul"]
     model_length = max(3., model_length)
     if random:
-        scale = (3 + model_length/30)
+        #scale = (3 + model_length/30)
+        scale = (1 + model_length/50)
         lens = np.round(np.random.normal(loc=model_length, scale=scale, size=config["num_models"])).astype(np.int32)
         lens = np.maximum(lens, 3)
         return lens
     else:
         return [model_length] * config["num_models"]
     
     
@@ -115,26 +116,34 @@
 
 def run_learnMSA(train_filename,
                  out_filename,
                  config, 
                  model_generator=None,
                  batch_generator=None,
                  ref_filename="", 
+                 align_insertions=False,
+                 insertion_aligner="famsa",
+                 aligner_threads=0,
+                 insertion_slice_dir="tmp",
                  verbose=True, 
                   initial_model_length_callback=get_initial_model_lengths,
                  select_best_for_comparison=True):
     """ Wraps fit_and_align and adds file parsing, verbosity, model selection, reference file comparison and an outfile file.
     Args: 
         train_filename: Path of a fasta file with the sequences. 
         out_filename: Filepath of the output fasta file with the aligned sequences.
         config: Configuration that can be used to control training and decoding (see msa_hmm.config.make_default).
         model_generator: Optional callback that generates a user defined model (if None, the default model generator will be used). 
         batch_generator: Optional callback that generates sequence batches defined by user(if None, the default batch generator will be used).
         ref_filename: Optional filepath to a reference alignment. If given, the computed alignment is scored and 
                         the score is returned along with the alignment.
+        align_insertions: If true, a third party aligner is used to align long insertions after the main MSA step.
+        insertion_aligner: Tool to align insertions; "famsa" is installed by default and "clustalo" or "t_coffee" are supported but must be installed manually.
+        aligner_threads: Number of threads to use by the aligner.
+        insertion_slice_dir: Directory where the aligned insertion slices are stored.
         verbose: If False, all output messages will be disabled.
         select_best_for_comparison: If False, all trained models, not just the one with highest score, will be scored.
     Returns:
         An AlignmentModel object.
     """
     if verbose:
         print("Training of", config["num_models"], "models on file", os.path.basename(train_filename))
@@ -162,15 +171,20 @@
         print("Out of memory. A resource was exhausted.")
         print("Try reducing the batch size (-b). The current batch size was: "+str(config["batch_size"])+".")
         sys.exit(e.error_code)
     am.best_model = select_model(am, config["model_criterion"], verbose)
         
     Path(os.path.dirname(out_filename)).mkdir(parents=True, exist_ok=True)
     t = time.time()
-    am.to_file(out_filename, am.best_model)
+    
+    if align_insertions:
+        aligned_insertions = make_aligned_insertions(am, insertion_slice_dir, insertion_aligner, aligner_threads, verbose=verbose)
+        am.to_file(out_filename, am.best_model, aligned_insertions = aligned_insertions)
+    else:
+        am.to_file(out_filename, am.best_model)
     
     if verbose:
         print("time for generating output:", "%.4f" % (time.time()-t))
         print("Wrote file", out_filename)
 
     if ref_filename != "":
         if select_best_for_comparison:
@@ -231,34 +245,34 @@
     ds = train.make_dataset(sorted_indices[:,0], 
                             batch_generator, 
                             batch_size,
                             shuffle=False)
     
     cell = msa_hmm_layer.cell
     
-    @tf.function(input_signature=[tf.TensorSpec(x.shape, dtype=x.dtype) for x in encoder.inputs])
-    def batch_posterior_state_probs(inputs, indices):
-        encoded_seq = encoder([inputs, indices]) 
+    @tf.function(input_signature=[[tf.TensorSpec(x.shape, dtype=x.dtype) for x in encoder.inputs]])
+    def batch_posterior_state_probs(inputs):
+        encoded_seq = encoder(inputs) 
         posterior_probs = msa_hmm_layer.state_posterior_log_probs(encoded_seq)
         posterior_probs = tf.math.exp(posterior_probs)
         #compute expected number of visits per hidden state and sum over batch dim
         posterior_probs = tf.reduce_sum(posterior_probs, -2)
         if reduce:
             posterior_probs = tf.reduce_sum(posterior_probs, 1) / num_indices
         return posterior_probs
     
     if reduce:
         posterior_probs = tf.zeros((cell.num_models, cell.max_num_states), cell.dtype) 
         for inputs, _ in ds:
-            posterior_probs += batch_posterior_state_probs(inputs[0], inputs[1])
+            posterior_probs += batch_posterior_state_probs(inputs)
         return posterior_probs.numpy()
     else:
         posterior_probs = np.zeros((cell.num_models, num_indices, cell.max_num_states), cell.dtype) 
         for i, (inputs, _) in enumerate(ds):
-            posterior_probs[:,i*batch_size : (i+1)*batch_size] = batch_posterior_state_probs(inputs[0], inputs[1])
+            posterior_probs[:,i*batch_size : (i+1)*batch_size] = batch_posterior_state_probs(inputs)
         return posterior_probs
     
         
 def get_discard_or_expand_positions(am, 
                                     del_t=0.5, 
                                     ins_t=0.5):
     """ Given an AlignmentModel, computes positions for match expansions and discards based on the posterior state probabilities.
```

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/AlignmentModel.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/AlignmentModel.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,142 @@
 import learnMSA.msa_hmm.Priors as priors
 import learnMSA.msa_hmm.Transitioner as trans
 import learnMSA.msa_hmm.Emitter as emit
 import json
 import shutil
 from pathlib import Path
 
+        
+# utility class used in AlignmentModel storing useful information on a specific alignment
+class AlignmentMetaData():
+    def __init__(self, 
+                 core_blocks, 
+                 left_flank, 
+                 right_flank, 
+                 unannotated_segments):
+        self.consensus = np.stack([C for C,_,_,_ in core_blocks])
+        self.insertion_lens = np.stack([IL for _,IL,_,_ in core_blocks])
+        self.insertion_start = np.stack([IS for _,_,IS,_ in core_blocks])
+        self.finished = np.stack([f for _,_,_,f in core_blocks])
+        self.left_flank_len = np.stack(left_flank[0])
+        self.left_flank_start = np.stack(left_flank[1])
+        self.right_flank_len = np.stack(right_flank[0])
+        self.right_flank_start = np.stack(right_flank[1])
+        if len(unannotated_segments) > 0:
+            self.unannotated_segments_len = np.stack([l for l,_ in unannotated_segments])
+            self.unannotated_segments_start = np.stack([s for _,s in unannotated_segments])
+            self.unannotated_segment_lens_total = np.amax(self.unannotated_segments_len, axis=1)
+        else:
+            self.unannotated_segment_lens_total = 0
+        self.num_repeats = self.consensus.shape[0]
+        self.consensus_len = self.consensus.shape[1]
+        self.left_flank_len_total = np.amax(self.left_flank_len)
+        self.right_flank_len_total = np.amax(self.right_flank_len)
+        self.insertion_lens_total = np.amax(self.insertion_lens, axis=1)
+        self.alignment_len = (self.left_flank_len_total + 
+                              self.consensus_len*self.num_repeats + 
+                              np.sum(self.insertion_lens_total) + 
+                              np.sum(self.unannotated_segment_lens_total) +
+                              self.right_flank_len_total)
+        
+        
+class AlignedInsertions():
+    def __init__(self, 
+                 aligned_insertions = None,
+                 aligned_left_flank = None,
+                 aligned_right_flank = None,
+                 aligned_unannotated_segments = None):
+        """ 
+        Args: 
+            aligned_insertions: List of lists of pairs (indices, fasta file with aligned slices) or None. Inner lists have length equal to length of model -1. Outer list has length num_repeats.
+            aligned_left_flank: A pair (indices, fasta file with aligned slices) or None.
+            aligned_right_flank: A pair (indices, fasta file with aligned slices) or None.
+            unannotated_data: List of pairs (indices, fasta file with aligned slices) or None of length num_repeats-1.
+        """
+        self.aligned_insertions = aligned_insertions
+        self.aligned_left_flank = aligned_left_flank
+        self.aligned_right_flank = aligned_right_flank
+        self.aligned_unannotated_segments = aligned_unannotated_segments
+        
+        def _process(fasta_file):
+            custom_columns = np.zeros((fasta_file.num_seq, np.amax(fasta_file.alignment_len)), dtype=np.int32)
+            for i in range(fasta_file.num_seq):
+                cols = fasta_file.get_membership_targets(i)
+                custom_columns[i, :cols.size] = cols
+            return custom_columns
+                
+        
+        if aligned_insertions is None:
+            self.ext_insertions = 0
+        else:
+            self.custom_columns_insertions = []
+            for repeat in aligned_insertions:
+                self.custom_columns_insertions.append([])
+                for x in repeat:
+                    if x is None:
+                        self.custom_columns_insertions[-1].append(None)
+                    else:
+                        self.custom_columns_insertions[-1].append(_process(x[1]))
+            self.ext_insertions = np.array([[np.amax(x)+1 if x is not None else 0 for x in repeats] for repeats in self.custom_columns_insertions])
+        
+        if aligned_left_flank is None:
+            self.ext_left_flank = 0
+        else:
+            self.custom_columns_left_flank = _process(aligned_left_flank[1])
+            self.ext_left_flank = np.amax(self.custom_columns_left_flank)+1
+        
+        if aligned_right_flank is None:
+            self.ext_right_flank = 0
+        else:
+            self.custom_columns_right_flank = _process(aligned_right_flank[1])
+            self.ext_right_flank = np.amax(self.custom_columns_right_flank)+1
+            
+        if aligned_unannotated_segments is None:
+            self.ext_unannotated = 0
+        else:
+            self.custom_columns_unannotated_segments = [_process(x[1]) if x is not None else None for x in aligned_unannotated_segments]
+            self.ext_unannotated = np.array([np.amax(x)+1 if x is not None else 0 for x in self.custom_columns_unannotated_segments])
+    
+    def get_custom_columns_insertion(self, batch_indices, r):
+        if self.aligned_insertions is None:
+            return None
+        else:
+            return [self._get_custom_columns(batch_indices, self.aligned_insertions[r][i][0], self.custom_columns_insertions[r][i], self.ext_insertions[r,i])
+                       if self.aligned_insertions[r][i] is not None else None
+                       for i in range(len(self.aligned_insertions[r]))]
+    
+    def get_custom_columns_left_flank(self, batch_indices):
+        if self.aligned_left_flank is None:
+            return None
+        else:
+            return self._get_custom_columns(batch_indices, self.aligned_left_flank[0], self.custom_columns_left_flank, self.ext_left_flank)
+    
+    def get_custom_columns_right_flank(self, batch_indices):
+        if self.aligned_right_flank is None:
+            return None
+        else:
+            return self._get_custom_columns(batch_indices, self.aligned_right_flank[0], self.custom_columns_right_flank, self.ext_right_flank)
+        
+    def get_custom_columns_unannotated_segment(self, batch_indices, r):
+        if self.aligned_unannotated_segments is None:
+            return None
+        else:
+            if self.aligned_unannotated_segments[r] is None:
+                return None
+            else:
+                return self._get_custom_columns(batch_indices, self.aligned_unannotated_segments[r][0], self.custom_columns_unannotated_segments[r], self.ext_unannotated[r])
+            
+    def _get_custom_columns(self, batch_indices, custom_indices, custom_columns, max_len):
+        columns = np.stack([np.arange(max_len)]*batch_indices.shape[0])
+        for i, c in zip(custom_indices, custom_columns):
+            columns[batch_indices == i, :c.size] = c 
+        return columns
+        
+
+
 
 class AlignmentModel():
     """ Decodes alignments from a number of models, stores them in a memory friendly representation and
         generates table-form (memory unfriendly) alignments on demand (batch-wise mode possible).
     Args:
         fasta_file: A fasta file with the sequences to decode.
         batch_generator: An already configured batch generator.
@@ -79,112 +207,119 @@
                                                             cell_copy,
                                                             models,
                                                             self.encoder_model)
         for i,l,max_lik_seqs in zip(models, cell_copy.length, state_seqs_max_lik):
             decoded_data = AlignmentModel.decode(l,max_lik_seqs)
             self.metadata[i] = AlignmentMetaData(*decoded_data)
         
-    def to_string(self, model_index, batch_size=100000, add_block_sep=True):
+    def to_string(self, model_index, batch_size=100000, add_block_sep=True, aligned_insertions : AlignedInsertions = AlignedInsertions()):
         """ Uses one model to decode an alignment and returns the sequences with gaps in a list.
             Note that this method is not suitable im memory is limited and alignment depths and width are large.
         Args:
             model_index: Specifies the model for decoding. Use a suitable criterion like loglik to decide for a model.
             batch_size: Defines how many sequences are decoded at a time with no effect on the output MSA. It can be useful to
                         lower this if memory is sufficient to store the table-form alignment but GPU memory used for decoding a batch is limited.
             add_block_sep: If true, columns containing a special character are added to the alignment indicating domain boundaries.
+            aligned_insertions: Can be used to override insertion metadata if insertions are aligned after the main procedure.
         """
         alignment_strings_all = []
         n = self.indices.size
         i = 0
         while i < n:
             batch_indices = np.arange(i, min(n, i+batch_size))
-            batch_alignment = self.get_batch_alignment(model_index, batch_indices, add_block_sep)
+            batch_alignment = self.get_batch_alignment(model_index, batch_indices, add_block_sep, aligned_insertions)
             alignment_strings = self.batch_to_string(batch_alignment)
             alignment_strings_all.extend(alignment_strings)
             i += batch_size
         return alignment_strings_all
     
-    def to_file(self, filepath, model_index, batch_size=100000, add_block_sep=False):
+    def to_file(self, filepath, model_index, batch_size=100000, add_block_sep=False, aligned_insertions : AlignedInsertions = AlignedInsertions()):
         """ Uses one model to decode an alignment and stores it in fasta file format. Currently no other output format is supported.
             The file is written batch wise. The memory required for this operation must be large enough to hold decode and store a single batch
             of aligned sequences but not the whole alignment.
         Args:
             model_index: Specifies the model for decoding. Use a suitable criterion like loglik to decide for a model.
             batch_size: Defines how many sequences are decoded at a time with no effect on the output MSA. It can be useful to
                         lower this if memory is sufficient to store the table-form alignment but GPU memory used for decoding a batch is limited.
             add_block_sep: If true, columns containing a special character are added to the alignment indicating domain boundaries.
+            aligned_insertions: Can be used to override insertion metadata if insertions are aligned after the main procedure.
         """
         with open(filepath, "w") as output_file:
             n = self.indices.size
             i = 0
             while i < n:
                 batch_indices = np.arange(i, min(n, i+batch_size))
-                batch_alignment = self.get_batch_alignment(model_index, batch_indices, add_block_sep)
+                batch_alignment = self.get_batch_alignment(model_index, batch_indices, add_block_sep, aligned_insertions)
                 alignment_strings = self.batch_to_string(batch_alignment)
                 for s, seq_ind in zip(alignment_strings, batch_indices):
                     seq_id = self.fasta_file.seq_ids[self.indices[seq_ind]]
                     output_file.write(">"+seq_id+"\n")
                     output_file.write(s+"\n")
                 i += batch_size
     
-    def get_batch_alignment(self, model_index, batch_indices, add_block_sep):
+    def get_batch_alignment(self, model_index, batch_indices, add_block_sep, aligned_insertions : AlignedInsertions = AlignedInsertions()):
         """ Returns a dense matrix representing a subset of sequences
             as specified by batch_indices with respect to the alignment of all sequences
             (i.e. the sub alignment can contain gap-only columns and stacking all batches 
             yields a complete alignment).
         Args:
             model_index: Specifies the model for decoding. Use a suitable criterion like loglik to decide for a model.
             batch_indices: Sequence indices / indices of alignment rows.
             add_block_sep: If true, columns containing a special character are added to the alignment indicating domain boundaries.
+            aligned_insertions: Can be used to override insertion metadata if insertions are aligned after the main procedure.
         """
         if not model_index in self.metadata:
             self._build_alignment([model_index])
+        data = self.metadata[model_index]
         b = batch_indices.size
         sequences = np.zeros((b, self.fasta_file.max_len), dtype=np.uint16) + (fasta.s-1)
         for i,j in enumerate(batch_indices):
             l = self.fasta_file.seq_lens[self.indices[j]]
             sequences[i, :l] = self.fasta_file.get_raw_seq(self.indices[j])
         blocks = []  
         if add_block_sep:
             sep = np.zeros((b,1), dtype=np.uint16) + 2*fasta.s
         left_flank_block = AlignmentModel.get_insertion_block(sequences, 
-                                               self.metadata[model_index].left_flank_len[batch_indices],
-                                               self.metadata[model_index].left_flank_len_total,
-                                               self.metadata[model_index].left_flank_start[batch_indices],
-                                               align_to_right=True)
+                                               data.left_flank_len[batch_indices],
+                                               max(data.left_flank_len_total, aligned_insertions.ext_left_flank),
+                                               data.left_flank_start[batch_indices],
+                                               adjust_to_right=True,
+                                               custom_columns=aligned_insertions.get_custom_columns_left_flank(batch_indices))
         blocks.append(left_flank_block)
         if add_block_sep:
             blocks.append(sep)
-        for i in range(self.metadata[model_index].num_repeats):
-            consensus = self.metadata[model_index].consensus[i]
-            ins_len = self.metadata[model_index].insertion_lens[i]
-            ins_start = self.metadata[model_index].insertion_start[i]
-            ins_len_total = self.metadata[model_index].insertion_lens_total[i]
+        for i in range(data.num_repeats):
+            consensus = data.consensus[i]
+            ins_len = data.insertion_lens[i]
+            ins_start = data.insertion_start[i]
             alignment_block = AlignmentModel.get_alignment_block(sequences, 
                                                   consensus[batch_indices], 
                                                   ins_len[batch_indices], 
-                                                  ins_len_total,
-                                                  ins_start[batch_indices])
+                                                  np.maximum(data.insertion_lens_total, aligned_insertions.ext_insertions)[i],
+                                                  ins_start[batch_indices],
+                                                  custom_columns=aligned_insertions.get_custom_columns_insertion(batch_indices, i))
             blocks.append(alignment_block)
             if add_block_sep:
                 blocks.append(sep)
-            if i < self.metadata[model_index].num_repeats-1:
-                unannotated_segment_l = self.metadata[model_index].unannotated_segments_len[i]
-                unannotated_segment_s = self.metadata[model_index].unannotated_segments_start[i]
+            if i < data.num_repeats-1:
+                unannotated_segment_l = data.unannotated_segments_len[i]
+                unannotated_segment_s = data.unannotated_segments_start[i]
                 unannotated_block = AlignmentModel.get_insertion_block(sequences, 
                                                         unannotated_segment_l[batch_indices],
-                                                        self.metadata[model_index].unannotated_segment_lens_total[i],
-                                                        unannotated_segment_s[batch_indices])
+                                                        np.maximum(data.unannotated_segment_lens_total, aligned_insertions.ext_unannotated)[i],
+                                                        unannotated_segment_s[batch_indices],
+                                                        custom_columns=aligned_insertions.get_custom_columns_unannotated_segment(batch_indices, i))
                 blocks.append(unannotated_block)
                 if add_block_sep:
                     blocks.append(sep)
         right_flank_block = AlignmentModel.get_insertion_block(sequences, 
-                                               self.metadata[model_index].right_flank_len[batch_indices],
-                                               self.metadata[model_index].right_flank_len_total,
-                                               self.metadata[model_index].right_flank_start[batch_indices])
+                                               data.right_flank_len[batch_indices],
+                                               max(data.right_flank_len_total, aligned_insertions.ext_right_flank),
+                                               data.right_flank_start[batch_indices],
+                                               custom_columns=aligned_insertions.get_custom_columns_right_flank(batch_indices))
         blocks.append(right_flank_block)
         batch_alignment = np.concatenate(blocks, axis=1)
         return batch_alignment
     
     def batch_to_string(self, batch_alignment):
         """ Converts a dense matrix into string format.
         """
@@ -439,41 +574,44 @@
                 break
             unannotated_segments.append( cls.decode_flank(state_seqs_max_lik, 2*c, indices) )
         right_flank = cls.decode_flank(state_seqs_max_lik, 2*c+1, indices) 
         return core_blocks, left_flank, right_flank, unannotated_segments
 
 
     @classmethod
-    def get_insertion_block(cls, sequences, lens, maxlen, starts, align_to_right=False):
+    def get_insertion_block(cls, sequences, lens, maxlen, starts, adjust_to_right=False, custom_columns=None):
         """ Constructs one insertion block from an implicitly represented alignment.
         Args: 
         Returns:
         """
-        A = np.arange(sequences.shape[0])
-        block = np.zeros((sequences.shape[0], maxlen), dtype=np.uint8) + (fasta.s-1)
-        lens = np.copy(lens)
-        active = lens > 0
+        n = sequences.shape[0]
+        A = np.arange(n)
+        block = np.zeros((n, maxlen), dtype=np.uint8) + (fasta.s-1)
+        count_down_lens = np.copy(lens)
+        active = count_down_lens > 0
         i = 0
+        columns = np.stack([np.arange(maxlen)]*n) if custom_columns is None else custom_columns
         while np.any(active):
             aa = sequences[A[active], starts[active] + i]
-            block[active, i] = aa
-            lens -= 1
-            active = lens > 0
+            block[active, columns[active,i]] = aa
+            count_down_lens -= 1
+            active = count_down_lens > 0
             i += 1
-        if align_to_right:
+        if adjust_to_right and custom_columns is None:
             block_right_aligned = np.zeros_like(block) + (fasta.s-1)
             for i in range(maxlen):
+                
                 block_right_aligned[A, (maxlen-lens+i)%maxlen] = block[:, i]
             block = block_right_aligned
         block += fasta.s #lower case
         return block
 
 
     @classmethod
-    def get_alignment_block(cls, sequences, consensus, ins_len, ins_len_total, ins_start):
+    def get_alignment_block(cls, sequences, consensus, ins_len, ins_len_total, ins_start, custom_columns=None):
         """ Constructs one core model hit block from an implicitly represented alignment.
         Args: 
         Returns:
         """
         A = np.arange(sequences.shape[0])
         length = consensus.shape[1] + np.sum(ins_len_total)
         block = np.zeros((sequences.shape[0], length), dtype=np.uint8) + (fasta.s-1)
@@ -487,48 +625,14 @@
             no_gap = column != -1
             block[no_gap,i] = sequences[A[no_gap],column[no_gap]]
             i += 1
             #insertion
             block[:,i:i+ins_l_total] = cls.get_insertion_block(sequences,
                                                            ins_l,
                                                            ins_l_total, 
-                                                           ins_s)
+                                                           ins_s, 
+                                                           custom_columns = custom_columns[c] if custom_columns is not None else None)
             i += ins_l_total
         #final column
         no_gap = consensus[:,-1] != -1
         block[no_gap,i] = sequences[A[no_gap],consensus[:,-1][no_gap]]
-        return block
-
-    
-        
-        
-# utility class used in AlignmentModel storing useful information on a specific alignment
-class AlignmentMetaData():
-    def __init__(self, 
-                 core_blocks, 
-                 left_flank, 
-                 right_flank, 
-                 unannotated_segments):
-        self.consensus = np.stack([C for C,_,_,_ in core_blocks])
-        self.insertion_lens = np.stack([IL for _,IL,_,_ in core_blocks])
-        self.insertion_start = np.stack([IS for _,_,IS,_ in core_blocks])
-        self.finished = np.stack([f for _,_,_,f in core_blocks])
-        self.left_flank_len = np.stack(left_flank[0])
-        self.left_flank_start = np.stack(left_flank[1])
-        self.right_flank_len = np.stack(right_flank[0])
-        self.right_flank_start = np.stack(right_flank[1])
-        if len(unannotated_segments) > 0:
-            self.unannotated_segments_len = np.stack([l for l,_ in unannotated_segments])
-            self.unannotated_segments_start = np.stack([s for _,s in unannotated_segments])
-            self.unannotated_segment_lens_total = np.amax(self.unannotated_segments_len, axis=1)
-        else:
-            self.unannotated_segment_lens_total = 0
-        self.num_repeats = self.consensus.shape[0]
-        self.consensus_len = self.consensus.shape[1]
-        self.left_flank_len_total = np.amax(self.left_flank_len)
-        self.right_flank_len_total = np.amax(self.right_flank_len)
-        self.insertion_lens_total = np.amax(self.insertion_lens, axis=1)
-        self.alignment_len = (self.left_flank_len_total + 
-                              self.consensus_len*self.num_repeats + 
-                              np.sum(self.insertion_lens_total) + 
-                              np.sum(self.unannotated_segment_lens_total) +
-                              self.right_flank_len_total)
+        return block
```

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/AncProbsLayer.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/AncProbsLayer.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/Configuration.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/Configuration.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 #longer models and sequences require much more memory
 #we limit the batch size based on the longest model to train
 #the adpative batch size scales automatically with the number of GPUs
 def get_adaptive_batch_size(model_lengths, max_seq_len):
     num_gpu = len([x.name for x in tf.config.list_logical_devices() if x.device_type == 'GPU']) 
     num_devices = num_gpu + int(num_gpu==0) #account for the CPU-only case 
     model_length = max(model_lengths)
-    if max_seq_len < 200 and model_length < 200:
+    if max_seq_len < 200 and model_length < 180:
         return 512*num_devices
-    elif max_seq_len < 520 and model_length < 290:
+    elif max_seq_len < 520 and model_length < 230:
         return 256*num_devices
-    elif max_seq_len < 800 and model_length < 500:
+    elif max_seq_len < 700 and model_length < 420:
         return 128*num_devices
-    else:
+    elif max_seq_len < 850 and model_length < 550:
         return 64*num_devices
+    else:
+        return 32*num_devices
 
 #the configuration can be changed by experienced users
 #proper command line support for these parameters will be added in the future
 def make_default(default_num_models = 5):
     default = {
 
         "num_models" : default_num_models,
@@ -63,15 +65,26 @@
         "model_criterion" : "AIC", #AIC is slightly better than loglik on average over multiple benchmarks
         "encoder_weight_extractor" : None,
         "experimental_evolve_upper_half" : False,
         "allow_user_keys_in_config" : False
     }
     return default
 
+def _make_assert_text(message, current_value):
+    return message + f" Your input was {current_value}."
+
 def assert_config(config):
+    assert config["max_surgery_runs"] > 0, \
+        _make_assert_text("Requires as least 1 surgery run.", config["max_surgery_runs"])
+    assert config["length_init_quantile"] >= 0. and config["length_init_quantile"] <= 1., \
+        _make_assert_text("The given quantile is not in range [0,1].", config["length_init_quantile"])
+    assert config["surgery_quantile"] >= 0. and config["surgery_quantile"] <= 1., \
+        _make_assert_text("The given quantile is not in range [0,1].", config["surgery_quantile"])
+    assert config["len_mul"] >= 0., \
+        _make_assert_text("The multiplier must be greater than zero.", config["surgery_quantile"])
     assert "num_models" in config
     default = make_default(config["num_models"])
     for key in default:
         assert key in config, f"User configuration is missing key {key}."
     if not config["allow_user_keys_in_config"]:
         for key in config:
             assert key in default, f"Unrecognized key {key} in user configuration."
```

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/DirichletMixture.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/DirichletMixture.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/Emitter.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/Emitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,59 +59,66 @@
     def recurrent_init(self):
         """ Automatically called before each recurrent run. Should be used for setups that
             are only required once per application of the recurrent layer.
         """
         self.B = self.make_B()
         self.B_transposed = tf.transpose(self.B, [0,2,1])
         
-    def make_emission_matrix(self, em, ins, length):
+    def make_emission_matrix(self, i):
         """Constructs an emission matrix from kernels with a shared insertion distribution.
         Args:
-           s: Alphabet size.
-           em: Emission distribution logits (kernel).
-           ins: Shared insertion distribution (kernel).
-           length: Model length.
+           i: Model index.
         Returns:
             The emission matrix.
         """
+        em, ins = self.emission_kernel[i], self.insertion_kernel[i]
+        length = self.length[i]
+        return self.make_emission_matrix_from_kernels(em, ins, length)
+    
+    def make_emission_matrix_from_kernels(self, em, ins, length):
         s = em.shape[-1]
         emissions = tf.concat([tf.expand_dims(ins, 0), 
                                em, 
                                tf.stack([ins]*(length+1))] , axis=0)
         emissions = tf.nn.softmax(emissions)
         emissions = tf.concat([emissions, tf.zeros_like(emissions[:,:1])], axis=-1) 
         end_state_emission = tf.one_hot([s], s+1, dtype=em.dtype) 
         emissions = tf.concat([emissions, end_state_emission], axis=0)
         return emissions
         
     def make_B(self):
         emission_matrices = []
-        for em, ins, length in zip(self.emission_kernel, self.insertion_kernel, self.length):
-            em_mat = self.make_emission_matrix(em, ins, length) 
+        for i in range(self.num_models):
+            em_mat = self.make_emission_matrix(i) 
             padding = self.max_num_states - em_mat.shape[0]
             em_mat_pad = tf.pad(em_mat, [[0, padding], [0,0]])
             emission_matrices.append(em_mat_pad)
         B = tf.stack(emission_matrices, axis=0)
         return B
         
     def make_B_amino(self):
         """ A variant of make_B used for plotting the HMM. Can be overridden for more complex emissions. Per default this is equivalent to make_B
         """
         return self.make_B()
         
     def call(self, inputs):
         """ 
         Args: 
-                inputs: Shape (k, b, s) (Shape (b, s) works as well if all models should get the same input.)
+                inputs: A tensor of shape (k, ... , s) 
         Returns:
-                Shape (k, b, q)
+                A tensor with emission probabilities of shape (k, ... , q) where "..." is identical to inputs.
         """
+        input_shape = tf.shape(inputs)
+        inputs = tf.reshape(inputs, (tf.shape(inputs)[0], -1, input_shape[-1]))
         # batch matmul of k emission matrices with the b x s input matrix 
         # with broadcasting of the inputs
-        return tf.matmul(inputs, self.B_transposed)
+        emit = tf.matmul(inputs, self.B_transposed)
+        emit_shape = tf.concat([tf.shape(self.B_transposed)[:1], input_shape[1:-1], tf.shape(self.B_transposed)[-1:]], 0)
+        emit = tf.reshape(emit, emit_shape)
+        return emit
     
     def get_prior_log_density(self):
         return self.prior(self.make_B(), self.length)
     
     def duplicate(self, model_indices=None):
         if model_indices is None:
             model_indices = range(len(self.emission_init))
```

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/Fasta.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/Fasta.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,18 +18,22 @@
 # a class that reads sequences in fasta file format 
 # condensed representation of a potentially large sequence datatset
 # all sequences are stored in a flat array of 16bit integers
 # one-hot representations are only constructed on the fly for small batches
 class Fasta:
     def __init__(self, 
                  filename, #fasta file to parse
-                 aligned = False #automatically assumes an alignment if gaps are found, this flag only has to be set manually, if the file contains a gapless alignment
+                 aligned = False, #automatically assumes an alignment if gaps are found, this flag only has to be set manually, if the file contains a gapless alignment
+                 single_seq_ok = False,
+                 replace_BZJ = True
                 ):
         self.filename = filename
         self.aligned = aligned
+        self.single_seq_ok = single_seq_ok
+        self.replace_BZJ = replace_BZJ
         self.read_seqs(filename)
         if self.gaps:
             self.compute_targets()
 
             
             
     def read_seqs(self, filename):
@@ -42,22 +46,25 @@
             line = line.strip()
             if len(line)>0:
                 if line[0]=='>':
                     self.seq_ids.append(line[1:])
                     self.raw_seq.append("")
                 elif len(self.raw_seq) > 0:
                     self.raw_seq[-1] += line
+            
+        if self.replace_BZJ:
+            for c in ["b", "B", "z", "Z", "j", "J"]:
+                replace_in_strings(self.raw_seq, c, 'X')
                         
-                    
         self.gaps = self.validate()
         
         if self.gaps:    
             self.alignment_len = len(self.raw_seq[0])
             replace_in_strings(self.raw_seq, '.', '-')
-            
+                        
         for i,c in enumerate(alphabet[:-1]):
             replace_in_strings(self.raw_seq, c, str(i)+' ')
             replace_in_strings(self.raw_seq, c.lower(), str(i)+' ')
 
         #can store sequences with gaps as matrix
         if self.gaps:
             self.ref_seq = copy.deepcopy(self.raw_seq)
@@ -77,15 +84,15 @@
         self.num_seq = len(self.seq_lens)
         #also store the permutation of sequence indices that sorts by length
         self.sorted_indices = np.array([i for l,i in sorted(zip(self.seq_lens, range(self.num_seq)))]) 
         
         
     def validate(self):
         gaps = self.aligned
-        if len(self.raw_seq) == 1:
+        if len(self.raw_seq) == 1 and not self.single_seq_ok:
             raise SystemExit(f"File {self.filename} contains only a single sequence.") 
             
         if len(self.raw_seq) == 0:
             raise SystemExit(f"Can not read sequences from file {self.filename}. Expected a file in FASTA format containing at least 2 sequences.") 
                     
         #validate seq ids (required for anc.probs. to work correctly)
         if len(self.raw_seq) != len(self.seq_ids):
@@ -149,14 +156,19 @@
         #a mapping from raw position to column index
         #A-B--C -> 112223
         cumsum = np.cumsum(self.ref_seq != len(alphabet)-1, axis=1) 
         #112223 -> 0112223 -> [[(i+1) - i]] -> 101001
         diff = np.diff(np.insert(cumsum, 0, 0.0, axis=1), axis=1) 
         diff_where = [np.argwhere(diff[i,:]).flatten() for i in range(diff.shape[0])]
         self.membership_targets = np.concatenate(diff_where).flatten()
+        
+    def get_membership_targets(self, i):
+        s = self.starting_pos[i]
+        e = s + self.seq_lens[i]
+        return self.membership_targets[s:e]
       
     
     
     #returns a binary matrix indicating which residues correspond to which columns
     #if only a subset of the sequences is required, empty columns will be removed
     #output shape is (num_seq, num_columns, max_len_seq)
 #     def column_memberships(self, subset=None):
@@ -200,15 +212,15 @@
         for j in self.get_raw_seq(i):
             seq += alphabet[j]
         return seq
     
     
     def column_str(self, i):
         col = ""
-        for j in self.ref_seq[:,i]:
+        for j in self.ref_seq[i]:
             col += alphabet[j]
         return col
     
     
     #equivalent to modeler and developer/SP score respectively
     #batch size can be reduced to resolve memory issues, it does not affect the result
     def precision_recall(self, ref_fasta, batch=512, verbose=False):
```

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/Initializers.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/Initializers.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/MsaHmmCell.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/MsaHmmCell.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
         self.transitioner.cell_init(self)
         self.epsilon = tf.constant(1e-32, self.dtype)
         self.reverse = False
             
             
     def build(self, input_shape):
         self.dim = input_shape[-1]
+        if self.built:
+            return
         for em in self.emitter:
             em.build(input_shape)
         self.transitioner.build(input_shape)
         self.built = True
 
         
     def recurrent_init(self):
@@ -79,22 +81,21 @@
         """
         em_probs = self.emitter[0](inputs)
         for em in self.emitter[1:]:
             em_probs *= em(inputs)
         return em_probs
 
     
-    def call(self, inputs, states, training=None, init=False):
+    def call(self, emission_probs, states, training=None, init=False):
         """ Computes one recurrent step of the Forward DP.
         """
         old_scaled_forward, old_loglik = states
         old_scaled_forward = tf.reshape(old_scaled_forward, (self.num_models, -1, self.max_num_states))
         old_loglik = tf.reshape(old_loglik, (self.num_models, -1, 1))
-        inputs = tf.reshape(inputs, (self.num_models, -1, self.dim))
-        E = self.emission_probs(inputs)
+        E = tf.reshape(emission_probs, (self.num_models, -1, self.max_num_states))
         if init:
             R = old_scaled_forward
         else:
             R = self.transitioner(old_scaled_forward)
         scaled_forward = tf.multiply(E, R, name="scaled_forward")
         S = tf.reduce_sum(scaled_forward, axis=-1, keepdims=True)
         loglik = old_loglik + tf.math.log(S) 
@@ -146,15 +147,14 @@
         assert self.built, "Can only duplicate a cell that was built before (i.e. it has kernels)."
         if model_indices is None:
             model_indices = range(self.num_models)
         sub_lengths = [self.length[i] for i in model_indices]
         sub_emitter = [e.duplicate(model_indices) for e in self.emitter]
         sub_transitioner = self.transitioner.duplicate(model_indices)
         subset_cell = MsaHmmCell(sub_lengths, sub_emitter, sub_transitioner)
-        subset_cell.dim = self.dim
         return subset_cell
     
     
     #configures the cell for the backward recursion
     def reverse_direction(self):
         self.transitioner.transpose()
         self.reverse = not self.reverse
```

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/MsaHmmLayer.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/MsaHmmLayer.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,15 +18,18 @@
                                                 return_sequences=True, 
                                                 return_state=True,
                                                 go_backwards=True)
         self.use_prior = use_prior 
         
         
     def build(self, input_shape):
-        self.rnn.build((None, input_shape[-2], input_shape[-1])) #also builds the cell
+        # build the cell 
+        self.cell.build((None, input_shape[-2], input_shape[-1]))
+        # build the RNN layer with a different input shape
+        self.rnn.build((None, input_shape[-2], self.cell.max_num_states))
         self.built = True
         
         
     def forward_recursion(self, inputs, training=False):
         """ Computes the forward recursion for multiple models where each model
             receives a batch of sequences as input.
         Args:
@@ -36,20 +39,21 @@
             log-likelihoods: Shape: (num_model, b)
         """
         #initialize transition- and emission-matricies
         self.cell.recurrent_init()
         num_model, b, seq_len, s = tf.unstack(tf.shape(inputs))
         initial_state = self.cell.get_initial_state(batch_size=b)
         #reshape to 3D inputs for RNN (cell will reshape back in each step)
-        inputs = tf.reshape(inputs, (num_model*b, seq_len, s))
+        emission_probs = self.cell.emission_probs(inputs)
+        emission_probs = tf.reshape(emission_probs, (num_model*b, seq_len, self.cell.max_num_states))
         #do one initialization step
         #this way, tf will compile two versions of the cell call, one with init=True and one without
-        forward_1, step_1_state = self.cell(inputs[:,0], initial_state, training, init=True)
+        forward_1, step_1_state = self.cell(emission_probs[:,0], initial_state, training, init=True)
         #run forward with the output of the first step as initial state
-        forward, _, loglik = self.rnn(inputs[:,1:], initial_state=step_1_state, training=training)
+        forward, _, loglik = self.rnn(emission_probs[:,1:], initial_state=step_1_state, training=training)
         #prepend the separate first step to the other forward steps
         forward = tf.concat([forward_1[:,tf.newaxis], forward], axis=1)
         forward = tf.reshape(forward, (num_model, b, seq_len, -1))
         loglik = tf.reshape(loglik, (num_model, b))
         return forward, loglik
     
     
@@ -60,19 +64,20 @@
             inputs: Sequences. Shape: (num_model, b, seq_len, s)
         Returns:
             backward variables: Shape: (num_model, b, seq_len, q)
         """
         self.cell.recurrent_init()
         num_model, b, seq_len, s = tf.unstack(tf.shape(inputs))
         initial_state = self.cell.get_initial_backward_state(batch_size=b)
-        inputs = tf.reshape(inputs, (num_model*b, seq_len, s))
+        emission_probs = self.cell.emission_probs(inputs)
+        emission_probs = tf.reshape(emission_probs, (num_model*b, seq_len, self.cell.max_num_states))
         self.cell.reverse_direction()
         #note that for backward, we can ignore the initial step like we did it in
         #forward, because we assume that all inputs have terminal tokens
-        backward, _, _ = self.rnn_backward(inputs, initial_state=initial_state)
+        backward, _, _ = self.rnn_backward(emission_probs, initial_state=initial_state)
         self.cell.reverse_direction()
         backward = tf.reshape(backward, (num_model, b, seq_len, -1))
         backward = tf.reverse(backward, [-2])
         return backward
     
     
     def state_posterior_log_probs(self, inputs):
```

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/Priors.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/Priors.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/Training.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/Training.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     ds = ds.batch(batch_size)
     ds = ds.map(lambda i: tf.numpy_function(func=batch_generator,
                 inp=[i], Tout=batch_generator.get_out_types()),
                 num_parallel_calls=tf.data.AUTOTUNE,
                 deterministic=True)
     ds_y = tf.data.Dataset.from_tensor_slices(tf.zeros(1)).batch(batch_size).repeat()
     ds = tf.data.Dataset.zip((ds, ds_y))
-    ds = ds.prefetch(tf.data.AUTOTUNE) #preprocessings and training steps in parallel
+    ds = ds.prefetch(2) #preprocessings and training steps in parallel
     return ds
     
 
 def fit_model(model_generator,
               batch_generator,
               fasta_file,
               indices,
```

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/Transitioner.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/Transitioner.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/Utility.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/Utility.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/Visualize.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/Visualize.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     plt.subplots_adjust(left=0.4, right=0.6, top=0.9, bottom=0.1)
     
     
 def plot_anc_probs(am, 
                    model_index,
                    seqs=[0,1,2], 
                    pos=list(range(6)), 
-                   rescale=True, 
+                   rescale=False, 
                    title="Site-wise ancestral probabilities"):
     n, m = len(seqs), len(pos)
     ds = msa_hmm.train.make_dataset(am.indices[seqs], 
                                     am.batch_generator,
                                     batch_size=n, 
                                     shuffle=False)
     for x,_ in ds:
```

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/Viterbi.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/Viterbi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,49 @@
 import tensorflow as tf
 import numpy as np
 import learnMSA.msa_hmm.Training as train
 import time
 
 
-def viterbi_step(gamma_prev, sequences_i, hmm_cell):
+def viterbi_step(gamma_prev, emission_probs_i, hmm_cell):
     """ Computes one Viterbi dynamic programming step.
     Args:
         gamma_prev: Viterbi values of the previous recursion. Shape (num_models, b, q)
-        sequences_i: i-th vertical sequence slice. Shape (num_models, b, s)
+        emission_probs_i: Emission probabilities of the i-th vertical input slice. Shape (num_models, b, q)
         hmm_cell: HMM cell with the models under which decoding should happen.
     """
     epsilon = tf.constant(np.finfo(np.float32).tiny)
-    
     #very very inefficient!?
     a = tf.expand_dims(hmm_cell.log_A_dense, 1) + tf.expand_dims(gamma_prev, -1)
-    #a = tf.linalg.matmul()
     a = tf.reduce_max(a, axis=-2)
-    
-    b = hmm_cell.emission_probs(sequences_i)
-    b += epsilon
-    b = tf.math.log(b)
+    b = tf.math.log(emission_probs_i + epsilon)
     gamma_next = a + b
     return gamma_next
 
 
 def viterbi_dyn_prog(sequences, hmm_cell):
     """ Logarithmic (underflow safe) viterbi capable of decoding many sequences in parallel on the GPU.
     Args:
         sequences: Tensor. Shape (num_models, b, L, s).
         hmm_cell: HMM cell with the models under which decoding should happen.
     Returns:
         Viterbi values (gamma) per model. Shape (num_model, b, L, q)
     """
     epsilon = tf.constant(np.finfo(np.float32).tiny)
     init = tf.transpose(hmm_cell.init_dist, (1,0,2)) #(num_models, 1, q)
-    b0 = hmm_cell.emission_probs(sequences[:,:,0])
+    emission_probs = hmm_cell.emission_probs(sequences)
+    b0 = emission_probs[:,:,0]
     gamma_val = tf.math.log(init+epsilon) + tf.math.log(b0+epsilon)
     gamma_val = tf.cast(gamma_val, dtype=hmm_cell.dtype) 
     L = tf.shape(sequences)[-2]
     #tf.function-compatible accumulation of results in a dynamically unrolled loop using TensorArray
     gamma = tf.TensorArray(hmm_cell.dtype, size=L)
     gamma = gamma.write(0, gamma_val)
     for i in tf.range(1, L):
-        gamma_val = viterbi_step(gamma_val, sequences[:,:,i], hmm_cell)
+        gamma_val = viterbi_step(gamma_val, emission_probs[:,:,i], hmm_cell)
         gamma = gamma.write(i, gamma_val) 
     gamma = tf.transpose(gamma.stack(), [1,2,0,3])
     return gamma
 
 
 def viterbi_backtracking_step(q, gamma_state, hmm_cell):
     """ Computes a Viterbi backtracking step in parallel for all models and batch elements.
@@ -131,39 +127,39 @@
                             batch_size,
                             shuffle=False)
     seq_len = fasta_file.seq_lens[sorted_indices[-1,0]]+1
     #initialize with terminal states
     state_seqs_max_lik = np.zeros((hmm_cell.num_models, indices.size, seq_len), 
                                   dtype=np.uint16) 
     if encoder:
-        @tf.function(input_signature=[tf.TensorSpec(x.shape, dtype=x.dtype) for x in encoder.inputs])
-        def call_viterbi(inputs, indices):
-            encoded_seq = encoder([inputs, indices])
+        @tf.function(input_signature=[[tf.TensorSpec(x.shape, dtype=x.dtype) for x in encoder.inputs]])
+        def call_viterbi(inputs):
+            encoded_seq = encoder(inputs)
             #todo: this can be improved by encoding only for required models, not all
             encoded_seq = tf.gather(encoded_seq, model_ids, axis=0)
             viterbi_seq = viterbi(encoded_seq, hmm_cell)
             return viterbi_seq
     
     @tf.function(input_signature=(tf.TensorSpec(shape=[None, hmm_cell.num_models, None], dtype=tf.uint8),))
     def call_viterbi_single(inputs):
         if encoder is None:
             seq = tf.transpose(inputs, [1,0,2])
         else:
             seq = encoder(inputs) 
         #todo: this can be improved by encoding only for required models, not all
-        seq = tf.boolean_mask(seq, model_ids, axis=0)
+        seq = tf.gather(seq, model_ids, axis=0)
         return viterbi(seq, hmm_cell)
     
     for i,q in enumerate(hmm_cell.num_states):
         state_seqs_max_lik[i] = q-1 #terminal state
     i = 0     
     for inputs, _ in ds:
         if hasattr(batch_generator, "return_only_sequences") and batch_generator.return_only_sequences:
             state_seqs_max_lik_batch = call_viterbi_single(inputs).numpy()
         else:
-            state_seqs_max_lik_batch = call_viterbi(inputs[0], inputs[1]).numpy()
+            state_seqs_max_lik_batch = call_viterbi(inputs).numpy()
         _,b,l = state_seqs_max_lik_batch.shape
         state_seqs_max_lik[:, i:i+b, :l] = state_seqs_max_lik_batch
         i += b 
     #reorder back to the original order 
     state_seqs_max_lik = state_seqs_max_lik[:,np.argsort(sorted_indices[:,1])]
     return state_seqs_max_lik
```

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/__init__.py` & `learnMSA-1.2.0/learnMSA/msa_hmm/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import learnMSA.msa_hmm.Viterbi as viterbi
 import learnMSA.msa_hmm.Align as align
+import learnMSA.msa_hmm.AlignmentModel as alignment_model
 from learnMSA.msa_hmm.AlignmentModel import AlignmentModel
 import learnMSA.msa_hmm.Fasta as fasta
 import learnMSA.msa_hmm.Training as train
 import learnMSA.msa_hmm.Emitter as emit
 import learnMSA.msa_hmm.Transitioner as trans
 import learnMSA.msa_hmm.MsaHmmCell as cell
 from learnMSA.msa_hmm.MsaHmmCell import MsaHmmCell
```

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.index` & `learnMSA-1.2.0/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.1.2/learnMSA.egg-info/SOURCES.txt` & `learnMSA-1.2.0/learnMSA.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 learnMSA.egg-info/PKG-INFO
 learnMSA.egg-info/SOURCES.txt
 learnMSA.egg-info/dependency_links.txt
 learnMSA.egg-info/entry_points.txt
 learnMSA.egg-info/requires.txt
 learnMSA.egg-info/top_level.txt
 learnMSA/msa_hmm/Align.py
+learnMSA/msa_hmm/AlignInsertions.py
 learnMSA/msa_hmm/AlignmentModel.py
 learnMSA/msa_hmm/AncProbsLayer.py
 learnMSA/msa_hmm/Configuration.py
 learnMSA/msa_hmm/DirichletMixture.py
 learnMSA/msa_hmm/Emitter.py
 learnMSA/msa_hmm/Fasta.py
 learnMSA/msa_hmm/Initializers.py
```

### Comparing `learnMSA-1.1.2/setup.py` & `learnMSA-1.2.0/setup.py`

 * *Files identical despite different names*

