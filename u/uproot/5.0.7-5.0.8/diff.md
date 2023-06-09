# Comparing `tmp/uproot-5.0.7.tar.gz` & `tmp/uproot-5.0.8.tar.gz`

## Comparing `uproot-5.0.7.tar` & `uproot-5.0.8.tar`

### file list

```diff
@@ -1,237 +1,238 @@
--rw-r--r--   0        0        0    13217 2020-02-02 00:00:00.000000 uproot-5.0.7/.all-contributorsrc
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 uproot-5.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 uproot-5.0.7/.readthedocs.yml
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.0.7/CITATION.cff
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 uproot-5.0.7/.github/dependabot.yml
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 uproot-5.0.7/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 uproot-5.0.7/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 uproot-5.0.7/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 uproot-5.0.7/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 uproot-5.0.7/.github/workflows/build-test.yml
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 uproot-5.0.7/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 uproot-5.0.7/.github/workflows/semantic-pr-title.yml
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 uproot-5.0.7/dev/example-objects.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 uproot-5.0.7/dev/make-models.py
--rw-r--r--   0        0        0    95009 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-img/diagrams/abstraction-layers.png
--rw-r--r--   0        0        0    39940 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-img/diagrams/abstraction-layers.svg
--rw-r--r--   0        0        0    49015 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-img/diagrams/example-dask-graph.png
--rw-r--r--   0        0        0    70413 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-img/diagrams/uproot-awkward-timeline.png
--rw-r--r--   0        0        0    28715 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-img/diagrams/uproot-awkward-timeline.svg
--rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-img/logo/logo-300px-white.png
--rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-img/logo/logo-600px.png
--rw-r--r--   0        0        0     7695 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-img/logo/logo.svg
--rw-r--r--   0        0        0   223219 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-img/photos/switcheroo.jpg
--rw-r--r--   0        0        0    69252 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-sphinx/basic.rst
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-sphinx/conf.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-sphinx/index.rst
--rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-sphinx/make_changelog.py
--rw-r--r--   0        0        0    10359 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-sphinx/prepare_docstrings.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-sphinx/requirements.txt
--rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-sphinx/uproot3-to-4.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 uproot-5.0.7/docs-sphinx/_templates/breadcrumbs.html
--rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/__init__.py
--rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/_awkward_forth.py
--rw-r--r--   0        0        0    35154 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/_dask.py
--rw-r--r--   0        0        0    32174 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/_util.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behavior.py
--rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/cache.py
--rw-r--r--   0        0        0    16839 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/compression.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/const.py
--rw-r--r--   0        0        0    71187 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/containers.py
--rw-r--r--   0        0        0    20423 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/deserialization.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/dynamic.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/exceptions.py
--rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/extras.py
--rw-r--r--   0        0        0    65811 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/model.py
--rw-r--r--   0        0        0     9549 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/pyroot.py
--rw-r--r--   0        0        0    98269 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/reading.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/serialization.py
--rw-r--r--   0        0        0    69151 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/streamers.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/version.py
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/RooCurve.py
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/RooHist.py
--rw-r--r--   0        0        0    10052 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TAxis.py
--rw-r--r--   0        0        0   130388 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TBranch.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TBranchElement.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TDatime.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TGraph.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TGraphAsymmErrors.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TGraphErrors.py
--rw-r--r--   0        0        0    12171 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TH1.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TH2.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TH2Poly.py
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TH3.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TParameter.py
--rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TProfile.py
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TProfile2D.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TProfile3D.py
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/TTree.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/behaviors/__init__.py
--rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/interpretation/__init__.py
--rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/interpretation/grouped.py
--rw-r--r--   0        0        0    40728 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/interpretation/identify.py
--rw-r--r--   0        0        0    14973 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/interpretation/jagged.py
--rw-r--r--   0        0        0    37252 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/interpretation/library.py
--rw-r--r--   0        0        0    23068 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/interpretation/numerical.py
--rw-r--r--   0        0        0    34143 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/interpretation/objects.py
--rw-r--r--   0        0        0    18835 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/interpretation/strings.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/language/__init__.py
--rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/language/python.py
--rw-r--r--   0        0        0    25744 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/RNTuple.py
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TArray.py
--rw-r--r--   0        0        0    25313 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TAtt.py
--rw-r--r--   0        0        0    11179 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TBasket.py
--rw-r--r--   0        0        0    37043 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TBranch.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TClonesArray.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TDatime.py
--rw-r--r--   0        0        0    35496 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TGraph.py
--rw-r--r--   0        0        0   212956 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TH.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/THashList.py
--rw-r--r--   0        0        0    33898 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TLeaf.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TList.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TMatrixT.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TNamed.py
--rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TObjArray.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TObjString.py
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TObject.py
--rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TRef.py
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TString.py
--rw-r--r--   0        0        0     7255 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TTable.py
--rw-r--r--   0        0        0    46935 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/TTree.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/models/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/sink/__init__.py
--rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/sink/file.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/source/__init__.py
--rw-r--r--   0        0        0    16003 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/source/chunk.py
--rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/source/cursor.py
--rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/source/file.py
--rw-r--r--   0        0        0    14154 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/source/futures.py
--rw-r--r--   0        0        0    25910 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/source/http.py
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/source/object.py
--rw-r--r--   0        0        0    15697 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/source/xrootd.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/writing/__init__.py
--rw-r--r--   0        0        0    82851 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/writing/_cascade.py
--rw-r--r--   0        0        0    31855 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/writing/_cascadentuple.py
--rw-r--r--   0        0        0    55862 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/writing/_cascadetree.py
--rw-r--r--   0        0        0    79676 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/writing/identify.py
--rw-r--r--   0        0        0    80263 2020-02-02 00:00:00.000000 uproot-5.0.7/src/uproot/writing/writable.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/__init__.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/conftest.py
--rw-r--r--   0        0        0    15805 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0001-source-class.py
--rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0006-notify-when-downloaded.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0007-single-chunk-interface.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0008-start-interpretation.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0009-nested-directories.py
--rw-r--r--   0        0        0    29196 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0010-start-streamers.py
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0011-generate-classes-from-streamers.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0013-rntuple-anchor.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0014-all-ttree-versions.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0016-interpretations.py
--rw-r--r--   0        0        0     9682 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0017-multi-basket-multi-branch-fetch.py
--rw-r--r--   0        0        0    33935 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0018-array-fetching-interface.py
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0022-number-of-branches.py
--rw-r--r--   0        0        0    13960 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0023-more-interpretations-1.py
--rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0023-ttree-versions.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0028-fallback-to-read-streamer.py
--rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0029-more-string-types.py
--rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0031-test-stl-containers.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0033-more-interpretations-2.py
--rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0034-generic-objects-in-ttrees.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0035-datatype-generality.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0038-memberwise-serialization.py
--rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0043-iterate-function.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0044-concatenate-function.py
--rw-r--r--   0        0        0    68981 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0046-histograms-bh-hist.py
--rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0053-parents-should-not-be-bases.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0058-detach-model-objects-from-files.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0066-fix-http-fallback-freeze.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0067-common-entry-offsets.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0081-dont-parse-colons.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0087-memberwise-splitting-not-implemented-messages.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0088-read-with-http.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0099-read-from-file-object.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0112-fix-pandas-with-cut.py
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0118-fix-name-fetch-again.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0123-atlas-issues.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0126-turn-unknown-emptyarrays-into-known-types.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0167-use-the-common-histogram-interface.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0172-allow-allocators-in-vector-typenames.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0173-empty-and-multiprocessing-bugs.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0182-complain-about-missing-files.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0194-fix-lost-cuts-in-iterate.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0220-contiguous-byte-ranges-in-http.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0228_read-TProfiles.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0240-read_TGraphAsymmErrors.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0278-specializations-for-TParameter.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0302-pickle.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0303-empty-jagged-array.py
--rw-r--r--   0        0        0    14234 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0320-start-working-on-ROOT-writing.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0322-writablefile-infrastructure.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0325-fix-windows-file-uris.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0329-update-existing-root-files.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0335-empty-ttree-division-by-zero.py
--rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0341-manipulate-streamer-info.py
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0344-writabledirectory-can-read.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0345-bulk-copy-method.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0349-write-TObjString.py
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0350-read-RooCurve-RooHist.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0351-write-TList.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0352-write-THashList.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0384-move-behavior_of-and-fix-383.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0398-dimensions-in-leaflist.py
--rw-r--r--   0        0        0    26536 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0405-write-a-histogram.py
--rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0406-write-a-ttree.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0407-read-TDatime.py
--rw-r--r--   0        0        0    17062 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0412-write-multidimensional-numpy-to-ttree.py
--rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0414-write-jagged-arrays.py
--rw-r--r--   0        0        0    16674 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0416-writing-compressed-data.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0418-read-TTable.py
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0420-pyroot-uproot-interoperability.py
--rw-r--r--   0        0        0    17479 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0422-hist-integration.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0430-global_index-for-tuples-of-DataFrames.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0438-TClonesArray-is-not-AsGrouped.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0439-check-awkward-before-numpy.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0442-regular-TClonesArray.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0472-tstreamerinfo-for-ttree.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0475-remember-to-update-freesegments.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0484-manually-add-model-for-TMatrixTSym_double_.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0487-implement-asdtypeinplace.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0498-create-leaf-branch-in-extend.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0519-remove-memmap-copy.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0520-dynamic-classes-cant-be-abc-subclasses.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0569-fBits-is-4-bytes.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0576-unicode-in-names.py
--rw-r--r--   0        0        0    25906 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0578-dask-for-numpy.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0580-round-trip-for-no-flow-histograms.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0589-explicitly-interpret-RVec-type.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0603-dask-delayed-open.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0609-num-enteries-func.py
--rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0610-awkward-form.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0630-rntuple-basics.py
--rw-r--r--   0        0        0    58430 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0637-setup-tests-for-AwkwardForth.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0643-reading-vector-pair-TLorentzVector-int.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0651-implement-transformed-axis.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0652_dask-for-awkward.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0662-rntuple-stl-containers.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0700-dask-empty-arrays.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0705-rntuple-writing-metadata.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0750-avoid-empty-TBasket-issue.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0755-dask-awkward-column-projection.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0791-protect-uproot-project_columns-from-dask-node-names.py
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0798_DAOD_PHYSLITE.py
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0808-fix_awkward_form_for_AsStridedObjects.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0816-separate-AwkwardForth-machines-by-TBranch.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0832-ak_add_doc-should-also-add-to-typetracer.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0840-support-tleafG.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0841-fix-814.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0844-fix-delete-hist-from-root.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0852-fix-strided-interp-extra-offsets.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0870-writing-arrays-of-type-unknown-fix-822.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/test_0876-uproot-dask-blind-steps.py
--rw-r--r--   0        0        0   128147 2020-02-02 00:00:00.000000 uproot-5.0.7/tests/samples/h_dynamic.pkl
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 uproot-5.0.7/.gitignore
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 uproot-5.0.7/LICENSE
--rw-r--r--   0        0        0    25899 2020-02-02 00:00:00.000000 uproot-5.0.7/README.md
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 uproot-5.0.7/pyproject.toml
--rw-r--r--   0        0        0    28208 2020-02-02 00:00:00.000000 uproot-5.0.7/PKG-INFO
+-rw-r--r--   0        0        0    13217 2020-02-02 00:00:00.000000 uproot-5.0.8/.all-contributorsrc
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 uproot-5.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 uproot-5.0.8/.readthedocs.yml
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.0.8/CITATION.cff
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/workflows/build-test.yml
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 uproot-5.0.8/.github/workflows/semantic-pr-title.yml
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 uproot-5.0.8/dev/example-objects.py
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 uproot-5.0.8/dev/make-models.py
+-rw-r--r--   0        0        0    95009 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/diagrams/abstraction-layers.png
+-rw-r--r--   0        0        0    39940 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/diagrams/abstraction-layers.svg
+-rw-r--r--   0        0        0    49015 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/diagrams/example-dask-graph.png
+-rw-r--r--   0        0        0    70413 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/diagrams/uproot-awkward-timeline.png
+-rw-r--r--   0        0        0    28715 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/diagrams/uproot-awkward-timeline.svg
+-rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/logo/logo-300px-white.png
+-rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/logo/logo-600px.png
+-rw-r--r--   0        0        0     7695 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/logo/logo.svg
+-rw-r--r--   0        0        0   223219 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-img/photos/switcheroo.jpg
+-rw-r--r--   0        0        0    69252 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/basic.rst
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/conf.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/index.rst
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/make_changelog.py
+-rw-r--r--   0        0        0    10359 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/prepare_docstrings.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/requirements.txt
+-rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/uproot3-to-4.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 uproot-5.0.8/docs-sphinx/_templates/breadcrumbs.html
+-rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/__init__.py
+-rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/_awkward_forth.py
+-rw-r--r--   0        0        0    41220 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/_dask.py
+-rw-r--r--   0        0        0    34514 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/_util.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behavior.py
+-rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/cache.py
+-rw-r--r--   0        0        0    16839 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/compression.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/const.py
+-rw-r--r--   0        0        0    71187 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/containers.py
+-rw-r--r--   0        0        0    20423 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/deserialization.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/dynamic.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/exceptions.py
+-rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/extras.py
+-rw-r--r--   0        0        0    65811 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/model.py
+-rw-r--r--   0        0        0     9549 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/pyroot.py
+-rw-r--r--   0        0        0    98265 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/reading.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/serialization.py
+-rw-r--r--   0        0        0    69210 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/streamers.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/version.py
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/RooCurve.py
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/RooHist.py
+-rw-r--r--   0        0        0    10049 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TAxis.py
+-rw-r--r--   0        0        0   130424 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TBranch.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TBranchElement.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TDatime.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TGraph.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TGraphAsymmErrors.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TGraphErrors.py
+-rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TH1.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TH2.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TH2Poly.py
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TH3.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TParameter.py
+-rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TProfile.py
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TProfile2D.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TProfile3D.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/TTree.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/behaviors/__init__.py
+-rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/__init__.py
+-rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/grouped.py
+-rw-r--r--   0        0        0    40728 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/identify.py
+-rw-r--r--   0        0        0    14973 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/jagged.py
+-rw-r--r--   0        0        0    37252 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/library.py
+-rw-r--r--   0        0        0    23068 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/numerical.py
+-rw-r--r--   0        0        0    34143 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/objects.py
+-rw-r--r--   0        0        0    18835 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/interpretation/strings.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/language/__init__.py
+-rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/language/python.py
+-rw-r--r--   0        0        0    25744 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/RNTuple.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TArray.py
+-rw-r--r--   0        0        0    25379 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TAtt.py
+-rw-r--r--   0        0        0    11179 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TBasket.py
+-rw-r--r--   0        0        0    37043 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TBranch.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TClonesArray.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TDatime.py
+-rw-r--r--   0        0        0    35595 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TGraph.py
+-rw-r--r--   0        0        0   213682 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TH.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/THashList.py
+-rw-r--r--   0        0        0    33898 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TLeaf.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TList.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TMatrixT.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TNamed.py
+-rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TObjArray.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TObjString.py
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TObject.py
+-rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TRef.py
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TString.py
+-rw-r--r--   0        0        0     7255 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TTable.py
+-rw-r--r--   0        0        0    46956 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/TTree.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/models/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/sink/__init__.py
+-rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/sink/file.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/__init__.py
+-rw-r--r--   0        0        0    16003 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/chunk.py
+-rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/cursor.py
+-rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/file.py
+-rw-r--r--   0        0        0    14154 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/futures.py
+-rw-r--r--   0        0        0    25910 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/http.py
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/object.py
+-rw-r--r--   0        0        0    15697 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/source/xrootd.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/writing/__init__.py
+-rw-r--r--   0        0        0    82851 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/writing/_cascade.py
+-rw-r--r--   0        0        0    31855 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/writing/_cascadentuple.py
+-rw-r--r--   0        0        0    56422 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/writing/_cascadetree.py
+-rw-r--r--   0        0        0    79676 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/writing/identify.py
+-rw-r--r--   0        0        0    80251 2020-02-02 00:00:00.000000 uproot-5.0.8/src/uproot/writing/writable.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/conftest.py
+-rw-r--r--   0        0        0    15805 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0001-source-class.py
+-rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0006-notify-when-downloaded.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0007-single-chunk-interface.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0008-start-interpretation.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0009-nested-directories.py
+-rw-r--r--   0        0        0    29196 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0010-start-streamers.py
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0011-generate-classes-from-streamers.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0013-rntuple-anchor.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0014-all-ttree-versions.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0016-interpretations.py
+-rw-r--r--   0        0        0     9682 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0017-multi-basket-multi-branch-fetch.py
+-rw-r--r--   0        0        0    33935 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0018-array-fetching-interface.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0022-number-of-branches.py
+-rw-r--r--   0        0        0    13960 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0023-more-interpretations-1.py
+-rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0023-ttree-versions.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0028-fallback-to-read-streamer.py
+-rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0029-more-string-types.py
+-rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0031-test-stl-containers.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0033-more-interpretations-2.py
+-rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0034-generic-objects-in-ttrees.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0035-datatype-generality.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0038-memberwise-serialization.py
+-rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0043-iterate-function.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0044-concatenate-function.py
+-rw-r--r--   0        0        0    68981 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0046-histograms-bh-hist.py
+-rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0053-parents-should-not-be-bases.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0058-detach-model-objects-from-files.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0066-fix-http-fallback-freeze.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0067-common-entry-offsets.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0081-dont-parse-colons.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0087-memberwise-splitting-not-implemented-messages.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0088-read-with-http.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0099-read-from-file-object.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0112-fix-pandas-with-cut.py
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0118-fix-name-fetch-again.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0123-atlas-issues.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0126-turn-unknown-emptyarrays-into-known-types.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0167-use-the-common-histogram-interface.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0172-allow-allocators-in-vector-typenames.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0173-empty-and-multiprocessing-bugs.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0182-complain-about-missing-files.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0194-fix-lost-cuts-in-iterate.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0220-contiguous-byte-ranges-in-http.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0228_read-TProfiles.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0240-read_TGraphAsymmErrors.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0278-specializations-for-TParameter.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0302-pickle.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0303-empty-jagged-array.py
+-rw-r--r--   0        0        0    14234 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0320-start-working-on-ROOT-writing.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0322-writablefile-infrastructure.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0325-fix-windows-file-uris.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0329-update-existing-root-files.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0335-empty-ttree-division-by-zero.py
+-rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0341-manipulate-streamer-info.py
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0344-writabledirectory-can-read.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0345-bulk-copy-method.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0349-write-TObjString.py
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0350-read-RooCurve-RooHist.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0351-write-TList.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0352-write-THashList.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0384-move-behavior_of-and-fix-383.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0398-dimensions-in-leaflist.py
+-rw-r--r--   0        0        0    26536 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0405-write-a-histogram.py
+-rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0406-write-a-ttree.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0407-read-TDatime.py
+-rw-r--r--   0        0        0    17062 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0412-write-multidimensional-numpy-to-ttree.py
+-rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0414-write-jagged-arrays.py
+-rw-r--r--   0        0        0    16674 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0416-writing-compressed-data.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0418-read-TTable.py
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0420-pyroot-uproot-interoperability.py
+-rw-r--r--   0        0        0    17479 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0422-hist-integration.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0430-global_index-for-tuples-of-DataFrames.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0438-TClonesArray-is-not-AsGrouped.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0439-check-awkward-before-numpy.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0442-regular-TClonesArray.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0472-tstreamerinfo-for-ttree.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0475-remember-to-update-freesegments.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0484-manually-add-model-for-TMatrixTSym_double_.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0487-implement-asdtypeinplace.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0498-create-leaf-branch-in-extend.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0519-remove-memmap-copy.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0520-dynamic-classes-cant-be-abc-subclasses.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0569-fBits-is-4-bytes.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0576-unicode-in-names.py
+-rw-r--r--   0        0        0    25906 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0578-dask-for-numpy.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0580-round-trip-for-no-flow-histograms.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0589-explicitly-interpret-RVec-type.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0603-dask-delayed-open.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0609-num-enteries-func.py
+-rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0610-awkward-form.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0630-rntuple-basics.py
+-rw-r--r--   0        0        0    58430 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0637-setup-tests-for-AwkwardForth.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0643-reading-vector-pair-TLorentzVector-int.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0651-implement-transformed-axis.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0652_dask-for-awkward.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0662-rntuple-stl-containers.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0700-dask-empty-arrays.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0705-rntuple-writing-metadata.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0750-avoid-empty-TBasket-issue.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0755-dask-awkward-column-projection.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0791-protect-uproot-project_columns-from-dask-node-names.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0798_DAOD_PHYSLITE.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0808-fix_awkward_form_for_AsStridedObjects.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0816-separate-AwkwardForth-machines-by-TBranch.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0832-ak_add_doc-should-also-add-to-typetracer.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0840-support-tleafG.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0841-fix-814.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0844-fix-delete-hist-from-root.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0852-fix-strided-interp-extra-offsets.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0870-writing-arrays-of-type-unknown-fix-822.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0876-uproot-dask-blind-steps.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/test_0886-fix-awkward-form-breadcrumbs.py
+-rw-r--r--   0        0        0   128147 2020-02-02 00:00:00.000000 uproot-5.0.8/tests/samples/h_dynamic.pkl
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 uproot-5.0.8/.gitignore
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 uproot-5.0.8/LICENSE
+-rw-r--r--   0        0        0    25899 2020-02-02 00:00:00.000000 uproot-5.0.8/README.md
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 uproot-5.0.8/pyproject.toml
+-rw-r--r--   0        0        0    28208 2020-02-02 00:00:00.000000 uproot-5.0.8/PKG-INFO
```

