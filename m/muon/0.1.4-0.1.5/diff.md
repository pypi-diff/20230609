# Comparing `tmp/muon-0.1.4.tar.gz` & `tmp/muon-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muon-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "muon-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `muon-0.1.4.tar` & `muon-0.1.5.tar`

### file list

```diff
@@ -1,772 +1,772 @@
--rw-r--r--   0        0        0     4937 2023-06-07 09:07:57.080380 muon-0.1.4/README.md
--rw-r--r--   0        0        0      343 2023-06-07 09:07:57.085093 muon-0.1.4/muon/__init__.py
--rw-r--r--   0        0        0       97 2023-02-20 20:04:01.127617 muon-0.1.4/muon/_atac/__init__.py
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.127870 muon-0.1.4/muon/_atac/_ref/jaspar/MA0002.2.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.128008 muon-0.1.4/muon/_atac/_ref/jaspar/MA0003.4.pfm
--rw-r--r--   0        0        0      149 2023-02-20 20:04:01.128199 muon-0.1.4/muon/_atac/_ref/jaspar/MA0004.1.pfm
--rw-r--r--   0        0        0      149 2023-02-20 20:04:01.128343 muon-0.1.4/muon/_atac/_ref/jaspar/MA0006.1.pfm
--rw-r--r--   0        0        0      466 2023-02-20 20:04:01.128493 muon-0.1.4/muon/_atac/_ref/jaspar/MA0007.3.pfm
--rw-r--r--   0        0        0      435 2023-02-20 20:04:01.128651 muon-0.1.4/muon/_atac/_ref/jaspar/MA0009.2.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.128808 muon-0.1.4/muon/_atac/_ref/jaspar/MA0014.3.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.129002 muon-0.1.4/muon/_atac/_ref/jaspar/MA0017.2.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.129214 muon-0.1.4/muon/_atac/_ref/jaspar/MA0018.4.pfm
--rw-r--r--   0        0        0      318 2023-02-20 20:04:01.129440 muon-0.1.4/muon/_atac/_ref/jaspar/MA0019.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.129703 muon-0.1.4/muon/_atac/_ref/jaspar/MA0024.3.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.129915 muon-0.1.4/muon/_atac/_ref/jaspar/MA0025.2.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.130046 muon-0.1.4/muon/_atac/_ref/jaspar/MA0027.2.pfm
--rw-r--r--   0        0        0      274 2023-02-20 20:04:01.130202 muon-0.1.4/muon/_atac/_ref/jaspar/MA0028.2.pfm
--rw-r--r--   0        0        0      373 2023-02-20 20:04:01.130334 muon-0.1.4/muon/_atac/_ref/jaspar/MA0029.1.pfm
--rw-r--r--   0        0        0      373 2023-02-20 20:04:01.130461 muon-0.1.4/muon/_atac/_ref/jaspar/MA0030.1.pfm
--rw-r--r--   0        0        0      205 2023-02-20 20:04:01.130575 muon-0.1.4/muon/_atac/_ref/jaspar/MA0031.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.130696 muon-0.1.4/muon/_atac/_ref/jaspar/MA0032.2.pfm
--rw-r--r--   0        0        0      185 2023-02-20 20:04:01.130824 muon-0.1.4/muon/_atac/_ref/jaspar/MA0033.2.pfm
--rw-r--r--   0        0        0      304 2023-02-20 20:04:01.131076 muon-0.1.4/muon/_atac/_ref/jaspar/MA0035.4.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.131237 muon-0.1.4/muon/_atac/_ref/jaspar/MA0036.3.pfm
--rw-r--r--   0        0        0      210 2023-02-20 20:04:01.131379 muon-0.1.4/muon/_atac/_ref/jaspar/MA0037.3.pfm
--rw-r--r--   0        0        0      329 2023-02-20 20:04:01.131524 muon-0.1.4/muon/_atac/_ref/jaspar/MA0038.2.pfm
--rw-r--r--   0        0        0      332 2023-02-20 20:04:01.131656 muon-0.1.4/muon/_atac/_ref/jaspar/MA0039.4.pfm
--rw-r--r--   0        0        0      288 2023-02-20 20:04:01.131787 muon-0.1.4/muon/_atac/_ref/jaspar/MA0040.1.pfm
--rw-r--r--   0        0        0      318 2023-02-20 20:04:01.131919 muon-0.1.4/muon/_atac/_ref/jaspar/MA0041.1.pfm
--rw-r--r--   0        0        0      182 2023-02-20 20:04:01.132055 muon-0.1.4/muon/_atac/_ref/jaspar/MA0042.2.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.132205 muon-0.1.4/muon/_atac/_ref/jaspar/MA0043.3.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.132361 muon-0.1.4/muon/_atac/_ref/jaspar/MA0046.2.pfm
--rw-r--r--   0        0        0      305 2023-02-20 20:04:01.132497 muon-0.1.4/muon/_atac/_ref/jaspar/MA0047.3.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.132642 muon-0.1.4/muon/_atac/_ref/jaspar/MA0048.2.pfm
--rw-r--r--   0        0        0      576 2023-02-20 20:04:01.132775 muon-0.1.4/muon/_atac/_ref/jaspar/MA0050.2.pfm
--rw-r--r--   0        0        0      484 2023-02-20 20:04:01.132908 muon-0.1.4/muon/_atac/_ref/jaspar/MA0051.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.133039 muon-0.1.4/muon/_atac/_ref/jaspar/MA0052.4.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.133170 muon-0.1.4/muon/_atac/_ref/jaspar/MA0056.2.pfm
--rw-r--r--   0        0        0      260 2023-02-20 20:04:01.133293 muon-0.1.4/muon/_atac/_ref/jaspar/MA0057.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.133546 muon-0.1.4/muon/_atac/_ref/jaspar/MA0058.3.pfm
--rw-r--r--   0        0        0      288 2023-02-20 20:04:01.133717 muon-0.1.4/muon/_atac/_ref/jaspar/MA0059.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.133873 muon-0.1.4/muon/_atac/_ref/jaspar/MA0060.3.pfm
--rw-r--r--   0        0        0      388 2023-02-20 20:04:01.134025 muon-0.1.4/muon/_atac/_ref/jaspar/MA0062.3.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.134166 muon-0.1.4/muon/_atac/_ref/jaspar/MA0063.2.pfm
--rw-r--r--   0        0        0      407 2023-02-20 20:04:01.134332 muon-0.1.4/muon/_atac/_ref/jaspar/MA0065.2.pfm
--rw-r--r--   0        0        0      541 2023-02-20 20:04:01.134684 muon-0.1.4/muon/_atac/_ref/jaspar/MA0066.1.pfm
--rw-r--r--   0        0        0      205 2023-02-20 20:04:01.134941 muon-0.1.4/muon/_atac/_ref/jaspar/MA0067.1.pfm
--rw-r--r--   0        0        0      210 2023-02-20 20:04:01.135150 muon-0.1.4/muon/_atac/_ref/jaspar/MA0068.2.pfm
--rw-r--r--   0        0        0      373 2023-02-20 20:04:01.135352 muon-0.1.4/muon/_atac/_ref/jaspar/MA0069.1.pfm
--rw-r--r--   0        0        0      316 2023-02-20 20:04:01.135495 muon-0.1.4/muon/_atac/_ref/jaspar/MA0070.1.pfm
--rw-r--r--   0        0        0      261 2023-02-20 20:04:01.135630 muon-0.1.4/muon/_atac/_ref/jaspar/MA0071.1.pfm
--rw-r--r--   0        0        0      373 2023-02-20 20:04:01.135784 muon-0.1.4/muon/_atac/_ref/jaspar/MA0072.1.pfm
--rw-r--r--   0        0        0      540 2023-02-20 20:04:01.135917 muon-0.1.4/muon/_atac/_ref/jaspar/MA0073.1.pfm
--rw-r--r--   0        0        0      400 2023-02-20 20:04:01.136054 muon-0.1.4/muon/_atac/_ref/jaspar/MA0074.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.136186 muon-0.1.4/muon/_atac/_ref/jaspar/MA0075.3.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.136308 muon-0.1.4/muon/_atac/_ref/jaspar/MA0076.2.pfm
--rw-r--r--   0        0        0      233 2023-02-20 20:04:01.136474 muon-0.1.4/muon/_atac/_ref/jaspar/MA0077.1.pfm
--rw-r--r--   0        0        0      232 2023-02-20 20:04:01.136632 muon-0.1.4/muon/_atac/_ref/jaspar/MA0078.1.pfm
--rw-r--r--   0        0        0      414 2023-02-20 20:04:01.136781 muon-0.1.4/muon/_atac/_ref/jaspar/MA0079.4.pfm
--rw-r--r--   0        0        0      556 2023-02-20 20:04:01.136915 muon-0.1.4/muon/_atac/_ref/jaspar/MA0080.5.pfm
--rw-r--r--   0        0        0      441 2023-02-20 20:04:01.137065 muon-0.1.4/muon/_atac/_ref/jaspar/MA0081.2.pfm
--rw-r--r--   0        0        0      436 2023-02-20 20:04:01.137219 muon-0.1.4/muon/_atac/_ref/jaspar/MA0083.3.pfm
--rw-r--r--   0        0        0      233 2023-02-20 20:04:01.137344 muon-0.1.4/muon/_atac/_ref/jaspar/MA0084.1.pfm
--rw-r--r--   0        0        0      177 2023-02-20 20:04:01.137576 muon-0.1.4/muon/_atac/_ref/jaspar/MA0087.1.pfm
--rw-r--r--   0        0        0      436 2023-02-20 20:04:01.137761 muon-0.1.4/muon/_atac/_ref/jaspar/MA0088.2.pfm
--rw-r--r--   0        0        0      437 2023-02-20 20:04:01.137906 muon-0.1.4/muon/_atac/_ref/jaspar/MA0089.2.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.138046 muon-0.1.4/muon/_atac/_ref/jaspar/MA0090.3.pfm
--rw-r--r--   0        0        0      318 2023-02-20 20:04:01.138183 muon-0.1.4/muon/_atac/_ref/jaspar/MA0091.1.pfm
--rw-r--r--   0        0        0      261 2023-02-20 20:04:01.138326 muon-0.1.4/muon/_atac/_ref/jaspar/MA0092.1.pfm
--rw-r--r--   0        0        0      388 2023-02-20 20:04:01.138469 muon-0.1.4/muon/_atac/_ref/jaspar/MA0093.3.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.138600 muon-0.1.4/muon/_atac/_ref/jaspar/MA0095.2.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.138839 muon-0.1.4/muon/_atac/_ref/jaspar/MA0098.3.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.138997 muon-0.1.4/muon/_atac/_ref/jaspar/MA0099.3.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.139184 muon-0.1.4/muon/_atac/_ref/jaspar/MA0100.3.pfm
--rw-r--r--   0        0        0      260 2023-02-20 20:04:01.139338 muon-0.1.4/muon/_atac/_ref/jaspar/MA0101.1.pfm
--rw-r--r--   0        0        0      388 2023-02-20 20:04:01.139523 muon-0.1.4/muon/_atac/_ref/jaspar/MA0102.4.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.139819 muon-0.1.4/muon/_atac/_ref/jaspar/MA0103.3.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.140063 muon-0.1.4/muon/_atac/_ref/jaspar/MA0104.4.pfm
--rw-r--r--   0        0        0      354 2023-02-20 20:04:01.140242 muon-0.1.4/muon/_atac/_ref/jaspar/MA0105.4.pfm
--rw-r--r--   0        0        0      496 2023-02-20 20:04:01.140644 muon-0.1.4/muon/_atac/_ref/jaspar/MA0106.3.pfm
--rw-r--r--   0        0        0      261 2023-02-20 20:04:01.141075 muon-0.1.4/muon/_atac/_ref/jaspar/MA0107.1.pfm
--rw-r--r--   0        0        0      406 2023-02-20 20:04:01.141327 muon-0.1.4/muon/_atac/_ref/jaspar/MA0108.2.pfm
--rw-r--r--   0        0        0      264 2023-02-20 20:04:01.141518 muon-0.1.4/muon/_atac/_ref/jaspar/MA0109.1.pfm
--rw-r--r--   0        0        0      288 2023-02-20 20:04:01.141706 muon-0.1.4/muon/_atac/_ref/jaspar/MA0111.1.pfm
--rw-r--r--   0        0        0      462 2023-02-20 20:04:01.142064 muon-0.1.4/muon/_atac/_ref/jaspar/MA0112.3.pfm
--rw-r--r--   0        0        0      468 2023-02-20 20:04:01.142282 muon-0.1.4/muon/_atac/_ref/jaspar/MA0113.3.pfm
--rw-r--r--   0        0        0      359 2023-02-20 20:04:01.142434 muon-0.1.4/muon/_atac/_ref/jaspar/MA0114.4.pfm
--rw-r--r--   0        0        0      457 2023-02-20 20:04:01.142706 muon-0.1.4/muon/_atac/_ref/jaspar/MA0115.1.pfm
--rw-r--r--   0        0        0      401 2023-02-20 20:04:01.143015 muon-0.1.4/muon/_atac/_ref/jaspar/MA0116.1.pfm
--rw-r--r--   0        0        0      325 2023-02-20 20:04:01.143269 muon-0.1.4/muon/_atac/_ref/jaspar/MA0117.2.pfm
--rw-r--r--   0        0        0      373 2023-02-20 20:04:01.143565 muon-0.1.4/muon/_atac/_ref/jaspar/MA0119.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.143773 muon-0.1.4/muon/_atac/_ref/jaspar/MA0122.3.pfm
--rw-r--r--   0        0        0      242 2023-02-20 20:04:01.144054 muon-0.1.4/muon/_atac/_ref/jaspar/MA0124.2.pfm
--rw-r--r--   0        0        0      205 2023-02-20 20:04:01.144340 muon-0.1.4/muon/_atac/_ref/jaspar/MA0125.1.pfm
--rw-r--r--   0        0        0      148 2023-02-20 20:04:01.144556 muon-0.1.4/muon/_atac/_ref/jaspar/MA0130.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.144775 muon-0.1.4/muon/_atac/_ref/jaspar/MA0131.2.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.144986 muon-0.1.4/muon/_atac/_ref/jaspar/MA0132.2.pfm
--rw-r--r--   0        0        0      344 2023-02-20 20:04:01.145188 muon-0.1.4/muon/_atac/_ref/jaspar/MA0135.1.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.145402 muon-0.1.4/muon/_atac/_ref/jaspar/MA0136.2.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.145697 muon-0.1.4/muon/_atac/_ref/jaspar/MA0137.3.pfm
--rw-r--r--   0        0        0      576 2023-02-20 20:04:01.145894 muon-0.1.4/muon/_atac/_ref/jaspar/MA0138.2.pfm
--rw-r--r--   0        0        0      518 2023-02-20 20:04:01.146162 muon-0.1.4/muon/_atac/_ref/jaspar/MA0139.1.pfm
--rw-r--r--   0        0        0      494 2023-02-20 20:04:01.146437 muon-0.1.4/muon/_atac/_ref/jaspar/MA0140.2.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.146654 muon-0.1.4/muon/_atac/_ref/jaspar/MA0141.3.pfm
--rw-r--r--   0        0        0      406 2023-02-20 20:04:01.146921 muon-0.1.4/muon/_atac/_ref/jaspar/MA0142.1.pfm
--rw-r--r--   0        0        0      304 2023-02-20 20:04:01.147096 muon-0.1.4/muon/_atac/_ref/jaspar/MA0143.4.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.147245 muon-0.1.4/muon/_atac/_ref/jaspar/MA0144.2.pfm
--rw-r--r--   0        0        0      266 2023-02-20 20:04:01.147379 muon-0.1.4/muon/_atac/_ref/jaspar/MA0145.3.pfm
--rw-r--r--   0        0        0      378 2023-02-20 20:04:01.147531 muon-0.1.4/muon/_atac/_ref/jaspar/MA0146.2.pfm
--rw-r--r--   0        0        0      327 2023-02-20 20:04:01.147676 muon-0.1.4/muon/_atac/_ref/jaspar/MA0147.3.pfm
--rw-r--r--   0        0        0      333 2023-02-20 20:04:01.147806 muon-0.1.4/muon/_atac/_ref/jaspar/MA0148.4.pfm
--rw-r--r--   0        0        0      486 2023-02-20 20:04:01.147960 muon-0.1.4/muon/_atac/_ref/jaspar/MA0149.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.148257 muon-0.1.4/muon/_atac/_ref/jaspar/MA0150.2.pfm
--rw-r--r--   0        0        0      149 2023-02-20 20:04:01.148412 muon-0.1.4/muon/_atac/_ref/jaspar/MA0151.1.pfm
--rw-r--r--   0        0        0      177 2023-02-20 20:04:01.148598 muon-0.1.4/muon/_atac/_ref/jaspar/MA0152.1.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.148839 muon-0.1.4/muon/_atac/_ref/jaspar/MA0153.2.pfm
--rw-r--r--   0        0        0      415 2023-02-20 20:04:01.149056 muon-0.1.4/muon/_atac/_ref/jaspar/MA0154.4.pfm
--rw-r--r--   0        0        0      317 2023-02-20 20:04:01.149246 muon-0.1.4/muon/_atac/_ref/jaspar/MA0155.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.149377 muon-0.1.4/muon/_atac/_ref/jaspar/MA0156.2.pfm
--rw-r--r--   0        0        0      207 2023-02-20 20:04:01.149513 muon-0.1.4/muon/_atac/_ref/jaspar/MA0157.2.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.149648 muon-0.1.4/muon/_atac/_ref/jaspar/MA0158.2.pfm
--rw-r--r--   0        0        0      458 2023-02-20 20:04:01.149783 muon-0.1.4/muon/_atac/_ref/jaspar/MA0159.1.pfm
--rw-r--r--   0        0        0      204 2023-02-20 20:04:01.149967 muon-0.1.4/muon/_atac/_ref/jaspar/MA0160.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.150213 muon-0.1.4/muon/_atac/_ref/jaspar/MA0161.2.pfm
--rw-r--r--   0        0        0      385 2023-02-20 20:04:01.150429 muon-0.1.4/muon/_atac/_ref/jaspar/MA0162.4.pfm
--rw-r--r--   0        0        0      373 2023-02-20 20:04:01.150577 muon-0.1.4/muon/_atac/_ref/jaspar/MA0163.1.pfm
--rw-r--r--   0        0        0      177 2023-02-20 20:04:01.150710 muon-0.1.4/muon/_atac/_ref/jaspar/MA0164.1.pfm
--rw-r--r--   0        0        0      409 2023-02-20 20:04:01.150852 muon-0.1.4/muon/_atac/_ref/jaspar/MA0258.2.pfm
--rw-r--r--   0        0        0      207 2023-02-20 20:04:01.151007 muon-0.1.4/muon/_atac/_ref/jaspar/MA0259.1.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.151132 muon-0.1.4/muon/_atac/_ref/jaspar/MA0442.2.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.151252 muon-0.1.4/muon/_atac/_ref/jaspar/MA0461.2.pfm
--rw-r--r--   0        0        0      302 2023-02-20 20:04:01.151446 muon-0.1.4/muon/_atac/_ref/jaspar/MA0462.2.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.151583 muon-0.1.4/muon/_atac/_ref/jaspar/MA0463.2.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.151712 muon-0.1.4/muon/_atac/_ref/jaspar/MA0464.2.pfm
--rw-r--r--   0        0        0      329 2023-02-20 20:04:01.151832 muon-0.1.4/muon/_atac/_ref/jaspar/MA0465.2.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.151948 muon-0.1.4/muon/_atac/_ref/jaspar/MA0466.2.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.152062 muon-0.1.4/muon/_atac/_ref/jaspar/MA0467.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.152175 muon-0.1.4/muon/_atac/_ref/jaspar/MA0468.1.pfm
--rw-r--r--   0        0        0      441 2023-02-20 20:04:01.152287 muon-0.1.4/muon/_atac/_ref/jaspar/MA0469.3.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.152401 muon-0.1.4/muon/_atac/_ref/jaspar/MA0470.2.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.152672 muon-0.1.4/muon/_atac/_ref/jaspar/MA0471.2.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.152867 muon-0.1.4/muon/_atac/_ref/jaspar/MA0472.2.pfm
--rw-r--r--   0        0        0      386 2023-02-20 20:04:01.153007 muon-0.1.4/muon/_atac/_ref/jaspar/MA0473.3.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.153137 muon-0.1.4/muon/_atac/_ref/jaspar/MA0474.2.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.153257 muon-0.1.4/muon/_atac/_ref/jaspar/MA0475.2.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.153372 muon-0.1.4/muon/_atac/_ref/jaspar/MA0476.1.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.153488 muon-0.1.4/muon/_atac/_ref/jaspar/MA0477.2.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.153639 muon-0.1.4/muon/_atac/_ref/jaspar/MA0478.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.153938 muon-0.1.4/muon/_atac/_ref/jaspar/MA0479.1.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.154153 muon-0.1.4/muon/_atac/_ref/jaspar/MA0480.1.pfm
--rw-r--r--   0        0        0      304 2023-02-20 20:04:01.154318 muon-0.1.4/muon/_atac/_ref/jaspar/MA0481.3.pfm
--rw-r--r--   0        0        0      332 2023-02-20 20:04:01.154488 muon-0.1.4/muon/_atac/_ref/jaspar/MA0482.2.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.154636 muon-0.1.4/muon/_atac/_ref/jaspar/MA0483.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.154780 muon-0.1.4/muon/_atac/_ref/jaspar/MA0484.2.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.154902 muon-0.1.4/muon/_atac/_ref/jaspar/MA0485.2.pfm
--rw-r--r--   0        0        0      350 2023-02-20 20:04:01.155021 muon-0.1.4/muon/_atac/_ref/jaspar/MA0486.2.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.155249 muon-0.1.4/muon/_atac/_ref/jaspar/MA0488.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.155454 muon-0.1.4/muon/_atac/_ref/jaspar/MA0489.1.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.155691 muon-0.1.4/muon/_atac/_ref/jaspar/MA0490.2.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.155911 muon-0.1.4/muon/_atac/_ref/jaspar/MA0491.2.pfm
--rw-r--r--   0        0        0      413 2023-02-20 20:04:01.156132 muon-0.1.4/muon/_atac/_ref/jaspar/MA0492.1.pfm
--rw-r--r--   0        0        0      294 2023-02-20 20:04:01.156332 muon-0.1.4/muon/_atac/_ref/jaspar/MA0493.1.pfm
--rw-r--r--   0        0        0      517 2023-02-20 20:04:01.156652 muon-0.1.4/muon/_atac/_ref/jaspar/MA0494.1.pfm
--rw-r--r--   0        0        0      442 2023-02-20 20:04:01.157021 muon-0.1.4/muon/_atac/_ref/jaspar/MA0495.3.pfm
--rw-r--r--   0        0        0      415 2023-02-20 20:04:01.157261 muon-0.1.4/muon/_atac/_ref/jaspar/MA0496.3.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.157480 muon-0.1.4/muon/_atac/_ref/jaspar/MA0497.1.pfm
--rw-r--r--   0        0        0      191 2023-02-20 20:04:01.157826 muon-0.1.4/muon/_atac/_ref/jaspar/MA0498.2.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.158061 muon-0.1.4/muon/_atac/_ref/jaspar/MA0499.2.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.158305 muon-0.1.4/muon/_atac/_ref/jaspar/MA0500.2.pfm
--rw-r--r--   0        0        0      405 2023-02-20 20:04:01.158537 muon-0.1.4/muon/_atac/_ref/jaspar/MA0501.1.pfm
--rw-r--r--   0        0        0      327 2023-02-20 20:04:01.158753 muon-0.1.4/muon/_atac/_ref/jaspar/MA0502.2.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.158959 muon-0.1.4/muon/_atac/_ref/jaspar/MA0503.1.pfm
--rw-r--r--   0        0        0      406 2023-02-20 20:04:01.159150 muon-0.1.4/muon/_atac/_ref/jaspar/MA0504.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.159288 muon-0.1.4/muon/_atac/_ref/jaspar/MA0505.1.pfm
--rw-r--r--   0        0        0      295 2023-02-20 20:04:01.159411 muon-0.1.4/muon/_atac/_ref/jaspar/MA0506.1.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.159538 muon-0.1.4/muon/_atac/_ref/jaspar/MA0507.1.pfm
--rw-r--r--   0        0        0      302 2023-02-20 20:04:01.159738 muon-0.1.4/muon/_atac/_ref/jaspar/MA0508.3.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.159929 muon-0.1.4/muon/_atac/_ref/jaspar/MA0509.2.pfm
--rw-r--r--   0        0        0      437 2023-02-20 20:04:01.160149 muon-0.1.4/muon/_atac/_ref/jaspar/MA0510.2.pfm
--rw-r--r--   0        0        0      243 2023-02-20 20:04:01.160350 muon-0.1.4/muon/_atac/_ref/jaspar/MA0511.2.pfm
--rw-r--r--   0        0        0      386 2023-02-20 20:04:01.160507 muon-0.1.4/muon/_atac/_ref/jaspar/MA0512.2.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.160645 muon-0.1.4/muon/_atac/_ref/jaspar/MA0513.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.160795 muon-0.1.4/muon/_atac/_ref/jaspar/MA0514.1.pfm
--rw-r--r--   0        0        0      264 2023-02-20 20:04:01.160932 muon-0.1.4/muon/_atac/_ref/jaspar/MA0515.1.pfm
--rw-r--r--   0        0        0      464 2023-02-20 20:04:01.161140 muon-0.1.4/muon/_atac/_ref/jaspar/MA0516.2.pfm
--rw-r--r--   0        0        0      405 2023-02-20 20:04:01.161317 muon-0.1.4/muon/_atac/_ref/jaspar/MA0517.1.pfm
--rw-r--r--   0        0        0      382 2023-02-20 20:04:01.161453 muon-0.1.4/muon/_atac/_ref/jaspar/MA0518.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.161623 muon-0.1.4/muon/_atac/_ref/jaspar/MA0519.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.161755 muon-0.1.4/muon/_atac/_ref/jaspar/MA0520.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.161909 muon-0.1.4/muon/_atac/_ref/jaspar/MA0521.1.pfm
--rw-r--r--   0        0        0      301 2023-02-20 20:04:01.162094 muon-0.1.4/muon/_atac/_ref/jaspar/MA0522.3.pfm
--rw-r--r--   0        0        0      382 2023-02-20 20:04:01.162248 muon-0.1.4/muon/_atac/_ref/jaspar/MA0523.1.pfm
--rw-r--r--   0        0        0      327 2023-02-20 20:04:01.162382 muon-0.1.4/muon/_atac/_ref/jaspar/MA0524.2.pfm
--rw-r--r--   0        0        0      492 2023-02-20 20:04:01.162529 muon-0.1.4/muon/_atac/_ref/jaspar/MA0525.2.pfm
--rw-r--r--   0        0        0      385 2023-02-20 20:04:01.162664 muon-0.1.4/muon/_atac/_ref/jaspar/MA0526.3.pfm
--rw-r--r--   0        0        0      407 2023-02-20 20:04:01.162838 muon-0.1.4/muon/_atac/_ref/jaspar/MA0527.1.pfm
--rw-r--r--   0        0        0      331 2023-02-20 20:04:01.162976 muon-0.1.4/muon/_atac/_ref/jaspar/MA0528.2.pfm
--rw-r--r--   0        0        0      404 2023-02-20 20:04:01.163165 muon-0.1.4/muon/_atac/_ref/jaspar/MA0591.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.163301 muon-0.1.4/muon/_atac/_ref/jaspar/MA0592.3.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.163417 muon-0.1.4/muon/_atac/_ref/jaspar/MA0593.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.163561 muon-0.1.4/muon/_atac/_ref/jaspar/MA0594.2.pfm
--rw-r--r--   0        0        0      263 2023-02-20 20:04:01.163688 muon-0.1.4/muon/_atac/_ref/jaspar/MA0595.1.pfm
--rw-r--r--   0        0        0      262 2023-02-20 20:04:01.163825 muon-0.1.4/muon/_atac/_ref/jaspar/MA0596.1.pfm
--rw-r--r--   0        0        0      236 2023-02-20 20:04:01.163954 muon-0.1.4/muon/_atac/_ref/jaspar/MA0597.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.164202 muon-0.1.4/muon/_atac/_ref/jaspar/MA0598.3.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.164422 muon-0.1.4/muon/_atac/_ref/jaspar/MA0599.1.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.164636 muon-0.1.4/muon/_atac/_ref/jaspar/MA0600.2.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.164777 muon-0.1.4/muon/_atac/_ref/jaspar/MA0601.1.pfm
--rw-r--r--   0        0        0      376 2023-02-20 20:04:01.164899 muon-0.1.4/muon/_atac/_ref/jaspar/MA0602.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.165015 muon-0.1.4/muon/_atac/_ref/jaspar/MA0603.1.pfm
--rw-r--r--   0        0        0      210 2023-02-20 20:04:01.165128 muon-0.1.4/muon/_atac/_ref/jaspar/MA0604.1.pfm
--rw-r--r--   0        0        0      329 2023-02-20 20:04:01.165239 muon-0.1.4/muon/_atac/_ref/jaspar/MA0605.2.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.165380 muon-0.1.4/muon/_atac/_ref/jaspar/MA0606.1.pfm
--rw-r--r--   0        0        0      210 2023-02-20 20:04:01.165573 muon-0.1.4/muon/_atac/_ref/jaspar/MA0607.1.pfm
--rw-r--r--   0        0        0      236 2023-02-20 20:04:01.165690 muon-0.1.4/muon/_atac/_ref/jaspar/MA0608.1.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.165810 muon-0.1.4/muon/_atac/_ref/jaspar/MA0609.2.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.165928 muon-0.1.4/muon/_atac/_ref/jaspar/MA0610.1.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.166161 muon-0.1.4/muon/_atac/_ref/jaspar/MA0611.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.166333 muon-0.1.4/muon/_atac/_ref/jaspar/MA0612.2.pfm
--rw-r--r--   0        0        0      208 2023-02-20 20:04:01.166588 muon-0.1.4/muon/_atac/_ref/jaspar/MA0613.1.pfm
--rw-r--r--   0        0        0      208 2023-02-20 20:04:01.166762 muon-0.1.4/muon/_atac/_ref/jaspar/MA0614.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.166996 muon-0.1.4/muon/_atac/_ref/jaspar/MA0615.1.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.167151 muon-0.1.4/muon/_atac/_ref/jaspar/MA0616.2.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.167289 muon-0.1.4/muon/_atac/_ref/jaspar/MA0618.1.pfm
--rw-r--r--   0        0        0      239 2023-02-20 20:04:01.167427 muon-0.1.4/muon/_atac/_ref/jaspar/MA0619.1.pfm
--rw-r--r--   0        0        0      500 2023-02-20 20:04:01.167646 muon-0.1.4/muon/_atac/_ref/jaspar/MA0620.3.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.167866 muon-0.1.4/muon/_atac/_ref/jaspar/MA0621.1.pfm
--rw-r--r--   0        0        0      211 2023-02-20 20:04:01.168043 muon-0.1.4/muon/_atac/_ref/jaspar/MA0622.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.168207 muon-0.1.4/muon/_atac/_ref/jaspar/MA0623.2.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.168456 muon-0.1.4/muon/_atac/_ref/jaspar/MA0624.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.168661 muon-0.1.4/muon/_atac/_ref/jaspar/MA0625.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.168872 muon-0.1.4/muon/_atac/_ref/jaspar/MA0626.1.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.169038 muon-0.1.4/muon/_atac/_ref/jaspar/MA0627.2.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.169194 muon-0.1.4/muon/_atac/_ref/jaspar/MA0628.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.169321 muon-0.1.4/muon/_atac/_ref/jaspar/MA0629.1.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.169451 muon-0.1.4/muon/_atac/_ref/jaspar/MA0630.1.pfm
--rw-r--r--   0        0        0      459 2023-02-20 20:04:01.169598 muon-0.1.4/muon/_atac/_ref/jaspar/MA0631.1.pfm
--rw-r--r--   0        0        0      275 2023-02-20 20:04:01.169737 muon-0.1.4/muon/_atac/_ref/jaspar/MA0632.2.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.169869 muon-0.1.4/muon/_atac/_ref/jaspar/MA0633.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.170033 muon-0.1.4/muon/_atac/_ref/jaspar/MA0634.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.170169 muon-0.1.4/muon/_atac/_ref/jaspar/MA0635.1.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.170404 muon-0.1.4/muon/_atac/_ref/jaspar/MA0636.1.pfm
--rw-r--r--   0        0        0      407 2023-02-20 20:04:01.170543 muon-0.1.4/muon/_atac/_ref/jaspar/MA0637.1.pfm
--rw-r--r--   0        0        0      377 2023-02-20 20:04:01.170680 muon-0.1.4/muon/_atac/_ref/jaspar/MA0638.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.170835 muon-0.1.4/muon/_atac/_ref/jaspar/MA0639.1.pfm
--rw-r--r--   0        0        0      388 2023-02-20 20:04:01.170962 muon-0.1.4/muon/_atac/_ref/jaspar/MA0640.2.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.171090 muon-0.1.4/muon/_atac/_ref/jaspar/MA0641.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.171220 muon-0.1.4/muon/_atac/_ref/jaspar/MA0642.1.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.171496 muon-0.1.4/muon/_atac/_ref/jaspar/MA0643.1.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.171673 muon-0.1.4/muon/_atac/_ref/jaspar/MA0644.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.171821 muon-0.1.4/muon/_atac/_ref/jaspar/MA0645.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.171958 muon-0.1.4/muon/_atac/_ref/jaspar/MA0646.1.pfm
--rw-r--r--   0        0        0      325 2023-02-20 20:04:01.172098 muon-0.1.4/muon/_atac/_ref/jaspar/MA0647.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.172232 muon-0.1.4/muon/_atac/_ref/jaspar/MA0648.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.172364 muon-0.1.4/muon/_atac/_ref/jaspar/MA0649.1.pfm
--rw-r--r--   0        0        0      295 2023-02-20 20:04:01.172489 muon-0.1.4/muon/_atac/_ref/jaspar/MA0650.2.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.172628 muon-0.1.4/muon/_atac/_ref/jaspar/MA0651.1.pfm
--rw-r--r--   0        0        0      383 2023-02-20 20:04:01.172839 muon-0.1.4/muon/_atac/_ref/jaspar/MA0652.1.pfm
--rw-r--r--   0        0        0      407 2023-02-20 20:04:01.172988 muon-0.1.4/muon/_atac/_ref/jaspar/MA0653.1.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.173125 muon-0.1.4/muon/_atac/_ref/jaspar/MA0654.1.pfm
--rw-r--r--   0        0        0      238 2023-02-20 20:04:01.173267 muon-0.1.4/muon/_atac/_ref/jaspar/MA0655.1.pfm
--rw-r--r--   0        0        0      329 2023-02-20 20:04:01.173418 muon-0.1.4/muon/_atac/_ref/jaspar/MA0656.1.pfm
--rw-r--r--   0        0        0      493 2023-02-20 20:04:01.173560 muon-0.1.4/muon/_atac/_ref/jaspar/MA0657.1.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.173804 muon-0.1.4/muon/_atac/_ref/jaspar/MA0658.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.173966 muon-0.1.4/muon/_atac/_ref/jaspar/MA0659.2.pfm
--rw-r--r--   0        0        0      325 2023-02-20 20:04:01.174124 muon-0.1.4/muon/_atac/_ref/jaspar/MA0660.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.174260 muon-0.1.4/muon/_atac/_ref/jaspar/MA0661.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.174396 muon-0.1.4/muon/_atac/_ref/jaspar/MA0662.1.pfm
--rw-r--r--   0        0        0      265 2023-02-20 20:04:01.174604 muon-0.1.4/muon/_atac/_ref/jaspar/MA0663.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.174781 muon-0.1.4/muon/_atac/_ref/jaspar/MA0664.1.pfm
--rw-r--r--   0        0        0      262 2023-02-20 20:04:01.174955 muon-0.1.4/muon/_atac/_ref/jaspar/MA0665.1.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.175095 muon-0.1.4/muon/_atac/_ref/jaspar/MA0666.1.pfm
--rw-r--r--   0        0        0      264 2023-02-20 20:04:01.175229 muon-0.1.4/muon/_atac/_ref/jaspar/MA0667.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.175401 muon-0.1.4/muon/_atac/_ref/jaspar/MA0668.1.pfm
--rw-r--r--   0        0        0      264 2023-02-20 20:04:01.175571 muon-0.1.4/muon/_atac/_ref/jaspar/MA0669.1.pfm
--rw-r--r--   0        0        0      276 2023-02-20 20:04:01.175727 muon-0.1.4/muon/_atac/_ref/jaspar/MA0670.1.pfm
--rw-r--r--   0        0        0      244 2023-02-20 20:04:01.175867 muon-0.1.4/muon/_atac/_ref/jaspar/MA0671.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.175993 muon-0.1.4/muon/_atac/_ref/jaspar/MA0672.1.pfm
--rw-r--r--   0        0        0      243 2023-02-20 20:04:01.176116 muon-0.1.4/muon/_atac/_ref/jaspar/MA0673.1.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.176250 muon-0.1.4/muon/_atac/_ref/jaspar/MA0674.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.176388 muon-0.1.4/muon/_atac/_ref/jaspar/MA0675.1.pfm
--rw-r--r--   0        0        0      241 2023-02-20 20:04:01.176522 muon-0.1.4/muon/_atac/_ref/jaspar/MA0676.1.pfm
--rw-r--r--   0        0        0      378 2023-02-20 20:04:01.176722 muon-0.1.4/muon/_atac/_ref/jaspar/MA0677.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.176948 muon-0.1.4/muon/_atac/_ref/jaspar/MA0678.1.pfm
--rw-r--r--   0        0        0      444 2023-02-20 20:04:01.177157 muon-0.1.4/muon/_atac/_ref/jaspar/MA0679.2.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.177358 muon-0.1.4/muon/_atac/_ref/jaspar/MA0680.1.pfm
--rw-r--r--   0        0        0      442 2023-02-20 20:04:01.177563 muon-0.1.4/muon/_atac/_ref/jaspar/MA0681.2.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.177763 muon-0.1.4/muon/_atac/_ref/jaspar/MA0682.2.pfm
--rw-r--r--   0        0        0      437 2023-02-20 20:04:01.177896 muon-0.1.4/muon/_atac/_ref/jaspar/MA0683.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.178029 muon-0.1.4/muon/_atac/_ref/jaspar/MA0684.2.pfm
--rw-r--r--   0        0        0      466 2023-02-20 20:04:01.178213 muon-0.1.4/muon/_atac/_ref/jaspar/MA0685.1.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.178389 muon-0.1.4/muon/_atac/_ref/jaspar/MA0686.1.pfm
--rw-r--r--   0        0        0      377 2023-02-20 20:04:01.178534 muon-0.1.4/muon/_atac/_ref/jaspar/MA0687.1.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.178676 muon-0.1.4/muon/_atac/_ref/jaspar/MA0688.1.pfm
--rw-r--r--   0        0        0      294 2023-02-20 20:04:01.178813 muon-0.1.4/muon/_atac/_ref/jaspar/MA0689.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.179025 muon-0.1.4/muon/_atac/_ref/jaspar/MA0690.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.179242 muon-0.1.4/muon/_atac/_ref/jaspar/MA0691.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.179437 muon-0.1.4/muon/_atac/_ref/jaspar/MA0692.1.pfm
--rw-r--r--   0        0        0      211 2023-02-20 20:04:01.179612 muon-0.1.4/muon/_atac/_ref/jaspar/MA0693.2.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.179747 muon-0.1.4/muon/_atac/_ref/jaspar/MA0694.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.179892 muon-0.1.4/muon/_atac/_ref/jaspar/MA0695.1.pfm
--rw-r--r--   0        0        0      385 2023-02-20 20:04:01.180043 muon-0.1.4/muon/_atac/_ref/jaspar/MA0696.1.pfm
--rw-r--r--   0        0        0      405 2023-02-20 20:04:01.180186 muon-0.1.4/muon/_atac/_ref/jaspar/MA0697.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.180340 muon-0.1.4/muon/_atac/_ref/jaspar/MA0698.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.180559 muon-0.1.4/muon/_atac/_ref/jaspar/MA0699.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.180728 muon-0.1.4/muon/_atac/_ref/jaspar/MA0700.2.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.180873 muon-0.1.4/muon/_atac/_ref/jaspar/MA0701.2.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.181019 muon-0.1.4/muon/_atac/_ref/jaspar/MA0702.2.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.181138 muon-0.1.4/muon/_atac/_ref/jaspar/MA0703.2.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.181257 muon-0.1.4/muon/_atac/_ref/jaspar/MA0704.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.181388 muon-0.1.4/muon/_atac/_ref/jaspar/MA0705.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.181560 muon-0.1.4/muon/_atac/_ref/jaspar/MA0706.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.181849 muon-0.1.4/muon/_atac/_ref/jaspar/MA0707.1.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.182009 muon-0.1.4/muon/_atac/_ref/jaspar/MA0708.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.182143 muon-0.1.4/muon/_atac/_ref/jaspar/MA0709.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.182287 muon-0.1.4/muon/_atac/_ref/jaspar/MA0710.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.182426 muon-0.1.4/muon/_atac/_ref/jaspar/MA0711.1.pfm
--rw-r--r--   0        0        0      332 2023-02-20 20:04:01.182570 muon-0.1.4/muon/_atac/_ref/jaspar/MA0712.2.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.182694 muon-0.1.4/muon/_atac/_ref/jaspar/MA0713.1.pfm
--rw-r--r--   0        0        0      244 2023-02-20 20:04:01.182807 muon-0.1.4/muon/_atac/_ref/jaspar/MA0714.1.pfm
--rw-r--r--   0        0        0      293 2023-02-20 20:04:01.183050 muon-0.1.4/muon/_atac/_ref/jaspar/MA0715.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.183230 muon-0.1.4/muon/_atac/_ref/jaspar/MA0716.1.pfm
--rw-r--r--   0        0        0      218 2023-02-20 20:04:01.183378 muon-0.1.4/muon/_atac/_ref/jaspar/MA0717.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.183511 muon-0.1.4/muon/_atac/_ref/jaspar/MA0718.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.183644 muon-0.1.4/muon/_atac/_ref/jaspar/MA0719.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.183773 muon-0.1.4/muon/_atac/_ref/jaspar/MA0720.1.pfm
--rw-r--r--   0        0        0      218 2023-02-20 20:04:01.183902 muon-0.1.4/muon/_atac/_ref/jaspar/MA0721.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.184028 muon-0.1.4/muon/_atac/_ref/jaspar/MA0722.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.184155 muon-0.1.4/muon/_atac/_ref/jaspar/MA0723.1.pfm
--rw-r--r--   0        0        0      244 2023-02-20 20:04:01.184338 muon-0.1.4/muon/_atac/_ref/jaspar/MA0724.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.184494 muon-0.1.4/muon/_atac/_ref/jaspar/MA0725.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.184645 muon-0.1.4/muon/_atac/_ref/jaspar/MA0726.1.pfm
--rw-r--r--   0        0        0      470 2023-02-20 20:04:01.184809 muon-0.1.4/muon/_atac/_ref/jaspar/MA0727.1.pfm
--rw-r--r--   0        0        0      405 2023-02-20 20:04:01.184970 muon-0.1.4/muon/_atac/_ref/jaspar/MA0728.1.pfm
--rw-r--r--   0        0        0      488 2023-02-20 20:04:01.185132 muon-0.1.4/muon/_atac/_ref/jaspar/MA0729.1.pfm
--rw-r--r--   0        0        0      462 2023-02-20 20:04:01.185282 muon-0.1.4/muon/_atac/_ref/jaspar/MA0730.1.pfm
--rw-r--r--   0        0        0      459 2023-02-20 20:04:01.185439 muon-0.1.4/muon/_atac/_ref/jaspar/MA0731.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.185635 muon-0.1.4/muon/_atac/_ref/jaspar/MA0732.1.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.185940 muon-0.1.4/muon/_atac/_ref/jaspar/MA0733.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.186130 muon-0.1.4/muon/_atac/_ref/jaspar/MA0734.2.pfm
--rw-r--r--   0        0        0      438 2023-02-20 20:04:01.186280 muon-0.1.4/muon/_atac/_ref/jaspar/MA0735.1.pfm
--rw-r--r--   0        0        0      379 2023-02-20 20:04:01.186418 muon-0.1.4/muon/_atac/_ref/jaspar/MA0736.1.pfm
--rw-r--r--   0        0        0      377 2023-02-20 20:04:01.186550 muon-0.1.4/muon/_atac/_ref/jaspar/MA0737.1.pfm
--rw-r--r--   0        0        0      242 2023-02-20 20:04:01.186682 muon-0.1.4/muon/_atac/_ref/jaspar/MA0738.1.pfm
--rw-r--r--   0        0        0      242 2023-02-20 20:04:01.186814 muon-0.1.4/muon/_atac/_ref/jaspar/MA0739.1.pfm
--rw-r--r--   0        0        0      380 2023-02-20 20:04:01.186995 muon-0.1.4/muon/_atac/_ref/jaspar/MA0740.1.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.187203 muon-0.1.4/muon/_atac/_ref/jaspar/MA0741.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.187364 muon-0.1.4/muon/_atac/_ref/jaspar/MA0742.1.pfm
--rw-r--r--   0        0        0      444 2023-02-20 20:04:01.187578 muon-0.1.4/muon/_atac/_ref/jaspar/MA0743.2.pfm
--rw-r--r--   0        0        0      444 2023-02-20 20:04:01.187879 muon-0.1.4/muon/_atac/_ref/jaspar/MA0744.2.pfm
--rw-r--r--   0        0        0      359 2023-02-20 20:04:01.188048 muon-0.1.4/muon/_atac/_ref/jaspar/MA0745.2.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.188200 muon-0.1.4/muon/_atac/_ref/jaspar/MA0746.2.pfm
--rw-r--r--   0        0        0      320 2023-02-20 20:04:01.188338 muon-0.1.4/muon/_atac/_ref/jaspar/MA0747.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.188589 muon-0.1.4/muon/_atac/_ref/jaspar/MA0748.2.pfm
--rw-r--r--   0        0        0      354 2023-02-20 20:04:01.188780 muon-0.1.4/muon/_atac/_ref/jaspar/MA0749.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.188999 muon-0.1.4/muon/_atac/_ref/jaspar/MA0750.2.pfm
--rw-r--r--   0        0        0      410 2023-02-20 20:04:01.189286 muon-0.1.4/muon/_atac/_ref/jaspar/MA0751.1.pfm
--rw-r--r--   0        0        0      465 2023-02-20 20:04:01.189565 muon-0.1.4/muon/_atac/_ref/jaspar/MA0752.1.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.189744 muon-0.1.4/muon/_atac/_ref/jaspar/MA0753.2.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.189886 muon-0.1.4/muon/_atac/_ref/jaspar/MA0754.1.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.190120 muon-0.1.4/muon/_atac/_ref/jaspar/MA0755.1.pfm
--rw-r--r--   0        0        0      381 2023-02-20 20:04:01.190364 muon-0.1.4/muon/_atac/_ref/jaspar/MA0756.1.pfm
--rw-r--r--   0        0        0      383 2023-02-20 20:04:01.190526 muon-0.1.4/muon/_atac/_ref/jaspar/MA0757.1.pfm
--rw-r--r--   0        0        0      379 2023-02-20 20:04:01.190700 muon-0.1.4/muon/_atac/_ref/jaspar/MA0758.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.190886 muon-0.1.4/muon/_atac/_ref/jaspar/MA0759.1.pfm
--rw-r--r--   0        0        0      263 2023-02-20 20:04:01.191053 muon-0.1.4/muon/_atac/_ref/jaspar/MA0760.1.pfm
--rw-r--r--   0        0        0      385 2023-02-20 20:04:01.191190 muon-0.1.4/muon/_atac/_ref/jaspar/MA0761.2.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.191323 muon-0.1.4/muon/_atac/_ref/jaspar/MA0762.1.pfm
--rw-r--r--   0        0        0      265 2023-02-20 20:04:01.191469 muon-0.1.4/muon/_atac/_ref/jaspar/MA0763.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.191616 muon-0.1.4/muon/_atac/_ref/jaspar/MA0764.2.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.191801 muon-0.1.4/muon/_atac/_ref/jaspar/MA0765.2.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.191945 muon-0.1.4/muon/_atac/_ref/jaspar/MA0766.2.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.192072 muon-0.1.4/muon/_atac/_ref/jaspar/MA0767.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.192259 muon-0.1.4/muon/_atac/_ref/jaspar/MA0768.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.192520 muon-0.1.4/muon/_atac/_ref/jaspar/MA0769.2.pfm
--rw-r--r--   0        0        0      351 2023-02-20 20:04:01.192696 muon-0.1.4/muon/_atac/_ref/jaspar/MA0770.1.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.192838 muon-0.1.4/muon/_atac/_ref/jaspar/MA0771.1.pfm
--rw-r--r--   0        0        0      379 2023-02-20 20:04:01.192976 muon-0.1.4/muon/_atac/_ref/jaspar/MA0772.1.pfm
--rw-r--r--   0        0        0      327 2023-02-20 20:04:01.193108 muon-0.1.4/muon/_atac/_ref/jaspar/MA0773.1.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.193240 muon-0.1.4/muon/_atac/_ref/jaspar/MA0774.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.193384 muon-0.1.4/muon/_atac/_ref/jaspar/MA0775.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.193580 muon-0.1.4/muon/_atac/_ref/jaspar/MA0776.1.pfm
--rw-r--r--   0        0        0      406 2023-02-20 20:04:01.193801 muon-0.1.4/muon/_atac/_ref/jaspar/MA0777.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.193956 muon-0.1.4/muon/_atac/_ref/jaspar/MA0778.1.pfm
--rw-r--r--   0        0        0      466 2023-02-20 20:04:01.194172 muon-0.1.4/muon/_atac/_ref/jaspar/MA0779.1.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.194405 muon-0.1.4/muon/_atac/_ref/jaspar/MA0780.1.pfm
--rw-r--r--   0        0        0      466 2023-02-20 20:04:01.194678 muon-0.1.4/muon/_atac/_ref/jaspar/MA0781.1.pfm
--rw-r--r--   0        0        0      413 2023-02-20 20:04:01.194916 muon-0.1.4/muon/_atac/_ref/jaspar/MA0782.2.pfm
--rw-r--r--   0        0        0      320 2023-02-20 20:04:01.195134 muon-0.1.4/muon/_atac/_ref/jaspar/MA0783.1.pfm
--rw-r--r--   0        0        0      381 2023-02-20 20:04:01.195299 muon-0.1.4/muon/_atac/_ref/jaspar/MA0784.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.195543 muon-0.1.4/muon/_atac/_ref/jaspar/MA0785.1.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.195767 muon-0.1.4/muon/_atac/_ref/jaspar/MA0786.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.195998 muon-0.1.4/muon/_atac/_ref/jaspar/MA0787.1.pfm
--rw-r--r--   0        0        0      351 2023-02-20 20:04:01.196179 muon-0.1.4/muon/_atac/_ref/jaspar/MA0788.1.pfm
--rw-r--r--   0        0        0      242 2023-02-20 20:04:01.196372 muon-0.1.4/muon/_atac/_ref/jaspar/MA0789.1.pfm
--rw-r--r--   0        0        0      383 2023-02-20 20:04:01.196577 muon-0.1.4/muon/_atac/_ref/jaspar/MA0790.1.pfm
--rw-r--r--   0        0        0      437 2023-02-20 20:04:01.196760 muon-0.1.4/muon/_atac/_ref/jaspar/MA0791.1.pfm
--rw-r--r--   0        0        0      243 2023-02-20 20:04:01.196917 muon-0.1.4/muon/_atac/_ref/jaspar/MA0792.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.197158 muon-0.1.4/muon/_atac/_ref/jaspar/MA0793.1.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.197360 muon-0.1.4/muon/_atac/_ref/jaspar/MA0794.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.197516 muon-0.1.4/muon/_atac/_ref/jaspar/MA0795.1.pfm
--rw-r--r--   0        0        0      322 2023-02-20 20:04:01.197664 muon-0.1.4/muon/_atac/_ref/jaspar/MA0796.1.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.197825 muon-0.1.4/muon/_atac/_ref/jaspar/MA0797.1.pfm
--rw-r--r--   0        0        0      382 2023-02-20 20:04:01.197963 muon-0.1.4/muon/_atac/_ref/jaspar/MA0798.2.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.198125 muon-0.1.4/muon/_atac/_ref/jaspar/MA0799.1.pfm
--rw-r--r--   0        0        0      355 2023-02-20 20:04:01.198260 muon-0.1.4/muon/_atac/_ref/jaspar/MA0800.1.pfm
--rw-r--r--   0        0        0      217 2023-02-20 20:04:01.198393 muon-0.1.4/muon/_atac/_ref/jaspar/MA0801.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.198518 muon-0.1.4/muon/_atac/_ref/jaspar/MA0802.1.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.198633 muon-0.1.4/muon/_atac/_ref/jaspar/MA0803.1.pfm
--rw-r--r--   0        0        0      554 2023-02-20 20:04:01.198752 muon-0.1.4/muon/_atac/_ref/jaspar/MA0804.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.198875 muon-0.1.4/muon/_atac/_ref/jaspar/MA0805.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.199006 muon-0.1.4/muon/_atac/_ref/jaspar/MA0806.1.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.199144 muon-0.1.4/muon/_atac/_ref/jaspar/MA0807.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.199276 muon-0.1.4/muon/_atac/_ref/jaspar/MA0808.1.pfm
--rw-r--r--   0        0        0      332 2023-02-20 20:04:01.199401 muon-0.1.4/muon/_atac/_ref/jaspar/MA0809.2.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.199557 muon-0.1.4/muon/_atac/_ref/jaspar/MA0810.1.pfm
--rw-r--r--   0        0        0      325 2023-02-20 20:04:01.199782 muon-0.1.4/muon/_atac/_ref/jaspar/MA0811.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.199922 muon-0.1.4/muon/_atac/_ref/jaspar/MA0812.1.pfm
--rw-r--r--   0        0        0      351 2023-02-20 20:04:01.200054 muon-0.1.4/muon/_atac/_ref/jaspar/MA0813.1.pfm
--rw-r--r--   0        0        0      388 2023-02-20 20:04:01.200175 muon-0.1.4/muon/_atac/_ref/jaspar/MA0814.2.pfm
--rw-r--r--   0        0        0      353 2023-02-20 20:04:01.200304 muon-0.1.4/muon/_atac/_ref/jaspar/MA0815.1.pfm
--rw-r--r--   0        0        0      265 2023-02-20 20:04:01.200435 muon-0.1.4/muon/_atac/_ref/jaspar/MA0816.1.pfm
--rw-r--r--   0        0        0      325 2023-02-20 20:04:01.200560 muon-0.1.4/muon/_atac/_ref/jaspar/MA0817.1.pfm
--rw-r--r--   0        0        0      266 2023-02-20 20:04:01.200687 muon-0.1.4/muon/_atac/_ref/jaspar/MA0818.1.pfm
--rw-r--r--   0        0        0      265 2023-02-20 20:04:01.200836 muon-0.1.4/muon/_atac/_ref/jaspar/MA0819.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.200962 muon-0.1.4/muon/_atac/_ref/jaspar/MA0820.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.201086 muon-0.1.4/muon/_atac/_ref/jaspar/MA0821.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.201218 muon-0.1.4/muon/_atac/_ref/jaspar/MA0822.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.201352 muon-0.1.4/muon/_atac/_ref/jaspar/MA0823.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.201480 muon-0.1.4/muon/_atac/_ref/jaspar/MA0825.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.201600 muon-0.1.4/muon/_atac/_ref/jaspar/MA0826.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.201715 muon-0.1.4/muon/_atac/_ref/jaspar/MA0827.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.201847 muon-0.1.4/muon/_atac/_ref/jaspar/MA0828.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.202022 muon-0.1.4/muon/_atac/_ref/jaspar/MA0829.2.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.202193 muon-0.1.4/muon/_atac/_ref/jaspar/MA0830.2.pfm
--rw-r--r--   0        0        0      206 2023-02-20 20:04:01.202358 muon-0.1.4/muon/_atac/_ref/jaspar/MA0831.2.pfm
--rw-r--r--   0        0        0      376 2023-02-20 20:04:01.202531 muon-0.1.4/muon/_atac/_ref/jaspar/MA0832.1.pfm
--rw-r--r--   0        0        0      385 2023-02-20 20:04:01.202702 muon-0.1.4/muon/_atac/_ref/jaspar/MA0833.2.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.202870 muon-0.1.4/muon/_atac/_ref/jaspar/MA0834.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.203039 muon-0.1.4/muon/_atac/_ref/jaspar/MA0835.2.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.203207 muon-0.1.4/muon/_atac/_ref/jaspar/MA0836.2.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.203380 muon-0.1.4/muon/_atac/_ref/jaspar/MA0837.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.203533 muon-0.1.4/muon/_atac/_ref/jaspar/MA0838.1.pfm
--rw-r--r--   0        0        0      380 2023-02-20 20:04:01.203650 muon-0.1.4/muon/_atac/_ref/jaspar/MA0839.1.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.203772 muon-0.1.4/muon/_atac/_ref/jaspar/MA0840.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.203894 muon-0.1.4/muon/_atac/_ref/jaspar/MA0841.1.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.204023 muon-0.1.4/muon/_atac/_ref/jaspar/MA0842.2.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.204152 muon-0.1.4/muon/_atac/_ref/jaspar/MA0843.1.pfm
--rw-r--r--   0        0        0      382 2023-02-20 20:04:01.204282 muon-0.1.4/muon/_atac/_ref/jaspar/MA0844.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.204431 muon-0.1.4/muon/_atac/_ref/jaspar/MA0845.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.204569 muon-0.1.4/muon/_atac/_ref/jaspar/MA0846.1.pfm
--rw-r--r--   0        0        0      355 2023-02-20 20:04:01.204779 muon-0.1.4/muon/_atac/_ref/jaspar/MA0847.2.pfm
--rw-r--r--   0        0        0      183 2023-02-20 20:04:01.204926 muon-0.1.4/muon/_atac/_ref/jaspar/MA0848.1.pfm
--rw-r--r--   0        0        0      182 2023-02-20 20:04:01.205058 muon-0.1.4/muon/_atac/_ref/jaspar/MA0849.1.pfm
--rw-r--r--   0        0        0      179 2023-02-20 20:04:01.205175 muon-0.1.4/muon/_atac/_ref/jaspar/MA0850.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.205376 muon-0.1.4/muon/_atac/_ref/jaspar/MA0851.1.pfm
--rw-r--r--   0        0        0      380 2023-02-20 20:04:01.205566 muon-0.1.4/muon/_atac/_ref/jaspar/MA0852.2.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.205714 muon-0.1.4/muon/_atac/_ref/jaspar/MA0853.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.205917 muon-0.1.4/muon/_atac/_ref/jaspar/MA0854.1.pfm
--rw-r--r--   0        0        0      382 2023-02-20 20:04:01.206068 muon-0.1.4/muon/_atac/_ref/jaspar/MA0855.1.pfm
--rw-r--r--   0        0        0      385 2023-02-20 20:04:01.206209 muon-0.1.4/muon/_atac/_ref/jaspar/MA0856.1.pfm
--rw-r--r--   0        0        0      437 2023-02-20 20:04:01.206385 muon-0.1.4/muon/_atac/_ref/jaspar/MA0857.1.pfm
--rw-r--r--   0        0        0      459 2023-02-20 20:04:01.206619 muon-0.1.4/muon/_atac/_ref/jaspar/MA0858.1.pfm
--rw-r--r--   0        0        0      442 2023-02-20 20:04:01.206756 muon-0.1.4/muon/_atac/_ref/jaspar/MA0859.1.pfm
--rw-r--r--   0        0        0      463 2023-02-20 20:04:01.206883 muon-0.1.4/muon/_atac/_ref/jaspar/MA0860.1.pfm
--rw-r--r--   0        0        0      495 2023-02-20 20:04:01.207013 muon-0.1.4/muon/_atac/_ref/jaspar/MA0861.1.pfm
--rw-r--r--   0        0        0      210 2023-02-20 20:04:01.207146 muon-0.1.4/muon/_atac/_ref/jaspar/MA0862.1.pfm
--rw-r--r--   0        0        0      373 2023-02-20 20:04:01.207344 muon-0.1.4/muon/_atac/_ref/jaspar/MA0863.1.pfm
--rw-r--r--   0        0        0      438 2023-02-20 20:04:01.207504 muon-0.1.4/muon/_atac/_ref/jaspar/MA0864.2.pfm
--rw-r--r--   0        0        0      317 2023-02-20 20:04:01.207654 muon-0.1.4/muon/_atac/_ref/jaspar/MA0865.1.pfm
--rw-r--r--   0        0        0      409 2023-02-20 20:04:01.207796 muon-0.1.4/muon/_atac/_ref/jaspar/MA0866.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.207934 muon-0.1.4/muon/_atac/_ref/jaspar/MA0867.2.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.208203 muon-0.1.4/muon/_atac/_ref/jaspar/MA0868.2.pfm
--rw-r--r--   0        0        0      402 2023-02-20 20:04:01.208350 muon-0.1.4/muon/_atac/_ref/jaspar/MA0869.1.pfm
--rw-r--r--   0        0        0      409 2023-02-20 20:04:01.208496 muon-0.1.4/muon/_atac/_ref/jaspar/MA0870.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.208721 muon-0.1.4/muon/_atac/_ref/jaspar/MA0871.2.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.208953 muon-0.1.4/muon/_atac/_ref/jaspar/MA0872.1.pfm
--rw-r--r--   0        0        0      295 2023-02-20 20:04:01.209114 muon-0.1.4/muon/_atac/_ref/jaspar/MA0873.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.209250 muon-0.1.4/muon/_atac/_ref/jaspar/MA0874.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.209379 muon-0.1.4/muon/_atac/_ref/jaspar/MA0875.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.209507 muon-0.1.4/muon/_atac/_ref/jaspar/MA0876.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.209634 muon-0.1.4/muon/_atac/_ref/jaspar/MA0877.2.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.209751 muon-0.1.4/muon/_atac/_ref/jaspar/MA0878.2.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.209865 muon-0.1.4/muon/_atac/_ref/jaspar/MA0879.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.210067 muon-0.1.4/muon/_atac/_ref/jaspar/MA0880.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.210218 muon-0.1.4/muon/_atac/_ref/jaspar/MA0881.1.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.210410 muon-0.1.4/muon/_atac/_ref/jaspar/MA0882.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.210677 muon-0.1.4/muon/_atac/_ref/jaspar/MA0883.1.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.210956 muon-0.1.4/muon/_atac/_ref/jaspar/MA0884.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.211122 muon-0.1.4/muon/_atac/_ref/jaspar/MA0885.1.pfm
--rw-r--r--   0        0        0      274 2023-02-20 20:04:01.211264 muon-0.1.4/muon/_atac/_ref/jaspar/MA0886.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.211396 muon-0.1.4/muon/_atac/_ref/jaspar/MA0887.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.211536 muon-0.1.4/muon/_atac/_ref/jaspar/MA0888.1.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.211664 muon-0.1.4/muon/_atac/_ref/jaspar/MA0889.1.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.211820 muon-0.1.4/muon/_atac/_ref/jaspar/MA0890.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.212028 muon-0.1.4/muon/_atac/_ref/jaspar/MA0891.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.212192 muon-0.1.4/muon/_atac/_ref/jaspar/MA0892.1.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.212329 muon-0.1.4/muon/_atac/_ref/jaspar/MA0893.2.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.212465 muon-0.1.4/muon/_atac/_ref/jaspar/MA0894.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.212652 muon-0.1.4/muon/_atac/_ref/jaspar/MA0895.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.212802 muon-0.1.4/muon/_atac/_ref/jaspar/MA0896.1.pfm
--rw-r--r--   0        0        0      459 2023-02-20 20:04:01.212929 muon-0.1.4/muon/_atac/_ref/jaspar/MA0897.1.pfm
--rw-r--r--   0        0        0      459 2023-02-20 20:04:01.213056 muon-0.1.4/muon/_atac/_ref/jaspar/MA0898.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.213295 muon-0.1.4/muon/_atac/_ref/jaspar/MA0899.1.pfm
--rw-r--r--   0        0        0      218 2023-02-20 20:04:01.213460 muon-0.1.4/muon/_atac/_ref/jaspar/MA0900.2.pfm
--rw-r--r--   0        0        0      388 2023-02-20 20:04:01.213605 muon-0.1.4/muon/_atac/_ref/jaspar/MA0901.2.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.213738 muon-0.1.4/muon/_atac/_ref/jaspar/MA0902.2.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.213872 muon-0.1.4/muon/_atac/_ref/jaspar/MA0903.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.214007 muon-0.1.4/muon/_atac/_ref/jaspar/MA0904.2.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.214172 muon-0.1.4/muon/_atac/_ref/jaspar/MA0905.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.214294 muon-0.1.4/muon/_atac/_ref/jaspar/MA0906.1.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.214412 muon-0.1.4/muon/_atac/_ref/jaspar/MA0907.1.pfm
--rw-r--r--   0        0        0      265 2023-02-20 20:04:01.214617 muon-0.1.4/muon/_atac/_ref/jaspar/MA0908.1.pfm
--rw-r--r--   0        0        0      294 2023-02-20 20:04:01.214761 muon-0.1.4/muon/_atac/_ref/jaspar/MA0909.2.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.214894 muon-0.1.4/muon/_atac/_ref/jaspar/MA0910.2.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.215021 muon-0.1.4/muon/_atac/_ref/jaspar/MA0911.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.215149 muon-0.1.4/muon/_atac/_ref/jaspar/MA0912.2.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.215277 muon-0.1.4/muon/_atac/_ref/jaspar/MA0913.2.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.215401 muon-0.1.4/muon/_atac/_ref/jaspar/MA0914.1.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.215528 muon-0.1.4/muon/_atac/_ref/jaspar/MA1099.2.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.215690 muon-0.1.4/muon/_atac/_ref/jaspar/MA1100.2.pfm
--rw-r--r--   0        0        0      528 2023-02-20 20:04:01.215823 muon-0.1.4/muon/_atac/_ref/jaspar/MA1101.2.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.215949 muon-0.1.4/muon/_atac/_ref/jaspar/MA1102.2.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.216081 muon-0.1.4/muon/_atac/_ref/jaspar/MA1103.2.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.216217 muon-0.1.4/muon/_atac/_ref/jaspar/MA1104.2.pfm
--rw-r--r--   0        0        0      329 2023-02-20 20:04:01.216357 muon-0.1.4/muon/_atac/_ref/jaspar/MA1105.2.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.216486 muon-0.1.4/muon/_atac/_ref/jaspar/MA1106.1.pfm
--rw-r--r--   0        0        0      441 2023-02-20 20:04:01.216613 muon-0.1.4/muon/_atac/_ref/jaspar/MA1107.2.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.216804 muon-0.1.4/muon/_atac/_ref/jaspar/MA1108.2.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.216975 muon-0.1.4/muon/_atac/_ref/jaspar/MA1109.1.pfm
--rw-r--r--   0        0        0      294 2023-02-20 20:04:01.217115 muon-0.1.4/muon/_atac/_ref/jaspar/MA1110.1.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.217242 muon-0.1.4/muon/_atac/_ref/jaspar/MA1111.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.217369 muon-0.1.4/muon/_atac/_ref/jaspar/MA1112.2.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.217501 muon-0.1.4/muon/_atac/_ref/jaspar/MA1113.2.pfm
--rw-r--r--   0        0        0      468 2023-02-20 20:04:01.217631 muon-0.1.4/muon/_atac/_ref/jaspar/MA1114.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.217853 muon-0.1.4/muon/_atac/_ref/jaspar/MA1115.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.217997 muon-0.1.4/muon/_atac/_ref/jaspar/MA1116.1.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.218147 muon-0.1.4/muon/_atac/_ref/jaspar/MA1117.1.pfm
--rw-r--r--   0        0        0      294 2023-02-20 20:04:01.218277 muon-0.1.4/muon/_atac/_ref/jaspar/MA1118.1.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.218405 muon-0.1.4/muon/_atac/_ref/jaspar/MA1119.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.218539 muon-0.1.4/muon/_atac/_ref/jaspar/MA1120.1.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.218658 muon-0.1.4/muon/_atac/_ref/jaspar/MA1121.1.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.218775 muon-0.1.4/muon/_atac/_ref/jaspar/MA1122.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.218901 muon-0.1.4/muon/_atac/_ref/jaspar/MA1123.2.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.219029 muon-0.1.4/muon/_atac/_ref/jaspar/MA1124.1.pfm
--rw-r--r--   0        0        0      329 2023-02-20 20:04:01.219161 muon-0.1.4/muon/_atac/_ref/jaspar/MA1125.1.pfm
--rw-r--r--   0        0        0      435 2023-02-20 20:04:01.219353 muon-0.1.4/muon/_atac/_ref/jaspar/MA1126.1.pfm
--rw-r--r--   0        0        0      295 2023-02-20 20:04:01.219496 muon-0.1.4/muon/_atac/_ref/jaspar/MA1127.1.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.219632 muon-0.1.4/muon/_atac/_ref/jaspar/MA1128.1.pfm
--rw-r--r--   0        0        0      266 2023-02-20 20:04:01.219764 muon-0.1.4/muon/_atac/_ref/jaspar/MA1129.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.219895 muon-0.1.4/muon/_atac/_ref/jaspar/MA1130.1.pfm
--rw-r--r--   0        0        0      295 2023-02-20 20:04:01.220027 muon-0.1.4/muon/_atac/_ref/jaspar/MA1131.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.220140 muon-0.1.4/muon/_atac/_ref/jaspar/MA1132.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.220312 muon-0.1.4/muon/_atac/_ref/jaspar/MA1133.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.220567 muon-0.1.4/muon/_atac/_ref/jaspar/MA1134.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.220715 muon-0.1.4/muon/_atac/_ref/jaspar/MA1135.1.pfm
--rw-r--r--   0        0        0      266 2023-02-20 20:04:01.220955 muon-0.1.4/muon/_atac/_ref/jaspar/MA1136.1.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.221115 muon-0.1.4/muon/_atac/_ref/jaspar/MA1137.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.221324 muon-0.1.4/muon/_atac/_ref/jaspar/MA1138.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.221579 muon-0.1.4/muon/_atac/_ref/jaspar/MA1139.1.pfm
--rw-r--r--   0        0        0      321 2023-02-20 20:04:01.221785 muon-0.1.4/muon/_atac/_ref/jaspar/MA1140.2.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.221952 muon-0.1.4/muon/_atac/_ref/jaspar/MA1141.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.222102 muon-0.1.4/muon/_atac/_ref/jaspar/MA1142.1.pfm
--rw-r--r--   0        0        0      266 2023-02-20 20:04:01.222248 muon-0.1.4/muon/_atac/_ref/jaspar/MA1143.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.222406 muon-0.1.4/muon/_atac/_ref/jaspar/MA1144.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.222597 muon-0.1.4/muon/_atac/_ref/jaspar/MA1145.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.222733 muon-0.1.4/muon/_atac/_ref/jaspar/MA1146.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.223033 muon-0.1.4/muon/_atac/_ref/jaspar/MA1147.1.pfm
--rw-r--r--   0        0        0      492 2023-02-20 20:04:01.223217 muon-0.1.4/muon/_atac/_ref/jaspar/MA1148.1.pfm
--rw-r--r--   0        0        0      492 2023-02-20 20:04:01.223509 muon-0.1.4/muon/_atac/_ref/jaspar/MA1149.1.pfm
--rw-r--r--   0        0        0      294 2023-02-20 20:04:01.223666 muon-0.1.4/muon/_atac/_ref/jaspar/MA1150.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.223804 muon-0.1.4/muon/_atac/_ref/jaspar/MA1151.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.223945 muon-0.1.4/muon/_atac/_ref/jaspar/MA1152.1.pfm
--rw-r--r--   0        0        0      210 2023-02-20 20:04:01.224175 muon-0.1.4/muon/_atac/_ref/jaspar/MA1153.1.pfm
--rw-r--r--   0        0        0      461 2023-02-20 20:04:01.224372 muon-0.1.4/muon/_atac/_ref/jaspar/MA1154.1.pfm
--rw-r--r--   0        0        0      409 2023-02-20 20:04:01.224519 muon-0.1.4/muon/_atac/_ref/jaspar/MA1155.1.pfm
--rw-r--r--   0        0        0      580 2023-02-20 20:04:01.224658 muon-0.1.4/muon/_atac/_ref/jaspar/MA1418.1.pfm
--rw-r--r--   0        0        0      415 2023-02-20 20:04:01.224792 muon-0.1.4/muon/_atac/_ref/jaspar/MA1419.1.pfm
--rw-r--r--   0        0        0      377 2023-02-20 20:04:01.224911 muon-0.1.4/muon/_atac/_ref/jaspar/MA1420.1.pfm
--rw-r--r--   0        0        0      320 2023-02-20 20:04:01.225024 muon-0.1.4/muon/_atac/_ref/jaspar/MA1421.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.225135 muon-0.1.4/muon/_atac/_ref/jaspar/MA1463.1.pfm
--rw-r--r--   0        0        0      274 2023-02-20 20:04:01.225280 muon-0.1.4/muon/_atac/_ref/jaspar/MA1464.1.pfm
--rw-r--r--   0        0        0      379 2023-02-20 20:04:01.225410 muon-0.1.4/muon/_atac/_ref/jaspar/MA1466.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.225535 muon-0.1.4/muon/_atac/_ref/jaspar/MA1467.1.pfm
--rw-r--r--   0        0        0      266 2023-02-20 20:04:01.225663 muon-0.1.4/muon/_atac/_ref/jaspar/MA1468.1.pfm
--rw-r--r--   0        0        0      545 2023-02-20 20:04:01.225797 muon-0.1.4/muon/_atac/_ref/jaspar/MA1470.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.225931 muon-0.1.4/muon/_atac/_ref/jaspar/MA1471.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.226062 muon-0.1.4/muon/_atac/_ref/jaspar/MA1472.1.pfm
--rw-r--r--   0        0        0      301 2023-02-20 20:04:01.226195 muon-0.1.4/muon/_atac/_ref/jaspar/MA1473.1.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.226324 muon-0.1.4/muon/_atac/_ref/jaspar/MA1474.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.226454 muon-0.1.4/muon/_atac/_ref/jaspar/MA1475.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.226575 muon-0.1.4/muon/_atac/_ref/jaspar/MA1476.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.226692 muon-0.1.4/muon/_atac/_ref/jaspar/MA1478.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.226818 muon-0.1.4/muon/_atac/_ref/jaspar/MA1479.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.226943 muon-0.1.4/muon/_atac/_ref/jaspar/MA1480.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.227067 muon-0.1.4/muon/_atac/_ref/jaspar/MA1481.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.227192 muon-0.1.4/muon/_atac/_ref/jaspar/MA1483.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.227321 muon-0.1.4/muon/_atac/_ref/jaspar/MA1484.1.pfm
--rw-r--r--   0        0        0      382 2023-02-20 20:04:01.227465 muon-0.1.4/muon/_atac/_ref/jaspar/MA1485.1.pfm
--rw-r--r--   0        0        0      407 2023-02-20 20:04:01.227621 muon-0.1.4/muon/_atac/_ref/jaspar/MA1487.1.pfm
--rw-r--r--   0        0        0      206 2023-02-20 20:04:01.227747 muon-0.1.4/muon/_atac/_ref/jaspar/MA1489.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.227875 muon-0.1.4/muon/_atac/_ref/jaspar/MA1491.1.pfm
--rw-r--r--   0        0        0      265 2023-02-20 20:04:01.227992 muon-0.1.4/muon/_atac/_ref/jaspar/MA1493.1.pfm
--rw-r--r--   0        0        0      406 2023-02-20 20:04:01.228102 muon-0.1.4/muon/_atac/_ref/jaspar/MA1494.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.228234 muon-0.1.4/muon/_atac/_ref/jaspar/MA1495.1.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.228360 muon-0.1.4/muon/_atac/_ref/jaspar/MA1496.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.228484 muon-0.1.4/muon/_atac/_ref/jaspar/MA1497.1.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.228626 muon-0.1.4/muon/_atac/_ref/jaspar/MA1498.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.228743 muon-0.1.4/muon/_atac/_ref/jaspar/MA1499.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.228869 muon-0.1.4/muon/_atac/_ref/jaspar/MA1500.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.228988 muon-0.1.4/muon/_atac/_ref/jaspar/MA1501.1.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.229112 muon-0.1.4/muon/_atac/_ref/jaspar/MA1502.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.229232 muon-0.1.4/muon/_atac/_ref/jaspar/MA1503.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.229356 muon-0.1.4/muon/_atac/_ref/jaspar/MA1504.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.229479 muon-0.1.4/muon/_atac/_ref/jaspar/MA1505.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.229615 muon-0.1.4/muon/_atac/_ref/jaspar/MA1506.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.229793 muon-0.1.4/muon/_atac/_ref/jaspar/MA1507.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.229937 muon-0.1.4/muon/_atac/_ref/jaspar/MA1508.1.pfm
--rw-r--r--   0        0        0      240 2023-02-20 20:04:01.230073 muon-0.1.4/muon/_atac/_ref/jaspar/MA1509.1.pfm
--rw-r--r--   0        0        0      301 2023-02-20 20:04:01.230206 muon-0.1.4/muon/_atac/_ref/jaspar/MA1511.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.230346 muon-0.1.4/muon/_atac/_ref/jaspar/MA1512.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.230489 muon-0.1.4/muon/_atac/_ref/jaspar/MA1513.1.pfm
--rw-r--r--   0        0        0      413 2023-02-20 20:04:01.230629 muon-0.1.4/muon/_atac/_ref/jaspar/MA1514.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.230765 muon-0.1.4/muon/_atac/_ref/jaspar/MA1515.1.pfm
--rw-r--r--   0        0        0      301 2023-02-20 20:04:01.231009 muon-0.1.4/muon/_atac/_ref/jaspar/MA1516.1.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.231155 muon-0.1.4/muon/_atac/_ref/jaspar/MA1517.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.231338 muon-0.1.4/muon/_atac/_ref/jaspar/MA1518.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.231554 muon-0.1.4/muon/_atac/_ref/jaspar/MA1519.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.231783 muon-0.1.4/muon/_atac/_ref/jaspar/MA1520.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.231988 muon-0.1.4/muon/_atac/_ref/jaspar/MA1521.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.232242 muon-0.1.4/muon/_atac/_ref/jaspar/MA1522.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.232450 muon-0.1.4/muon/_atac/_ref/jaspar/MA1523.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.232609 muon-0.1.4/muon/_atac/_ref/jaspar/MA1524.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.232836 muon-0.1.4/muon/_atac/_ref/jaspar/MA1525.1.pfm
--rw-r--r--   0        0        0      464 2023-02-20 20:04:01.233044 muon-0.1.4/muon/_atac/_ref/jaspar/MA1527.1.pfm
--rw-r--r--   0        0        0      468 2023-02-20 20:04:01.233216 muon-0.1.4/muon/_atac/_ref/jaspar/MA1528.1.pfm
--rw-r--r--   0        0        0      496 2023-02-20 20:04:01.233390 muon-0.1.4/muon/_atac/_ref/jaspar/MA1529.1.pfm
--rw-r--r--   0        0        0      242 2023-02-20 20:04:01.233547 muon-0.1.4/muon/_atac/_ref/jaspar/MA1530.1.pfm
--rw-r--r--   0        0        0      409 2023-02-20 20:04:01.233681 muon-0.1.4/muon/_atac/_ref/jaspar/MA1531.1.pfm
--rw-r--r--   0        0        0      407 2023-02-20 20:04:01.233825 muon-0.1.4/muon/_atac/_ref/jaspar/MA1532.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.233948 muon-0.1.4/muon/_atac/_ref/jaspar/MA1533.1.pfm
--rw-r--r--   0        0        0      246 2023-02-20 20:04:01.234116 muon-0.1.4/muon/_atac/_ref/jaspar/MA1534.1.pfm
--rw-r--r--   0        0        0      244 2023-02-20 20:04:01.234297 muon-0.1.4/muon/_atac/_ref/jaspar/MA1535.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.234459 muon-0.1.4/muon/_atac/_ref/jaspar/MA1536.1.pfm
--rw-r--r--   0        0        0      414 2023-02-20 20:04:01.234596 muon-0.1.4/muon/_atac/_ref/jaspar/MA1537.1.pfm
--rw-r--r--   0        0        0      410 2023-02-20 20:04:01.234729 muon-0.1.4/muon/_atac/_ref/jaspar/MA1538.1.pfm
--rw-r--r--   0        0        0      410 2023-02-20 20:04:01.234866 muon-0.1.4/muon/_atac/_ref/jaspar/MA1539.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.235136 muon-0.1.4/muon/_atac/_ref/jaspar/MA1540.1.pfm
--rw-r--r--   0        0        0      464 2023-02-20 20:04:01.235358 muon-0.1.4/muon/_atac/_ref/jaspar/MA1541.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.235515 muon-0.1.4/muon/_atac/_ref/jaspar/MA1542.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.235678 muon-0.1.4/muon/_atac/_ref/jaspar/MA1544.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.235820 muon-0.1.4/muon/_atac/_ref/jaspar/MA1545.1.pfm
--rw-r--r--   0        0        0      436 2023-02-20 20:04:01.235994 muon-0.1.4/muon/_atac/_ref/jaspar/MA1546.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.236132 muon-0.1.4/muon/_atac/_ref/jaspar/MA1547.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.236257 muon-0.1.4/muon/_atac/_ref/jaspar/MA1548.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.236385 muon-0.1.4/muon/_atac/_ref/jaspar/MA1549.1.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.236513 muon-0.1.4/muon/_atac/_ref/jaspar/MA1550.1.pfm
--rw-r--r--   0        0        0      378 2023-02-20 20:04:01.236638 muon-0.1.4/muon/_atac/_ref/jaspar/MA1552.1.pfm
--rw-r--r--   0        0        0      381 2023-02-20 20:04:01.236755 muon-0.1.4/muon/_atac/_ref/jaspar/MA1553.1.pfm
--rw-r--r--   0        0        0      236 2023-02-20 20:04:01.236870 muon-0.1.4/muon/_atac/_ref/jaspar/MA1554.1.pfm
--rw-r--r--   0        0        0      380 2023-02-20 20:04:01.237080 muon-0.1.4/muon/_atac/_ref/jaspar/MA1555.1.pfm
--rw-r--r--   0        0        0      380 2023-02-20 20:04:01.237253 muon-0.1.4/muon/_atac/_ref/jaspar/MA1556.1.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.237399 muon-0.1.4/muon/_atac/_ref/jaspar/MA1557.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.237536 muon-0.1.4/muon/_atac/_ref/jaspar/MA1558.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.237661 muon-0.1.4/muon/_atac/_ref/jaspar/MA1559.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.237789 muon-0.1.4/muon/_atac/_ref/jaspar/MA1560.1.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.237910 muon-0.1.4/muon/_atac/_ref/jaspar/MA1561.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.238061 muon-0.1.4/muon/_atac/_ref/jaspar/MA1562.1.pfm
--rw-r--r--   0        0        0      211 2023-02-20 20:04:01.238263 muon-0.1.4/muon/_atac/_ref/jaspar/MA1563.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.238458 muon-0.1.4/muon/_atac/_ref/jaspar/MA1564.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.238592 muon-0.1.4/muon/_atac/_ref/jaspar/MA1565.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.238716 muon-0.1.4/muon/_atac/_ref/jaspar/MA1566.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.238852 muon-0.1.4/muon/_atac/_ref/jaspar/MA1567.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.239087 muon-0.1.4/muon/_atac/_ref/jaspar/MA1568.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.239229 muon-0.1.4/muon/_atac/_ref/jaspar/MA1569.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.239364 muon-0.1.4/muon/_atac/_ref/jaspar/MA1570.1.pfm
--rw-r--r--   0        0        0      325 2023-02-20 20:04:01.239603 muon-0.1.4/muon/_atac/_ref/jaspar/MA1571.1.pfm
--rw-r--r--   0        0        0      325 2023-02-20 20:04:01.239846 muon-0.1.4/muon/_atac/_ref/jaspar/MA1572.1.pfm
--rw-r--r--   0        0        0      518 2023-02-20 20:04:01.240037 muon-0.1.4/muon/_atac/_ref/jaspar/MA1573.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.240254 muon-0.1.4/muon/_atac/_ref/jaspar/MA1574.1.pfm
--rw-r--r--   0        0        0      522 2023-02-20 20:04:01.240427 muon-0.1.4/muon/_atac/_ref/jaspar/MA1575.1.pfm
--rw-r--r--   0        0        0      518 2023-02-20 20:04:01.240572 muon-0.1.4/muon/_atac/_ref/jaspar/MA1576.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.240712 muon-0.1.4/muon/_atac/_ref/jaspar/MA1577.1.pfm
--rw-r--r--   0        0        0      265 2023-02-20 20:04:01.240996 muon-0.1.4/muon/_atac/_ref/jaspar/MA1578.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.241200 muon-0.1.4/muon/_atac/_ref/jaspar/MA1579.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.241367 muon-0.1.4/muon/_atac/_ref/jaspar/MA1580.1.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.241515 muon-0.1.4/muon/_atac/_ref/jaspar/MA1581.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.241650 muon-0.1.4/muon/_atac/_ref/jaspar/MA1583.1.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.241783 muon-0.1.4/muon/_atac/_ref/jaspar/MA1584.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.241906 muon-0.1.4/muon/_atac/_ref/jaspar/MA1585.1.pfm
--rw-r--r--   0        0        0      379 2023-02-20 20:04:01.242022 muon-0.1.4/muon/_atac/_ref/jaspar/MA1587.1.pfm
--rw-r--r--   0        0        0      410 2023-02-20 20:04:01.242148 muon-0.1.4/muon/_atac/_ref/jaspar/MA1588.1.pfm
--rw-r--r--   0        0        0      576 2023-02-20 20:04:01.242272 muon-0.1.4/muon/_atac/_ref/jaspar/MA1589.1.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.242475 muon-0.1.4/muon/_atac/_ref/jaspar/MA1592.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.242638 muon-0.1.4/muon/_atac/_ref/jaspar/MA1593.1.pfm
--rw-r--r--   0        0        0      661 2023-02-20 20:04:01.242800 muon-0.1.4/muon/_atac/_ref/jaspar/MA1594.1.pfm
--rw-r--r--   0        0        0      436 2023-02-20 20:04:01.242947 muon-0.1.4/muon/_atac/_ref/jaspar/MA1596.1.pfm
--rw-r--r--   0        0        0      461 2023-02-20 20:04:01.243086 muon-0.1.4/muon/_atac/_ref/jaspar/MA1597.1.pfm
--rw-r--r--   0        0        0      436 2023-02-20 20:04:01.243217 muon-0.1.4/muon/_atac/_ref/jaspar/MA1599.1.pfm
--rw-r--r--   0        0        0      492 2023-02-20 20:04:01.243339 muon-0.1.4/muon/_atac/_ref/jaspar/MA1600.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.243472 muon-0.1.4/muon/_atac/_ref/jaspar/MA1601.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.243708 muon-0.1.4/muon/_atac/_ref/jaspar/MA1602.1.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.243925 muon-0.1.4/muon/_atac/_ref/jaspar/MA1603.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.244186 muon-0.1.4/muon/_atac/_ref/jaspar/MA1604.1.pfm
--rw-r--r--   0        0        0      304 2023-02-20 20:04:01.244357 muon-0.1.4/muon/_atac/_ref/jaspar/MA1606.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.244526 muon-0.1.4/muon/_atac/_ref/jaspar/MA1607.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.244667 muon-0.1.4/muon/_atac/_ref/jaspar/MA1608.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.244842 muon-0.1.4/muon/_atac/_ref/jaspar/MA1615.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.244965 muon-0.1.4/muon/_atac/_ref/jaspar/MA1616.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.245084 muon-0.1.4/muon/_atac/_ref/jaspar/MA1618.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.245273 muon-0.1.4/muon/_atac/_ref/jaspar/MA1619.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.245445 muon-0.1.4/muon/_atac/_ref/jaspar/MA1620.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.245588 muon-0.1.4/muon/_atac/_ref/jaspar/MA1621.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.245721 muon-0.1.4/muon/_atac/_ref/jaspar/MA1622.1.pfm
--rw-r--r--   0        0        0      354 2023-02-20 20:04:01.245872 muon-0.1.4/muon/_atac/_ref/jaspar/MA1623.1.pfm
--rw-r--r--   0        0        0      327 2023-02-20 20:04:01.246015 muon-0.1.4/muon/_atac/_ref/jaspar/MA1624.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.246178 muon-0.1.4/muon/_atac/_ref/jaspar/MA1625.1.pfm
--rw-r--r--   0        0        0      382 2023-02-20 20:04:01.246312 muon-0.1.4/muon/_atac/_ref/jaspar/MA1627.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.246446 muon-0.1.4/muon/_atac/_ref/jaspar/MA1628.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.246617 muon-0.1.4/muon/_atac/_ref/jaspar/MA1629.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.246764 muon-0.1.4/muon/_atac/_ref/jaspar/MA1630.1.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.246905 muon-0.1.4/muon/_atac/_ref/jaspar/MA1631.1.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.247037 muon-0.1.4/muon/_atac/_ref/jaspar/MA1632.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.247164 muon-0.1.4/muon/_atac/_ref/jaspar/MA1633.1.pfm
--rw-r--r--   0        0        0      303 2023-02-20 20:04:01.247296 muon-0.1.4/muon/_atac/_ref/jaspar/MA1634.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.247424 muon-0.1.4/muon/_atac/_ref/jaspar/MA1635.1.pfm
--rw-r--r--   0        0        0      413 2023-02-20 20:04:01.247568 muon-0.1.4/muon/_atac/_ref/jaspar/MA1636.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.247736 muon-0.1.4/muon/_atac/_ref/jaspar/MA1637.1.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.247900 muon-0.1.4/muon/_atac/_ref/jaspar/MA1638.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.248024 muon-0.1.4/muon/_atac/_ref/jaspar/MA1639.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.248141 muon-0.1.4/muon/_atac/_ref/jaspar/MA1640.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.248265 muon-0.1.4/muon/_atac/_ref/jaspar/MA1641.1.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.248405 muon-0.1.4/muon/_atac/_ref/jaspar/MA1642.1.pfm
--rw-r--r--   0        0        0      579 2023-02-20 20:04:01.248541 muon-0.1.4/muon/_atac/_ref/jaspar/MA1643.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.248668 muon-0.1.4/muon/_atac/_ref/jaspar/MA1644.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.248889 muon-0.1.4/muon/_atac/_ref/jaspar/MA1645.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.249094 muon-0.1.4/muon/_atac/_ref/jaspar/MA1646.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.249275 muon-0.1.4/muon/_atac/_ref/jaspar/MA1647.1.pfm
--rw-r--r--   0        0        0      304 2023-02-20 20:04:01.249453 muon-0.1.4/muon/_atac/_ref/jaspar/MA1648.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.249627 muon-0.1.4/muon/_atac/_ref/jaspar/MA1649.1.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.249800 muon-0.1.4/muon/_atac/_ref/jaspar/MA1650.1.pfm
--rw-r--r--   0        0        0      576 2023-02-20 20:04:01.249944 muon-0.1.4/muon/_atac/_ref/jaspar/MA1651.1.pfm
--rw-r--r--   0        0        0      381 2023-02-20 20:04:01.250073 muon-0.1.4/muon/_atac/_ref/jaspar/MA1652.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.250202 muon-0.1.4/muon/_atac/_ref/jaspar/MA1653.1.pfm
--rw-r--r--   0        0        0      629 2023-02-20 20:04:01.250397 muon-0.1.4/muon/_atac/_ref/jaspar/MA1654.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.250597 muon-0.1.4/muon/_atac/_ref/jaspar/MA1655.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.250745 muon-0.1.4/muon/_atac/_ref/jaspar/MA1656.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.250891 muon-0.1.4/muon/_atac/_ref/jaspar/MA1657.1.pfm
--rw-r--r--   0        0        0      302 2023-02-20 20:04:01.251035 muon-0.1.4/muon/_atac/_ref/jaspar/MA1683.1.pfm
--rw-r--r--   0        0        0    11673 2023-02-20 20:04:01.251258 muon-0.1.4/muon/_atac/_ref/jaspar/motif_to_gene.txt
--rw-r--r--   0        0        0     4491 2023-02-20 20:04:01.251460 muon-0.1.4/muon/_atac/io.py
--rw-r--r--   0        0        0    12725 2023-06-07 09:07:57.086211 muon-0.1.4/muon/_atac/plot.py
--rw-r--r--   0        0        0     7133 2023-02-20 20:04:01.251976 muon-0.1.4/muon/_atac/preproc.py
--rw-r--r--   0        0        0    44213 2023-06-07 09:07:57.087492 muon-0.1.4/muon/_atac/tools.py
--rw-r--r--   0        0        0      316 2023-06-07 09:07:57.088441 muon-0.1.4/muon/_atac/utils.py
--rw-r--r--   0        0        0        0 2023-02-20 20:04:01.252851 muon-0.1.4/muon/_core/__init__.py
--rw-r--r--   0        0        0     2032 2023-02-20 20:04:01.252993 muon-0.1.4/muon/_core/config.py
--rw-r--r--   0        0        0     3135 2023-02-20 20:04:41.107395 muon-0.1.4/muon/_core/io.py
--rw-r--r--   0        0        0    16661 2023-06-07 09:07:57.089174 muon-0.1.4/muon/_core/plot.py
--rw-r--r--   0        0        0    35383 2023-06-07 09:07:57.090694 muon-0.1.4/muon/_core/preproc.py
--rw-r--r--   0        0        0    52258 2023-06-07 09:07:57.091700 muon-0.1.4/muon/_core/tools.py
--rw-r--r--   0        0        0     8448 2023-02-20 20:04:01.254933 muon-0.1.4/muon/_core/utils.py
--rw-r--r--   0        0        0       46 2023-02-20 20:04:01.255165 muon-0.1.4/muon/_prot/__init__.py
--rw-r--r--   0        0        0      723 2023-02-20 20:04:01.255299 muon-0.1.4/muon/_prot/io.py
--rw-r--r--   0        0        0    10314 2023-06-07 09:07:57.092293 muon-0.1.4/muon/_prot/preproc.py
--rw-r--r--   0        0        0        0 2023-02-20 20:04:01.255631 muon-0.1.4/muon/_rna/__init__.py
--rw-r--r--   0        0        0     1270 2023-02-20 20:04:01.255794 muon-0.1.4/muon/_rna/utils.py
--rw-r--r--   0        0        0       21 2023-02-20 20:04:01.255949 muon-0.1.4/muon/atac.py
--rw-r--r--   0        0        0       21 2023-02-20 20:04:01.256101 muon-0.1.4/muon/prot.py
--rw-r--r--   0        0        0       20 2023-02-20 20:04:01.256224 muon-0.1.4/muon/rna.py
--rw-r--r--   0        0        0     1242 2023-06-07 09:07:57.092944 muon-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6313 1970-01-01 00:00:00.000000 muon-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4937 2023-06-07 09:07:57.080380 muon-0.1.5/README.md
+-rw-r--r--   0        0        0      343 2023-06-09 01:08:06.568554 muon-0.1.5/muon/__init__.py
+-rw-r--r--   0        0        0       97 2023-02-20 20:04:01.127617 muon-0.1.5/muon/_atac/__init__.py
+-rw-r--r--   0        0        0      296 2023-02-20 20:04:01.127870 muon-0.1.5/muon/_atac/_ref/jaspar/MA0002.2.pfm
+-rw-r--r--   0        0        0      384 2023-02-20 20:04:01.128008 muon-0.1.5/muon/_atac/_ref/jaspar/MA0003.4.pfm
+-rw-r--r--   0        0        0      149 2023-02-20 20:04:01.128199 muon-0.1.5/muon/_atac/_ref/jaspar/MA0004.1.pfm
+-rw-r--r--   0        0        0      149 2023-02-20 20:04:01.128343 muon-0.1.5/muon/_atac/_ref/jaspar/MA0006.1.pfm
+-rw-r--r--   0        0        0      466 2023-02-20 20:04:01.128493 muon-0.1.5/muon/_atac/_ref/jaspar/MA0007.3.pfm
+-rw-r--r--   0        0        0      435 2023-02-20 20:04:01.128651 muon-0.1.5/muon/_atac/_ref/jaspar/MA0009.2.pfm
+-rw-r--r--   0        0        0      324 2023-02-20 20:04:01.128808 muon-0.1.5/muon/_atac/_ref/jaspar/MA0014.3.pfm
+-rw-r--r--   0        0        0      357 2023-02-20 20:04:01.129002 muon-0.1.5/muon/_atac/_ref/jaspar/MA0017.2.pfm
+-rw-r--r--   0        0        0      360 2023-02-20 20:04:01.129214 muon-0.1.5/muon/_atac/_ref/jaspar/MA0018.4.pfm
+-rw-r--r--   0        0        0      318 2023-02-20 20:04:01.129440 muon-0.1.5/muon/_atac/_ref/jaspar/MA0019.1.pfm
+-rw-r--r--   0        0        0      323 2023-02-20 20:04:01.129703 muon-0.1.5/muon/_atac/_ref/jaspar/MA0024.3.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.129915 muon-0.1.5/muon/_atac/_ref/jaspar/MA0025.2.pfm
+-rw-r--r--   0        0        0      213 2023-02-20 20:04:01.130046 muon-0.1.5/muon/_atac/_ref/jaspar/MA0027.2.pfm
+-rw-r--r--   0        0        0      274 2023-02-20 20:04:01.130202 muon-0.1.5/muon/_atac/_ref/jaspar/MA0028.2.pfm
+-rw-r--r--   0        0        0      373 2023-02-20 20:04:01.130334 muon-0.1.5/muon/_atac/_ref/jaspar/MA0029.1.pfm
+-rw-r--r--   0        0        0      373 2023-02-20 20:04:01.130461 muon-0.1.5/muon/_atac/_ref/jaspar/MA0030.1.pfm
+-rw-r--r--   0        0        0      205 2023-02-20 20:04:01.130575 muon-0.1.5/muon/_atac/_ref/jaspar/MA0031.1.pfm
+-rw-r--r--   0        0        0      299 2023-02-20 20:04:01.130696 muon-0.1.5/muon/_atac/_ref/jaspar/MA0032.2.pfm
+-rw-r--r--   0        0        0      185 2023-02-20 20:04:01.130824 muon-0.1.5/muon/_atac/_ref/jaspar/MA0033.2.pfm
+-rw-r--r--   0        0        0      304 2023-02-20 20:04:01.131076 muon-0.1.5/muon/_atac/_ref/jaspar/MA0035.4.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.131237 muon-0.1.5/muon/_atac/_ref/jaspar/MA0036.3.pfm
+-rw-r--r--   0        0        0      210 2023-02-20 20:04:01.131379 muon-0.1.5/muon/_atac/_ref/jaspar/MA0037.3.pfm
+-rw-r--r--   0        0        0      329 2023-02-20 20:04:01.131524 muon-0.1.5/muon/_atac/_ref/jaspar/MA0038.2.pfm
+-rw-r--r--   0        0        0      332 2023-02-20 20:04:01.131656 muon-0.1.5/muon/_atac/_ref/jaspar/MA0039.4.pfm
+-rw-r--r--   0        0        0      288 2023-02-20 20:04:01.131787 muon-0.1.5/muon/_atac/_ref/jaspar/MA0040.1.pfm
+-rw-r--r--   0        0        0      318 2023-02-20 20:04:01.131919 muon-0.1.5/muon/_atac/_ref/jaspar/MA0041.1.pfm
+-rw-r--r--   0        0        0      182 2023-02-20 20:04:01.132055 muon-0.1.5/muon/_atac/_ref/jaspar/MA0042.2.pfm
+-rw-r--r--   0        0        0      384 2023-02-20 20:04:01.132205 muon-0.1.5/muon/_atac/_ref/jaspar/MA0043.3.pfm
+-rw-r--r--   0        0        0      412 2023-02-20 20:04:01.132361 muon-0.1.5/muon/_atac/_ref/jaspar/MA0046.2.pfm
+-rw-r--r--   0        0        0      305 2023-02-20 20:04:01.132497 muon-0.1.5/muon/_atac/_ref/jaspar/MA0047.3.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.132642 muon-0.1.5/muon/_atac/_ref/jaspar/MA0048.2.pfm
+-rw-r--r--   0        0        0      576 2023-02-20 20:04:01.132775 muon-0.1.5/muon/_atac/_ref/jaspar/MA0050.2.pfm
+-rw-r--r--   0        0        0      484 2023-02-20 20:04:01.132908 muon-0.1.5/muon/_atac/_ref/jaspar/MA0051.1.pfm
+-rw-r--r--   0        0        0      412 2023-02-20 20:04:01.133039 muon-0.1.5/muon/_atac/_ref/jaspar/MA0052.4.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.133170 muon-0.1.5/muon/_atac/_ref/jaspar/MA0056.2.pfm
+-rw-r--r--   0        0        0      260 2023-02-20 20:04:01.133293 muon-0.1.5/muon/_atac/_ref/jaspar/MA0057.1.pfm
+-rw-r--r--   0        0        0      271 2023-02-20 20:04:01.133546 muon-0.1.5/muon/_atac/_ref/jaspar/MA0058.3.pfm
+-rw-r--r--   0        0        0      288 2023-02-20 20:04:01.133717 muon-0.1.5/muon/_atac/_ref/jaspar/MA0059.1.pfm
+-rw-r--r--   0        0        0      298 2023-02-20 20:04:01.133873 muon-0.1.5/muon/_atac/_ref/jaspar/MA0060.3.pfm
+-rw-r--r--   0        0        0      388 2023-02-20 20:04:01.134025 muon-0.1.5/muon/_atac/_ref/jaspar/MA0062.3.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.134166 muon-0.1.5/muon/_atac/_ref/jaspar/MA0063.2.pfm
+-rw-r--r--   0        0        0      407 2023-02-20 20:04:01.134332 muon-0.1.5/muon/_atac/_ref/jaspar/MA0065.2.pfm
+-rw-r--r--   0        0        0      541 2023-02-20 20:04:01.134684 muon-0.1.5/muon/_atac/_ref/jaspar/MA0066.1.pfm
+-rw-r--r--   0        0        0      205 2023-02-20 20:04:01.134941 muon-0.1.5/muon/_atac/_ref/jaspar/MA0067.1.pfm
+-rw-r--r--   0        0        0      210 2023-02-20 20:04:01.135150 muon-0.1.5/muon/_atac/_ref/jaspar/MA0068.2.pfm
+-rw-r--r--   0        0        0      373 2023-02-20 20:04:01.135352 muon-0.1.5/muon/_atac/_ref/jaspar/MA0069.1.pfm
+-rw-r--r--   0        0        0      316 2023-02-20 20:04:01.135495 muon-0.1.5/muon/_atac/_ref/jaspar/MA0070.1.pfm
+-rw-r--r--   0        0        0      261 2023-02-20 20:04:01.135630 muon-0.1.5/muon/_atac/_ref/jaspar/MA0071.1.pfm
+-rw-r--r--   0        0        0      373 2023-02-20 20:04:01.135784 muon-0.1.5/muon/_atac/_ref/jaspar/MA0072.1.pfm
+-rw-r--r--   0        0        0      540 2023-02-20 20:04:01.135917 muon-0.1.5/muon/_atac/_ref/jaspar/MA0073.1.pfm
+-rw-r--r--   0        0        0      400 2023-02-20 20:04:01.136054 muon-0.1.5/muon/_atac/_ref/jaspar/MA0074.1.pfm
+-rw-r--r--   0        0        0      215 2023-02-20 20:04:01.136186 muon-0.1.5/muon/_atac/_ref/jaspar/MA0075.3.pfm
+-rw-r--r--   0        0        0      297 2023-02-20 20:04:01.136308 muon-0.1.5/muon/_atac/_ref/jaspar/MA0076.2.pfm
+-rw-r--r--   0        0        0      233 2023-02-20 20:04:01.136474 muon-0.1.5/muon/_atac/_ref/jaspar/MA0077.1.pfm
+-rw-r--r--   0        0        0      232 2023-02-20 20:04:01.136632 muon-0.1.5/muon/_atac/_ref/jaspar/MA0078.1.pfm
+-rw-r--r--   0        0        0      414 2023-02-20 20:04:01.136781 muon-0.1.5/muon/_atac/_ref/jaspar/MA0079.4.pfm
+-rw-r--r--   0        0        0      556 2023-02-20 20:04:01.136915 muon-0.1.5/muon/_atac/_ref/jaspar/MA0080.5.pfm
+-rw-r--r--   0        0        0      441 2023-02-20 20:04:01.137065 muon-0.1.5/muon/_atac/_ref/jaspar/MA0081.2.pfm
+-rw-r--r--   0        0        0      436 2023-02-20 20:04:01.137219 muon-0.1.5/muon/_atac/_ref/jaspar/MA0083.3.pfm
+-rw-r--r--   0        0        0      233 2023-02-20 20:04:01.137344 muon-0.1.5/muon/_atac/_ref/jaspar/MA0084.1.pfm
+-rw-r--r--   0        0        0      177 2023-02-20 20:04:01.137576 muon-0.1.5/muon/_atac/_ref/jaspar/MA0087.1.pfm
+-rw-r--r--   0        0        0      436 2023-02-20 20:04:01.137761 muon-0.1.5/muon/_atac/_ref/jaspar/MA0088.2.pfm
+-rw-r--r--   0        0        0      437 2023-02-20 20:04:01.137906 muon-0.1.5/muon/_atac/_ref/jaspar/MA0089.2.pfm
+-rw-r--r--   0        0        0      360 2023-02-20 20:04:01.138046 muon-0.1.5/muon/_atac/_ref/jaspar/MA0090.3.pfm
+-rw-r--r--   0        0        0      318 2023-02-20 20:04:01.138183 muon-0.1.5/muon/_atac/_ref/jaspar/MA0091.1.pfm
+-rw-r--r--   0        0        0      261 2023-02-20 20:04:01.138326 muon-0.1.5/muon/_atac/_ref/jaspar/MA0092.1.pfm
+-rw-r--r--   0        0        0      388 2023-02-20 20:04:01.138469 muon-0.1.5/muon/_atac/_ref/jaspar/MA0093.3.pfm
+-rw-r--r--   0        0        0      326 2023-02-20 20:04:01.138600 muon-0.1.5/muon/_atac/_ref/jaspar/MA0095.2.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.138839 muon-0.1.5/muon/_atac/_ref/jaspar/MA0098.3.pfm
+-rw-r--r--   0        0        0      267 2023-02-20 20:04:01.138997 muon-0.1.5/muon/_atac/_ref/jaspar/MA0099.3.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.139184 muon-0.1.5/muon/_atac/_ref/jaspar/MA0100.3.pfm
+-rw-r--r--   0        0        0      260 2023-02-20 20:04:01.139338 muon-0.1.5/muon/_atac/_ref/jaspar/MA0101.1.pfm
+-rw-r--r--   0        0        0      388 2023-02-20 20:04:01.139523 muon-0.1.5/muon/_atac/_ref/jaspar/MA0102.4.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.139819 muon-0.1.5/muon/_atac/_ref/jaspar/MA0103.3.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.140063 muon-0.1.5/muon/_atac/_ref/jaspar/MA0104.4.pfm
+-rw-r--r--   0        0        0      354 2023-02-20 20:04:01.140242 muon-0.1.5/muon/_atac/_ref/jaspar/MA0105.4.pfm
+-rw-r--r--   0        0        0      496 2023-02-20 20:04:01.140644 muon-0.1.5/muon/_atac/_ref/jaspar/MA0106.3.pfm
+-rw-r--r--   0        0        0      261 2023-02-20 20:04:01.141075 muon-0.1.5/muon/_atac/_ref/jaspar/MA0107.1.pfm
+-rw-r--r--   0        0        0      406 2023-02-20 20:04:01.141327 muon-0.1.5/muon/_atac/_ref/jaspar/MA0108.2.pfm
+-rw-r--r--   0        0        0      264 2023-02-20 20:04:01.141518 muon-0.1.5/muon/_atac/_ref/jaspar/MA0109.1.pfm
+-rw-r--r--   0        0        0      288 2023-02-20 20:04:01.141706 muon-0.1.5/muon/_atac/_ref/jaspar/MA0111.1.pfm
+-rw-r--r--   0        0        0      462 2023-02-20 20:04:01.142064 muon-0.1.5/muon/_atac/_ref/jaspar/MA0112.3.pfm
+-rw-r--r--   0        0        0      468 2023-02-20 20:04:01.142282 muon-0.1.5/muon/_atac/_ref/jaspar/MA0113.3.pfm
+-rw-r--r--   0        0        0      359 2023-02-20 20:04:01.142434 muon-0.1.5/muon/_atac/_ref/jaspar/MA0114.4.pfm
+-rw-r--r--   0        0        0      457 2023-02-20 20:04:01.142706 muon-0.1.5/muon/_atac/_ref/jaspar/MA0115.1.pfm
+-rw-r--r--   0        0        0      401 2023-02-20 20:04:01.143015 muon-0.1.5/muon/_atac/_ref/jaspar/MA0116.1.pfm
+-rw-r--r--   0        0        0      325 2023-02-20 20:04:01.143269 muon-0.1.5/muon/_atac/_ref/jaspar/MA0117.2.pfm
+-rw-r--r--   0        0        0      373 2023-02-20 20:04:01.143565 muon-0.1.5/muon/_atac/_ref/jaspar/MA0119.1.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.143773 muon-0.1.5/muon/_atac/_ref/jaspar/MA0122.3.pfm
+-rw-r--r--   0        0        0      242 2023-02-20 20:04:01.144054 muon-0.1.5/muon/_atac/_ref/jaspar/MA0124.2.pfm
+-rw-r--r--   0        0        0      205 2023-02-20 20:04:01.144340 muon-0.1.5/muon/_atac/_ref/jaspar/MA0125.1.pfm
+-rw-r--r--   0        0        0      148 2023-02-20 20:04:01.144556 muon-0.1.5/muon/_atac/_ref/jaspar/MA0130.1.pfm
+-rw-r--r--   0        0        0      323 2023-02-20 20:04:01.144775 muon-0.1.5/muon/_atac/_ref/jaspar/MA0131.2.pfm
+-rw-r--r--   0        0        0      215 2023-02-20 20:04:01.144986 muon-0.1.5/muon/_atac/_ref/jaspar/MA0132.2.pfm
+-rw-r--r--   0        0        0      344 2023-02-20 20:04:01.145188 muon-0.1.5/muon/_atac/_ref/jaspar/MA0135.1.pfm
+-rw-r--r--   0        0        0      297 2023-02-20 20:04:01.145402 muon-0.1.5/muon/_atac/_ref/jaspar/MA0136.2.pfm
+-rw-r--r--   0        0        0      297 2023-02-20 20:04:01.145697 muon-0.1.5/muon/_atac/_ref/jaspar/MA0137.3.pfm
+-rw-r--r--   0        0        0      576 2023-02-20 20:04:01.145894 muon-0.1.5/muon/_atac/_ref/jaspar/MA0138.2.pfm
+-rw-r--r--   0        0        0      518 2023-02-20 20:04:01.146162 muon-0.1.5/muon/_atac/_ref/jaspar/MA0139.1.pfm
+-rw-r--r--   0        0        0      494 2023-02-20 20:04:01.146437 muon-0.1.5/muon/_atac/_ref/jaspar/MA0140.2.pfm
+-rw-r--r--   0        0        0      296 2023-02-20 20:04:01.146654 muon-0.1.5/muon/_atac/_ref/jaspar/MA0141.3.pfm
+-rw-r--r--   0        0        0      406 2023-02-20 20:04:01.146921 muon-0.1.5/muon/_atac/_ref/jaspar/MA0142.1.pfm
+-rw-r--r--   0        0        0      304 2023-02-20 20:04:01.147096 muon-0.1.5/muon/_atac/_ref/jaspar/MA0143.4.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.147245 muon-0.1.5/muon/_atac/_ref/jaspar/MA0144.2.pfm
+-rw-r--r--   0        0        0      266 2023-02-20 20:04:01.147379 muon-0.1.5/muon/_atac/_ref/jaspar/MA0145.3.pfm
+-rw-r--r--   0        0        0      378 2023-02-20 20:04:01.147531 muon-0.1.5/muon/_atac/_ref/jaspar/MA0146.2.pfm
+-rw-r--r--   0        0        0      327 2023-02-20 20:04:01.147676 muon-0.1.5/muon/_atac/_ref/jaspar/MA0147.3.pfm
+-rw-r--r--   0        0        0      333 2023-02-20 20:04:01.147806 muon-0.1.5/muon/_atac/_ref/jaspar/MA0148.4.pfm
+-rw-r--r--   0        0        0      486 2023-02-20 20:04:01.147960 muon-0.1.5/muon/_atac/_ref/jaspar/MA0149.1.pfm
+-rw-r--r--   0        0        0      408 2023-02-20 20:04:01.148257 muon-0.1.5/muon/_atac/_ref/jaspar/MA0150.2.pfm
+-rw-r--r--   0        0        0      149 2023-02-20 20:04:01.148412 muon-0.1.5/muon/_atac/_ref/jaspar/MA0151.1.pfm
+-rw-r--r--   0        0        0      177 2023-02-20 20:04:01.148598 muon-0.1.5/muon/_atac/_ref/jaspar/MA0152.1.pfm
+-rw-r--r--   0        0        0      357 2023-02-20 20:04:01.148839 muon-0.1.5/muon/_atac/_ref/jaspar/MA0153.2.pfm
+-rw-r--r--   0        0        0      415 2023-02-20 20:04:01.149056 muon-0.1.5/muon/_atac/_ref/jaspar/MA0154.4.pfm
+-rw-r--r--   0        0        0      317 2023-02-20 20:04:01.149246 muon-0.1.5/muon/_atac/_ref/jaspar/MA0155.1.pfm
+-rw-r--r--   0        0        0      271 2023-02-20 20:04:01.149377 muon-0.1.5/muon/_atac/_ref/jaspar/MA0156.2.pfm
+-rw-r--r--   0        0        0      207 2023-02-20 20:04:01.149513 muon-0.1.5/muon/_atac/_ref/jaspar/MA0157.2.pfm
+-rw-r--r--   0        0        0      213 2023-02-20 20:04:01.149648 muon-0.1.5/muon/_atac/_ref/jaspar/MA0158.2.pfm
+-rw-r--r--   0        0        0      458 2023-02-20 20:04:01.149783 muon-0.1.5/muon/_atac/_ref/jaspar/MA0159.1.pfm
+-rw-r--r--   0        0        0      204 2023-02-20 20:04:01.149967 muon-0.1.5/muon/_atac/_ref/jaspar/MA0160.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.150213 muon-0.1.5/muon/_atac/_ref/jaspar/MA0161.2.pfm
+-rw-r--r--   0        0        0      385 2023-02-20 20:04:01.150429 muon-0.1.5/muon/_atac/_ref/jaspar/MA0162.4.pfm
+-rw-r--r--   0        0        0      373 2023-02-20 20:04:01.150577 muon-0.1.5/muon/_atac/_ref/jaspar/MA0163.1.pfm
+-rw-r--r--   0        0        0      177 2023-02-20 20:04:01.150710 muon-0.1.5/muon/_atac/_ref/jaspar/MA0164.1.pfm
+-rw-r--r--   0        0        0      409 2023-02-20 20:04:01.150852 muon-0.1.5/muon/_atac/_ref/jaspar/MA0258.2.pfm
+-rw-r--r--   0        0        0      207 2023-02-20 20:04:01.151007 muon-0.1.5/muon/_atac/_ref/jaspar/MA0259.1.pfm
+-rw-r--r--   0        0        0      296 2023-02-20 20:04:01.151132 muon-0.1.5/muon/_atac/_ref/jaspar/MA0442.2.pfm
+-rw-r--r--   0        0        0      267 2023-02-20 20:04:01.151252 muon-0.1.5/muon/_atac/_ref/jaspar/MA0461.2.pfm
+-rw-r--r--   0        0        0      302 2023-02-20 20:04:01.151446 muon-0.1.5/muon/_atac/_ref/jaspar/MA0462.2.pfm
+-rw-r--r--   0        0        0      440 2023-02-20 20:04:01.151583 muon-0.1.5/muon/_atac/_ref/jaspar/MA0463.2.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.151712 muon-0.1.5/muon/_atac/_ref/jaspar/MA0464.2.pfm
+-rw-r--r--   0        0        0      329 2023-02-20 20:04:01.151832 muon-0.1.5/muon/_atac/_ref/jaspar/MA0465.2.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.151948 muon-0.1.5/muon/_atac/_ref/jaspar/MA0466.2.pfm
+-rw-r--r--   0        0        0      297 2023-02-20 20:04:01.152062 muon-0.1.5/muon/_atac/_ref/jaspar/MA0467.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.152175 muon-0.1.5/muon/_atac/_ref/jaspar/MA0468.1.pfm
+-rw-r--r--   0        0        0      441 2023-02-20 20:04:01.152287 muon-0.1.5/muon/_atac/_ref/jaspar/MA0469.3.pfm
+-rw-r--r--   0        0        0      384 2023-02-20 20:04:01.152401 muon-0.1.5/muon/_atac/_ref/jaspar/MA0470.2.pfm
+-rw-r--r--   0        0        0      357 2023-02-20 20:04:01.152672 muon-0.1.5/muon/_atac/_ref/jaspar/MA0471.2.pfm
+-rw-r--r--   0        0        0      296 2023-02-20 20:04:01.152867 muon-0.1.5/muon/_atac/_ref/jaspar/MA0472.2.pfm
+-rw-r--r--   0        0        0      386 2023-02-20 20:04:01.153007 muon-0.1.5/muon/_atac/_ref/jaspar/MA0473.3.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.153137 muon-0.1.5/muon/_atac/_ref/jaspar/MA0474.2.pfm
+-rw-r--r--   0        0        0      273 2023-02-20 20:04:01.153257 muon-0.1.5/muon/_atac/_ref/jaspar/MA0475.2.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.153372 muon-0.1.5/muon/_atac/_ref/jaspar/MA0476.1.pfm
+-rw-r--r--   0        0        0      360 2023-02-20 20:04:01.153488 muon-0.1.5/muon/_atac/_ref/jaspar/MA0477.2.pfm
+-rw-r--r--   0        0        0      298 2023-02-20 20:04:01.153639 muon-0.1.5/muon/_atac/_ref/jaspar/MA0478.1.pfm
+-rw-r--r--   0        0        0      299 2023-02-20 20:04:01.153938 muon-0.1.5/muon/_atac/_ref/jaspar/MA0479.1.pfm
+-rw-r--r--   0        0        0      297 2023-02-20 20:04:01.154153 muon-0.1.5/muon/_atac/_ref/jaspar/MA0480.1.pfm
+-rw-r--r--   0        0        0      304 2023-02-20 20:04:01.154318 muon-0.1.5/muon/_atac/_ref/jaspar/MA0481.3.pfm
+-rw-r--r--   0        0        0      332 2023-02-20 20:04:01.154488 muon-0.1.5/muon/_atac/_ref/jaspar/MA0482.2.pfm
+-rw-r--r--   0        0        0      296 2023-02-20 20:04:01.154636 muon-0.1.5/muon/_atac/_ref/jaspar/MA0483.1.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.154780 muon-0.1.5/muon/_atac/_ref/jaspar/MA0484.2.pfm
+-rw-r--r--   0        0        0      270 2023-02-20 20:04:01.154902 muon-0.1.5/muon/_atac/_ref/jaspar/MA0485.2.pfm
+-rw-r--r--   0        0        0      350 2023-02-20 20:04:01.155021 muon-0.1.5/muon/_atac/_ref/jaspar/MA0486.2.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.155249 muon-0.1.5/muon/_atac/_ref/jaspar/MA0488.1.pfm
+-rw-r--r--   0        0        0      384 2023-02-20 20:04:01.155454 muon-0.1.5/muon/_atac/_ref/jaspar/MA0489.1.pfm
+-rw-r--r--   0        0        0      360 2023-02-20 20:04:01.155691 muon-0.1.5/muon/_atac/_ref/jaspar/MA0490.2.pfm
+-rw-r--r--   0        0        0      360 2023-02-20 20:04:01.155911 muon-0.1.5/muon/_atac/_ref/jaspar/MA0491.2.pfm
+-rw-r--r--   0        0        0      413 2023-02-20 20:04:01.156132 muon-0.1.5/muon/_atac/_ref/jaspar/MA0492.1.pfm
+-rw-r--r--   0        0        0      294 2023-02-20 20:04:01.156332 muon-0.1.5/muon/_atac/_ref/jaspar/MA0493.1.pfm
+-rw-r--r--   0        0        0      517 2023-02-20 20:04:01.156652 muon-0.1.5/muon/_atac/_ref/jaspar/MA0494.1.pfm
+-rw-r--r--   0        0        0      442 2023-02-20 20:04:01.157021 muon-0.1.5/muon/_atac/_ref/jaspar/MA0495.3.pfm
+-rw-r--r--   0        0        0      415 2023-02-20 20:04:01.157261 muon-0.1.5/muon/_atac/_ref/jaspar/MA0496.3.pfm
+-rw-r--r--   0        0        0      408 2023-02-20 20:04:01.157480 muon-0.1.5/muon/_atac/_ref/jaspar/MA0497.1.pfm
+-rw-r--r--   0        0        0      191 2023-02-20 20:04:01.157826 muon-0.1.5/muon/_atac/_ref/jaspar/MA0498.2.pfm
+-rw-r--r--   0        0        0      357 2023-02-20 20:04:01.158061 muon-0.1.5/muon/_atac/_ref/jaspar/MA0499.2.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.158305 muon-0.1.5/muon/_atac/_ref/jaspar/MA0500.2.pfm
+-rw-r--r--   0        0        0      405 2023-02-20 20:04:01.158537 muon-0.1.5/muon/_atac/_ref/jaspar/MA0501.1.pfm
+-rw-r--r--   0        0        0      327 2023-02-20 20:04:01.158753 muon-0.1.5/muon/_atac/_ref/jaspar/MA0502.2.pfm
+-rw-r--r--   0        0        0      297 2023-02-20 20:04:01.158959 muon-0.1.5/muon/_atac/_ref/jaspar/MA0503.1.pfm
+-rw-r--r--   0        0        0      406 2023-02-20 20:04:01.159150 muon-0.1.5/muon/_atac/_ref/jaspar/MA0504.1.pfm
+-rw-r--r--   0        0        0      408 2023-02-20 20:04:01.159288 muon-0.1.5/muon/_atac/_ref/jaspar/MA0505.1.pfm
+-rw-r--r--   0        0        0      295 2023-02-20 20:04:01.159411 muon-0.1.5/muon/_atac/_ref/jaspar/MA0506.1.pfm
+-rw-r--r--   0        0        0      352 2023-02-20 20:04:01.159538 muon-0.1.5/muon/_atac/_ref/jaspar/MA0507.1.pfm
+-rw-r--r--   0        0        0      302 2023-02-20 20:04:01.159738 muon-0.1.5/muon/_atac/_ref/jaspar/MA0508.3.pfm
+-rw-r--r--   0        0        0      384 2023-02-20 20:04:01.159929 muon-0.1.5/muon/_atac/_ref/jaspar/MA0509.2.pfm
+-rw-r--r--   0        0        0      437 2023-02-20 20:04:01.160149 muon-0.1.5/muon/_atac/_ref/jaspar/MA0510.2.pfm
+-rw-r--r--   0        0        0      243 2023-02-20 20:04:01.160350 muon-0.1.5/muon/_atac/_ref/jaspar/MA0511.2.pfm
+-rw-r--r--   0        0        0      386 2023-02-20 20:04:01.160507 muon-0.1.5/muon/_atac/_ref/jaspar/MA0512.2.pfm
+-rw-r--r--   0        0        0      352 2023-02-20 20:04:01.160645 muon-0.1.5/muon/_atac/_ref/jaspar/MA0513.1.pfm
+-rw-r--r--   0        0        0      267 2023-02-20 20:04:01.160795 muon-0.1.5/muon/_atac/_ref/jaspar/MA0514.1.pfm
+-rw-r--r--   0        0        0      264 2023-02-20 20:04:01.160932 muon-0.1.5/muon/_atac/_ref/jaspar/MA0515.1.pfm
+-rw-r--r--   0        0        0      464 2023-02-20 20:04:01.161140 muon-0.1.5/muon/_atac/_ref/jaspar/MA0516.2.pfm
+-rw-r--r--   0        0        0      405 2023-02-20 20:04:01.161317 muon-0.1.5/muon/_atac/_ref/jaspar/MA0517.1.pfm
+-rw-r--r--   0        0        0      382 2023-02-20 20:04:01.161453 muon-0.1.5/muon/_atac/_ref/jaspar/MA0518.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.161623 muon-0.1.5/muon/_atac/_ref/jaspar/MA0519.1.pfm
+-rw-r--r--   0        0        0      408 2023-02-20 20:04:01.161755 muon-0.1.5/muon/_atac/_ref/jaspar/MA0520.1.pfm
+-rw-r--r--   0        0        0      298 2023-02-20 20:04:01.161909 muon-0.1.5/muon/_atac/_ref/jaspar/MA0521.1.pfm
+-rw-r--r--   0        0        0      301 2023-02-20 20:04:01.162094 muon-0.1.5/muon/_atac/_ref/jaspar/MA0522.3.pfm
+-rw-r--r--   0        0        0      382 2023-02-20 20:04:01.162248 muon-0.1.5/muon/_atac/_ref/jaspar/MA0523.1.pfm
+-rw-r--r--   0        0        0      327 2023-02-20 20:04:01.162382 muon-0.1.5/muon/_atac/_ref/jaspar/MA0524.2.pfm
+-rw-r--r--   0        0        0      492 2023-02-20 20:04:01.162529 muon-0.1.5/muon/_atac/_ref/jaspar/MA0525.2.pfm
+-rw-r--r--   0        0        0      385 2023-02-20 20:04:01.162664 muon-0.1.5/muon/_atac/_ref/jaspar/MA0526.3.pfm
+-rw-r--r--   0        0        0      407 2023-02-20 20:04:01.162838 muon-0.1.5/muon/_atac/_ref/jaspar/MA0527.1.pfm
+-rw-r--r--   0        0        0      331 2023-02-20 20:04:01.162976 muon-0.1.5/muon/_atac/_ref/jaspar/MA0528.2.pfm
+-rw-r--r--   0        0        0      404 2023-02-20 20:04:01.163165 muon-0.1.5/muon/_atac/_ref/jaspar/MA0591.1.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.163301 muon-0.1.5/muon/_atac/_ref/jaspar/MA0592.3.pfm
+-rw-r--r--   0        0        0      296 2023-02-20 20:04:01.163417 muon-0.1.5/muon/_atac/_ref/jaspar/MA0593.1.pfm
+-rw-r--r--   0        0        0      267 2023-02-20 20:04:01.163561 muon-0.1.5/muon/_atac/_ref/jaspar/MA0594.2.pfm
+-rw-r--r--   0        0        0      263 2023-02-20 20:04:01.163688 muon-0.1.5/muon/_atac/_ref/jaspar/MA0595.1.pfm
+-rw-r--r--   0        0        0      262 2023-02-20 20:04:01.163825 muon-0.1.5/muon/_atac/_ref/jaspar/MA0596.1.pfm
+-rw-r--r--   0        0        0      236 2023-02-20 20:04:01.163954 muon-0.1.5/muon/_atac/_ref/jaspar/MA0597.1.pfm
+-rw-r--r--   0        0        0      412 2023-02-20 20:04:01.164202 muon-0.1.5/muon/_atac/_ref/jaspar/MA0598.3.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.164422 muon-0.1.5/muon/_atac/_ref/jaspar/MA0599.1.pfm
+-rw-r--r--   0        0        0      440 2023-02-20 20:04:01.164636 muon-0.1.5/muon/_atac/_ref/jaspar/MA0600.2.pfm
+-rw-r--r--   0        0        0      296 2023-02-20 20:04:01.164777 muon-0.1.5/muon/_atac/_ref/jaspar/MA0601.1.pfm
+-rw-r--r--   0        0        0      376 2023-02-20 20:04:01.164899 muon-0.1.5/muon/_atac/_ref/jaspar/MA0602.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.165015 muon-0.1.5/muon/_atac/_ref/jaspar/MA0603.1.pfm
+-rw-r--r--   0        0        0      210 2023-02-20 20:04:01.165128 muon-0.1.5/muon/_atac/_ref/jaspar/MA0604.1.pfm
+-rw-r--r--   0        0        0      329 2023-02-20 20:04:01.165239 muon-0.1.5/muon/_atac/_ref/jaspar/MA0605.2.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.165380 muon-0.1.5/muon/_atac/_ref/jaspar/MA0606.1.pfm
+-rw-r--r--   0        0        0      210 2023-02-20 20:04:01.165573 muon-0.1.5/muon/_atac/_ref/jaspar/MA0607.1.pfm
+-rw-r--r--   0        0        0      236 2023-02-20 20:04:01.165690 muon-0.1.5/muon/_atac/_ref/jaspar/MA0608.1.pfm
+-rw-r--r--   0        0        0      440 2023-02-20 20:04:01.165810 muon-0.1.5/muon/_atac/_ref/jaspar/MA0609.2.pfm
+-rw-r--r--   0        0        0      296 2023-02-20 20:04:01.165928 muon-0.1.5/muon/_atac/_ref/jaspar/MA0610.1.pfm
+-rw-r--r--   0        0        0      212 2023-02-20 20:04:01.166161 muon-0.1.5/muon/_atac/_ref/jaspar/MA0611.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.166333 muon-0.1.5/muon/_atac/_ref/jaspar/MA0612.2.pfm
+-rw-r--r--   0        0        0      208 2023-02-20 20:04:01.166588 muon-0.1.5/muon/_atac/_ref/jaspar/MA0613.1.pfm
+-rw-r--r--   0        0        0      208 2023-02-20 20:04:01.166762 muon-0.1.5/muon/_atac/_ref/jaspar/MA0614.1.pfm
+-rw-r--r--   0        0        0      460 2023-02-20 20:04:01.166996 muon-0.1.5/muon/_atac/_ref/jaspar/MA0615.1.pfm
+-rw-r--r--   0        0        0      270 2023-02-20 20:04:01.167151 muon-0.1.5/muon/_atac/_ref/jaspar/MA0616.2.pfm
+-rw-r--r--   0        0        0      212 2023-02-20 20:04:01.167289 muon-0.1.5/muon/_atac/_ref/jaspar/MA0618.1.pfm
+-rw-r--r--   0        0        0      239 2023-02-20 20:04:01.167427 muon-0.1.5/muon/_atac/_ref/jaspar/MA0619.1.pfm
+-rw-r--r--   0        0        0      500 2023-02-20 20:04:01.167646 muon-0.1.5/muon/_atac/_ref/jaspar/MA0620.3.pfm
+-rw-r--r--   0        0        0      296 2023-02-20 20:04:01.167866 muon-0.1.5/muon/_atac/_ref/jaspar/MA0621.1.pfm
+-rw-r--r--   0        0        0      211 2023-02-20 20:04:01.168043 muon-0.1.5/muon/_atac/_ref/jaspar/MA0622.1.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.168207 muon-0.1.5/muon/_atac/_ref/jaspar/MA0623.2.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.168456 muon-0.1.5/muon/_atac/_ref/jaspar/MA0624.1.pfm
+-rw-r--r--   0        0        0      267 2023-02-20 20:04:01.168661 muon-0.1.5/muon/_atac/_ref/jaspar/MA0625.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.168872 muon-0.1.5/muon/_atac/_ref/jaspar/MA0626.1.pfm
+-rw-r--r--   0        0        0      360 2023-02-20 20:04:01.169038 muon-0.1.5/muon/_atac/_ref/jaspar/MA0627.2.pfm
+-rw-r--r--   0        0        0      267 2023-02-20 20:04:01.169194 muon-0.1.5/muon/_atac/_ref/jaspar/MA0628.1.pfm
+-rw-r--r--   0        0        0      460 2023-02-20 20:04:01.169321 muon-0.1.5/muon/_atac/_ref/jaspar/MA0629.1.pfm
+-rw-r--r--   0        0        0      212 2023-02-20 20:04:01.169451 muon-0.1.5/muon/_atac/_ref/jaspar/MA0630.1.pfm
+-rw-r--r--   0        0        0      459 2023-02-20 20:04:01.169598 muon-0.1.5/muon/_atac/_ref/jaspar/MA0631.1.pfm
+-rw-r--r--   0        0        0      275 2023-02-20 20:04:01.169737 muon-0.1.5/muon/_atac/_ref/jaspar/MA0632.2.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.169869 muon-0.1.5/muon/_atac/_ref/jaspar/MA0633.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.170033 muon-0.1.5/muon/_atac/_ref/jaspar/MA0634.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.170169 muon-0.1.5/muon/_atac/_ref/jaspar/MA0635.1.pfm
+-rw-r--r--   0        0        0      270 2023-02-20 20:04:01.170404 muon-0.1.5/muon/_atac/_ref/jaspar/MA0636.1.pfm
+-rw-r--r--   0        0        0      407 2023-02-20 20:04:01.170543 muon-0.1.5/muon/_atac/_ref/jaspar/MA0637.1.pfm
+-rw-r--r--   0        0        0      377 2023-02-20 20:04:01.170680 muon-0.1.5/muon/_atac/_ref/jaspar/MA0638.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.170835 muon-0.1.5/muon/_atac/_ref/jaspar/MA0639.1.pfm
+-rw-r--r--   0        0        0      388 2023-02-20 20:04:01.170962 muon-0.1.5/muon/_atac/_ref/jaspar/MA0640.2.pfm
+-rw-r--r--   0        0        0      324 2023-02-20 20:04:01.171090 muon-0.1.5/muon/_atac/_ref/jaspar/MA0641.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.171220 muon-0.1.5/muon/_atac/_ref/jaspar/MA0642.1.pfm
+-rw-r--r--   0        0        0      273 2023-02-20 20:04:01.171496 muon-0.1.5/muon/_atac/_ref/jaspar/MA0643.1.pfm
+-rw-r--r--   0        0        0      273 2023-02-20 20:04:01.171673 muon-0.1.5/muon/_atac/_ref/jaspar/MA0644.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.171821 muon-0.1.5/muon/_atac/_ref/jaspar/MA0645.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.171958 muon-0.1.5/muon/_atac/_ref/jaspar/MA0646.1.pfm
+-rw-r--r--   0        0        0      325 2023-02-20 20:04:01.172098 muon-0.1.5/muon/_atac/_ref/jaspar/MA0647.1.pfm
+-rw-r--r--   0        0        0      271 2023-02-20 20:04:01.172232 muon-0.1.5/muon/_atac/_ref/jaspar/MA0648.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.172364 muon-0.1.5/muon/_atac/_ref/jaspar/MA0649.1.pfm
+-rw-r--r--   0        0        0      295 2023-02-20 20:04:01.172489 muon-0.1.5/muon/_atac/_ref/jaspar/MA0650.2.pfm
+-rw-r--r--   0        0        0      297 2023-02-20 20:04:01.172628 muon-0.1.5/muon/_atac/_ref/jaspar/MA0651.1.pfm
+-rw-r--r--   0        0        0      383 2023-02-20 20:04:01.172839 muon-0.1.5/muon/_atac/_ref/jaspar/MA0652.1.pfm
+-rw-r--r--   0        0        0      407 2023-02-20 20:04:01.172988 muon-0.1.5/muon/_atac/_ref/jaspar/MA0653.1.pfm
+-rw-r--r--   0        0        0      212 2023-02-20 20:04:01.173125 muon-0.1.5/muon/_atac/_ref/jaspar/MA0654.1.pfm
+-rw-r--r--   0        0        0      238 2023-02-20 20:04:01.173267 muon-0.1.5/muon/_atac/_ref/jaspar/MA0655.1.pfm
+-rw-r--r--   0        0        0      329 2023-02-20 20:04:01.173418 muon-0.1.5/muon/_atac/_ref/jaspar/MA0656.1.pfm
+-rw-r--r--   0        0        0      493 2023-02-20 20:04:01.173560 muon-0.1.5/muon/_atac/_ref/jaspar/MA0657.1.pfm
+-rw-r--r--   0        0        0      270 2023-02-20 20:04:01.173804 muon-0.1.5/muon/_atac/_ref/jaspar/MA0658.1.pfm
+-rw-r--r--   0        0        0      412 2023-02-20 20:04:01.173966 muon-0.1.5/muon/_atac/_ref/jaspar/MA0659.2.pfm
+-rw-r--r--   0        0        0      325 2023-02-20 20:04:01.174124 muon-0.1.5/muon/_atac/_ref/jaspar/MA0660.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.174260 muon-0.1.5/muon/_atac/_ref/jaspar/MA0661.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.174396 muon-0.1.5/muon/_atac/_ref/jaspar/MA0662.1.pfm
+-rw-r--r--   0        0        0      265 2023-02-20 20:04:01.174604 muon-0.1.5/muon/_atac/_ref/jaspar/MA0663.1.pfm
+-rw-r--r--   0        0        0      267 2023-02-20 20:04:01.174781 muon-0.1.5/muon/_atac/_ref/jaspar/MA0664.1.pfm
+-rw-r--r--   0        0        0      262 2023-02-20 20:04:01.174955 muon-0.1.5/muon/_atac/_ref/jaspar/MA0665.1.pfm
+-rw-r--r--   0        0        0      213 2023-02-20 20:04:01.175095 muon-0.1.5/muon/_atac/_ref/jaspar/MA0666.1.pfm
+-rw-r--r--   0        0        0      264 2023-02-20 20:04:01.175229 muon-0.1.5/muon/_atac/_ref/jaspar/MA0667.1.pfm
+-rw-r--r--   0        0        0      267 2023-02-20 20:04:01.175401 muon-0.1.5/muon/_atac/_ref/jaspar/MA0668.1.pfm
+-rw-r--r--   0        0        0      264 2023-02-20 20:04:01.175571 muon-0.1.5/muon/_atac/_ref/jaspar/MA0669.1.pfm
+-rw-r--r--   0        0        0      276 2023-02-20 20:04:01.175727 muon-0.1.5/muon/_atac/_ref/jaspar/MA0670.1.pfm
+-rw-r--r--   0        0        0      244 2023-02-20 20:04:01.175867 muon-0.1.5/muon/_atac/_ref/jaspar/MA0671.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.175993 muon-0.1.5/muon/_atac/_ref/jaspar/MA0672.1.pfm
+-rw-r--r--   0        0        0      243 2023-02-20 20:04:01.176116 muon-0.1.5/muon/_atac/_ref/jaspar/MA0673.1.pfm
+-rw-r--r--   0        0        0      212 2023-02-20 20:04:01.176250 muon-0.1.5/muon/_atac/_ref/jaspar/MA0674.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.176388 muon-0.1.5/muon/_atac/_ref/jaspar/MA0675.1.pfm
+-rw-r--r--   0        0        0      241 2023-02-20 20:04:01.176522 muon-0.1.5/muon/_atac/_ref/jaspar/MA0676.1.pfm
+-rw-r--r--   0        0        0      378 2023-02-20 20:04:01.176722 muon-0.1.5/muon/_atac/_ref/jaspar/MA0677.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.176948 muon-0.1.5/muon/_atac/_ref/jaspar/MA0678.1.pfm
+-rw-r--r--   0        0        0      444 2023-02-20 20:04:01.177157 muon-0.1.5/muon/_atac/_ref/jaspar/MA0679.2.pfm
+-rw-r--r--   0        0        0      267 2023-02-20 20:04:01.177358 muon-0.1.5/muon/_atac/_ref/jaspar/MA0680.1.pfm
+-rw-r--r--   0        0        0      442 2023-02-20 20:04:01.177563 muon-0.1.5/muon/_atac/_ref/jaspar/MA0681.2.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.177763 muon-0.1.5/muon/_atac/_ref/jaspar/MA0682.2.pfm
+-rw-r--r--   0        0        0      437 2023-02-20 20:04:01.177896 muon-0.1.5/muon/_atac/_ref/jaspar/MA0683.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.178029 muon-0.1.5/muon/_atac/_ref/jaspar/MA0684.2.pfm
+-rw-r--r--   0        0        0      466 2023-02-20 20:04:01.178213 muon-0.1.5/muon/_atac/_ref/jaspar/MA0685.1.pfm
+-rw-r--r--   0        0        0      297 2023-02-20 20:04:01.178389 muon-0.1.5/muon/_atac/_ref/jaspar/MA0686.1.pfm
+-rw-r--r--   0        0        0      377 2023-02-20 20:04:01.178534 muon-0.1.5/muon/_atac/_ref/jaspar/MA0687.1.pfm
+-rw-r--r--   0        0        0      297 2023-02-20 20:04:01.178676 muon-0.1.5/muon/_atac/_ref/jaspar/MA0688.1.pfm
+-rw-r--r--   0        0        0      294 2023-02-20 20:04:01.178813 muon-0.1.5/muon/_atac/_ref/jaspar/MA0689.1.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.179025 muon-0.1.5/muon/_atac/_ref/jaspar/MA0690.1.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.179242 muon-0.1.5/muon/_atac/_ref/jaspar/MA0691.1.pfm
+-rw-r--r--   0        0        0      271 2023-02-20 20:04:01.179437 muon-0.1.5/muon/_atac/_ref/jaspar/MA0692.1.pfm
+-rw-r--r--   0        0        0      211 2023-02-20 20:04:01.179612 muon-0.1.5/muon/_atac/_ref/jaspar/MA0693.2.pfm
+-rw-r--r--   0        0        0      324 2023-02-20 20:04:01.179747 muon-0.1.5/muon/_atac/_ref/jaspar/MA0694.1.pfm
+-rw-r--r--   0        0        0      324 2023-02-20 20:04:01.179892 muon-0.1.5/muon/_atac/_ref/jaspar/MA0695.1.pfm
+-rw-r--r--   0        0        0      385 2023-02-20 20:04:01.180043 muon-0.1.5/muon/_atac/_ref/jaspar/MA0696.1.pfm
+-rw-r--r--   0        0        0      405 2023-02-20 20:04:01.180186 muon-0.1.5/muon/_atac/_ref/jaspar/MA0697.1.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.180340 muon-0.1.5/muon/_atac/_ref/jaspar/MA0698.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.180559 muon-0.1.5/muon/_atac/_ref/jaspar/MA0699.1.pfm
+-rw-r--r--   0        0        0      299 2023-02-20 20:04:01.180728 muon-0.1.5/muon/_atac/_ref/jaspar/MA0700.2.pfm
+-rw-r--r--   0        0        0      215 2023-02-20 20:04:01.180873 muon-0.1.5/muon/_atac/_ref/jaspar/MA0701.2.pfm
+-rw-r--r--   0        0        0      213 2023-02-20 20:04:01.181019 muon-0.1.5/muon/_atac/_ref/jaspar/MA0702.2.pfm
+-rw-r--r--   0        0        0      297 2023-02-20 20:04:01.181138 muon-0.1.5/muon/_atac/_ref/jaspar/MA0703.2.pfm
+-rw-r--r--   0        0        0      213 2023-02-20 20:04:01.181257 muon-0.1.5/muon/_atac/_ref/jaspar/MA0704.1.pfm
+-rw-r--r--   0        0        0      214 2023-02-20 20:04:01.181388 muon-0.1.5/muon/_atac/_ref/jaspar/MA0705.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.181560 muon-0.1.5/muon/_atac/_ref/jaspar/MA0706.1.pfm
+-rw-r--r--   0        0        0      267 2023-02-20 20:04:01.181849 muon-0.1.5/muon/_atac/_ref/jaspar/MA0707.1.pfm
+-rw-r--r--   0        0        0      213 2023-02-20 20:04:01.182009 muon-0.1.5/muon/_atac/_ref/jaspar/MA0708.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.182143 muon-0.1.5/muon/_atac/_ref/jaspar/MA0709.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.182287 muon-0.1.5/muon/_atac/_ref/jaspar/MA0710.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.182426 muon-0.1.5/muon/_atac/_ref/jaspar/MA0711.1.pfm
+-rw-r--r--   0        0        0      332 2023-02-20 20:04:01.182570 muon-0.1.5/muon/_atac/_ref/jaspar/MA0712.2.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.182694 muon-0.1.5/muon/_atac/_ref/jaspar/MA0713.1.pfm
+-rw-r--r--   0        0        0      244 2023-02-20 20:04:01.182807 muon-0.1.5/muon/_atac/_ref/jaspar/MA0714.1.pfm
+-rw-r--r--   0        0        0      293 2023-02-20 20:04:01.183050 muon-0.1.5/muon/_atac/_ref/jaspar/MA0715.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.183230 muon-0.1.5/muon/_atac/_ref/jaspar/MA0716.1.pfm
+-rw-r--r--   0        0        0      218 2023-02-20 20:04:01.183378 muon-0.1.5/muon/_atac/_ref/jaspar/MA0717.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.183511 muon-0.1.5/muon/_atac/_ref/jaspar/MA0718.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.183644 muon-0.1.5/muon/_atac/_ref/jaspar/MA0719.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.183773 muon-0.1.5/muon/_atac/_ref/jaspar/MA0720.1.pfm
+-rw-r--r--   0        0        0      218 2023-02-20 20:04:01.183902 muon-0.1.5/muon/_atac/_ref/jaspar/MA0721.1.pfm
+-rw-r--r--   0        0        0      214 2023-02-20 20:04:01.184028 muon-0.1.5/muon/_atac/_ref/jaspar/MA0722.1.pfm
+-rw-r--r--   0        0        0      215 2023-02-20 20:04:01.184155 muon-0.1.5/muon/_atac/_ref/jaspar/MA0723.1.pfm
+-rw-r--r--   0        0        0      244 2023-02-20 20:04:01.184338 muon-0.1.5/muon/_atac/_ref/jaspar/MA0724.1.pfm
+-rw-r--r--   0        0        0      214 2023-02-20 20:04:01.184494 muon-0.1.5/muon/_atac/_ref/jaspar/MA0725.1.pfm
+-rw-r--r--   0        0        0      214 2023-02-20 20:04:01.184645 muon-0.1.5/muon/_atac/_ref/jaspar/MA0726.1.pfm
+-rw-r--r--   0        0        0      470 2023-02-20 20:04:01.184809 muon-0.1.5/muon/_atac/_ref/jaspar/MA0727.1.pfm
+-rw-r--r--   0        0        0      405 2023-02-20 20:04:01.184970 muon-0.1.5/muon/_atac/_ref/jaspar/MA0728.1.pfm
+-rw-r--r--   0        0        0      488 2023-02-20 20:04:01.185132 muon-0.1.5/muon/_atac/_ref/jaspar/MA0729.1.pfm
+-rw-r--r--   0        0        0      462 2023-02-20 20:04:01.185282 muon-0.1.5/muon/_atac/_ref/jaspar/MA0730.1.pfm
+-rw-r--r--   0        0        0      459 2023-02-20 20:04:01.185439 muon-0.1.5/muon/_atac/_ref/jaspar/MA0731.1.pfm
+-rw-r--r--   0        0        0      408 2023-02-20 20:04:01.185635 muon-0.1.5/muon/_atac/_ref/jaspar/MA0732.1.pfm
+-rw-r--r--   0        0        0      440 2023-02-20 20:04:01.185940 muon-0.1.5/muon/_atac/_ref/jaspar/MA0733.1.pfm
+-rw-r--r--   0        0        0      412 2023-02-20 20:04:01.186130 muon-0.1.5/muon/_atac/_ref/jaspar/MA0734.2.pfm
+-rw-r--r--   0        0        0      438 2023-02-20 20:04:01.186280 muon-0.1.5/muon/_atac/_ref/jaspar/MA0735.1.pfm
+-rw-r--r--   0        0        0      379 2023-02-20 20:04:01.186418 muon-0.1.5/muon/_atac/_ref/jaspar/MA0736.1.pfm
+-rw-r--r--   0        0        0      377 2023-02-20 20:04:01.186550 muon-0.1.5/muon/_atac/_ref/jaspar/MA0737.1.pfm
+-rw-r--r--   0        0        0      242 2023-02-20 20:04:01.186682 muon-0.1.5/muon/_atac/_ref/jaspar/MA0738.1.pfm
+-rw-r--r--   0        0        0      242 2023-02-20 20:04:01.186814 muon-0.1.5/muon/_atac/_ref/jaspar/MA0739.1.pfm
+-rw-r--r--   0        0        0      380 2023-02-20 20:04:01.186995 muon-0.1.5/muon/_atac/_ref/jaspar/MA0740.1.pfm
+-rw-r--r--   0        0        0      297 2023-02-20 20:04:01.187203 muon-0.1.5/muon/_atac/_ref/jaspar/MA0741.1.pfm
+-rw-r--r--   0        0        0      408 2023-02-20 20:04:01.187364 muon-0.1.5/muon/_atac/_ref/jaspar/MA0742.1.pfm
+-rw-r--r--   0        0        0      444 2023-02-20 20:04:01.187578 muon-0.1.5/muon/_atac/_ref/jaspar/MA0743.2.pfm
+-rw-r--r--   0        0        0      444 2023-02-20 20:04:01.187879 muon-0.1.5/muon/_atac/_ref/jaspar/MA0744.2.pfm
+-rw-r--r--   0        0        0      359 2023-02-20 20:04:01.188048 muon-0.1.5/muon/_atac/_ref/jaspar/MA0745.2.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.188200 muon-0.1.5/muon/_atac/_ref/jaspar/MA0746.2.pfm
+-rw-r--r--   0        0        0      320 2023-02-20 20:04:01.188338 muon-0.1.5/muon/_atac/_ref/jaspar/MA0747.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.188589 muon-0.1.5/muon/_atac/_ref/jaspar/MA0748.2.pfm
+-rw-r--r--   0        0        0      354 2023-02-20 20:04:01.188780 muon-0.1.5/muon/_atac/_ref/jaspar/MA0749.1.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.188999 muon-0.1.5/muon/_atac/_ref/jaspar/MA0750.2.pfm
+-rw-r--r--   0        0        0      410 2023-02-20 20:04:01.189286 muon-0.1.5/muon/_atac/_ref/jaspar/MA0751.1.pfm
+-rw-r--r--   0        0        0      465 2023-02-20 20:04:01.189565 muon-0.1.5/muon/_atac/_ref/jaspar/MA0752.1.pfm
+-rw-r--r--   0        0        0      352 2023-02-20 20:04:01.189744 muon-0.1.5/muon/_atac/_ref/jaspar/MA0753.2.pfm
+-rw-r--r--   0        0        0      273 2023-02-20 20:04:01.189886 muon-0.1.5/muon/_atac/_ref/jaspar/MA0754.1.pfm
+-rw-r--r--   0        0        0      273 2023-02-20 20:04:01.190120 muon-0.1.5/muon/_atac/_ref/jaspar/MA0755.1.pfm
+-rw-r--r--   0        0        0      381 2023-02-20 20:04:01.190364 muon-0.1.5/muon/_atac/_ref/jaspar/MA0756.1.pfm
+-rw-r--r--   0        0        0      383 2023-02-20 20:04:01.190526 muon-0.1.5/muon/_atac/_ref/jaspar/MA0757.1.pfm
+-rw-r--r--   0        0        0      379 2023-02-20 20:04:01.190700 muon-0.1.5/muon/_atac/_ref/jaspar/MA0758.1.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.190886 muon-0.1.5/muon/_atac/_ref/jaspar/MA0759.1.pfm
+-rw-r--r--   0        0        0      263 2023-02-20 20:04:01.191053 muon-0.1.5/muon/_atac/_ref/jaspar/MA0760.1.pfm
+-rw-r--r--   0        0        0      385 2023-02-20 20:04:01.191190 muon-0.1.5/muon/_atac/_ref/jaspar/MA0761.2.pfm
+-rw-r--r--   0        0        0      297 2023-02-20 20:04:01.191323 muon-0.1.5/muon/_atac/_ref/jaspar/MA0762.1.pfm
+-rw-r--r--   0        0        0      265 2023-02-20 20:04:01.191469 muon-0.1.5/muon/_atac/_ref/jaspar/MA0763.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.191616 muon-0.1.5/muon/_atac/_ref/jaspar/MA0764.2.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.191801 muon-0.1.5/muon/_atac/_ref/jaspar/MA0765.2.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.191945 muon-0.1.5/muon/_atac/_ref/jaspar/MA0766.2.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.192072 muon-0.1.5/muon/_atac/_ref/jaspar/MA0767.1.pfm
+-rw-r--r--   0        0        0      408 2023-02-20 20:04:01.192259 muon-0.1.5/muon/_atac/_ref/jaspar/MA0768.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.192520 muon-0.1.5/muon/_atac/_ref/jaspar/MA0769.2.pfm
+-rw-r--r--   0        0        0      351 2023-02-20 20:04:01.192696 muon-0.1.5/muon/_atac/_ref/jaspar/MA0770.1.pfm
+-rw-r--r--   0        0        0      357 2023-02-20 20:04:01.192838 muon-0.1.5/muon/_atac/_ref/jaspar/MA0771.1.pfm
+-rw-r--r--   0        0        0      379 2023-02-20 20:04:01.192976 muon-0.1.5/muon/_atac/_ref/jaspar/MA0772.1.pfm
+-rw-r--r--   0        0        0      327 2023-02-20 20:04:01.193108 muon-0.1.5/muon/_atac/_ref/jaspar/MA0773.1.pfm
+-rw-r--r--   0        0        0      213 2023-02-20 20:04:01.193240 muon-0.1.5/muon/_atac/_ref/jaspar/MA0774.1.pfm
+-rw-r--r--   0        0        0      214 2023-02-20 20:04:01.193384 muon-0.1.5/muon/_atac/_ref/jaspar/MA0775.1.pfm
+-rw-r--r--   0        0        0      324 2023-02-20 20:04:01.193580 muon-0.1.5/muon/_atac/_ref/jaspar/MA0776.1.pfm
+-rw-r--r--   0        0        0      406 2023-02-20 20:04:01.193801 muon-0.1.5/muon/_atac/_ref/jaspar/MA0777.1.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.193956 muon-0.1.5/muon/_atac/_ref/jaspar/MA0778.1.pfm
+-rw-r--r--   0        0        0      466 2023-02-20 20:04:01.194172 muon-0.1.5/muon/_atac/_ref/jaspar/MA0779.1.pfm
+-rw-r--r--   0        0        0      270 2023-02-20 20:04:01.194405 muon-0.1.5/muon/_atac/_ref/jaspar/MA0780.1.pfm
+-rw-r--r--   0        0        0      466 2023-02-20 20:04:01.194678 muon-0.1.5/muon/_atac/_ref/jaspar/MA0781.1.pfm
+-rw-r--r--   0        0        0      413 2023-02-20 20:04:01.194916 muon-0.1.5/muon/_atac/_ref/jaspar/MA0782.2.pfm
+-rw-r--r--   0        0        0      320 2023-02-20 20:04:01.195134 muon-0.1.5/muon/_atac/_ref/jaspar/MA0783.1.pfm
+-rw-r--r--   0        0        0      381 2023-02-20 20:04:01.195299 muon-0.1.5/muon/_atac/_ref/jaspar/MA0784.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.195543 muon-0.1.5/muon/_atac/_ref/jaspar/MA0785.1.pfm
+-rw-r--r--   0        0        0      326 2023-02-20 20:04:01.195767 muon-0.1.5/muon/_atac/_ref/jaspar/MA0786.1.pfm
+-rw-r--r--   0        0        0      323 2023-02-20 20:04:01.195998 muon-0.1.5/muon/_atac/_ref/jaspar/MA0787.1.pfm
+-rw-r--r--   0        0        0      351 2023-02-20 20:04:01.196179 muon-0.1.5/muon/_atac/_ref/jaspar/MA0788.1.pfm
+-rw-r--r--   0        0        0      242 2023-02-20 20:04:01.196372 muon-0.1.5/muon/_atac/_ref/jaspar/MA0789.1.pfm
+-rw-r--r--   0        0        0      383 2023-02-20 20:04:01.196577 muon-0.1.5/muon/_atac/_ref/jaspar/MA0790.1.pfm
+-rw-r--r--   0        0        0      437 2023-02-20 20:04:01.196760 muon-0.1.5/muon/_atac/_ref/jaspar/MA0791.1.pfm
+-rw-r--r--   0        0        0      243 2023-02-20 20:04:01.196917 muon-0.1.5/muon/_atac/_ref/jaspar/MA0792.1.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.197158 muon-0.1.5/muon/_atac/_ref/jaspar/MA0793.1.pfm
+-rw-r--r--   0        0        0      326 2023-02-20 20:04:01.197360 muon-0.1.5/muon/_atac/_ref/jaspar/MA0794.1.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.197516 muon-0.1.5/muon/_atac/_ref/jaspar/MA0795.1.pfm
+-rw-r--r--   0        0        0      322 2023-02-20 20:04:01.197664 muon-0.1.5/muon/_atac/_ref/jaspar/MA0796.1.pfm
+-rw-r--r--   0        0        0      326 2023-02-20 20:04:01.197825 muon-0.1.5/muon/_atac/_ref/jaspar/MA0797.1.pfm
+-rw-r--r--   0        0        0      382 2023-02-20 20:04:01.197963 muon-0.1.5/muon/_atac/_ref/jaspar/MA0798.2.pfm
+-rw-r--r--   0        0        0      440 2023-02-20 20:04:01.198125 muon-0.1.5/muon/_atac/_ref/jaspar/MA0799.1.pfm
+-rw-r--r--   0        0        0      355 2023-02-20 20:04:01.198260 muon-0.1.5/muon/_atac/_ref/jaspar/MA0800.1.pfm
+-rw-r--r--   0        0        0      217 2023-02-20 20:04:01.198393 muon-0.1.5/muon/_atac/_ref/jaspar/MA0801.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.198518 muon-0.1.5/muon/_atac/_ref/jaspar/MA0802.1.pfm
+-rw-r--r--   0        0        0      213 2023-02-20 20:04:01.198633 muon-0.1.5/muon/_atac/_ref/jaspar/MA0803.1.pfm
+-rw-r--r--   0        0        0      554 2023-02-20 20:04:01.198752 muon-0.1.5/muon/_atac/_ref/jaspar/MA0804.1.pfm
+-rw-r--r--   0        0        0      215 2023-02-20 20:04:01.198875 muon-0.1.5/muon/_atac/_ref/jaspar/MA0805.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.199006 muon-0.1.5/muon/_atac/_ref/jaspar/MA0806.1.pfm
+-rw-r--r--   0        0        0      212 2023-02-20 20:04:01.199144 muon-0.1.5/muon/_atac/_ref/jaspar/MA0807.1.pfm
+-rw-r--r--   0        0        0      215 2023-02-20 20:04:01.199276 muon-0.1.5/muon/_atac/_ref/jaspar/MA0808.1.pfm
+-rw-r--r--   0        0        0      332 2023-02-20 20:04:01.199401 muon-0.1.5/muon/_atac/_ref/jaspar/MA0809.2.pfm
+-rw-r--r--   0        0        0      326 2023-02-20 20:04:01.199557 muon-0.1.5/muon/_atac/_ref/jaspar/MA0810.1.pfm
+-rw-r--r--   0        0        0      325 2023-02-20 20:04:01.199782 muon-0.1.5/muon/_atac/_ref/jaspar/MA0811.1.pfm
+-rw-r--r--   0        0        0      299 2023-02-20 20:04:01.199922 muon-0.1.5/muon/_atac/_ref/jaspar/MA0812.1.pfm
+-rw-r--r--   0        0        0      351 2023-02-20 20:04:01.200054 muon-0.1.5/muon/_atac/_ref/jaspar/MA0813.1.pfm
+-rw-r--r--   0        0        0      388 2023-02-20 20:04:01.200175 muon-0.1.5/muon/_atac/_ref/jaspar/MA0814.2.pfm
+-rw-r--r--   0        0        0      353 2023-02-20 20:04:01.200304 muon-0.1.5/muon/_atac/_ref/jaspar/MA0815.1.pfm
+-rw-r--r--   0        0        0      265 2023-02-20 20:04:01.200435 muon-0.1.5/muon/_atac/_ref/jaspar/MA0816.1.pfm
+-rw-r--r--   0        0        0      325 2023-02-20 20:04:01.200560 muon-0.1.5/muon/_atac/_ref/jaspar/MA0817.1.pfm
+-rw-r--r--   0        0        0      266 2023-02-20 20:04:01.200687 muon-0.1.5/muon/_atac/_ref/jaspar/MA0818.1.pfm
+-rw-r--r--   0        0        0      265 2023-02-20 20:04:01.200836 muon-0.1.5/muon/_atac/_ref/jaspar/MA0819.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.200962 muon-0.1.5/muon/_atac/_ref/jaspar/MA0820.1.pfm
+-rw-r--r--   0        0        0      323 2023-02-20 20:04:01.201086 muon-0.1.5/muon/_atac/_ref/jaspar/MA0821.1.pfm
+-rw-r--r--   0        0        0      323 2023-02-20 20:04:01.201218 muon-0.1.5/muon/_atac/_ref/jaspar/MA0822.1.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.201352 muon-0.1.5/muon/_atac/_ref/jaspar/MA0823.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.201480 muon-0.1.5/muon/_atac/_ref/jaspar/MA0825.1.pfm
+-rw-r--r--   0        0        0      271 2023-02-20 20:04:01.201600 muon-0.1.5/muon/_atac/_ref/jaspar/MA0826.1.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.201715 muon-0.1.5/muon/_atac/_ref/jaspar/MA0827.1.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.201847 muon-0.1.5/muon/_atac/_ref/jaspar/MA0828.1.pfm
+-rw-r--r--   0        0        0      384 2023-02-20 20:04:01.202022 muon-0.1.5/muon/_atac/_ref/jaspar/MA0829.2.pfm
+-rw-r--r--   0        0        0      357 2023-02-20 20:04:01.202193 muon-0.1.5/muon/_atac/_ref/jaspar/MA0830.2.pfm
+-rw-r--r--   0        0        0      206 2023-02-20 20:04:01.202358 muon-0.1.5/muon/_atac/_ref/jaspar/MA0831.2.pfm
+-rw-r--r--   0        0        0      376 2023-02-20 20:04:01.202531 muon-0.1.5/muon/_atac/_ref/jaspar/MA0832.1.pfm
+-rw-r--r--   0        0        0      385 2023-02-20 20:04:01.202702 muon-0.1.5/muon/_atac/_ref/jaspar/MA0833.2.pfm
+-rw-r--r--   0        0        0      384 2023-02-20 20:04:01.202870 muon-0.1.5/muon/_atac/_ref/jaspar/MA0834.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.203039 muon-0.1.5/muon/_atac/_ref/jaspar/MA0835.2.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.203207 muon-0.1.5/muon/_atac/_ref/jaspar/MA0836.2.pfm
+-rw-r--r--   0        0        0      270 2023-02-20 20:04:01.203380 muon-0.1.5/muon/_atac/_ref/jaspar/MA0837.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.203533 muon-0.1.5/muon/_atac/_ref/jaspar/MA0838.1.pfm
+-rw-r--r--   0        0        0      380 2023-02-20 20:04:01.203650 muon-0.1.5/muon/_atac/_ref/jaspar/MA0839.1.pfm
+-rw-r--r--   0        0        0      326 2023-02-20 20:04:01.203772 muon-0.1.5/muon/_atac/_ref/jaspar/MA0840.1.pfm
+-rw-r--r--   0        0        0      299 2023-02-20 20:04:01.203894 muon-0.1.5/muon/_atac/_ref/jaspar/MA0841.1.pfm
+-rw-r--r--   0        0        0      357 2023-02-20 20:04:01.204023 muon-0.1.5/muon/_atac/_ref/jaspar/MA0842.2.pfm
+-rw-r--r--   0        0        0      326 2023-02-20 20:04:01.204152 muon-0.1.5/muon/_atac/_ref/jaspar/MA0843.1.pfm
+-rw-r--r--   0        0        0      382 2023-02-20 20:04:01.204282 muon-0.1.5/muon/_atac/_ref/jaspar/MA0844.1.pfm
+-rw-r--r--   0        0        0      298 2023-02-20 20:04:01.204431 muon-0.1.5/muon/_atac/_ref/jaspar/MA0845.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.204569 muon-0.1.5/muon/_atac/_ref/jaspar/MA0846.1.pfm
+-rw-r--r--   0        0        0      355 2023-02-20 20:04:01.204779 muon-0.1.5/muon/_atac/_ref/jaspar/MA0847.2.pfm
+-rw-r--r--   0        0        0      183 2023-02-20 20:04:01.204926 muon-0.1.5/muon/_atac/_ref/jaspar/MA0848.1.pfm
+-rw-r--r--   0        0        0      182 2023-02-20 20:04:01.205058 muon-0.1.5/muon/_atac/_ref/jaspar/MA0849.1.pfm
+-rw-r--r--   0        0        0      179 2023-02-20 20:04:01.205175 muon-0.1.5/muon/_atac/_ref/jaspar/MA0850.1.pfm
+-rw-r--r--   0        0        0      460 2023-02-20 20:04:01.205376 muon-0.1.5/muon/_atac/_ref/jaspar/MA0851.1.pfm
+-rw-r--r--   0        0        0      380 2023-02-20 20:04:01.205566 muon-0.1.5/muon/_atac/_ref/jaspar/MA0852.2.pfm
+-rw-r--r--   0        0        0      460 2023-02-20 20:04:01.205714 muon-0.1.5/muon/_atac/_ref/jaspar/MA0853.1.pfm
+-rw-r--r--   0        0        0      460 2023-02-20 20:04:01.205917 muon-0.1.5/muon/_atac/_ref/jaspar/MA0854.1.pfm
+-rw-r--r--   0        0        0      382 2023-02-20 20:04:01.206068 muon-0.1.5/muon/_atac/_ref/jaspar/MA0855.1.pfm
+-rw-r--r--   0        0        0      385 2023-02-20 20:04:01.206209 muon-0.1.5/muon/_atac/_ref/jaspar/MA0856.1.pfm
+-rw-r--r--   0        0        0      437 2023-02-20 20:04:01.206385 muon-0.1.5/muon/_atac/_ref/jaspar/MA0857.1.pfm
+-rw-r--r--   0        0        0      459 2023-02-20 20:04:01.206619 muon-0.1.5/muon/_atac/_ref/jaspar/MA0858.1.pfm
+-rw-r--r--   0        0        0      442 2023-02-20 20:04:01.206756 muon-0.1.5/muon/_atac/_ref/jaspar/MA0859.1.pfm
+-rw-r--r--   0        0        0      463 2023-02-20 20:04:01.206883 muon-0.1.5/muon/_atac/_ref/jaspar/MA0860.1.pfm
+-rw-r--r--   0        0        0      495 2023-02-20 20:04:01.207013 muon-0.1.5/muon/_atac/_ref/jaspar/MA0861.1.pfm
+-rw-r--r--   0        0        0      210 2023-02-20 20:04:01.207146 muon-0.1.5/muon/_atac/_ref/jaspar/MA0862.1.pfm
+-rw-r--r--   0        0        0      373 2023-02-20 20:04:01.207344 muon-0.1.5/muon/_atac/_ref/jaspar/MA0863.1.pfm
+-rw-r--r--   0        0        0      438 2023-02-20 20:04:01.207504 muon-0.1.5/muon/_atac/_ref/jaspar/MA0864.2.pfm
+-rw-r--r--   0        0        0      317 2023-02-20 20:04:01.207654 muon-0.1.5/muon/_atac/_ref/jaspar/MA0865.1.pfm
+-rw-r--r--   0        0        0      409 2023-02-20 20:04:01.207796 muon-0.1.5/muon/_atac/_ref/jaspar/MA0866.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.207934 muon-0.1.5/muon/_atac/_ref/jaspar/MA0867.2.pfm
+-rw-r--r--   0        0        0      270 2023-02-20 20:04:01.208203 muon-0.1.5/muon/_atac/_ref/jaspar/MA0868.2.pfm
+-rw-r--r--   0        0        0      402 2023-02-20 20:04:01.208350 muon-0.1.5/muon/_atac/_ref/jaspar/MA0869.1.pfm
+-rw-r--r--   0        0        0      409 2023-02-20 20:04:01.208496 muon-0.1.5/muon/_atac/_ref/jaspar/MA0870.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.208721 muon-0.1.5/muon/_atac/_ref/jaspar/MA0871.2.pfm
+-rw-r--r--   0        0        0      352 2023-02-20 20:04:01.208953 muon-0.1.5/muon/_atac/_ref/jaspar/MA0872.1.pfm
+-rw-r--r--   0        0        0      295 2023-02-20 20:04:01.209114 muon-0.1.5/muon/_atac/_ref/jaspar/MA0873.1.pfm
+-rw-r--r--   0        0        0      460 2023-02-20 20:04:01.209250 muon-0.1.5/muon/_atac/_ref/jaspar/MA0874.1.pfm
+-rw-r--r--   0        0        0      215 2023-02-20 20:04:01.209379 muon-0.1.5/muon/_atac/_ref/jaspar/MA0875.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.209507 muon-0.1.5/muon/_atac/_ref/jaspar/MA0876.1.pfm
+-rw-r--r--   0        0        0      214 2023-02-20 20:04:01.209634 muon-0.1.5/muon/_atac/_ref/jaspar/MA0877.2.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.209751 muon-0.1.5/muon/_atac/_ref/jaspar/MA0878.2.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.209865 muon-0.1.5/muon/_atac/_ref/jaspar/MA0879.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.210067 muon-0.1.5/muon/_atac/_ref/jaspar/MA0880.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.210218 muon-0.1.5/muon/_atac/_ref/jaspar/MA0881.1.pfm
+-rw-r--r--   0        0        0      212 2023-02-20 20:04:01.210410 muon-0.1.5/muon/_atac/_ref/jaspar/MA0882.1.pfm
+-rw-r--r--   0        0        0      460 2023-02-20 20:04:01.210677 muon-0.1.5/muon/_atac/_ref/jaspar/MA0883.1.pfm
+-rw-r--r--   0        0        0      352 2023-02-20 20:04:01.210956 muon-0.1.5/muon/_atac/_ref/jaspar/MA0884.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.211122 muon-0.1.5/muon/_atac/_ref/jaspar/MA0885.1.pfm
+-rw-r--r--   0        0        0      274 2023-02-20 20:04:01.211264 muon-0.1.5/muon/_atac/_ref/jaspar/MA0886.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.211396 muon-0.1.5/muon/_atac/_ref/jaspar/MA0887.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.211536 muon-0.1.5/muon/_atac/_ref/jaspar/MA0888.1.pfm
+-rw-r--r--   0        0        0      273 2023-02-20 20:04:01.211664 muon-0.1.5/muon/_atac/_ref/jaspar/MA0889.1.pfm
+-rw-r--r--   0        0        0      273 2023-02-20 20:04:01.211820 muon-0.1.5/muon/_atac/_ref/jaspar/MA0890.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.212028 muon-0.1.5/muon/_atac/_ref/jaspar/MA0891.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.212192 muon-0.1.5/muon/_atac/_ref/jaspar/MA0892.1.pfm
+-rw-r--r--   0        0        0      212 2023-02-20 20:04:01.212329 muon-0.1.5/muon/_atac/_ref/jaspar/MA0893.2.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.212465 muon-0.1.5/muon/_atac/_ref/jaspar/MA0894.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.212652 muon-0.1.5/muon/_atac/_ref/jaspar/MA0895.1.pfm
+-rw-r--r--   0        0        0      460 2023-02-20 20:04:01.212802 muon-0.1.5/muon/_atac/_ref/jaspar/MA0896.1.pfm
+-rw-r--r--   0        0        0      459 2023-02-20 20:04:01.212929 muon-0.1.5/muon/_atac/_ref/jaspar/MA0897.1.pfm
+-rw-r--r--   0        0        0      459 2023-02-20 20:04:01.213056 muon-0.1.5/muon/_atac/_ref/jaspar/MA0898.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.213295 muon-0.1.5/muon/_atac/_ref/jaspar/MA0899.1.pfm
+-rw-r--r--   0        0        0      218 2023-02-20 20:04:01.213460 muon-0.1.5/muon/_atac/_ref/jaspar/MA0900.2.pfm
+-rw-r--r--   0        0        0      388 2023-02-20 20:04:01.213605 muon-0.1.5/muon/_atac/_ref/jaspar/MA0901.2.pfm
+-rw-r--r--   0        0        0      215 2023-02-20 20:04:01.213738 muon-0.1.5/muon/_atac/_ref/jaspar/MA0902.2.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.213872 muon-0.1.5/muon/_atac/_ref/jaspar/MA0903.1.pfm
+-rw-r--r--   0        0        0      214 2023-02-20 20:04:01.214007 muon-0.1.5/muon/_atac/_ref/jaspar/MA0904.2.pfm
+-rw-r--r--   0        0        0      270 2023-02-20 20:04:01.214172 muon-0.1.5/muon/_atac/_ref/jaspar/MA0905.1.pfm
+-rw-r--r--   0        0        0      298 2023-02-20 20:04:01.214294 muon-0.1.5/muon/_atac/_ref/jaspar/MA0906.1.pfm
+-rw-r--r--   0        0        0      296 2023-02-20 20:04:01.214412 muon-0.1.5/muon/_atac/_ref/jaspar/MA0907.1.pfm
+-rw-r--r--   0        0        0      265 2023-02-20 20:04:01.214617 muon-0.1.5/muon/_atac/_ref/jaspar/MA0908.1.pfm
+-rw-r--r--   0        0        0      294 2023-02-20 20:04:01.214761 muon-0.1.5/muon/_atac/_ref/jaspar/MA0909.2.pfm
+-rw-r--r--   0        0        0      213 2023-02-20 20:04:01.214894 muon-0.1.5/muon/_atac/_ref/jaspar/MA0910.2.pfm
+-rw-r--r--   0        0        0      324 2023-02-20 20:04:01.215021 muon-0.1.5/muon/_atac/_ref/jaspar/MA0911.1.pfm
+-rw-r--r--   0        0        0      215 2023-02-20 20:04:01.215149 muon-0.1.5/muon/_atac/_ref/jaspar/MA0912.2.pfm
+-rw-r--r--   0        0        0      271 2023-02-20 20:04:01.215277 muon-0.1.5/muon/_atac/_ref/jaspar/MA0913.2.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.215401 muon-0.1.5/muon/_atac/_ref/jaspar/MA0914.1.pfm
+-rw-r--r--   0        0        0      273 2023-02-20 20:04:01.215528 muon-0.1.5/muon/_atac/_ref/jaspar/MA1099.2.pfm
+-rw-r--r--   0        0        0      270 2023-02-20 20:04:01.215690 muon-0.1.5/muon/_atac/_ref/jaspar/MA1100.2.pfm
+-rw-r--r--   0        0        0      528 2023-02-20 20:04:01.215823 muon-0.1.5/muon/_atac/_ref/jaspar/MA1101.2.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.215949 muon-0.1.5/muon/_atac/_ref/jaspar/MA1102.2.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.216081 muon-0.1.5/muon/_atac/_ref/jaspar/MA1103.2.pfm
+-rw-r--r--   0        0        0      360 2023-02-20 20:04:01.216217 muon-0.1.5/muon/_atac/_ref/jaspar/MA1104.2.pfm
+-rw-r--r--   0        0        0      329 2023-02-20 20:04:01.216357 muon-0.1.5/muon/_atac/_ref/jaspar/MA1105.2.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.216486 muon-0.1.5/muon/_atac/_ref/jaspar/MA1106.1.pfm
+-rw-r--r--   0        0        0      441 2023-02-20 20:04:01.216613 muon-0.1.5/muon/_atac/_ref/jaspar/MA1107.2.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.216804 muon-0.1.5/muon/_atac/_ref/jaspar/MA1108.2.pfm
+-rw-r--r--   0        0        0      352 2023-02-20 20:04:01.216975 muon-0.1.5/muon/_atac/_ref/jaspar/MA1109.1.pfm
+-rw-r--r--   0        0        0      294 2023-02-20 20:04:01.217115 muon-0.1.5/muon/_atac/_ref/jaspar/MA1110.1.pfm
+-rw-r--r--   0        0        0      296 2023-02-20 20:04:01.217242 muon-0.1.5/muon/_atac/_ref/jaspar/MA1111.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.217369 muon-0.1.5/muon/_atac/_ref/jaspar/MA1112.2.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.217501 muon-0.1.5/muon/_atac/_ref/jaspar/MA1113.2.pfm
+-rw-r--r--   0        0        0      468 2023-02-20 20:04:01.217631 muon-0.1.5/muon/_atac/_ref/jaspar/MA1114.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.217853 muon-0.1.5/muon/_atac/_ref/jaspar/MA1115.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.217997 muon-0.1.5/muon/_atac/_ref/jaspar/MA1116.1.pfm
+-rw-r--r--   0        0        0      297 2023-02-20 20:04:01.218147 muon-0.1.5/muon/_atac/_ref/jaspar/MA1117.1.pfm
+-rw-r--r--   0        0        0      294 2023-02-20 20:04:01.218277 muon-0.1.5/muon/_atac/_ref/jaspar/MA1118.1.pfm
+-rw-r--r--   0        0        0      440 2023-02-20 20:04:01.218405 muon-0.1.5/muon/_atac/_ref/jaspar/MA1119.1.pfm
+-rw-r--r--   0        0        0      298 2023-02-20 20:04:01.218539 muon-0.1.5/muon/_atac/_ref/jaspar/MA1120.1.pfm
+-rw-r--r--   0        0        0      352 2023-02-20 20:04:01.218658 muon-0.1.5/muon/_atac/_ref/jaspar/MA1121.1.pfm
+-rw-r--r--   0        0        0      296 2023-02-20 20:04:01.218775 muon-0.1.5/muon/_atac/_ref/jaspar/MA1122.1.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.218901 muon-0.1.5/muon/_atac/_ref/jaspar/MA1123.2.pfm
+-rw-r--r--   0        0        0      357 2023-02-20 20:04:01.219029 muon-0.1.5/muon/_atac/_ref/jaspar/MA1124.1.pfm
+-rw-r--r--   0        0        0      329 2023-02-20 20:04:01.219161 muon-0.1.5/muon/_atac/_ref/jaspar/MA1125.1.pfm
+-rw-r--r--   0        0        0      435 2023-02-20 20:04:01.219353 muon-0.1.5/muon/_atac/_ref/jaspar/MA1126.1.pfm
+-rw-r--r--   0        0        0      295 2023-02-20 20:04:01.219496 muon-0.1.5/muon/_atac/_ref/jaspar/MA1127.1.pfm
+-rw-r--r--   0        0        0      352 2023-02-20 20:04:01.219632 muon-0.1.5/muon/_atac/_ref/jaspar/MA1128.1.pfm
+-rw-r--r--   0        0        0      266 2023-02-20 20:04:01.219764 muon-0.1.5/muon/_atac/_ref/jaspar/MA1129.1.pfm
+-rw-r--r--   0        0        0      324 2023-02-20 20:04:01.219895 muon-0.1.5/muon/_atac/_ref/jaspar/MA1130.1.pfm
+-rw-r--r--   0        0        0      295 2023-02-20 20:04:01.220027 muon-0.1.5/muon/_atac/_ref/jaspar/MA1131.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.220140 muon-0.1.5/muon/_atac/_ref/jaspar/MA1132.1.pfm
+-rw-r--r--   0        0        0      323 2023-02-20 20:04:01.220312 muon-0.1.5/muon/_atac/_ref/jaspar/MA1133.1.pfm
+-rw-r--r--   0        0        0      324 2023-02-20 20:04:01.220567 muon-0.1.5/muon/_atac/_ref/jaspar/MA1134.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.220715 muon-0.1.5/muon/_atac/_ref/jaspar/MA1135.1.pfm
+-rw-r--r--   0        0        0      266 2023-02-20 20:04:01.220955 muon-0.1.5/muon/_atac/_ref/jaspar/MA1136.1.pfm
+-rw-r--r--   0        0        0      352 2023-02-20 20:04:01.221115 muon-0.1.5/muon/_atac/_ref/jaspar/MA1137.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.221324 muon-0.1.5/muon/_atac/_ref/jaspar/MA1138.1.pfm
+-rw-r--r--   0        0        0      324 2023-02-20 20:04:01.221579 muon-0.1.5/muon/_atac/_ref/jaspar/MA1139.1.pfm
+-rw-r--r--   0        0        0      321 2023-02-20 20:04:01.221785 muon-0.1.5/muon/_atac/_ref/jaspar/MA1140.2.pfm
+-rw-r--r--   0        0        0      352 2023-02-20 20:04:01.221952 muon-0.1.5/muon/_atac/_ref/jaspar/MA1141.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.222102 muon-0.1.5/muon/_atac/_ref/jaspar/MA1142.1.pfm
+-rw-r--r--   0        0        0      266 2023-02-20 20:04:01.222248 muon-0.1.5/muon/_atac/_ref/jaspar/MA1143.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.222406 muon-0.1.5/muon/_atac/_ref/jaspar/MA1144.1.pfm
+-rw-r--r--   0        0        0      408 2023-02-20 20:04:01.222597 muon-0.1.5/muon/_atac/_ref/jaspar/MA1145.1.pfm
+-rw-r--r--   0        0        0      408 2023-02-20 20:04:01.222733 muon-0.1.5/muon/_atac/_ref/jaspar/MA1146.1.pfm
+-rw-r--r--   0        0        0      408 2023-02-20 20:04:01.223033 muon-0.1.5/muon/_atac/_ref/jaspar/MA1147.1.pfm
+-rw-r--r--   0        0        0      492 2023-02-20 20:04:01.223217 muon-0.1.5/muon/_atac/_ref/jaspar/MA1148.1.pfm
+-rw-r--r--   0        0        0      492 2023-02-20 20:04:01.223509 muon-0.1.5/muon/_atac/_ref/jaspar/MA1149.1.pfm
+-rw-r--r--   0        0        0      294 2023-02-20 20:04:01.223666 muon-0.1.5/muon/_atac/_ref/jaspar/MA1150.1.pfm
+-rw-r--r--   0        0        0      324 2023-02-20 20:04:01.223804 muon-0.1.5/muon/_atac/_ref/jaspar/MA1151.1.pfm
+-rw-r--r--   0        0        0      267 2023-02-20 20:04:01.223945 muon-0.1.5/muon/_atac/_ref/jaspar/MA1152.1.pfm
+-rw-r--r--   0        0        0      210 2023-02-20 20:04:01.224175 muon-0.1.5/muon/_atac/_ref/jaspar/MA1153.1.pfm
+-rw-r--r--   0        0        0      461 2023-02-20 20:04:01.224372 muon-0.1.5/muon/_atac/_ref/jaspar/MA1154.1.pfm
+-rw-r--r--   0        0        0      409 2023-02-20 20:04:01.224519 muon-0.1.5/muon/_atac/_ref/jaspar/MA1155.1.pfm
+-rw-r--r--   0        0        0      580 2023-02-20 20:04:01.224658 muon-0.1.5/muon/_atac/_ref/jaspar/MA1418.1.pfm
+-rw-r--r--   0        0        0      415 2023-02-20 20:04:01.224792 muon-0.1.5/muon/_atac/_ref/jaspar/MA1419.1.pfm
+-rw-r--r--   0        0        0      377 2023-02-20 20:04:01.224911 muon-0.1.5/muon/_atac/_ref/jaspar/MA1420.1.pfm
+-rw-r--r--   0        0        0      320 2023-02-20 20:04:01.225024 muon-0.1.5/muon/_atac/_ref/jaspar/MA1421.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.225135 muon-0.1.5/muon/_atac/_ref/jaspar/MA1463.1.pfm
+-rw-r--r--   0        0        0      274 2023-02-20 20:04:01.225280 muon-0.1.5/muon/_atac/_ref/jaspar/MA1464.1.pfm
+-rw-r--r--   0        0        0      379 2023-02-20 20:04:01.225410 muon-0.1.5/muon/_atac/_ref/jaspar/MA1466.1.pfm
+-rw-r--r--   0        0        0      267 2023-02-20 20:04:01.225535 muon-0.1.5/muon/_atac/_ref/jaspar/MA1467.1.pfm
+-rw-r--r--   0        0        0      266 2023-02-20 20:04:01.225663 muon-0.1.5/muon/_atac/_ref/jaspar/MA1468.1.pfm
+-rw-r--r--   0        0        0      545 2023-02-20 20:04:01.225797 muon-0.1.5/muon/_atac/_ref/jaspar/MA1470.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.225931 muon-0.1.5/muon/_atac/_ref/jaspar/MA1471.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.226062 muon-0.1.5/muon/_atac/_ref/jaspar/MA1472.1.pfm
+-rw-r--r--   0        0        0      301 2023-02-20 20:04:01.226195 muon-0.1.5/muon/_atac/_ref/jaspar/MA1473.1.pfm
+-rw-r--r--   0        0        0      326 2023-02-20 20:04:01.226324 muon-0.1.5/muon/_atac/_ref/jaspar/MA1474.1.pfm
+-rw-r--r--   0        0        0      324 2023-02-20 20:04:01.226454 muon-0.1.5/muon/_atac/_ref/jaspar/MA1475.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.226575 muon-0.1.5/muon/_atac/_ref/jaspar/MA1476.1.pfm
+-rw-r--r--   0        0        0      324 2023-02-20 20:04:01.226692 muon-0.1.5/muon/_atac/_ref/jaspar/MA1478.1.pfm
+-rw-r--r--   0        0        0      323 2023-02-20 20:04:01.226818 muon-0.1.5/muon/_atac/_ref/jaspar/MA1479.1.pfm
+-rw-r--r--   0        0        0      271 2023-02-20 20:04:01.226943 muon-0.1.5/muon/_atac/_ref/jaspar/MA1480.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.227067 muon-0.1.5/muon/_atac/_ref/jaspar/MA1481.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.227192 muon-0.1.5/muon/_atac/_ref/jaspar/MA1483.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.227321 muon-0.1.5/muon/_atac/_ref/jaspar/MA1484.1.pfm
+-rw-r--r--   0        0        0      382 2023-02-20 20:04:01.227465 muon-0.1.5/muon/_atac/_ref/jaspar/MA1485.1.pfm
+-rw-r--r--   0        0        0      407 2023-02-20 20:04:01.227621 muon-0.1.5/muon/_atac/_ref/jaspar/MA1487.1.pfm
+-rw-r--r--   0        0        0      206 2023-02-20 20:04:01.227747 muon-0.1.5/muon/_atac/_ref/jaspar/MA1489.1.pfm
+-rw-r--r--   0        0        0      412 2023-02-20 20:04:01.227875 muon-0.1.5/muon/_atac/_ref/jaspar/MA1491.1.pfm
+-rw-r--r--   0        0        0      265 2023-02-20 20:04:01.227992 muon-0.1.5/muon/_atac/_ref/jaspar/MA1493.1.pfm
+-rw-r--r--   0        0        0      406 2023-02-20 20:04:01.228102 muon-0.1.5/muon/_atac/_ref/jaspar/MA1494.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.228234 muon-0.1.5/muon/_atac/_ref/jaspar/MA1495.1.pfm
+-rw-r--r--   0        0        0      213 2023-02-20 20:04:01.228360 muon-0.1.5/muon/_atac/_ref/jaspar/MA1496.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.228484 muon-0.1.5/muon/_atac/_ref/jaspar/MA1497.1.pfm
+-rw-r--r--   0        0        0      213 2023-02-20 20:04:01.228626 muon-0.1.5/muon/_atac/_ref/jaspar/MA1498.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.228743 muon-0.1.5/muon/_atac/_ref/jaspar/MA1499.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.228869 muon-0.1.5/muon/_atac/_ref/jaspar/MA1500.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.228988 muon-0.1.5/muon/_atac/_ref/jaspar/MA1501.1.pfm
+-rw-r--r--   0        0        0      213 2023-02-20 20:04:01.229112 muon-0.1.5/muon/_atac/_ref/jaspar/MA1502.1.pfm
+-rw-r--r--   0        0        0      267 2023-02-20 20:04:01.229232 muon-0.1.5/muon/_atac/_ref/jaspar/MA1503.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.229356 muon-0.1.5/muon/_atac/_ref/jaspar/MA1504.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.229479 muon-0.1.5/muon/_atac/_ref/jaspar/MA1505.1.pfm
+-rw-r--r--   0        0        0      298 2023-02-20 20:04:01.229615 muon-0.1.5/muon/_atac/_ref/jaspar/MA1506.1.pfm
+-rw-r--r--   0        0        0      214 2023-02-20 20:04:01.229793 muon-0.1.5/muon/_atac/_ref/jaspar/MA1507.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.229937 muon-0.1.5/muon/_atac/_ref/jaspar/MA1508.1.pfm
+-rw-r--r--   0        0        0      240 2023-02-20 20:04:01.230073 muon-0.1.5/muon/_atac/_ref/jaspar/MA1509.1.pfm
+-rw-r--r--   0        0        0      301 2023-02-20 20:04:01.230206 muon-0.1.5/muon/_atac/_ref/jaspar/MA1511.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.230346 muon-0.1.5/muon/_atac/_ref/jaspar/MA1512.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.230489 muon-0.1.5/muon/_atac/_ref/jaspar/MA1513.1.pfm
+-rw-r--r--   0        0        0      413 2023-02-20 20:04:01.230629 muon-0.1.5/muon/_atac/_ref/jaspar/MA1514.1.pfm
+-rw-r--r--   0        0        0      299 2023-02-20 20:04:01.230765 muon-0.1.5/muon/_atac/_ref/jaspar/MA1515.1.pfm
+-rw-r--r--   0        0        0      301 2023-02-20 20:04:01.231009 muon-0.1.5/muon/_atac/_ref/jaspar/MA1516.1.pfm
+-rw-r--r--   0        0        0      296 2023-02-20 20:04:01.231155 muon-0.1.5/muon/_atac/_ref/jaspar/MA1517.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.231338 muon-0.1.5/muon/_atac/_ref/jaspar/MA1518.1.pfm
+-rw-r--r--   0        0        0      215 2023-02-20 20:04:01.231554 muon-0.1.5/muon/_atac/_ref/jaspar/MA1519.1.pfm
+-rw-r--r--   0        0        0      408 2023-02-20 20:04:01.231783 muon-0.1.5/muon/_atac/_ref/jaspar/MA1520.1.pfm
+-rw-r--r--   0        0        0      412 2023-02-20 20:04:01.231988 muon-0.1.5/muon/_atac/_ref/jaspar/MA1521.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.232242 muon-0.1.5/muon/_atac/_ref/jaspar/MA1522.1.pfm
+-rw-r--r--   0        0        0      267 2023-02-20 20:04:01.232450 muon-0.1.5/muon/_atac/_ref/jaspar/MA1523.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.232609 muon-0.1.5/muon/_atac/_ref/jaspar/MA1524.1.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.232836 muon-0.1.5/muon/_atac/_ref/jaspar/MA1525.1.pfm
+-rw-r--r--   0        0        0      464 2023-02-20 20:04:01.233044 muon-0.1.5/muon/_atac/_ref/jaspar/MA1527.1.pfm
+-rw-r--r--   0        0        0      468 2023-02-20 20:04:01.233216 muon-0.1.5/muon/_atac/_ref/jaspar/MA1528.1.pfm
+-rw-r--r--   0        0        0      496 2023-02-20 20:04:01.233390 muon-0.1.5/muon/_atac/_ref/jaspar/MA1529.1.pfm
+-rw-r--r--   0        0        0      242 2023-02-20 20:04:01.233547 muon-0.1.5/muon/_atac/_ref/jaspar/MA1530.1.pfm
+-rw-r--r--   0        0        0      409 2023-02-20 20:04:01.233681 muon-0.1.5/muon/_atac/_ref/jaspar/MA1531.1.pfm
+-rw-r--r--   0        0        0      407 2023-02-20 20:04:01.233825 muon-0.1.5/muon/_atac/_ref/jaspar/MA1532.1.pfm
+-rw-r--r--   0        0        0      460 2023-02-20 20:04:01.233948 muon-0.1.5/muon/_atac/_ref/jaspar/MA1533.1.pfm
+-rw-r--r--   0        0        0      246 2023-02-20 20:04:01.234116 muon-0.1.5/muon/_atac/_ref/jaspar/MA1534.1.pfm
+-rw-r--r--   0        0        0      244 2023-02-20 20:04:01.234297 muon-0.1.5/muon/_atac/_ref/jaspar/MA1535.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.234459 muon-0.1.5/muon/_atac/_ref/jaspar/MA1536.1.pfm
+-rw-r--r--   0        0        0      414 2023-02-20 20:04:01.234596 muon-0.1.5/muon/_atac/_ref/jaspar/MA1537.1.pfm
+-rw-r--r--   0        0        0      410 2023-02-20 20:04:01.234729 muon-0.1.5/muon/_atac/_ref/jaspar/MA1538.1.pfm
+-rw-r--r--   0        0        0      410 2023-02-20 20:04:01.234866 muon-0.1.5/muon/_atac/_ref/jaspar/MA1539.1.pfm
+-rw-r--r--   0        0        0      298 2023-02-20 20:04:01.235136 muon-0.1.5/muon/_atac/_ref/jaspar/MA1540.1.pfm
+-rw-r--r--   0        0        0      464 2023-02-20 20:04:01.235358 muon-0.1.5/muon/_atac/_ref/jaspar/MA1541.1.pfm
+-rw-r--r--   0        0        0      271 2023-02-20 20:04:01.235515 muon-0.1.5/muon/_atac/_ref/jaspar/MA1542.1.pfm
+-rw-r--r--   0        0        0      384 2023-02-20 20:04:01.235678 muon-0.1.5/muon/_atac/_ref/jaspar/MA1544.1.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.235820 muon-0.1.5/muon/_atac/_ref/jaspar/MA1545.1.pfm
+-rw-r--r--   0        0        0      436 2023-02-20 20:04:01.235994 muon-0.1.5/muon/_atac/_ref/jaspar/MA1546.1.pfm
+-rw-r--r--   0        0        0      216 2023-02-20 20:04:01.236132 muon-0.1.5/muon/_atac/_ref/jaspar/MA1547.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.236257 muon-0.1.5/muon/_atac/_ref/jaspar/MA1548.1.pfm
+-rw-r--r--   0        0        0      271 2023-02-20 20:04:01.236385 muon-0.1.5/muon/_atac/_ref/jaspar/MA1549.1.pfm
+-rw-r--r--   0        0        0      440 2023-02-20 20:04:01.236513 muon-0.1.5/muon/_atac/_ref/jaspar/MA1550.1.pfm
+-rw-r--r--   0        0        0      378 2023-02-20 20:04:01.236638 muon-0.1.5/muon/_atac/_ref/jaspar/MA1552.1.pfm
+-rw-r--r--   0        0        0      381 2023-02-20 20:04:01.236755 muon-0.1.5/muon/_atac/_ref/jaspar/MA1553.1.pfm
+-rw-r--r--   0        0        0      236 2023-02-20 20:04:01.236870 muon-0.1.5/muon/_atac/_ref/jaspar/MA1554.1.pfm
+-rw-r--r--   0        0        0      380 2023-02-20 20:04:01.237080 muon-0.1.5/muon/_atac/_ref/jaspar/MA1555.1.pfm
+-rw-r--r--   0        0        0      380 2023-02-20 20:04:01.237253 muon-0.1.5/muon/_atac/_ref/jaspar/MA1556.1.pfm
+-rw-r--r--   0        0        0      270 2023-02-20 20:04:01.237399 muon-0.1.5/muon/_atac/_ref/jaspar/MA1557.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.237536 muon-0.1.5/muon/_atac/_ref/jaspar/MA1558.1.pfm
+-rw-r--r--   0        0        0      271 2023-02-20 20:04:01.237661 muon-0.1.5/muon/_atac/_ref/jaspar/MA1559.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.237789 muon-0.1.5/muon/_atac/_ref/jaspar/MA1560.1.pfm
+-rw-r--r--   0        0        0      296 2023-02-20 20:04:01.237910 muon-0.1.5/muon/_atac/_ref/jaspar/MA1561.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.238061 muon-0.1.5/muon/_atac/_ref/jaspar/MA1562.1.pfm
+-rw-r--r--   0        0        0      211 2023-02-20 20:04:01.238263 muon-0.1.5/muon/_atac/_ref/jaspar/MA1563.1.pfm
+-rw-r--r--   0        0        0      324 2023-02-20 20:04:01.238458 muon-0.1.5/muon/_atac/_ref/jaspar/MA1564.1.pfm
+-rw-r--r--   0        0        0      323 2023-02-20 20:04:01.238592 muon-0.1.5/muon/_atac/_ref/jaspar/MA1565.1.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.238716 muon-0.1.5/muon/_atac/_ref/jaspar/MA1566.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.238852 muon-0.1.5/muon/_atac/_ref/jaspar/MA1567.1.pfm
+-rw-r--r--   0        0        0      324 2023-02-20 20:04:01.239087 muon-0.1.5/muon/_atac/_ref/jaspar/MA1568.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.239229 muon-0.1.5/muon/_atac/_ref/jaspar/MA1569.1.pfm
+-rw-r--r--   0        0        0      267 2023-02-20 20:04:01.239364 muon-0.1.5/muon/_atac/_ref/jaspar/MA1570.1.pfm
+-rw-r--r--   0        0        0      325 2023-02-20 20:04:01.239603 muon-0.1.5/muon/_atac/_ref/jaspar/MA1571.1.pfm
+-rw-r--r--   0        0        0      325 2023-02-20 20:04:01.239846 muon-0.1.5/muon/_atac/_ref/jaspar/MA1572.1.pfm
+-rw-r--r--   0        0        0      518 2023-02-20 20:04:01.240037 muon-0.1.5/muon/_atac/_ref/jaspar/MA1573.1.pfm
+-rw-r--r--   0        0        0      412 2023-02-20 20:04:01.240254 muon-0.1.5/muon/_atac/_ref/jaspar/MA1574.1.pfm
+-rw-r--r--   0        0        0      522 2023-02-20 20:04:01.240427 muon-0.1.5/muon/_atac/_ref/jaspar/MA1575.1.pfm
+-rw-r--r--   0        0        0      518 2023-02-20 20:04:01.240572 muon-0.1.5/muon/_atac/_ref/jaspar/MA1576.1.pfm
+-rw-r--r--   0        0        0      215 2023-02-20 20:04:01.240712 muon-0.1.5/muon/_atac/_ref/jaspar/MA1577.1.pfm
+-rw-r--r--   0        0        0      265 2023-02-20 20:04:01.240996 muon-0.1.5/muon/_atac/_ref/jaspar/MA1578.1.pfm
+-rw-r--r--   0        0        0      408 2023-02-20 20:04:01.241200 muon-0.1.5/muon/_atac/_ref/jaspar/MA1579.1.pfm
+-rw-r--r--   0        0        0      268 2023-02-20 20:04:01.241367 muon-0.1.5/muon/_atac/_ref/jaspar/MA1580.1.pfm
+-rw-r--r--   0        0        0      352 2023-02-20 20:04:01.241515 muon-0.1.5/muon/_atac/_ref/jaspar/MA1581.1.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.241650 muon-0.1.5/muon/_atac/_ref/jaspar/MA1583.1.pfm
+-rw-r--r--   0        0        0      440 2023-02-20 20:04:01.241783 muon-0.1.5/muon/_atac/_ref/jaspar/MA1584.1.pfm
+-rw-r--r--   0        0        0      269 2023-02-20 20:04:01.241906 muon-0.1.5/muon/_atac/_ref/jaspar/MA1585.1.pfm
+-rw-r--r--   0        0        0      379 2023-02-20 20:04:01.242022 muon-0.1.5/muon/_atac/_ref/jaspar/MA1587.1.pfm
+-rw-r--r--   0        0        0      410 2023-02-20 20:04:01.242148 muon-0.1.5/muon/_atac/_ref/jaspar/MA1588.1.pfm
+-rw-r--r--   0        0        0      576 2023-02-20 20:04:01.242272 muon-0.1.5/muon/_atac/_ref/jaspar/MA1589.1.pfm
+-rw-r--r--   0        0        0      440 2023-02-20 20:04:01.242475 muon-0.1.5/muon/_atac/_ref/jaspar/MA1592.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.242638 muon-0.1.5/muon/_atac/_ref/jaspar/MA1593.1.pfm
+-rw-r--r--   0        0        0      661 2023-02-20 20:04:01.242800 muon-0.1.5/muon/_atac/_ref/jaspar/MA1594.1.pfm
+-rw-r--r--   0        0        0      436 2023-02-20 20:04:01.242947 muon-0.1.5/muon/_atac/_ref/jaspar/MA1596.1.pfm
+-rw-r--r--   0        0        0      461 2023-02-20 20:04:01.243086 muon-0.1.5/muon/_atac/_ref/jaspar/MA1597.1.pfm
+-rw-r--r--   0        0        0      436 2023-02-20 20:04:01.243217 muon-0.1.5/muon/_atac/_ref/jaspar/MA1599.1.pfm
+-rw-r--r--   0        0        0      492 2023-02-20 20:04:01.243339 muon-0.1.5/muon/_atac/_ref/jaspar/MA1600.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.243472 muon-0.1.5/muon/_atac/_ref/jaspar/MA1601.1.pfm
+-rw-r--r--   0        0        0      323 2023-02-20 20:04:01.243708 muon-0.1.5/muon/_atac/_ref/jaspar/MA1602.1.pfm
+-rw-r--r--   0        0        0      357 2023-02-20 20:04:01.243925 muon-0.1.5/muon/_atac/_ref/jaspar/MA1603.1.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.244186 muon-0.1.5/muon/_atac/_ref/jaspar/MA1604.1.pfm
+-rw-r--r--   0        0        0      304 2023-02-20 20:04:01.244357 muon-0.1.5/muon/_atac/_ref/jaspar/MA1606.1.pfm
+-rw-r--r--   0        0        0      384 2023-02-20 20:04:01.244526 muon-0.1.5/muon/_atac/_ref/jaspar/MA1607.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.244667 muon-0.1.5/muon/_atac/_ref/jaspar/MA1608.1.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.244842 muon-0.1.5/muon/_atac/_ref/jaspar/MA1615.1.pfm
+-rw-r--r--   0        0        0      408 2023-02-20 20:04:01.244965 muon-0.1.5/muon/_atac/_ref/jaspar/MA1616.1.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.245084 muon-0.1.5/muon/_atac/_ref/jaspar/MA1618.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.245273 muon-0.1.5/muon/_atac/_ref/jaspar/MA1619.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.245445 muon-0.1.5/muon/_atac/_ref/jaspar/MA1620.1.pfm
+-rw-r--r--   0        0        0      384 2023-02-20 20:04:01.245588 muon-0.1.5/muon/_atac/_ref/jaspar/MA1621.1.pfm
+-rw-r--r--   0        0        0      384 2023-02-20 20:04:01.245721 muon-0.1.5/muon/_atac/_ref/jaspar/MA1622.1.pfm
+-rw-r--r--   0        0        0      354 2023-02-20 20:04:01.245872 muon-0.1.5/muon/_atac/_ref/jaspar/MA1623.1.pfm
+-rw-r--r--   0        0        0      327 2023-02-20 20:04:01.246015 muon-0.1.5/muon/_atac/_ref/jaspar/MA1624.1.pfm
+-rw-r--r--   0        0        0      408 2023-02-20 20:04:01.246178 muon-0.1.5/muon/_atac/_ref/jaspar/MA1625.1.pfm
+-rw-r--r--   0        0        0      382 2023-02-20 20:04:01.246312 muon-0.1.5/muon/_atac/_ref/jaspar/MA1627.1.pfm
+-rw-r--r--   0        0        0      299 2023-02-20 20:04:01.246446 muon-0.1.5/muon/_atac/_ref/jaspar/MA1628.1.pfm
+-rw-r--r--   0        0        0      384 2023-02-20 20:04:01.246617 muon-0.1.5/muon/_atac/_ref/jaspar/MA1629.1.pfm
+-rw-r--r--   0        0        0      298 2023-02-20 20:04:01.246764 muon-0.1.5/muon/_atac/_ref/jaspar/MA1630.1.pfm
+-rw-r--r--   0        0        0      357 2023-02-20 20:04:01.246905 muon-0.1.5/muon/_atac/_ref/jaspar/MA1631.1.pfm
+-rw-r--r--   0        0        0      360 2023-02-20 20:04:01.247037 muon-0.1.5/muon/_atac/_ref/jaspar/MA1632.1.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.247164 muon-0.1.5/muon/_atac/_ref/jaspar/MA1633.1.pfm
+-rw-r--r--   0        0        0      303 2023-02-20 20:04:01.247296 muon-0.1.5/muon/_atac/_ref/jaspar/MA1634.1.pfm
+-rw-r--r--   0        0        0      272 2023-02-20 20:04:01.247424 muon-0.1.5/muon/_atac/_ref/jaspar/MA1635.1.pfm
+-rw-r--r--   0        0        0      413 2023-02-20 20:04:01.247568 muon-0.1.5/muon/_atac/_ref/jaspar/MA1636.1.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.247736 muon-0.1.5/muon/_atac/_ref/jaspar/MA1637.1.pfm
+-rw-r--r--   0        0        0      273 2023-02-20 20:04:01.247900 muon-0.1.5/muon/_atac/_ref/jaspar/MA1638.1.pfm
+-rw-r--r--   0        0        0      356 2023-02-20 20:04:01.248024 muon-0.1.5/muon/_atac/_ref/jaspar/MA1639.1.pfm
+-rw-r--r--   0        0        0      412 2023-02-20 20:04:01.248141 muon-0.1.5/muon/_atac/_ref/jaspar/MA1640.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.248265 muon-0.1.5/muon/_atac/_ref/jaspar/MA1641.1.pfm
+-rw-r--r--   0        0        0      357 2023-02-20 20:04:01.248405 muon-0.1.5/muon/_atac/_ref/jaspar/MA1642.1.pfm
+-rw-r--r--   0        0        0      579 2023-02-20 20:04:01.248541 muon-0.1.5/muon/_atac/_ref/jaspar/MA1643.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.248668 muon-0.1.5/muon/_atac/_ref/jaspar/MA1644.1.pfm
+-rw-r--r--   0        0        0      384 2023-02-20 20:04:01.248889 muon-0.1.5/muon/_atac/_ref/jaspar/MA1645.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.249094 muon-0.1.5/muon/_atac/_ref/jaspar/MA1646.1.pfm
+-rw-r--r--   0        0        0      300 2023-02-20 20:04:01.249275 muon-0.1.5/muon/_atac/_ref/jaspar/MA1647.1.pfm
+-rw-r--r--   0        0        0      304 2023-02-20 20:04:01.249453 muon-0.1.5/muon/_atac/_ref/jaspar/MA1648.1.pfm
+-rw-r--r--   0        0        0      299 2023-02-20 20:04:01.249627 muon-0.1.5/muon/_atac/_ref/jaspar/MA1649.1.pfm
+-rw-r--r--   0        0        0      326 2023-02-20 20:04:01.249800 muon-0.1.5/muon/_atac/_ref/jaspar/MA1650.1.pfm
+-rw-r--r--   0        0        0      576 2023-02-20 20:04:01.249944 muon-0.1.5/muon/_atac/_ref/jaspar/MA1651.1.pfm
+-rw-r--r--   0        0        0      381 2023-02-20 20:04:01.250073 muon-0.1.5/muon/_atac/_ref/jaspar/MA1652.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.250202 muon-0.1.5/muon/_atac/_ref/jaspar/MA1653.1.pfm
+-rw-r--r--   0        0        0      629 2023-02-20 20:04:01.250397 muon-0.1.5/muon/_atac/_ref/jaspar/MA1654.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.250597 muon-0.1.5/muon/_atac/_ref/jaspar/MA1655.1.pfm
+-rw-r--r--   0        0        0      384 2023-02-20 20:04:01.250745 muon-0.1.5/muon/_atac/_ref/jaspar/MA1656.1.pfm
+-rw-r--r--   0        0        0      328 2023-02-20 20:04:01.250891 muon-0.1.5/muon/_atac/_ref/jaspar/MA1657.1.pfm
+-rw-r--r--   0        0        0      302 2023-02-20 20:04:01.251035 muon-0.1.5/muon/_atac/_ref/jaspar/MA1683.1.pfm
+-rw-r--r--   0        0        0    11673 2023-02-20 20:04:01.251258 muon-0.1.5/muon/_atac/_ref/jaspar/motif_to_gene.txt
+-rw-r--r--   0        0        0     4491 2023-02-20 20:04:01.251460 muon-0.1.5/muon/_atac/io.py
+-rw-r--r--   0        0        0    12779 2023-06-08 08:49:54.375686 muon-0.1.5/muon/_atac/plot.py
+-rw-r--r--   0        0        0     7133 2023-02-20 20:04:01.251976 muon-0.1.5/muon/_atac/preproc.py
+-rw-r--r--   0        0        0    44213 2023-06-07 09:07:57.087492 muon-0.1.5/muon/_atac/tools.py
+-rw-r--r--   0        0        0      316 2023-06-07 09:07:57.088441 muon-0.1.5/muon/_atac/utils.py
+-rw-r--r--   0        0        0        0 2023-02-20 20:04:01.252851 muon-0.1.5/muon/_core/__init__.py
+-rw-r--r--   0        0        0     2032 2023-02-20 20:04:01.252993 muon-0.1.5/muon/_core/config.py
+-rw-r--r--   0        0        0     3135 2023-02-20 20:04:41.107395 muon-0.1.5/muon/_core/io.py
+-rw-r--r--   0        0        0    16833 2023-06-08 08:49:54.376617 muon-0.1.5/muon/_core/plot.py
+-rw-r--r--   0        0        0    35383 2023-06-07 09:07:57.090694 muon-0.1.5/muon/_core/preproc.py
+-rw-r--r--   0        0        0    52375 2023-06-08 08:49:54.378345 muon-0.1.5/muon/_core/tools.py
+-rw-r--r--   0        0        0     8448 2023-02-20 20:04:01.254933 muon-0.1.5/muon/_core/utils.py
+-rw-r--r--   0        0        0       46 2023-02-20 20:04:01.255165 muon-0.1.5/muon/_prot/__init__.py
+-rw-r--r--   0        0        0      723 2023-02-20 20:04:01.255299 muon-0.1.5/muon/_prot/io.py
+-rw-r--r--   0        0        0    10314 2023-06-07 09:07:57.092293 muon-0.1.5/muon/_prot/preproc.py
+-rw-r--r--   0        0        0        0 2023-02-20 20:04:01.255631 muon-0.1.5/muon/_rna/__init__.py
+-rw-r--r--   0        0        0     1270 2023-02-20 20:04:01.255794 muon-0.1.5/muon/_rna/utils.py
+-rw-r--r--   0        0        0       21 2023-02-20 20:04:01.255949 muon-0.1.5/muon/atac.py
+-rw-r--r--   0        0        0       21 2023-02-20 20:04:01.256101 muon-0.1.5/muon/prot.py
+-rw-r--r--   0        0        0       20 2023-02-20 20:04:01.256224 muon-0.1.5/muon/rna.py
+-rw-r--r--   0        0        0     1242 2023-06-07 09:07:57.092944 muon-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6313 1970-01-01 00:00:00.000000 muon-0.1.5/PKG-INFO
```