### Comparing `uproot-5.0.7/.all-contributorsrc` & `uproot-5.0.8/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/CITATION.cff` & `uproot-5.0.8/CITATION.cff`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/.github/ISSUE_TEMPLATE/bug-report.md` & `uproot-5.0.8/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/.github/ISSUE_TEMPLATE/feature-request.md` & `uproot-5.0.8/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/.github/workflows/build-test.yml` & `uproot-5.0.8/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/.github/workflows/deploy.yml` & `uproot-5.0.8/.github/workflows/deploy.yml`

 * *Files 2% similar despite different names*

```diff
@@ -30,10 +30,10 @@
 
     steps:
     - uses: actions/download-artifact@v3
       with:
         name: artifact
         path: dist
 
-    - uses: pypa/gh-action-pypi-publish@v1.8.5
+    - uses: pypa/gh-action-pypi-publish@release/v1
       with:
         password: ${{ secrets.pypi_password }}
```

### Comparing `uproot-5.0.7/dev/example-objects.py` & `uproot-5.0.8/dev/example-objects.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/dev/make-models.py` & `uproot-5.0.8/dev/make-models.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-img/diagrams/abstraction-layers.png` & `uproot-5.0.8/docs-img/diagrams/abstraction-layers.png`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-img/diagrams/abstraction-layers.svg` & `uproot-5.0.8/docs-img/diagrams/abstraction-layers.svg`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-img/diagrams/example-dask-graph.png` & `uproot-5.0.8/docs-img/diagrams/example-dask-graph.png`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-img/diagrams/uproot-awkward-timeline.png` & `uproot-5.0.8/docs-img/diagrams/uproot-awkward-timeline.png`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-img/diagrams/uproot-awkward-timeline.svg` & `uproot-5.0.8/docs-img/diagrams/uproot-awkward-timeline.svg`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-img/logo/logo-300px-white.png` & `uproot-5.0.8/docs-img/logo/logo-300px-white.png`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-img/logo/logo-300px.png` & `uproot-5.0.8/docs-img/logo/logo-300px.png`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-img/logo/logo-600px.png` & `uproot-5.0.8/docs-img/logo/logo-600px.png`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-img/logo/logo.svg` & `uproot-5.0.8/docs-img/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-img/photos/switcheroo.jpg` & `uproot-5.0.8/docs-img/photos/switcheroo.jpg`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-sphinx/basic.rst` & `uproot-5.0.8/docs-sphinx/basic.rst`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-sphinx/conf.py` & `uproot-5.0.8/docs-sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-sphinx/index.rst` & `uproot-5.0.8/docs-sphinx/index.rst`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-sphinx/make_changelog.py` & `uproot-5.0.8/docs-sphinx/make_changelog.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-sphinx/prepare_docstrings.py` & `uproot-5.0.8/docs-sphinx/prepare_docstrings.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/docs-sphinx/uproot3-to-4.rst` & `uproot-5.0.8/docs-sphinx/uproot3-to-4.rst`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/__init__.py` & `uproot-5.0.8/src/uproot/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/_awkward_forth.py` & `uproot-5.0.8/src/uproot/_awkward_forth.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/_dask.py` & `uproot-5.0.8/src/uproot/_dask.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,24 +43,24 @@
             overrules the standard one.
         recursive (bool): If True, include all subbranches of branches as
             separate fields; otherwise, only search one level deep.
         full_paths (bool): If True, include the full path to each subbranch
             with slashes (``/``); otherwise, use the descendant's name as
             the field name.
         step_size (int or str): If an integer, the maximum number of entries to
-            include in each chunk; if a string, the maximum memory_size to include
-            in each chunk. The string must be a number followed by a memory unit,
+            include in each chunk/partition; if a string, the maximum memory_size to include
+            in each chunk/partition. The string must be a number followed by a memory unit,
             such as "100 MB". Mutually incompatible with steps_per_file: only set
             step_size or steps_per_file, not both. Cannot be used with
             ``open_files=False``.
         steps_per_file (int, default 1):
-            Subdivide files into the specified number of chunks. Mutually incompatible
+            Subdivide files into the specified number of chunks/partitions. Mutually incompatible
             with step_size: only set step_size or steps_per_file, not both.
             If both ``step_size`` and ``steps_per_file`` are unset,
-            ``steps_per_file``'s default value of 1 (whole file per chunk) is used,
+            ``steps_per_file``'s default value of 1 (whole file per chunk/partition) is used,
             regardless of ``open_files``.
         library (str or :doc:`uproot.interpretation.library.Library`): The library
             that is used to represent arrays. If ``library='np'`` it returns a dict
             of dask arrays and if ``library='ak'`` it returns a single dask-awkward
             array. ``library='pd'`` has not been implemented yet and will raise a
             ``NotImplementedError``.
         ak_add_doc (bool): If True and ``library="ak"``, add the TBranch ``title``
@@ -118,14 +118,19 @@
     * pathlib.Path: always interpreted as a filesystem path or URL only (no
       object-within-ROOT path), regardless of whether there are any colons.
       Examples: ``Path("rel:/file.root")``, ``Path("/abs/path:stuff.root")``
     * glob syntax in str/bytes and pathlib.Path.
       Examples: ``Path("rel/*.root")``, ``"/abs/*.root:tdirectory/ttree"``
     * dict: keys are filesystem paths, values are objects-within-ROOT paths.
       Example: ``{{"/data_v1/*.root": "ttree_v1", "/data_v2/*.root": "ttree_v2"}}``
+    * dict: keys are filesystem paths, values are dicts containing objects-within-ROOT and
+      steps (chunks/partitions) as a list of starts and stops or steps as a list of offsets
+      Example: ``{{"/data_v1/tree1.root": {"object_path": "ttree_v1", "steps": [[0, 10000], [15000, 20000], ...]},
+                   "/data_v1/tree2.root": {"object_path": "ttree_v1", "steps": [0, 10000, 20000, ...]}}}``
+      (This ``files`` pattern is incompatible with ``step_size`` and ``steps_per_file``.)
     * already-open TTree objects.
     * iterables of the above.
 
     Options (type; default):
 
     * file_handler (:doc:`uproot.source.chunk.Source` class; :doc:`uproot.source.file.MemmapSource`)
     * xrootd_handler (:doc:`uproot.source.chunk.Source` class; :doc:`uproot.source.xrootd.XRootDSource`)