### Comparing `muon-0.1.4/README.md` & `muon-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA0050.2.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA0050.2.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA0066.1.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA0066.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA0073.1.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA0073.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA0080.5.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA0080.5.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA0138.2.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA0138.2.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA0139.1.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA0139.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA0494.1.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA0494.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA0804.1.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA0804.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA1101.2.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA1101.2.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA1418.1.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA1418.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA1470.1.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA1470.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA1573.1.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA1573.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA1575.1.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA1575.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA1576.1.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA1576.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA1589.1.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA1589.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA1594.1.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA1594.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA1643.1.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA1643.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA1651.1.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA1651.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/MA1654.1.pfm` & `muon-0.1.5/muon/_atac/_ref/jaspar/MA1654.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/_ref/jaspar/motif_to_gene.txt` & `muon-0.1.5/muon/_atac/_ref/jaspar/motif_to_gene.txt`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/io.py` & `muon-0.1.5/muon/_atac/io.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/plot.py` & `muon-0.1.5/muon/_atac/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,22 +162,23 @@
 
         x, attr_names, _ = _average_peaks(
             adata=adata, keys=keys, average=average, func=func, use_raw=use_raw, layer=layer
         )
         ad = AnnData(x, obs=adata.obs, obsm=adata.obsm)
         retval = sc.pl.embedding(ad, basis=basis, color=attr_names, **kwargs)
         for aname in attr_names:
-            adata.uns[f"{aname}_colors"] = ad.uns[f"{aname}_colors"]
+            try:
+                adata.uns[f"{aname}_colors"] = ad.uns[f"{aname}_colors"]
+            except KeyError:
+                pass
         return retval
 
     else:
         return sc.pl.embedding(adata, basis=basis, use_raw=use_raw, layer=layer, **kwargs)
 
-    return None
-
 
 def pca(data: Union[AnnData, MuData], **kwargs) -> Union[Axes, List[Axes], None]:
     """
     Scatter plot for principle components
 
     See sc.pl.embedding for details.
     """
```

### Comparing `muon-0.1.4/muon/_atac/preproc.py` & `muon-0.1.5/muon/_atac/preproc.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_atac/tools.py` & `muon-0.1.5/muon/_atac/tools.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_core/config.py` & `muon-0.1.5/muon/_core/config.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_core/io.py` & `muon-0.1.5/muon/_core/io.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_core/plot.py` & `muon-0.1.5/muon/_core/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,18 @@
 
     # Note that use_raw and layers are not provided to the plotting function
     # as the corresponding values were fetched from individual modalities
     # and are now stored in .obs
     retval = sc.pl.scatter(ad, x=x, y=y, color=color, **kwargs)
     if color is not None:
         for col in color:
-            data.uns[f"{col}_colors"] = ad.uns[f"{col}_colors"]
+            try:
+                data.uns[f"{col}_colors"] = ad.uns[f"{col}_colors"]
+            except KeyError:
+                pass
     return retval
 
 
 #
 # Embedding
 #
 
@@ -198,17 +201,18 @@
         for i, k in enumerate(keys):
             mod_key_modifier[k] = k
             for m in data.mod:
                 if not keys_in_mod[m][i]:
                     k_clean = k
                     if k.startswith(f"{m}:"):
                         k_clean = k.split(":", 1)[1]
-                        mod_key_modifier[k] = k_clean
 
                     keys_in_mod[m][i] = k_clean in data.mod[m].var_names
+                    if keys_in_mod[m][i]:
+                        mod_key_modifier[k] = k_clean
                     if use_raw is None or use_raw:
                         if keys_in_mod[m][i] == False and data.mod[m].raw is not None:
                             keys_in_mod[m][i] = k_clean in data.mod[m].raw.var_names
 
         for m in data.mod:
             if np.sum(keys_in_mod[m]) > 0:
                 mod_keys = np.array(keys)[keys_in_mod[m]]
@@ -255,15 +259,18 @@
                 )
 
         color = [mod_key_modifier[k] for k in keys]
 
     ad = AnnData(obs=obs, obsm=adata.obsm, obsp=adata.obsp, uns=adata.uns)
     retval = sc.pl.embedding(ad, basis=basis_mod, color=color, **kwargs)
     for key, col in zip(keys, color):