@@ -145,15 +150,31 @@
       contiguous entries in ``TTrees``.
     * :doc:`uproot.behaviors.TBranch.concatenate`: returns a single
       concatenated array from ``TTrees``.
     * :doc:`uproot._dask.dask` (this function): returns an unevaluated Dask
       array from ``TTrees``.
     """
 
-    files = uproot._util.regularize_files(files)
+    files = uproot._util.regularize_files(files, steps_allowed=True)
+
+    is_3arg = [len(x) == 3 for x in files]
+    if any(is_3arg):
+        if not all(is_3arg):
+            raise TypeError(
+                "partition sizes for some but not all 'files' have been assigned"
+            )
+        if step_size is not unset:
+            raise TypeError(
+                "partition sizes for 'files' is incompatible with 'step_size'"
+            )
+        if steps_per_file is not unset:
+            raise TypeError(
+                "partition sizes for 'files' is incompatible with 'steps_per_file'"
+            )
+
     library = uproot.interpretation.library._regularize_library(library)
 
     if step_size is not unset and steps_per_file is not unset:
         raise TypeError(
             f"only 'step_size' or 'steps_per_file' should be set, not both; got step_size={step_size!r} and steps_per_file={steps_per_file!r}"
         )
     elif step_size is not unset:
@@ -420,28 +441,48 @@
     ):
         self.custom_classes = custom_classes
         self.allow_missing = allow_missing
         self.real_options = real_options
         self.key = key
         self.interp_options = interp_options
 
-    def __call__(self, file_path_object_path_istep_nsteps):
-        file_path, object_path, istep, nsteps = file_path_object_path_istep_nsteps
+    def __call__(self, file_path_object_path_istep_nsteps_ischunk):
+        (
+            file_path,
+            object_path,
+            istep_or_start,
+            nsteps_or_stop,
+            ischunk,
+        ) = file_path_object_path_istep_nsteps_ischunk
         ttree = uproot._util.regularize_object_path(
             file_path,
             object_path,
             self.custom_classes,
             self.allow_missing,
             self.real_options,
         )
         num_entries = ttree.num_entries
-        events_per_steps = math.ceil(num_entries / nsteps)
-        start, stop = (istep * events_per_steps), min(
-            (istep + 1) * events_per_steps, num_entries
-        )
+        start, stop = istep_or_start, nsteps_or_stop
+        if not ischunk:
+            events_per_steps = math.ceil(num_entries / nsteps_or_stop)
+            start, stop = (istep_or_start * events_per_steps), min(
+                (istep_or_start + 1) * events_per_steps, num_entries
+            )
+        elif (not 0 <= start < num_entries) or (not 0 <= stop <= num_entries):
+            raise ValueError(
+                f"""explicit entry start ({start}) or stop ({stop}) from uproot.dask 'files' argument is out of bounds for file
+
+    {ttree.file.file_path}
+
+TTree in path
+
+    {ttree.object_path}
+
+which has {num_entries} entries"""
+            )
 
         return ttree[self.key].array(
             library="np",
             entry_start=start,
             entry_stop=stop,
             ak_add_doc=self.interp_options["ak_add_doc"],
         )
@@ -458,19 +499,22 @@
     custom_classes,
     allow_missing,
     real_options,
     interp_options,
     steps_per_file,
 ):
     ttrees = []
+    explicit_chunks = []
     common_keys = None
     is_self = []
 
     count = 0
-    for file_path, object_path in files:
+    for file_object_maybechunks in files:
+        file_path, object_path = file_object_maybechunks[0:2]
+
         obj = uproot._util.regularize_object_path(
             file_path, object_path, custom_classes, allow_missing, real_options
         )
 
         if obj is not None:
             count += 1
 
@@ -483,14 +527,18 @@
                     return branch is original and filter_branch(branch)  # noqa: B023
 
             else:
                 is_self.append(False)
                 real_filter_branch = filter_branch
 
             ttrees.append(obj)
+            if len(file_object_maybechunks) == 3:
+                explicit_chunks.append(file_object_maybechunks[2])
+            else:
+                explicit_chunks = None  # they all have it or none of them have it
 
             new_keys = obj.keys(
                 recursive=recursive,
                 filter_name=filter_name,
                 filter_typename=filter_typename,
                 filter_branch=real_filter_branch,
                 full_paths=full_paths,
@@ -569,22 +617,39 @@
 
         chunks = []
         chunk_args = []
         for i, ttree in enumerate(ttrees):
             entry_start = 0
             entry_stop = ttree.num_entries
 
-            def foreach(start):
-                stop = min(start + entry_step, entry_stop)  # noqa: B023
-                length = stop - start
-                chunks.append(length)  # noqa: B023
-                chunk_args.append((i, start, stop))  # noqa: B023
-
-            for start in range(entry_start, entry_stop, entry_step):
-                foreach(start)
+            if explicit_chunks is None:
+                for start in range(entry_start, entry_stop, entry_step):
+                    stop = min(start + entry_step, entry_stop)
+                    length = stop - start
+                    if length > 0:
+                        chunks.append(length)
+                        chunk_args.append((i, start, stop))
+            else:
+                for start, stop in explicit_chunks[i]:
+                    if (not 0 <= start < entry_stop) or (not 0 <= stop <= entry_stop):
+                        raise ValueError(
+                            f"""explicit entry start ({start}) or stop ({stop}) from uproot.dask 'files' argument is out of bounds for file
+
+    {ttree.file.file_path}
+
+TTree in path
+
+    {ttree.object_path}
+
+which has {entry_stop} entries"""
+                        )
+                    length = stop - start
+                    if length > 0:
+                        chunks.append(length)
+                        chunk_args.append((i, start, stop))
 
         if len(chunk_args) == 0:
             chunks.append(0)
             chunk_args.append((0, 0, 0))
 
         dask_dict[key] = _dask_array_from_map(
             _UprootReadNumpy(ttrees, key, interp_options),
@@ -606,15 +671,15 @@
     full_paths,
     custom_classes,
     allow_missing,
     real_options,
     interp_options,
     steps_per_file,
 ):
-    ffile_path, fobject_path = files[0]
+    ffile_path, fobject_path = files[0][0:2]
     obj = uproot._util.regularize_object_path(
         ffile_path, fobject_path, custom_classes, allow_missing, real_options
     )
     common_keys = obj.keys(
         recursive=recursive,
         filter_name=filter_name,
         filter_typename=filter_typename,
@@ -627,32 +692,54 @@
     for key in common_keys:
         dt = obj[key].interpretation.numpy_dtype
         if dt.subdtype is None:
             inner_shape = ()
         else:
             dt, inner_shape = dt.subdtype
 
+        partitions = []
         partition_args = []
-        for ifile_path, iobject_path in files:
-            for istep in range(steps_per_file):
-                partition_args.append(
-                    (
-                        ifile_path,
-                        iobject_path,
-                        istep,
-                        steps_per_file,
+        for ifile_iobject_maybeichunks in files:
+            ifile_path, iobject_path = ifile_iobject_maybeichunks[0:2]
+
+            chunks = None
+            if len(ifile_iobject_maybeichunks) == 3:
+                chunks = ifile_iobject_maybeichunks[2]
+
+            if chunks is not None:
+                partitions.extend([stop - start for start, stop in chunks])
+                for start, stop in chunks:
+                    partition_args.append(
+                        (
+                            ifile_path,
+                            iobject_path,
+                            start,
+                            stop,
+                            True,
+                        )
+                    )
+            else:
+                partitions.extend([numpy.nan] * steps_per_file)
+                for istep in range(steps_per_file):
+                    partition_args.append(
+                        (
+                            ifile_path,
+                            iobject_path,
+                            istep,
+                            steps_per_file,
+                            False,
+                        )
                     )
-                )
 
         dask_dict[key] = _dask_array_from_map(
             _UprootOpenAndReadNumpy(
                 custom_classes, allow_missing, real_options, key, interp_options
             ),
             partition_args,
-            chunks=((numpy.nan,) * len(files) * steps_per_file,),
+            chunks=(tuple(partitions),),
             dtype=dt,
             label=f"{key}-from-uproot",
         )
     return dask_dict
 
 
 class _UprootRead:
@@ -751,28 +838,48 @@
         self.real_options = real_options
         self.common_keys = common_keys
         self.common_base_keys = common_base_keys
         self.interp_options = interp_options
         self.form_mapping = form_mapping
         self.rendered_form = rendered_form
 
-    def __call__(self, file_path_object_path_istep_nsteps):
-        file_path, object_path, istep, nsteps = file_path_object_path_istep_nsteps
+    def __call__(self, file_path_object_path_istep_nsteps_ischunk):
+        (
+            file_path,
+            object_path,
+            istep_or_start,
+            nsteps_or_stop,
+            ischunk,
+        ) = file_path_object_path_istep_nsteps_ischunk
         ttree = uproot._util.regularize_object_path(
             file_path,
             object_path,
             self.custom_classes,
             self.allow_missing,
             self.real_options,
         )
         num_entries = ttree.num_entries
-        events_per_step = math.ceil(num_entries / nsteps)
-        start, stop = (istep * events_per_step), min(
-            (istep + 1) * events_per_step, num_entries
-        )
+        start, stop = istep_or_start, nsteps_or_stop
+        if not ischunk:
+            events_per_step = math.ceil(num_entries / nsteps_or_stop)
+            start, stop = (istep_or_start * events_per_step), min(
+                (istep_or_start + 1) * events_per_step, num_entries
+            )
+        elif (not 0 <= start < num_entries) or (not 0 <= stop <= num_entries):
+            raise ValueError(
+                f"""explicit entry start ({start}) or stop ({stop}) from uproot.dask 'files' argument is out of bounds for file
+
+    {ttree.file.file_path}
+
+TTree in path
+
+    {ttree.object_path}
+
+which has {num_entries} entries"""
+            )
 
         if self.form_mapping is not None:
             awkward = uproot.extras.awkward()
 
             actual_form = self.rendered_form.select_columns(self.common_keys)
 
             mapping, buffer_key = self.form_mapping.create_column_mapping_and_key(
@@ -851,16 +958,17 @@
     parameters = {"__doc__": ttree.title} if ak_add_doc else None
 
     form = awkward.forms.RecordForm(contents, common_keys, parameters=parameters)
 
     if form_mapping is not None:
         form = form_mapping(form)
 
-    empty_arr = form.length_zero_array(
-        behavior=None if form_mapping is None else form_mapping.behavior
+    empty_arr = awkward.Array(
+        form.length_zero_array(highlevel=False),
+        behavior=None if form_mapping is None else form_mapping.behavior,
     )
 
     return dask_awkward.core.typetracer_array(empty_arr), form
 
 
 def _get_dak_array(
     files,
@@ -877,19 +985,22 @@
     form_mapping,
     steps_per_file,
 ):
     dask_awkward = uproot.extras.dask_awkward()
     awkward = uproot.extras.awkward()
 
     ttrees = []
+    explicit_chunks = []
     common_keys = None
     is_self = []
 
     count = 0
-    for file_path, object_path in files:
+    for file_object_maybechunks in files:
+        file_path, object_path = file_object_maybechunks[0:2]
+
         obj = uproot._util.regularize_object_path(
             file_path, object_path, custom_classes, allow_missing, real_options
         )
 
         if obj is not None:
             count += 1
 
@@ -902,14 +1013,18 @@
                     return branch is original and filter_branch(branch)  # noqa: B023
 
             else:
                 is_self.append(False)
                 real_filter_branch = filter_branch
 
             ttrees.append(obj)
+            if len(file_object_maybechunks) == 3:
+                explicit_chunks.append(file_object_maybechunks[2])
+            else:
+                explicit_chunks = None  # they all have it or none of them have it
 
             new_keys = obj.keys(
                 recursive=recursive,
                 filter_name=filter_name,
                 filter_typename=filter_typename,
                 filter_branch=real_filter_branch,
                 full_paths=full_paths,
@@ -972,47 +1087,70 @@
         ttree_step = _regularize_step_size(
             ttree, step_size, entry_start, entry_stop, branchid_interpretation
         )
         step_sum += int(ttree_step)
 
     entry_step = int(round(step_sum / len(ttrees)))
 
+    divisions = [0]
     partition_args = []
     for i, ttree in enumerate(ttrees):
         entry_start = 0
         entry_stop = ttree.num_entries
 
-        def foreach(start):
-            stop = min(start + entry_step, entry_stop)  # noqa: B023
-            partition_args.append((i, start, stop))  # noqa: B023
+        if explicit_chunks is None:
+            for start in range(entry_start, entry_stop, entry_step):
+                stop = min(start + entry_step, entry_stop)
+                length = stop - start
+                if length > 0:
+                    divisions.append(divisions[-1] + length)
+                    partition_args.append((i, start, stop))
+        else:
+            for start, stop in explicit_chunks[i]:
+                if (not 0 <= start < entry_stop) or (not 0 <= stop <= entry_stop):
+                    raise ValueError(
+                        f"""explicit entry start ({start}) or stop ({stop}) from uproot.dask 'files' argument is out of bounds for file
+
+    {ttree.file.file_path}
 
-        for start in range(entry_start, entry_stop, entry_step):
-            foreach(start)
+TTree in path
+
+    {ttree.object_path}
+
+which has {entry_stop} entries"""
+                    )
+                length = stop - start
+                if length > 0:
+                    divisions.append(divisions[-1] + length)
+                    partition_args.append((i, start, stop))
 
     meta, form = _get_meta_array(
         awkward,
         dask_awkward,
         ttrees[0],
         common_keys,
         form_mapping,
         interp_options.get("ak_add_doc"),
     )
 
     if len(partition_args) == 0:
+        divisions.append(0)
         partition_args.append((0, 0, 0))
+
     return dask_awkward.from_map(
         _UprootRead(
             ttrees,
             common_keys,
             common_keys,
             interp_options,
             form_mapping=form_mapping,
             rendered_form=None if form_mapping is None else form,
         ),
         partition_args,
+        divisions=tuple(divisions),
         label="from-uproot",
         behavior=None if form_mapping is None else form_mapping.behavior,
         meta=meta,
     )
 
 
 def _get_dak_array_delay_open(
@@ -1028,15 +1166,16 @@
     interp_options,
     form_mapping,
     steps_per_file,
 ):
     dask_awkward = uproot.extras.dask_awkward()
     awkward = uproot.extras.awkward()
 
-    ffile_path, fobject_path = files[0]
+    ffile_path, fobject_path = files[0][0:2]
+
     obj = uproot._util.regularize_object_path(
         ffile_path, fobject_path, custom_classes, allow_missing, real_options
     )
     common_keys = obj.keys(
         recursive=recursive,
         filter_name=filter_name,
         filter_typename=filter_typename,
@@ -1049,35 +1188,57 @@
         dask_awkward,
         obj,
         common_keys,
         form_mapping,
         interp_options.get("ak_add_doc"),
     )
 
+    divisions = [0]
     partition_args = []
-    for ifile_path, iobject_path in files:
-        for istep in range(steps_per_file):
-            partition_args.append(
-                (
-                    ifile_path,
-                    iobject_path,
-                    istep,
-                    steps_per_file,
+    for ifile_iobject_maybeichunks in files:
+        chunks = None
+        ifile_path, iobject_path = ifile_iobject_maybeichunks[0:2]
+        if len(ifile_iobject_maybeichunks) == 3:
+            chunks = ifile_iobject_maybeichunks[2]
+
+        if chunks is not None:
+            for start, stop in chunks:
+                divisions.append(divisions[-1] + (stop - start))
+                partition_args.append(
+                    (
+                        ifile_path,
+                        iobject_path,
+                        start,
+                        stop,
+                        True,
+                    )
+                )
+        else:
+            divisions = None  # they all have it or none of them have it
+            for istep in range(steps_per_file):
+                partition_args.append(
+                    (
+                        ifile_path,
+                        iobject_path,
+                        istep,
+                        steps_per_file,
+                        False,
+                    )
                 )
-            )
 
     return dask_awkward.from_map(
         _UprootOpenAndRead(
             custom_classes,
             allow_missing,
             real_options,
             common_keys,
             common_keys,
             interp_options,
             form_mapping=form_mapping,
             rendered_form=None if form_mapping is None else form,
         ),
         partition_args,
+        divisions=None if divisions is None else tuple(divisions),
         label="from-uproot",
         behavior=None if form_mapping is None else form_mapping.behavior,
         meta=meta,
     )
```

### Comparing `uproot-5.0.7/src/uproot/_util.py` & `uproot-5.0.8/src/uproot/_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -804,36 +804,69 @@
     return out
 
 
 _regularize_files_braces = re.compile(r"{([^}]*,)*([^}]*)}")
 _regularize_files_isglob = re.compile(r"[\*\?\[\]{}]")
 
 
-def _regularize_files_inner(files, parse_colon, counter, HasBranches):
+def regularize_steps(steps):
+    out = numpy.array(steps)
+
+    if isinstance(steps, dict) or not issubclass(out.dtype.type, numpy.integer):
+        raise TypeError(
+            "'files' argument's steps must be an iterable of integer offsets or start-stop pairs."
+        )
+
+    if len(out.shape) == 1:
+        if len(out) == 0 or not numpy.all(out[1:] >= out[:-1]):
+            raise ValueError(
+                "if 'files' argument's steps are (one-dimensional) offsets, they must be non-empty and monotonically increasing"
+            )
+
+    elif len(out.shape) == 2:
+        if not (out.shape[1] == 2 and all(out[:, 1] >= out[:, 0])):
+            raise ValueError(
+                "if 'files' argument's steps are (two-dimensional) start-stop pairs, all stops must be greater than or equal to their corresponding starts"
+            )
+
+    else:
+        raise TypeError(
+            "'files' argument's steps must be an iterable of integer offsets or a list of pairs of integer starts and stops."
+        )
+
+    if len(out.shape) == 1:
+        out = numpy.stack((out[:-1], out[1:]), axis=1)
+
+    return out.tolist()
+
+
+def _regularize_files_inner(files, parse_colon, counter, HasBranches, steps_allowed):
     files2 = regularize_path(files)
 
+    maybe_steps = None
+
     if isstr(files2) and not isstr(files):
         parse_colon = False
         files = files2
 
     if isstr(files):
         if parse_colon:
             file_path, object_path = file_object_path_split(files)
         else:
             file_path, object_path = files, None
 
         parsed_url = urlparse(file_path)
 
         if parsed_url.scheme.upper() in _remote_schemes:
-            yield file_path, object_path
+            yield file_path, object_path, maybe_steps
 
         else:
             expanded = os.path.expanduser(file_path)
             if _regularize_files_isglob.search(expanded) is None:
-                yield file_path, object_path
+                yield file_path, object_path, maybe_steps
 
             else:
                 matches = list(_regularize_files_braces.finditer(expanded))
                 if len(matches) == 0:
                     results = [expanded]
                 else:
                     results = []
@@ -845,63 +878,85 @@
                             tmp = tmp[: m.span()[0]] + c + tmp[m.span()[1] :]
                         results.append(tmp)
 
                 seen = set()
                 for result in results:
                     for match in glob.glob(result):
                         if match not in seen:
-                            yield match, object_path
+                            yield match, object_path, maybe_steps
                             seen.add(match)
 
     elif isinstance(files, HasBranches):
-        yield files, None
+        yield files, None, maybe_steps
 
     elif isinstance(files, dict):
-        for key, object_path in files.items():
-            for file_path, _ in _regularize_files_inner(
-                key, False, counter, HasBranches
+        for key, maybe_object_path in files.items():
+            if not isinstance(maybe_object_path, (type(None), str, dict)):
+                raise TypeError("object_path may only be a string, dict, or None")
+            if isinstance(maybe_object_path, dict):
+                maybe_steps = maybe_object_path.get("steps", None)
+                object_path = maybe_object_path.get("object_path", None)
+                if maybe_steps is not None:
+                    if not steps_allowed:
+                        raise TypeError(
+                            "unrecognized 'files' pattern for this function ('steps' are only allowed in uproot.dask)"
+                        )
+                    maybe_steps = regularize_steps(maybe_steps)
+            else:
+                object_path = maybe_object_path
+            for file_path, _, _ in _regularize_files_inner(
+                key,
+                False,
+                counter,
+                HasBranches,
+                steps_allowed,
             ):
-                yield file_path, object_path
+                yield file_path, object_path, maybe_steps
 
     elif isinstance(files, Iterable):
         for file in files:
             counter[0] += 1
-            for file_path, object_path in _regularize_files_inner(
-                file, parse_colon, counter, HasBranches
+            for file_path, object_path, maybe_steps in _regularize_files_inner(
+                file, parse_colon, counter, HasBranches, steps_allowed
             ):
-                yield file_path, object_path
+                yield file_path, object_path, maybe_steps
 
     else:
         raise TypeError(
             "'files' must be a file path/URL (string or Path), possibly with "
             "a glob pattern (for local files), a dict of "
             "{path/URL: TTree/TBranch name}, actual TTree/TBranch objects, or "
             f"an iterable of such things, not {files!r}"
         )
 
 
-def regularize_files(files):
+def regularize_files(files, steps_allowed):
     """
     Common code for regularizing the possible file inputs accepted by uproot so they can be used by uproot internal functions.
     """
     from uproot.behaviors.TBranch import HasBranches
 
     out = []
     seen = set()
     counter = [0]
-    for file_path, object_path in _regularize_files_inner(
-        files, True, counter, HasBranches
+    for file_path, object_path, maybe_steps in _regularize_files_inner(
+        files, True, counter, HasBranches, steps_allowed
     ):
         if isstr(file_path):
             key = (counter[0], file_path, object_path)
             if key not in seen:
                 out.append((file_path, object_path))
+                if maybe_steps is not None:
+                    out[-1] = (*out[-1], maybe_steps)
+
                 seen.add(key)
         else:
             out.append((file_path, object_path))
+            if maybe_steps is not None:
+                out[-1] = (*out[-1], maybe_steps)
 
     if len(out) == 0:
         raise _file_not_found(files)
 
     return out
```

### Comparing `uproot-5.0.7/src/uproot/behavior.py` & `uproot-5.0.8/src/uproot/behavior.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/cache.py` & `uproot-5.0.8/src/uproot/cache.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/compression.py` & `uproot-5.0.8/src/uproot/compression.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/const.py` & `uproot-5.0.8/src/uproot/const.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/containers.py` & `uproot-5.0.8/src/uproot/containers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/deserialization.py` & `uproot-5.0.8/src/uproot/deserialization.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/dynamic.py` & `uproot-5.0.8/src/uproot/dynamic.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/exceptions.py` & `uproot-5.0.8/src/uproot/exceptions.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/extras.py` & `uproot-5.0.8/src/uproot/extras.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/model.py` & `uproot-5.0.8/src/uproot/model.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/pyroot.py` & `uproot-5.0.8/src/uproot/pyroot.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/reading.py` & `uproot-5.0.8/src/uproot/reading.py`

 * *Files 0% similar despite different names*

```diff
@@ -1480,15 +1480,15 @@
         """
         Object path of the ``TDirectory`` as a single string, beginning and
         ending with ``/``. The root directory is a single slash, ``"/"``.
 
         See :ref:`uproot.reading.ReadOnlyDirectory.path` for the path as a
         tuple of strings.
         """
-        return "/".join(("", *self._path) + ("",)).replace("//", "/")
+        return "/".join(("", *self._path, "")).replace("//", "/")
 
     @property
     def file_path(self):
         """
         The original path to the file (converted to ``str`` if it was originally
         a ``pathlib.Path``).
         """
```

### Comparing `uproot-5.0.7/src/uproot/serialization.py` & `uproot-5.0.8/src/uproot/serialization.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/streamers.py` & `uproot-5.0.8/src/uproot/streamers.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,14 +238,15 @@
         ]
         awkward_form = [
             "    @classmethod",
             "    def awkward_form(cls, file, context):",
             "        from awkward.forms import NumpyForm, ListOffsetForm, RegularForm, RecordForm",
             "        if cls in context['breadcrumbs']:",
             "            raise uproot.interpretation.objects.CannotBeAwkward('classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded')",
+            "        context = context.copy()",
             "        context['breadcrumbs'] = context['breadcrumbs'] + (cls,)",
             "        contents = {}",
             "        if context['header']:",
             "            contents['@num_bytes'] = uproot._util.awkward_form(numpy.dtype('u4'), file, context)",
             "            contents['@instance_version'] = uproot._util.awkward_form(numpy.dtype('u2'), file, context)",
         ]
         fields = []
@@ -549,17 +550,18 @@
         else:
             self._members["fMaxIndex"] = cursor.array(
                 chunk, 5, _tstreamerelement_dtype1, context
             )
 
         self._members["fTypeName"] = _canonical_typename(cursor.string(chunk, context))
 
-        if self._members["fType"] == 11 and self._members["fTypeName"] in (
-            "Bool_t" or "bool"
-        ):
+        if self._members["fType"] == 11 and self._members["fTypeName"] in {
+            "Bool_t",
+            "bool",
+        }:
             self._members["fType"] = 18
 
         if self._instance_version <= 2:
             # FIXME
             # self._fSize = self._fArrayLength * gROOT->GetType(GetTypeName())->Size()
             pass
```

### Comparing `uproot-5.0.7/src/uproot/behaviors/RooCurve.py` & `uproot-5.0.8/src/uproot/behaviors/RooCurve.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/behaviors/RooHist.py` & `uproot-5.0.8/src/uproot/behaviors/RooHist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/behaviors/TAxis.py` & `uproot-5.0.8/src/uproot/behaviors/TAxis.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         """
         fNbins = self.member("fNbins")
         fLabels = self.member("fLabels", none_if_missing=True)
 
         if fLabels is not None and len(fLabels) == fNbins:
             out = [str(x) for x in fLabels]
             if flow:
-                return ["underflow", *out] + ["overflow"]
+                return ["underflow", *out, "overflow"]
             else:
                 return out
         else:
             return None
 
     def edges(self, flow=False):
         """
```

### Comparing `uproot-5.0.7/src/uproot/behaviors/TBranch.py` & `uproot-5.0.8/src/uproot/behaviors/TBranch.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     * :doc:`uproot.reading.open`: opens one file to read any of its objects.
     * :doc:`uproot.behaviors.TBranch.iterate` (this function): iterates through
       chunks of contiguous entries in ``TTrees``.
     * :doc:`uproot.behaviors.TBranch.concatenate`: returns a single concatenated
       array from ``TTrees``.
     * :doc:`uproot._dask.dask`: returns an unevaluated Dask array from ``TTrees``.
     """
-    files = uproot._util.regularize_files(files)
+    files = uproot._util.regularize_files(files, steps_allowed=False)
     decompression_executor, interpretation_executor = _regularize_executors(
         decompression_executor, interpretation_executor, None
     )
     library = uproot.interpretation.library._regularize_library(library)
 
     global_offset = 0
     for file_path, object_path in files:
@@ -339,15 +339,15 @@
     * :doc:`uproot.reading.open`: opens one file to read any of its objects.
     * :doc:`uproot.behaviors.TBranch.iterate`: iterates through chunks of
       contiguous entries in ``TTrees``.
     * :doc:`uproot.behaviors.TBranch.concatenate` (this function): returns a
       single concatenated array from ``TTrees``.
     * :doc:`uproot._dask.dask`: returns an unevaluated Dask array from ``TTrees``.
     """
-    files = uproot._util.regularize_files(files)
+    files = uproot._util.regularize_files(files, steps_allowed=False)
     decompression_executor, interpretation_executor = _regularize_executors(
         decompression_executor, interpretation_executor, None
     )
     library = uproot.interpretation.library._regularize_library(library)
 
     all_arrays = []
     global_start = 0
@@ -2486,15 +2486,15 @@
             interpretation.awkward_form(self.file)
         except uproot.interpretation.objects.CannotBeAwkward as err:
             raise ValueError(
                 """cannot produce Awkward Arrays for interpretation {} because
 
     {}
 
-instead, try library="np" instead of library="ak" or globally set uproot.default_library
+instead, try library="np" rather than library="ak" or globally set uproot.default_library
 
 in file {}
 in object {}""".format(
                     repr(interpretation),
                     err.because,
                     self.file.file_path,
                     self.object_path,
@@ -3233,12 +3233,12 @@
 
     def __setitem__(self, where, what):
         self.dict[where] = what
 
     def __delitem__(self, where):
         del self.dict[where]
 
-    def __iter__(self, where):
+    def __iter__(self):
         yield from self.dict
 
     def __len__(self):
         return len(self.dict)
```

### Comparing `uproot-5.0.7/src/uproot/behaviors/TBranchElement.py` & `uproot-5.0.8/src/uproot/behaviors/TBranchElement.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/behaviors/TGraph.py` & `uproot-5.0.8/src/uproot/behaviors/TGraph.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/behaviors/TGraphAsymmErrors.py` & `uproot-5.0.8/src/uproot/behaviors/TGraphAsymmErrors.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/behaviors/TH1.py` & `uproot-5.0.8/src/uproot/behaviors/TH1.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 def _boost_axis(axis, metadata):
     boost_histogram = uproot.extras.boost_histogram()
 
     fNbins = axis.member("fNbins")
     fXbins = axis.member("fXbins", none_if_missing=True)
 
-    if axis.member("fLabels") is not None:
-        fLabels = axis.member("fLabels")
+    fLabels = axis.member("fLabels", none_if_missing=True)
+    if fLabels is not None:
         try:
             labels = [int(x) for x in fLabels]
             category_cls = boost_histogram.axis.IntCategory
         except ValueError:
             labels = [str(x) for x in fLabels]
             category_cls = boost_histogram.axis.StrCategory
         out = category_cls(labels)
```

### Comparing `uproot-5.0.7/src/uproot/behaviors/TH2.py` & `uproot-5.0.8/src/uproot/behaviors/TH2.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/behaviors/TH2Poly.py` & `uproot-5.0.8/src/uproot/behaviors/TH2Poly.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/behaviors/TH3.py` & `uproot-5.0.8/src/uproot/behaviors/TH3.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/behaviors/TParameter.py` & `uproot-5.0.8/src/uproot/behaviors/TParameter.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/behaviors/TProfile.py` & `uproot-5.0.8/src/uproot/behaviors/TProfile.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/behaviors/TProfile2D.py` & `uproot-5.0.8/src/uproot/behaviors/TProfile2D.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/behaviors/TProfile3D.py` & `uproot-5.0.8/src/uproot/behaviors/TProfile3D.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/behaviors/TTree.py` & `uproot-5.0.8/src/uproot/behaviors/TTree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/behaviors/__init__.py` & `uproot-5.0.8/src/uproot/behaviors/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/interpretation/__init__.py` & `uproot-5.0.8/src/uproot/interpretation/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/interpretation/grouped.py` & `uproot-5.0.8/src/uproot/interpretation/grouped.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/interpretation/identify.py` & `uproot-5.0.8/src/uproot/interpretation/identify.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/interpretation/jagged.py` & `uproot-5.0.8/src/uproot/interpretation/jagged.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/interpretation/library.py` & `uproot-5.0.8/src/uproot/interpretation/library.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/interpretation/numerical.py` & `uproot-5.0.8/src/uproot/interpretation/numerical.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/interpretation/objects.py` & `uproot-5.0.8/src/uproot/interpretation/objects.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/interpretation/strings.py` & `uproot-5.0.8/src/uproot/interpretation/strings.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/language/__init__.py` & `uproot-5.0.8/src/uproot/language/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/language/python.py` & `uproot-5.0.8/src/uproot/language/python.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/RNTuple.py` & `uproot-5.0.8/src/uproot/models/RNTuple.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TArray.py` & `uproot-5.0.8/src/uproot/models/TArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TAtt.py` & `uproot-5.0.8/src/uproot/models/TAtt.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,14 +522,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -675,14 +676,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"),
                 file,
                 context,
```

### Comparing `uproot-5.0.7/src/uproot/models/TBasket.py` & `uproot-5.0.8/src/uproot/models/TBasket.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TBranch.py` & `uproot-5.0.8/src/uproot/models/TBranch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TClonesArray.py` & `uproot-5.0.8/src/uproot/models/TClonesArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TDatime.py` & `uproot-5.0.8/src/uproot/models/TDatime.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TGraph.py` & `uproot-5.0.8/src/uproot/models/TGraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,14 +245,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import ListOffsetForm, RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -451,14 +452,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import ListOffsetForm, RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -662,14 +664,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import ListOffsetForm, RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
```

### Comparing `uproot-5.0.7/src/uproot/models/TH.py` & `uproot-5.0.8/src/uproot/models/TH.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,14 +334,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -810,14 +811,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import ListOffsetForm, RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -1115,14 +1117,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -1324,14 +1327,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -1513,14 +1517,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -1675,14 +1680,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -1832,14 +1838,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -1989,14 +1996,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -2151,14 +2159,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -2313,14 +2322,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -2476,14 +2486,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -2634,14 +2645,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -2797,14 +2809,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -2960,14 +2973,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -3123,14 +3137,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -3287,14 +3302,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -3446,14 +3462,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -3610,14 +3627,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -3774,14 +3792,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -3974,14 +3993,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -4213,14 +4233,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
@@ -4454,14 +4475,15 @@
     def awkward_form(cls, file, context):
         from awkward.forms import RecordForm
 
         if cls in context["breadcrumbs"]:
             raise uproot.interpretation.objects.CannotBeAwkward(
                 "classes that can contain members of the same type cannot be Awkward Arrays because the depth of instances is unbounded"
             )
+        context = context.copy()
         context["breadcrumbs"] = context["breadcrumbs"] + (cls,)
         contents = {}
         if context["header"]:
             contents["@num_bytes"] = uproot._util.awkward_form(
                 numpy.dtype("u4"), file, context
             )
             contents["@instance_version"] = uproot._util.awkward_form(
```

### Comparing `uproot-5.0.7/src/uproot/models/THashList.py` & `uproot-5.0.8/src/uproot/models/THashList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TLeaf.py` & `uproot-5.0.8/src/uproot/models/TLeaf.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TList.py` & `uproot-5.0.8/src/uproot/models/TList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TMatrixT.py` & `uproot-5.0.8/src/uproot/models/TMatrixT.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TNamed.py` & `uproot-5.0.8/src/uproot/models/TNamed.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TObjArray.py` & `uproot-5.0.8/src/uproot/models/TObjArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TObjString.py` & `uproot-5.0.8/src/uproot/models/TObjString.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TObject.py` & `uproot-5.0.8/src/uproot/models/TObject.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TRef.py` & `uproot-5.0.8/src/uproot/models/TRef.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TString.py` & `uproot-5.0.8/src/uproot/models/TString.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TTable.py` & `uproot-5.0.8/src/uproot/models/TTable.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/models/TTree.py` & `uproot-5.0.8/src/uproot/models/TTree.py`

 * *Files 0% similar despite different names*

```diff
@@ -955,15 +955,15 @@
             ``"http://where/what.root:ttree"``,
             ``"https://username:password@where/secure.root:ttree"``,
             ``"rel/file.root:tdirectory/ttree"``, iterables of the previous examples.
 
     Returns an iterator over the number of entries over each TTree in the input.
     This is a shortcut method and reads lesser data than normal file opening.
     """