-        adata.uns[f"{key}_colors"] = ad.uns[f"{col}_colors"]
+        try:
+            adata.uns[f"{key}_colors"] = ad.uns[f"{col}_colors"]
+        except KeyError:
+            pass
     return retval
 
 
 def mofa(mdata: MuData, **kwargs) -> Union[Axes, List[Axes], None]:
     """
     Scatter plot in MOFA factors coordinates
```

### Comparing `muon-0.1.4/muon/_core/preproc.py` & `muon-0.1.5/muon/_core/preproc.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_core/tools.py` & `muon-0.1.5/muon/_core/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,18 @@
             expanded = orig.reindex(obs_names)
 
             # find indices in the expanded matrix to copy orig data
             expanded["ix"] = range(n)
             ix = expanded.join(orig, how="right").ix.values
 
             # set expanded data with part of the orig data
-            x[ix, :] = mdata[m].X
+            if issparse(mdata[m].X):
+                x[ix, :] = np.array(mdata[m].X.todense())
+            else:
+                x[ix, :] = mdata[m].X
             data[i] = x
 
     # Subset features if required
     if features_subset is not None:
         for i, m in enumerate(mdata.mod.keys()):
             if features_subset not in mdata.mod[m].var.columns:
                 raise KeyError(f"There is no column {features_subset} in .var for modality {m}")
```

### Comparing `muon-0.1.4/muon/_core/utils.py` & `muon-0.1.5/muon/_core/utils.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_prot/io.py` & `muon-0.1.5/muon/_prot/io.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_prot/preproc.py` & `muon-0.1.5/muon/_prot/preproc.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/muon/_rna/utils.py` & `muon-0.1.5/muon/_rna/utils.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/pyproject.toml` & `muon-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `muon-0.1.4/PKG-INFO` & `muon-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muon
-Version: 0.1.4
+Version: 0.1.5
 Summary: Multimodal omics analysis framework
 Home-page: https://github.com/scverse/muon
 Author: Danila Bredikhin
 Author-email: danila.bredikhin@embl.de
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
```