-    paths2 = uproot._util.regularize_files(paths)
+    paths2 = uproot._util.regularize_files(paths, steps_allowed=False)
 
     if isinstance(paths, dict):
         paths = list(paths.items())
     elif not uproot._util.isstr(paths):
         paths = [(uproot._util.file_object_path_split(path)) for path in paths]
     else:
         paths = [uproot._util.file_object_path_split(paths)]
```

### Comparing `uproot-5.0.7/src/uproot/models/__init__.py` & `uproot-5.0.8/src/uproot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/sink/__init__.py` & `uproot-5.0.8/src/uproot/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/sink/file.py` & `uproot-5.0.8/src/uproot/sink/file.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/source/__init__.py` & `uproot-5.0.8/src/uproot/source/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/source/chunk.py` & `uproot-5.0.8/src/uproot/source/chunk.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/source/cursor.py` & `uproot-5.0.8/src/uproot/source/cursor.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/source/file.py` & `uproot-5.0.8/src/uproot/source/file.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/source/futures.py` & `uproot-5.0.8/src/uproot/source/futures.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/source/http.py` & `uproot-5.0.8/src/uproot/source/http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/source/object.py` & `uproot-5.0.8/src/uproot/source/object.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/source/xrootd.py` & `uproot-5.0.8/src/uproot/source/xrootd.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/writing/__init__.py` & `uproot-5.0.8/src/uproot/writing/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/writing/_cascade.py` & `uproot-5.0.8/src/uproot/writing/_cascade.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/writing/_cascadentuple.py` & `uproot-5.0.8/src/uproot/writing/_cascadentuple.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/writing/_cascadetree.py` & `uproot-5.0.8/src/uproot/writing/_cascadetree.py`

 * *Files 1% similar despite different names*

```diff
@@ -979,16 +979,44 @@
             # single TLeaf
             leaf_name = datum["fName"].encode(errors="surrogateescape")
             leaf_title = (datum["fName"] + dims).encode(errors="surrogateescape")
             leaf_name_length = (1 if len(leaf_name) < 255 else 5) + len(leaf_name)
             leaf_title_length = (1 if len(leaf_title) < 255 else 5) + len(leaf_title)
 
             leaf_header = numpy.array(
-                [64, 0, 0, 76, 0, 1, 64, 0, 0, 54, 0, 2, 64, 0]
-                + [0, 30, 0, 1, 0, 1, 0, 0, 0, 0, 3, 0, 0, 0],
+                [
+                    64,
+                    0,
+                    0,
+                    76,
+                    0,
+                    1,
+                    64,
+                    0,
+                    0,
+                    54,
+                    0,
+                    2,
+                    64,
+                    0,
+                    0,
+                    30,
+                    0,
+                    1,
+                    0,
+                    1,
+                    0,
+                    0,
+                    0,
+                    0,
+                    3,
+                    0,
+                    0,
+                    0,
+                ],
                 numpy.uint8,
             )
             tmp = leaf_header[0:4].view(">u4")
             tmp[:] = (
                 numpy.uint32(
                     42 + leaf_name_length + leaf_title_length + special_struct.size
                 )
```

### Comparing `uproot-5.0.7/src/uproot/writing/identify.py` & `uproot-5.0.8/src/uproot/writing/identify.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/src/uproot/writing/writable.py` & `uproot-5.0.8/src/uproot/writing/writable.py`

 * *Files 0% similar despite different names*

```diff
@@ -530,15 +530,15 @@
 
     @property
     def object_path(self):
         """
         Path of directory names to this subdirectory as a single string, delimited
         by slashes.
         """
-        return "/".join(("", *self._path) + ("",)).replace("//", "/")
+        return "/".join(("", *self._path, "")).replace("//", "/")
 
     @property
     def file_path(self):
         """
         Filesystem path of the open file, or None if using a file-like object.
         """
         return self._file.file_path
@@ -1647,15 +1647,15 @@
 
     @property
     def object_path(self):
         """
         Path of directory names to this TTree as a single string, delimited by
         slashes.
         """
-        return "/".join(("", *self._path) + ("",)).replace("//", "/")
+        return "/".join(("", *self._path, "")).replace("//", "/")
 
     @property
     def file_path(self):
         """
         Filesystem path of the open file, or None if using a file-like object.
         """
         return self._file.file_path
@@ -1990,15 +1990,15 @@
 
     @property
     def object_path(self):
         """
         Path of directory names to this RNTuple as a single string, delimited by
         slashes.
         """
-        return "/".join(("", *self._path) + ("",)).replace("//", "/")
+        return "/".join(("", *self._path, "")).replace("//", "/")
 
     @property
     def file_path(self):
         """
         Filesystem path of the open file, or None if using a file-like object.
         """
         return self._file.file_path
```

### Comparing `uproot-5.0.7/tests/test_0001-source-class.py` & `uproot-5.0.8/tests/test_0001-source-class.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0006-notify-when-downloaded.py` & `uproot-5.0.8/tests/test_0006-notify-when-downloaded.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0007-single-chunk-interface.py` & `uproot-5.0.8/tests/test_0007-single-chunk-interface.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0008-start-interpretation.py` & `uproot-5.0.8/tests/test_0008-start-interpretation.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0009-nested-directories.py` & `uproot-5.0.8/tests/test_0009-nested-directories.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0010-start-streamers.py` & `uproot-5.0.8/tests/test_0010-start-streamers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0011-generate-classes-from-streamers.py` & `uproot-5.0.8/tests/test_0011-generate-classes-from-streamers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0013-rntuple-anchor.py` & `uproot-5.0.8/tests/test_0013-rntuple-anchor.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0014-all-ttree-versions.py` & `uproot-5.0.8/tests/test_0014-all-ttree-versions.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0016-interpretations.py` & `uproot-5.0.8/tests/test_0016-interpretations.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0017-multi-basket-multi-branch-fetch.py` & `uproot-5.0.8/tests/test_0017-multi-basket-multi-branch-fetch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0018-array-fetching-interface.py` & `uproot-5.0.8/tests/test_0018-array-fetching-interface.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0022-number-of-branches.py` & `uproot-5.0.8/tests/test_0022-number-of-branches.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0023-more-interpretations-1.py` & `uproot-5.0.8/tests/test_0023-more-interpretations-1.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0023-ttree-versions.py` & `uproot-5.0.8/tests/test_0023-ttree-versions.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0029-more-string-types.py` & `uproot-5.0.8/tests/test_0029-more-string-types.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0031-test-stl-containers.py` & `uproot-5.0.8/tests/test_0031-test-stl-containers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0033-more-interpretations-2.py` & `uproot-5.0.8/tests/test_0033-more-interpretations-2.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0034-generic-objects-in-ttrees.py` & `uproot-5.0.8/tests/test_0034-generic-objects-in-ttrees.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0035-datatype-generality.py` & `uproot-5.0.8/tests/test_0035-datatype-generality.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0038-memberwise-serialization.py` & `uproot-5.0.8/tests/test_0038-memberwise-serialization.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0043-iterate-function.py` & `uproot-5.0.8/tests/test_0043-iterate-function.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0044-concatenate-function.py` & `uproot-5.0.8/tests/test_0044-concatenate-function.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0046-histograms-bh-hist.py` & `uproot-5.0.8/tests/test_0046-histograms-bh-hist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0053-parents-should-not-be-bases.py` & `uproot-5.0.8/tests/test_0053-parents-should-not-be-bases.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0058-detach-model-objects-from-files.py` & `uproot-5.0.8/tests/test_0058-detach-model-objects-from-files.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0067-common-entry-offsets.py` & `uproot-5.0.8/tests/test_0067-common-entry-offsets.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0081-dont-parse-colons.py` & `uproot-5.0.8/tests/test_0081-dont-parse-colons.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0087-memberwise-splitting-not-implemented-messages.py` & `uproot-5.0.8/tests/test_0087-memberwise-splitting-not-implemented-messages.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0088-read-with-http.py` & `uproot-5.0.8/tests/test_0088-read-with-http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0099-read-from-file-object.py` & `uproot-5.0.8/tests/test_0099-read-from-file-object.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0112-fix-pandas-with-cut.py` & `uproot-5.0.8/tests/test_0112-fix-pandas-with-cut.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0118-fix-name-fetch-again.py` & `uproot-5.0.8/tests/test_0118-fix-name-fetch-again.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0167-use-the-common-histogram-interface.py` & `uproot-5.0.8/tests/test_0167-use-the-common-histogram-interface.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0173-empty-and-multiprocessing-bugs.py` & `uproot-5.0.8/tests/test_0173-empty-and-multiprocessing-bugs.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0182-complain-about-missing-files.py` & `uproot-5.0.8/tests/test_0182-complain-about-missing-files.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0220-contiguous-byte-ranges-in-http.py` & `uproot-5.0.8/tests/test_0220-contiguous-byte-ranges-in-http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0228_read-TProfiles.py` & `uproot-5.0.8/tests/test_0228_read-TProfiles.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0240-read_TGraphAsymmErrors.py` & `uproot-5.0.8/tests/test_0240-read_TGraphAsymmErrors.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0278-specializations-for-TParameter.py` & `uproot-5.0.8/tests/test_0278-specializations-for-TParameter.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0302-pickle.py` & `uproot-5.0.8/tests/test_0302-pickle.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0303-empty-jagged-array.py` & `uproot-5.0.8/tests/test_0303-empty-jagged-array.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0320-start-working-on-ROOT-writing.py` & `uproot-5.0.8/tests/test_0320-start-working-on-ROOT-writing.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0322-writablefile-infrastructure.py` & `uproot-5.0.8/tests/test_0322-writablefile-infrastructure.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0325-fix-windows-file-uris.py` & `uproot-5.0.8/tests/test_0325-fix-windows-file-uris.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0329-update-existing-root-files.py` & `uproot-5.0.8/tests/test_0329-update-existing-root-files.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0341-manipulate-streamer-info.py` & `uproot-5.0.8/tests/test_0341-manipulate-streamer-info.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0344-writabledirectory-can-read.py` & `uproot-5.0.8/tests/test_0344-writabledirectory-can-read.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0345-bulk-copy-method.py` & `uproot-5.0.8/tests/test_0345-bulk-copy-method.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0349-write-TObjString.py` & `uproot-5.0.8/tests/test_0349-write-TObjString.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0350-read-RooCurve-RooHist.py` & `uproot-5.0.8/tests/test_0350-read-RooCurve-RooHist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0351-write-TList.py` & `uproot-5.0.8/tests/test_0351-write-TList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0352-write-THashList.py` & `uproot-5.0.8/tests/test_0352-write-THashList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0384-move-behavior_of-and-fix-383.py` & `uproot-5.0.8/tests/test_0384-move-behavior_of-and-fix-383.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0398-dimensions-in-leaflist.py` & `uproot-5.0.8/tests/test_0398-dimensions-in-leaflist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0405-write-a-histogram.py` & `uproot-5.0.8/tests/test_0405-write-a-histogram.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0406-write-a-ttree.py` & `uproot-5.0.8/tests/test_0406-write-a-ttree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0407-read-TDatime.py` & `uproot-5.0.8/tests/test_0407-read-TDatime.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0412-write-multidimensional-numpy-to-ttree.py` & `uproot-5.0.8/tests/test_0412-write-multidimensional-numpy-to-ttree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0414-write-jagged-arrays.py` & `uproot-5.0.8/tests/test_0414-write-jagged-arrays.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0416-writing-compressed-data.py` & `uproot-5.0.8/tests/test_0416-writing-compressed-data.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0418-read-TTable.py` & `uproot-5.0.8/tests/test_0418-read-TTable.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0420-pyroot-uproot-interoperability.py` & `uproot-5.0.8/tests/test_0420-pyroot-uproot-interoperability.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0422-hist-integration.py` & `uproot-5.0.8/tests/test_0422-hist-integration.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0438-TClonesArray-is-not-AsGrouped.py` & `uproot-5.0.8/tests/test_0438-TClonesArray-is-not-AsGrouped.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0442-regular-TClonesArray.py` & `uproot-5.0.8/tests/test_0442-regular-TClonesArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0472-tstreamerinfo-for-ttree.py` & `uproot-5.0.8/tests/test_0472-tstreamerinfo-for-ttree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0475-remember-to-update-freesegments.py` & `uproot-5.0.8/tests/test_0475-remember-to-update-freesegments.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0487-implement-asdtypeinplace.py` & `uproot-5.0.8/tests/test_0487-implement-asdtypeinplace.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0498-create-leaf-branch-in-extend.py` & `uproot-5.0.8/tests/test_0498-create-leaf-branch-in-extend.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0576-unicode-in-names.py` & `uproot-5.0.8/tests/test_0576-unicode-in-names.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0578-dask-for-numpy.py` & `uproot-5.0.8/tests/test_0578-dask-for-numpy.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0580-round-trip-for-no-flow-histograms.py` & `uproot-5.0.8/tests/test_0580-round-trip-for-no-flow-histograms.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0589-explicitly-interpret-RVec-type.py` & `uproot-5.0.8/tests/test_0589-explicitly-interpret-RVec-type.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0609-num-enteries-func.py` & `uproot-5.0.8/tests/test_0609-num-enteries-func.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0610-awkward-form.py` & `uproot-5.0.8/tests/test_0610-awkward-form.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0630-rntuple-basics.py` & `uproot-5.0.8/tests/test_0630-rntuple-basics.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0637-setup-tests-for-AwkwardForth.py` & `uproot-5.0.8/tests/test_0637-setup-tests-for-AwkwardForth.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0643-reading-vector-pair-TLorentzVector-int.py` & `uproot-5.0.8/tests/test_0643-reading-vector-pair-TLorentzVector-int.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0651-implement-transformed-axis.py` & `uproot-5.0.8/tests/test_0651-implement-transformed-axis.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0652_dask-for-awkward.py` & `uproot-5.0.8/tests/test_0652_dask-for-awkward.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0662-rntuple-stl-containers.py` & `uproot-5.0.8/tests/test_0662-rntuple-stl-containers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0700-dask-empty-arrays.py` & `uproot-5.0.8/tests/test_0700-dask-empty-arrays.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0705-rntuple-writing-metadata.py` & `uproot-5.0.8/tests/test_0705-rntuple-writing-metadata.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0755-dask-awkward-column-projection.py` & `uproot-5.0.8/tests/test_0755-dask-awkward-column-projection.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0791-protect-uproot-project_columns-from-dask-node-names.py` & `uproot-5.0.8/tests/test_0791-protect-uproot-project_columns-from-dask-node-names.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0798_DAOD_PHYSLITE.py` & `uproot-5.0.8/tests/test_0798_DAOD_PHYSLITE.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0808-fix_awkward_form_for_AsStridedObjects.py` & `uproot-5.0.8/tests/test_0808-fix_awkward_form_for_AsStridedObjects.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0816-separate-AwkwardForth-machines-by-TBranch.py` & `uproot-5.0.8/tests/test_0816-separate-AwkwardForth-machines-by-TBranch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0832-ak_add_doc-should-also-add-to-typetracer.py` & `uproot-5.0.8/tests/test_0832-ak_add_doc-should-also-add-to-typetracer.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0840-support-tleafG.py` & `uproot-5.0.8/tests/test_0840-support-tleafG.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0841-fix-814.py` & `uproot-5.0.8/tests/test_0841-fix-814.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0844-fix-delete-hist-from-root.py` & `uproot-5.0.8/tests/test_0844-fix-delete-hist-from-root.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/test_0876-uproot-dask-blind-steps.py` & `uproot-5.0.8/tests/test_0876-uproot-dask-blind-steps.py`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/tests/samples/h_dynamic.pkl` & `uproot-5.0.8/tests/samples/h_dynamic.pkl`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/.gitignore` & `uproot-5.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/LICENSE` & `uproot-5.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/README.md` & `uproot-5.0.8/README.md`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/pyproject.toml` & `uproot-5.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uproot-5.0.7/PKG-INFO` & `uproot-5.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uproot
-Version: 5.0.7
+Version: 5.0.8
 Summary: ROOT I/O in pure Python and NumPy.
 Project-URL: Download, https://github.com/scikit-hep/uproot5/releases
 Project-URL: Homepage, https://github.com/scikit-hep/uproot5
 Author-email: Jim Pivarski <pivarski@princeton.edu>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

