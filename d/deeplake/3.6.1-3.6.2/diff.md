# Comparing `tmp/deeplake-3.6.1.tar.gz` & `tmp/deeplake-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.6.1.tar", last modified: Thu Jun  8 04:32:11 2023, max compression
+gzip compressed data, was "deeplake-3.6.2.tar", last modified: Fri Jun  9 15:01:52 2023, max compression
```

## Comparing `deeplake-3.6.1.tar` & `deeplake-3.6.2.tar`

### file list

```diff
@@ -1,398 +1,398 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.542436 deeplake-3.6.1/
--rw-r--r--   0 root         (0) root         (0)    15975 2023-06-08 04:31:41.000000 deeplake-3.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-08 04:31:41.000000 deeplake-3.6.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    26080 2023-06-08 04:32:11.542436 deeplake-3.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    25351 2023-06-08 04:31:41.000000 deeplake-3.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.512436 deeplake-3.6.1/deeplake/
--rw-r--r--   0 root         (0) root         (0)     2662 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.512436 deeplake-3.6.1/deeplake/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    96139 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4693 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/info.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/link.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/read.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/api/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 root         (0) root         (0)    85001 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     6968 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 root         (0) root         (0)     1797 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_events.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)    23489 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_link.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_linking.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 root         (0) root         (0)     7900 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_none.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 root         (0) root         (0)     5680 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 root         (0) root         (0)    10559 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_pop.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)    17730 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 root         (0) root         (0)     8477 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_reset.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_text.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 root         (0) root         (0)     7499 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_video.py
--rw-r--r--   0 root         (0) root         (0)     4153 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tests/test_views.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/api/tiled.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/auto/structured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/structured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/structured/base.py
--rw-r--r--   0 root         (0) root         (0)     6666 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/auto/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7975 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 root         (0) root         (0)    12440 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     5371 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/auto/unstructured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/auto/unstructured/coco/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 root         (0) root         (0)     6693 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4514 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 root         (0) root         (0)    12937 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/cli/auth.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/cli/commands.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/cli/test_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19099 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/client/config.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/client/log.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/client/test_client.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/client/utils.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/compression.py
--rw-r--r--   0 root         (0) root         (0)     7357 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/core/
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/core/chunk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/chunk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24150 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 root         (0) root         (0)    25311 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 root         (0) root         (0)     5446 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)   113335 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)    39478 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/compression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/core/compute/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/compute/process.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/compute/provider.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/compute/ray.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/compute/serial.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/compute/thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/core/dataset/
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171173 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    14834 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11965 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/dataset/deeplake_query_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5265 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/dataset/deeplake_query_tensor.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 root         (0) root         (0)     4769 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/core/index/
--rw-r--r--   0 root         (0) root         (0)      138 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17507 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/index/index.py
--rw-r--r--   0 root         (0) root         (0)    19800 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/io.py
--rw-r--r--   0 root         (0) root         (0)     4121 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/ipc.py
--rw-r--r--   0 root         (0) root         (0)    12418 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/link_creds.py
--rw-r--r--   0 root         (0) root         (0)    15995 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/linked_sample.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 root         (0) root         (0)     8835 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/core/meta/
--rw-r--r--   0 root         (0) root         (0)       97 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/core/meta/encode/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25591 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 root         (0) root         (0)    13495 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.522436 deeplake-3.6.1/deeplake/core/meta/encode/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     7515 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/meta.py
--rw-r--r--   0 root         (0) root         (0)    13344 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/partial_reader.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/partial_sample.py
--rw-r--r--   0 root         (0) root         (0)     5269 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/polygon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/core/query/
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/query/autocomplete.py
--rw-r--r--   0 root         (0) root         (0)    14326 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/query/filter.py
--rw-r--r--   0 root         (0) root         (0)     8905 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/query/query.py
--rw-r--r--   0 root         (0) root         (0)    20658 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/sample.py
--rw-r--r--   0 root         (0) root         (0)    22849 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/core/storage/
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13705 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/storage/azure.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 root         (0) root         (0)    19080 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/storage/gcs.py
--rw-r--r--   0 root         (0) root         (0)    13053 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/storage/google_drive.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/storage/local.py
--rw-r--r--   0 root         (0) root         (0)    19492 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/storage/memory.py
--rw-r--r--   0 root         (0) root         (0)     7111 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/storage/provider.py
--rw-r--r--   0 root         (0) root         (0)    25799 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/storage/s3.py
--rw-r--r--   0 root         (0) root         (0)    50140 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tensor.py
--rw-r--r--   0 root         (0) root         (0)     7485 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tensor_link.py
--rw-r--r--   0 root         (0) root         (0)     5152 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/core/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tests/test_compression.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tests/test_compute.py
--rw-r--r--   0 root         (0) root         (0)    12807 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tests/test_deeplake_indra_dataset.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)     4312 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tests/test_locking.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tests/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/core/tiling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tiling/serialize.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/core/transform/
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/transform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51556 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/transform/test_transform.py
--rw-r--r--   0 root         (0) root         (0)    29645 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/transform/transform.py
--rw-r--r--   0 root         (0) root         (0)     5860 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/core/vectorstore/
--rw-r--r--   0 root         (0) root         (0)      611 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24036 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/deeplake_vectorstore.py
--rw-r--r--   0 root         (0) root         (0)    29778 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/test_deeplake_vectorstore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/dataset/
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11363 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    10090 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/filter/
--rw-r--r--   0 root         (0) root         (0)      286 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/filter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3212 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/filter/filter.py
--rw-r--r--   0 root         (0) root         (0)     3542 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/filter/test_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/indra/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/indra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4510 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/indra/query.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/indra/test_indra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
--rw-r--r--   0 root         (0) root         (0)      275 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/indra/vector_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/ingestion/
--rw-r--r--   0 root         (0) root         (0)       93 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6455 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
--rw-r--r--   0 root         (0) root         (0)     5014 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/python/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/python/vector_search.py
--rw-r--r--   0 root         (0) root         (0)     8966 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/utils.py
--rw-r--r--   0 root         (0) root         (0)     2667 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/vectorstore/vector_search/vector_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/core/version_control/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/version_control/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 root         (0) root         (0)     4828 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 root         (0) root         (0)    19869 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 root         (0) root         (0)    84800 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/enterprise/
--rw-r--r--   0 root         (0) root         (0)      257 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/enterprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7381 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 root         (0) root         (0)    29584 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/enterprise/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 root         (0) root         (0)    25897 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 root         (0) root         (0)     1622 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/enterprise/test_query.py
--rw-r--r--   0 root         (0) root         (0)    22353 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/enterprise/util.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/hooks.py
--rw-r--r--   0 root         (0) root         (0)     5050 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/htype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/integrations/
--rw-r--r--   0 root         (0) root         (0)       99 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/integrations/huggingface/
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5503 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/integrations/mmdet/
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62754 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 root         (0) root         (0)     4739 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/integrations/pytorch/
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9772 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 root         (0) root         (0)     7140 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 root         (0) root         (0)     6919 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/integrations/tf/
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/tf/common.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/integrations/wandb/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/requirements/
--rw-r--r--   0 root         (0) root         (0)      476 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/requirements/common.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/requirements/plugins.txt
--rw-r--r--   0 root         (0) root         (0)      304 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/requirements/tests.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.532436 deeplake-3.6.1/deeplake/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/tests/client_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     4266 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     4018 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 root         (0) root         (0)    16165 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/tests/path_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2735 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.542436 deeplake-3.6.1/deeplake/util/
--rw-r--r--   0 root         (0) root         (0)       86 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/access_method.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/agreement.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/array_list.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/auto.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/bugout_reporter.py
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/bugout_token.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/cache_chain.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/casting.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/check_installation.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/check_latest_version.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     4597 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/class_label.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/compression.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/compute.py
--rw-r--r--   0 root         (0) root         (0)     5404 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/dataset.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/delete_entry.py
--rw-r--r--   0 root         (0) root         (0)    15912 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/diff.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/downsample.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/empty_sample.py
--rw-r--r--   0 root         (0) root         (0)    15682 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/encoder.py
--rw-r--r--   0 root         (0) root         (0)    34711 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/exif.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/from_tfds.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/generate_id.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/hash.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/htype.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/image.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/invalid_view_op.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/iteration_warning.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/join_chunks.py
--rw-r--r--   0 root         (0) root         (0)     6422 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/json.py
--rw-r--r--   0 root         (0) root         (0)     7261 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/keys.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/link.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/logging.py
--rw-r--r--   0 root         (0) root         (0)    37497 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/merge.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/modified.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/notebook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.542436 deeplake-3.6.1/deeplake/util/object_3d/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 root         (0) root         (0)     3221 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 root         (0) root         (0)    10213 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 root         (0) root         (0)     7187 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 root         (0) root         (0)     3986 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/path.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/pretty_print.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/remove_cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     4204 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/spinner.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/split.py
--rw-r--r--   0 root         (0) root         (0)     8435 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/storage.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/tag.py
--rw-r--r--   0 root         (0) root         (0)     1390 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/tensor_db.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.542436 deeplake-3.6.1/deeplake/util/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/tests/test_auto.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/tests/test_read.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/tests/test_tensor_db.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 root         (0) root         (0)      276 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/threading.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/token.py
--rw-r--r--   0 root         (0) root         (0)    25235 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/transform.py
--rw-r--r--   0 root         (0) root         (0)    31615 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/version_control.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/video.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/util/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.542436 deeplake-3.6.1/deeplake/visualizer/
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/visualizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6466 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-06-08 04:31:41.000000 deeplake-3.6.1/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:32:11.512436 deeplake-3.6.1/deeplake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    26080 2023-06-08 04:32:11.000000 deeplake-3.6.1/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12677 2023-06-08 04:32:11.000000 deeplake-3.6.1/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 04:32:11.000000 deeplake-3.6.1/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-08 04:32:11.000000 deeplake-3.6.1/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 04:32:11.000000 deeplake-3.6.1/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1075 2023-06-08 04:32:11.000000 deeplake-3.6.1/deeplake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-08 04:32:11.000000 deeplake-3.6.1/deeplake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-06-08 04:32:11.542436 deeplake-3.6.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3357 2023-06-08 04:31:41.000000 deeplake-3.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.265233 deeplake-3.6.2/
+-rw-r--r--   0 root         (0) root         (0)    15975 2023-06-09 15:00:23.000000 deeplake-3.6.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-09 15:00:23.000000 deeplake-3.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    26080 2023-06-09 15:01:52.265233 deeplake-3.6.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25351 2023-06-09 15:00:23.000000 deeplake-3.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.232733 deeplake-3.6.2/deeplake/
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.232733 deeplake-3.6.2/deeplake/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    96883 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/info.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/link.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.232733 deeplake-3.6.2/deeplake/api/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    85180 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_events.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)    25706 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 root         (0) root         (0)     7900 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_none.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 root         (0) root         (0)    10559 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)    18863 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_text.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 root         (0) root         (0)     7499 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_video.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_views.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tiled.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.232733 deeplake-3.6.2/deeplake/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.232733 deeplake-3.6.2/deeplake/auto/structured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/structured/base.py
+-rw-r--r--   0 root         (0) root         (0)     6666 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.232733 deeplake-3.6.2/deeplake/auto/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7975 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 root         (0) root         (0)    12440 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/auto/unstructured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4514 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/cli/auth.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/cli/commands.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/cli/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19099 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/client/config.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/client/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/compression.py
+-rw-r--r--   0 root         (0) root         (0)     7357 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/chunk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24150 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)   113519 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)    39478 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/compression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/compute/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/compute/process.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/compute/provider.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/compute/ray.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/compute/serial.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/compute/thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/dataset/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171829 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    15422 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11965 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/dataset/deeplake_query_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5265 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/dataset/deeplake_query_tensor.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/index/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/index/index.py
+-rw-r--r--   0 root         (0) root         (0)    19800 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/io.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    13074 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/link_creds.py
+-rw-r--r--   0 root         (0) root         (0)    15995 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/linked_sample.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/meta/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/meta/encode/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25591 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 root         (0) root         (0)    13495 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     7515 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/meta.py
+-rw-r--r--   0 root         (0) root         (0)    13344 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/partial_reader.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/partial_sample.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/polygon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/query/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)    14326 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/query/filter.py
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    20658 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/sample.py
+-rw-r--r--   0 root         (0) root         (0)    22849 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/storage/
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13705 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/azure.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 root         (0) root         (0)    19080 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/gcs.py
+-rw-r--r--   0 root         (0) root         (0)    13053 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/local.py
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/memory.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/provider.py
+-rw-r--r--   0 root         (0) root         (0)    25799 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/s3.py
+-rw-r--r--   0 root         (0) root         (0)    50140 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     7485 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tensor_link.py
+-rw-r--r--   0 root         (0) root         (0)     5152 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/test_deeplake_indra_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/tiling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/transform/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/transform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51556 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 root         (0) root         (0)    29645 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/transform/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5860 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/
+-rw-r--r--   0 root         (0) root         (0)      611 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24052 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/deeplake_vectorstore.py
+-rw-r--r--   0 root         (0) root         (0)    30075 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/test_deeplake_vectorstore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/dataset/
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11148 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    10090 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/filter/
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/filter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/filter/filter.py
+-rw-r--r--   0 root         (0) root         (0)     3542 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/filter/test_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4510 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/query.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/test_indra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6455 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
+-rw-r--r--   0 root         (0) root         (0)     5014 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     9551 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/version_control/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 root         (0) root         (0)    19869 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 root         (0) root         (0)    84800 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/enterprise/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 root         (0) root         (0)    29584 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 root         (0) root         (0)    25897 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/test_query.py
+-rw-r--r--   0 root         (0) root         (0)    22353 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/util.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/htype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/integrations/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/integrations/huggingface/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5503 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/integrations/mmdet/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62754 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/integrations/pytorch/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9862 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/integrations/tf/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/tf/common.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/integrations/wandb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/requirements/
+-rw-r--r--   0 root         (0) root         (0)      476 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/requirements/common.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/requirements/plugins.txt
+-rw-r--r--   0 root         (0) root         (0)      304 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/requirements/tests.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     4018 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)    16165 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.265233 deeplake-3.6.2/deeplake/util/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/access_method.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/agreement.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/array_list.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/auto.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/bugout_token.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/cache_chain.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/casting.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/check_installation.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/check_latest_version.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/class_label.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/compression.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/compute.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/delete_entry.py
+-rw-r--r--   0 root         (0) root         (0)    15912 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/diff.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/downsample.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/empty_sample.py
+-rw-r--r--   0 root         (0) root         (0)    15682 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    34773 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/exif.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/from_tfds.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/generate_id.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/hash.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/htype.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/image.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/iteration_warning.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/join_chunks.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/json.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/keys.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/link.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/logging.py
+-rw-r--r--   0 root         (0) root         (0)    37497 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/merge.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/modified.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.265233 deeplake-3.6.2/deeplake/util/object_3d/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/pretty_print.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/remove_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     4204 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/spinner.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/split.py
+-rw-r--r--   0 root         (0) root         (0)     8435 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/storage.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tensor_db.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.265233 deeplake-3.6.2/deeplake/util/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_read.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_tensor_db.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 root         (0) root         (0)      276 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/threading.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/token.py
+-rw-r--r--   0 root         (0) root         (0)    25235 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/transform.py
+-rw-r--r--   0 root         (0) root         (0)    31615 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/version_control.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/video.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.265233 deeplake-3.6.2/deeplake/visualizer/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/visualizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6466 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.232733 deeplake-3.6.2/deeplake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    26080 2023-06-09 15:01:52.000000 deeplake-3.6.2/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12677 2023-06-09 15:01:52.000000 deeplake-3.6.2/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 15:01:52.000000 deeplake-3.6.2/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-09 15:01:52.000000 deeplake-3.6.2/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 15:01:52.000000 deeplake-3.6.2/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-06-09 15:01:52.000000 deeplake-3.6.2/deeplake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-09 15:01:52.000000 deeplake-3.6.2/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-09 15:01:52.265233 deeplake-3.6.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-06-09 15:00:23.000000 deeplake-3.6.2/setup.py
```

### Comparing `deeplake-3.6.1/LICENSE` & `deeplake-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/PKG-INFO` & `deeplake-3.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.6.1
+Version: 3.6.2
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.6.1 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.6.2 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: azure
 Provides-Extra: dicom Provides-Extra: enterprise Provides-Extra: gcp Provides-
```

### Comparing `deeplake-3.6.1/README.md` & `deeplake-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/__init__.py` & `deeplake-3.6.2/deeplake/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "config",
     "delete",
     "copy",
     "rename",
 ]
 
 
-__version__ = "3.6.1"
+__version__ = "3.6.2"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
 deeplake_reporter.system_report(publish=True)
```

### Comparing `deeplake-3.6.1/deeplake/api/dataset.py` & `deeplake-3.6.2/deeplake/api/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     UserNotLoggedInException,
     TokenPermissionError,
     UnsupportedParameterException,
     DatasetCorruptError,
     CheckoutError,
     ReadOnlyModeError,
     LockedException,
+    BadRequestException,
 )
 from deeplake.util.storage import (
     get_storage_and_cache_chain,
     storage_provider_from_path,
 )
 from deeplake.util.compute import get_compute_provider
 from deeplake.util.remove_cache import get_base_storage
@@ -381,15 +382,14 @@
         Danger:
             Setting ``overwrite`` to ``True`` will delete all of your data if it exists! Be very careful when setting this parameter.
         """
         path, address = process_dataset_path(path)
 
         if org_id is not None and get_path_type(path) != "local":
             raise ValueError("org_id parameter can only be used with local datasets")
-
         db_engine = parse_runtime_parameters(path, runtime)["tensor_db"]
 
         if address:
             raise ValueError(
                 "deeplake.empty does not accept version address in the dataset path."
             )
 
@@ -527,14 +527,15 @@
             UserNotLoggedInException: When user is not logged in
             InvalidTokenException: If the specified toke is invalid
             TokenPermissionError: When there are permission or other errors related to token
             CheckoutError: If version address specified in the path cannot be found
             DatasetCorruptError: If loading the dataset failed due to corruption and ``reset`` is not ``True``
             ReadOnlyModeError: If reset is attempted in read-only mode
             LockedException: When attempting to open a dataset for writing when it is locked by another machine
+            ValueError: If ``org_id`` is specified for a non-local dataset
             Exception: Re-raises caught exception if reset cannot fix the issue
             ValueError: If the org id is provided but the dataset is not local
 
         Warning:
             Setting ``access_method`` to download will overwrite the local copy of the dataset if it was previously downloaded.
 
         Note:
@@ -845,15 +846,15 @@
             verbose (bool): If True, logs will be printed. Defaults to ``True``.
 
 
         Returns:
             Dataset: New dataset object.
 
         Raises:
-            ValueError: If the org id is provided but the dataset is not local
+            ValueError: If ``org_id`` is specified for a non-local dataset.
         """
         if isinstance(dest, Dataset):
             path = dest.path
         else:
             path = dest
 
         if org_id is not None and get_path_type(path) != "local":
@@ -1288,23 +1289,36 @@
 
         Returns:
             Dataset: The connected Deep Lake dataset.
 
         Raises:
             InvalidSourcePathError: If the ``src_path`` is not a valid s3, gcs or azure path.
             InvalidDestinationPathError: If ``dest_path``, or ``org_id`` and ``ds_name`` do not form a valid Deep Lake path.
+            TokenPermissionError: If the user does not have permission to create a dataset in the specified organization.
         """
-        path = connect_dataset_entry(
-            src_path=src_path,
-            creds_key=creds_key,
-            dest_path=dest_path,
-            org_id=org_id,
-            ds_name=ds_name,
-            token=token,
-        )
+        try:
+            path = connect_dataset_entry(
+                src_path=src_path,
+                creds_key=creds_key,
+                dest_path=dest_path,
+                org_id=org_id,
+                ds_name=ds_name,
+                token=token,
+            )
+        except BadRequestException:
+            check_param = "organization id" if org_id else "dataset path"
+            raise TokenPermissionError(
+                "You do not have permission to create a dataset in the specified "
+                + check_param
+                + "."
+                + " Please check the "
+                + check_param
+                + " and make sure"
+                + "that you have sufficient permissions to the organization."
+            )
         return deeplake.dataset(path, token=token, verbose=False)
 
     @staticmethod
     def ingest_coco(
         images_directory: Union[str, pathlib.Path],
         annotation_files: Union[str, pathlib.Path, List[str]],
         dest: Union[str, pathlib.Path],
```

### Comparing `deeplake-3.6.1/deeplake/api/info.py` & `deeplake-3.6.2/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/link.py` & `deeplake-3.6.2/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/link_tiled.py` & `deeplake-3.6.2/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/read.py` & `deeplake-3.6.2/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_access_method.py` & `deeplake-3.6.2/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_agreement.py` & `deeplake-3.6.2/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_api.py` & `deeplake-3.6.2/deeplake/api/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2279,19 +2279,25 @@
 @pytest.mark.parametrize("verify", [True, False])
 def test_bad_link(local_ds_generator, verify):
     with local_ds_generator() as ds:
         ds.create_tensor(
             "images", htype="link[image]", sample_compression="jpg", verify=verify
         )
         ds.images.append(deeplake.link("https://picsum.photos/200/200"))
+
+    if verify:
         with pytest.raises(SampleAppendError):
             ds.images.append(deeplake.link("https://picsum.photos/lalala"))
 
-    with local_ds_generator() as ds:
-        assert len(ds) == 1
+        with local_ds_generator() as ds:
+            assert len(ds) == 1
+    else:
+        ds.images.append(deeplake.link("https://picsum.photos/lalala"))
+        with local_ds_generator() as ds:
+            assert len(ds) == 2
 
 
 def test_rich(memory_ds):
     with memory_ds as ds:
         ds.create_tensor("x")
         ds.x.extend(list(range(10)))
     rich_print(ds)
```

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.6.2/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.6.2/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.6.2/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_dataset.py` & `deeplake-3.6.2/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_dicom.py` & `deeplake-3.6.2/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_downsample.py` & `deeplake-3.6.2/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_events.py` & `deeplake-3.6.2/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_grayscale.py` & `deeplake-3.6.2/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_info.py` & `deeplake-3.6.2/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.6.2/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_json.py` & `deeplake-3.6.2/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_link.py` & `deeplake-3.6.2/deeplake/api/tests/test_link.py`

 * *Files 14% similar despite different names*

```diff
@@ -370,15 +370,15 @@
             create_shape_tensor=False,
             create_sample_info_tensor=False,
         )
         ds.create_tensor("xyz")
         ds.add_creds_key("my_first_key")
         ds.add_creds_key("my_second_key")
 
-        assert ds.get_creds_keys() == ["my_first_key", "my_second_key"]
+        assert ds.get_creds_keys() == {"my_first_key", "my_second_key"}
 
         ds.populate_creds("my_first_key", {})
         ds.populate_creds("my_second_key", {})
         for i in range(10):
             creds_key = "my_first_key" if i % 2 == 0 else "my_second_key"
             sample = deeplake.link("https://picsum.photos/200/300", creds_key=creds_key)
             ds.link.append(sample)
@@ -570,16 +570,14 @@
     ds = local_ds_generator()
     with pytest.raises(ValueError):
         ds.img[0].numpy()
     ds.populate_creds("abc", {})
     assert ds.img[0].numpy().shape == (900, 900, 3)
     with pytest.raises(KeyError):
         ds.update_creds_key("xyz", "ghi")
-    with pytest.raises(ValueError):
-        ds.update_creds_key("abc", "def")
     ds.update_creds_key("abc", "new")
     assert ds.img[0].numpy().shape == (900, 900, 3)
     ds = local_ds_generator()
     with pytest.raises(ValueError):
         ds.img[0].numpy()
     ds.populate_creds("new", {})
     assert ds.img[0].numpy().shape == (900, 900, 3)
@@ -662,13 +660,77 @@
     ds.populate_creds(creds_key, from_environment=True)
     with ds:
         tensor = ds.create_tensor("abc", "link[image]", sample_compression="jpeg")
         tensor.append(deeplake.link(cat_path, creds_key))
 
     assert tensor[0].creds_key() == creds_key
     ds.add_creds_key("my_s3_creds", True)
-    assert ds.get_managed_creds_keys() == ["my_s3_creds"]
-    assert set(ds.get_creds_keys()) == {"my_s3_creds", "ENV"}
+    assert ds.get_managed_creds_keys() == {"my_s3_creds"}
+    assert ds.get_creds_keys() == {"my_s3_creds", "ENV"}
     ds.update_creds_key("my_s3_creds", managed=True)
     ds = hub_cloud_ds_generator()
-    assert ds.get_managed_creds_keys() == ["my_s3_creds"]
-    assert set(ds.get_creds_keys()) == {"my_s3_creds", "ENV"}
+    assert ds.get_managed_creds_keys() == {"my_s3_creds"}
+    assert ds.get_creds_keys() == {"my_s3_creds", "ENV"}
+
+
+def test_bad_link_no_verify(memory_ds):
+    with memory_ds as ds:
+        ds.add_creds_key("S3_CREDS")
+        ds.populate_creds("S3_CREDS", {})
+        ds.create_tensor(
+            "abc", htype="link[image]", sample_compression="jpg", verify=False
+        )
+        ds.abc.append(
+            deeplake.link("s3://some-bucket/does-not-exist.jpg", creds_key="S3_CREDS")
+        )
+
+        assert ds.abc[0]._linked_sample().path == "s3://some-bucket/does-not-exist.jpg"
+
+
+def test_update_creds_to_existing(hub_cloud_ds_generator, cat_path):
+    creds_key = "ENV"
+    ds = hub_cloud_ds_generator()
+    ds.add_creds_key(creds_key)
+    ds.populate_creds(creds_key, from_environment=True)
+
+    with ds:
+        tensor = ds.create_tensor("abc", "link[image]", sample_compression="jpeg")
+        tensor.append(deeplake.link(cat_path, creds_key))
+
+    ds.add_creds_key("my_s3_creds", managed=True)
+
+    with pytest.raises(ValueError):
+        ds.update_creds_key("ENV", "my_s3_creds")
+
+    with pytest.raises(ValueError):
+        ds.update_creds_key("my_s3_creds", "ENV")
+
+    with pytest.raises(ValueError):
+        ds.update_creds_key("ENV", "my_s3_creds", managed=False)
+
+    with pytest.raises(ValueError):
+        ds.update_creds_key("my_s3_creds", "ENV", managed=True)
+
+    with ds:
+        tensor.append(deeplake.link(cat_path, "my_s3_creds"))
+
+    ds.update_creds_key("ENV", "my_s3_creds", managed=True)
+    assert ds.get_managed_creds_keys() == {"my_s3_creds"}
+    assert ds.get_creds_keys() == {"my_s3_creds"}
+    assert ds.link_creds.creds_keys == ["my_s3_creds", "my_s3_creds"]
+
+    encoded_creds = ds.abc.chunk_engine.creds_encoder.get_encoded_creds_key(0)
+    creds_key = ds.link_creds.get_creds_key(encoded_creds)
+    assert creds_key == "my_s3_creds"
+
+    ds.update_creds_key("my_s3_creds", "ENV", managed=False)
+    assert ds.get_managed_creds_keys() == set()
+    assert ds.get_creds_keys() == {"ENV"}
+    assert ds.link_creds.creds_keys == ["ENV", "ENV"]
+
+    encoded_creds = ds.abc.chunk_engine.creds_encoder.get_encoded_creds_key(0)
+    creds_key = ds.link_creds.get_creds_key(encoded_creds)
+    assert creds_key == "ENV"
+
+    encoded_creds = ds.abc.chunk_engine.creds_encoder.get_encoded_creds_key(1)
+    creds_key = ds.link_creds.get_creds_key(encoded_creds)
+    assert creds_key == "ENV"
```

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.6.2/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_linking.py` & `deeplake-3.6.2/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_mesh.py` & `deeplake-3.6.2/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_meta.py` & `deeplake-3.6.2/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_nifti.py` & `deeplake-3.6.2/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_none.py` & `deeplake-3.6.2/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.6.2/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_pickle.py` & `deeplake-3.6.2/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.6.2/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_polygons.py` & `deeplake-3.6.2/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_pop.py` & `deeplake-3.6.2/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_readonly.py` & `deeplake-3.6.2/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_rechunk.py` & `deeplake-3.6.2/deeplake/api/tests/test_rechunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,7 +299,41 @@
     np.testing.assert_array_equal(
         ds.labels.numpy(), np.ones((300, 200), dtype=np.int64)
     )
     ds.checkout("main")
     np.testing.assert_array_equal(
         ds.labels.numpy(), np.ones((300, 200), dtype=np.int64)
     )
+
+
+def test_rechunk_text_like_lz4(local_ds):
+    @deeplake.compute
+    def upload(stuff, ds):
+        ds.append(stuff)
+
+    with local_ds as ds:
+        ds.create_tensor("text", htype="text", chunk_compression="lz4")
+        ds.create_tensor("json", htype="json", chunk_compression="lz4")
+        ds.create_tensor("list", htype="list", chunk_compression="lz4")
+
+        samples = [{"text": "hello", "json": {"a": 1, "b": 3}, "list": [1, 2, 3]}] * 10
+        samples[8] = {
+            "text": "hello world",
+            "json": {"a": 2, "b": 4},
+            "list": [4, 5, 6],
+        }
+
+        upload().eval(samples, ds, num_workers=2, disable_rechunk=True)
+
+    assert ds.text.chunk_engine.num_chunks == 2
+    assert ds.json.chunk_engine.num_chunks == 2
+    assert ds.list.chunk_engine.num_chunks == 2
+
+    ds.pop()
+
+    assert ds.text.chunk_engine.num_chunks == 1
+    assert ds.json.chunk_engine.num_chunks == 1
+    assert ds.list.chunk_engine.num_chunks == 1
+
+    assert ds.text[-1].data()["value"] == "hello world"
+    assert ds.json[-1].data()["value"] == [{"a": 2, "b": 4}]
+    assert ds.list[-1].data()["value"] == [4, 5, 6]
```

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_reset.py` & `deeplake-3.6.2/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_sample_info.py` & `deeplake-3.6.2/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_text.py` & `deeplake-3.6.2/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_update_samples.py` & `deeplake-3.6.2/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_video.py` & `deeplake-3.6.2/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tests/test_views.py` & `deeplake-3.6.2/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/api/tiled.py` & `deeplake-3.6.2/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/structured/base.py` & `deeplake-3.6.2/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/structured/dataframe.py` & `deeplake-3.6.2/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.6.2/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.6.2/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.6.2/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.6.2/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/unstructured/base.py` & `deeplake-3.6.2/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.6.2/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.6.2/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.6.2/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.6.2/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.6.2/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.6.2/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/unstructured/util.py` & `deeplake-3.6.2/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.6.2/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.6.2/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/cli/auth.py` & `deeplake-3.6.2/deeplake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/cli/test_cli.py` & `deeplake-3.6.2/deeplake/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/client/client.py` & `deeplake-3.6.2/deeplake/client/client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/client/config.py` & `deeplake-3.6.2/deeplake/client/config.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/client/log.py` & `deeplake-3.6.2/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/client/test_client.py` & `deeplake-3.6.2/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/client/utils.py` & `deeplake-3.6.2/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/compression.py` & `deeplake-3.6.2/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/constants.py` & `deeplake-3.6.2/deeplake/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/chunk/base_chunk.py` & `deeplake-3.6.2/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.6.2/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.6.2/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.6.2/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.6.2/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.6.2/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.6.2/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/chunk_engine.py` & `deeplake-3.6.2/deeplake/core/chunk_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     List,
     Tuple,
 )
 from deeplake.api.info import Info
 from deeplake.core.link_creds import LinkCreds
 from deeplake.core.linked_sample import LinkedSample
 from deeplake.core.meta.encode.base_encoder import LAST_SEEN_INDEX_COLUMN
-from deeplake.core.serialize import HEADER_SIZE_BYTES
+from deeplake.core.serialize import HEADER_SIZE_BYTES, text_to_bytes
 from deeplake.core.tensor_link import (
     cast_to_type,
     extend_downsample,
     get_link_transform,
 )
 from deeplake.core.version_control.commit_diff import CommitDiff
 from deeplake.core.partial_reader import PartialReader
@@ -1346,24 +1346,28 @@
 
     def _get_sample_object(
         self, sample_data, sample_shape, compression, dtype, decompress
     ):
         if isinstance(sample_data, Polygons):
             return sample_data
         if decompress:
-            sample = Sample(array=sample_data, shape=sample_shape)
+            if self.is_text_like:
+                byts, shape = text_to_bytes(sample_data, dtype, self.tensor_meta.htype)
+                sample = Sample(buffer=byts, shape=shape)
+            else:
+                sample = Sample(array=sample_data, shape=sample_shape)
         else:
             sample = Sample(
                 buffer=sample_data,
                 shape=sample_shape,
                 compression=compression,
                 dtype=dtype,
             )
 
-        if self.tensor_meta.htype in ("json", "text", "list"):
+        if self.is_text_like:
             sample.htype = self.tensor_meta.htype
         if self.tensor_meta.is_link:
             sample.htype = "text"
             sample = LinkedSample(sample.array[0])
         return sample
 
     def __rechunk(self, chunk: BaseChunk, chunk_row: int):
```

### Comparing `deeplake-3.6.1/deeplake/core/compression.py` & `deeplake-3.6.2/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/compute/process.py` & `deeplake-3.6.2/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/compute/provider.py` & `deeplake-3.6.2/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/compute/ray.py` & `deeplake-3.6.2/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/compute/serial.py` & `deeplake-3.6.2/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/compute/thread.py` & `deeplake-3.6.2/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/dataset/__init__.py` & `deeplake-3.6.2/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/dataset/dataset.py` & `deeplake-3.6.2/deeplake/core/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # type: ignore
 import os
 import uuid
 import json
 import posixpath
 from logging import warning
-from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union, Set
 from functools import partial
 
 import pathlib
 import numpy as np
 from time import time, sleep
 from tqdm import tqdm  # type: ignore
 
@@ -97,14 +97,15 @@
     SampleAppendingError,
     DatasetTooLargeToDelete,
     TensorTooLargeToDelete,
     GroupInfoNotSupportedError,
     TokenPermissionError,
     CheckoutError,
     DatasetCorruptError,
+    BadRequestException,
 )
 from deeplake.util.keys import (
     dataset_exists,
     get_dataset_info_key,
     get_dataset_meta_key,
     tensor_exists,
     get_queries_key,
@@ -589,14 +590,15 @@
         create_sample_info_tensor: bool = True,
         create_shape_tensor: bool = True,
         create_id_tensor: bool = True,
         verify: bool = True,
         exist_ok: bool = False,
         verbose: bool = True,
         downsampling: Optional[Tuple[int, int]] = None,
+        tiling_threshold: Optional[int] = None,
         **kwargs,
     ):
         """Creates a new tensor in the dataset.
 
         Examples:
             >>> # create dataset
             >>> ds = deeplake.dataset("path/to/dataset")
@@ -624,19 +626,20 @@
             sample_compression (str): All samples will be compressed in the provided format. If ``None``, samples are uncompressed. For ``link[]`` tensors, ``sample_compression`` is used only for optimizing dataset views.
             chunk_compression (str): All chunks will be compressed in the provided format. If ``None``, chunks are uncompressed. For ``link[]`` tensors, ``chunk_compression`` is used only for optimizing dataset views.
             hidden (bool): If ``True``, the tensor will be hidden from ds.tensors but can still be accessed via ``ds[tensor_name]``.
             create_sample_info_tensor (bool): If ``True``, meta data of individual samples will be saved in a hidden tensor. This data can be accessed via :attr:`tensor[i].sample_info <deeplake.core.tensor.Tensor.sample_info>`.
             create_shape_tensor (bool): If ``True``, an associated tensor containing shapes of each sample will be created.
             create_id_tensor (bool): If ``True``, an associated tensor containing unique ids for each sample will be created. This is useful for merge operations.
             verify (bool): Valid only for link htypes. If ``True``, all links will be verified before they are added to the tensor.
-                ``verify`` is always ``True`` even if specified as ``False`` if ``create_shape_tensor`` or ``create_sample_info_tensor`` is ``True``.
+                If ``False``, links will be added without verification but note that ``create_shape_tensor`` and ``create_sample_info_tensor`` will be set to ``False``.
             exist_ok (bool): If ``True``, the group is created if it does not exist. if ``False``, an error is raised if the group already exists.
             verbose (bool): Shows warnings if ``True``.
             downsampling (tuple[int, int]): If not ``None``, the tensor will be downsampled by the provided factors. For example, ``(2, 5)`` will downsample the tensor by a factor of 2 in both dimensions and create 5 layers of downsampled tensors.
                 Only support for image and mask htypes.
+            tiling_threshold (Optional, int): In MB. Tiles large images if their size exceeds this threshold. Set to -1 to disable tiling.
             **kwargs:
                 - ``htype`` defaults can be overridden by passing any of the compatible parameters.
                 - To see all htypes and their correspondent arguments, check out :ref:`Htypes`.
 
         Returns:
             Tensor: The new tensor, which can be accessed by ``dataset[name]`` or ``dataset.name``.
 
@@ -670,14 +673,15 @@
             create_sample_info_tensor,
             create_shape_tensor,
             create_id_tensor,
             verify,
             exist_ok,
             verbose,
             downsampling,
+            tiling_threshold=tiling_threshold,
             **kwargs,
         )
 
     @invalid_view_op
     def _create_tensor(
         self,
         name: str,
@@ -733,24 +737,18 @@
         tensor_name = posixpath.split(name)[1]
         if not tensor_name or tensor_name in dir(self):
             raise InvalidTensorNameError(tensor_name)
 
         downsampling_factor, number_of_layers = validate_downsampling(downsampling)
         kwargs["is_sequence"] = kwargs.get("is_sequence") or is_sequence
         kwargs["is_link"] = kwargs.get("is_link") or is_link
-        if (
-            kwargs["is_link"]
-            and not verify
-            and (create_shape_tensor or create_sample_info_tensor)
-            and verbose
-        ):
-            warnings.warn(
-                "Setting `verify` to True. `verify`, `create_shape_tensor` and `create_sample_info_tensor` should all be False if you do not want to verify your link samples."
-            )
-        kwargs["verify"] = create_shape_tensor or create_sample_info_tensor or verify
+        kwargs["verify"] = verify
+        if kwargs["is_link"] and not kwargs["verify"]:
+            create_shape_tensor = False
+            create_sample_info_tensor = False
 
         if not self._is_root():
             return self.root._create_tensor(
                 name=key,
                 htype=htype,
                 dtype=dtype,
                 sample_compression=sample_compression,
@@ -3814,23 +3812,36 @@
             org_id (str, optional): The organization to where the connected Deep Lake dataset will be added.
             ds_name (str, optional): The name of the connected Deep Lake dataset. Will be infered from ``dest_path`` or ``src_path`` if not provided.
             token (str, optional): Activeloop token used to fetch the managed credentials.
 
         Raises:
             InvalidSourcePathError: If the dataset's path is not a valid s3, gcs or azure path.
             InvalidDestinationPathError: If ``dest_path``, or ``org_id`` and ``ds_name`` do not form a valid Deep Lake path.
+            TokenPermissionError: If the user does not have permission to create a dataset in the specified organization.
         """
-        path = connect_dataset_entry(
-            src_path=self.path,
-            dest_path=dest_path,
-            org_id=org_id,
-            ds_name=ds_name,
-            creds_key=creds_key,
-            token=token,
-        )
+        try:
+            path = connect_dataset_entry(
+                src_path=self.path,
+                dest_path=dest_path,
+                org_id=org_id,
+                ds_name=ds_name,
+                creds_key=creds_key,
+                token=token,
+            )
+        except BadRequestException:
+            check_param = "organization id" if org_id else "dataset path"
+            raise TokenPermissionError(
+                "You do not have permission to create a dataset in the specified "
+                + check_param
+                + "."
+                + " Please check the "
+                + check_param
+                + " and make sure"
+                + "that you have sufficient permissions to the organization."
+            )
         self.__class__ = (
             deeplake.core.dataset.deeplake_cloud_dataset.DeepLakeCloudDataset
         )
         self._token = token
         self.path = path
         self.public = False
         self._load_link_creds()
@@ -3935,20 +3946,22 @@
             raise ValueError(
                 "Atleast one of new_creds_key or managed must be provided."
             )
         if managed:
             raise ValueError(
                 "Managed creds are not supported for datasets that are not connected to activeloop platform."
             )
-        replaced_index = self.link_creds.replace_creds(creds_key, new_creds_key)
-        save_link_creds(self.link_creds, self.storage, replaced_index=replaced_index)
+        replaced_indices = self.link_creds.replace_creds(creds_key, new_creds_key)
+        save_link_creds(
+            self.link_creds, self.storage, replaced_indices=replaced_indices
+        )
 
-    def get_creds_keys(self) -> List[str]:
-        """Returns the list of creds keys added to the dataset. These are used to fetch external data in linked tensors"""
-        return list(self.link_creds.creds_keys)
+    def get_creds_keys(self) -> Set[str]:
+        """Returns the set of creds keys added to the dataset. These are used to fetch external data in linked tensors"""
+        return set(self.link_creds.creds_keys)
 
     def get_managed_creds_keys(self) -> List[str]:
         """Returns the list of creds keys added to the dataset that are managed by Activeloop platform. These are used to fetch external data in linked tensors."""
         raise ValueError(
             "Managed creds are not supported for datasets that are not connected to activeloop platform."
         )
```

### Comparing `deeplake-3.6.1/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.6.2/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import posixpath
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, Set, Optional, Union
 from deeplake.client.utils import get_user_name
 from deeplake.constants import HUB_CLOUD_DEV_USERNAME
 from deeplake.core.dataset import Dataset
 from deeplake.client.client import DeepLakeBackendClient
 from deeplake.util.bugout_reporter import deeplake_reporter
 from deeplake.util.exceptions import (
     InvalidSourcePathError,
@@ -315,42 +315,53 @@
             >>> ds.update_creds_key("my_s3_key", "my_managed_key", True)
         """
         if new_creds_key is None and managed is None:
             raise ValueError(
                 "Atleast one of new_creds_key or managed must be provided."
             )
         key_index = self.link_creds.creds_mapping[creds_key] - 1
-        managed_info, replaced_index = None, None
+        managed_info, replaced_indices = None, None
         original_creds_key = creds_key
         original_key_is_managed = (
             original_creds_key in self.link_creds.managed_creds_keys
         )
 
         if new_creds_key is not None and new_creds_key != creds_key:
-            replaced_index = self.link_creds.replace_creds(creds_key, new_creds_key)
+            if new_creds_key in self.link_creds.creds_keys:
+                new_creds_managed = new_creds_key in self.link_creds.managed_creds_keys
+                old_creds_managed = (
+                    managed
+                    if managed is not None
+                    else (creds_key in self.link_creds.managed_creds_keys)
+                )
+                if new_creds_managed != old_creds_managed:
+                    raise ValueError(
+                        f"{new_creds_key} is already present in the dataset with a different management status."
+                    )
+            replaced_indices = self.link_creds.replace_creds(creds_key, new_creds_key)
             creds_key = new_creds_key
 
         try:
             if managed is not None:
                 management_changed = self.link_creds.change_creds_management(
                     creds_key, managed
                 )
                 if management_changed:
                     managed_info = (managed, key_index)
             if original_key_is_managed and managed is not False:
                 self.link_creds.populate_single_managed_creds(creds_key)
         except Exception:
-            if replaced_index is not None:
+            if replaced_indices is not None:
                 # revert the change
                 self.link_creds.replace_creds(new_creds_key, original_creds_key)
             raise
         save_link_creds(
             self.link_creds,
             self.storage,
-            replaced_index=replaced_index,
+            replaced_indices=replaced_indices,
             managed_info=managed_info,
         )
         self.link_creds.warn_missing_managed_creds()
 
     def _load_link_creds(self):
         """Loads the link creds from the storage."""
         super()._load_link_creds()
@@ -381,10 +392,10 @@
         return _TmpWriteAccess()
 
     def connect(self, *args, **kwargs):
         raise InvalidSourcePathError(
             f"The dataset being connected is already accessible via Deep Lake path {self.path}"
         )
 
-    def get_managed_creds_keys(self) -> List[str]:
-        """Returns the list of creds keys added to the dataset that are managed by Activeloop platform. These are used to fetch external data in linked tensors."""
-        return list(self.link_creds.managed_creds_keys)
+    def get_managed_creds_keys(self) -> Set[str]:
+        """Returns the set of creds keys added to the dataset that are managed by Activeloop platform. These are used to fetch external data in linked tensors."""
+        return set(self.link_creds.managed_creds_keys)
```

### Comparing `deeplake-3.6.1/deeplake/core/dataset/deeplake_query_dataset.py` & `deeplake-3.6.2/deeplake/core/dataset/deeplake_query_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/dataset/deeplake_query_tensor.py` & `deeplake-3.6.2/deeplake/core/dataset/deeplake_query_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/dataset/invalid_view.py` & `deeplake-3.6.2/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/dataset/view_entry.py` & `deeplake-3.6.2/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/fast_forwarding.py` & `deeplake-3.6.2/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/index/index.py` & `deeplake-3.6.2/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/io.py` & `deeplake-3.6.2/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/ipc.py` & `deeplake-3.6.2/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/link_creds.py` & `deeplake-3.6.2/deeplake/core/link_creds.py`

 * *Files 8% similar despite different names*

```diff
@@ -137,23 +137,41 @@
             creds = self.fetch_managed_creds(creds_key)
         self.creds_keys.append(creds_key)
         self.creds_mapping[creds_key] = len(self.creds_keys)
         if managed:
             self.managed_creds_keys.add(creds_key)
             self.populate_creds(creds_key, creds)
 
+    def _replace_with_existing_creds(self, old_creds_key: str, new_creds_key: str):
+        replaced_indices = []
+        for i in range(len(self.creds_keys)):
+            if self.creds_keys[i] == old_creds_key:
+                self.creds_keys[i] = new_creds_key
+                replaced_indices.append(i)
+
+        self.creds_dict.pop(old_creds_key, None)
+        self.creds_mapping.pop(old_creds_key, None)
+
+        self.managed_creds_keys.discard(old_creds_key)
+        self.used_creds_keys.discard(old_creds_key)
+
+        self.storage_providers.pop(old_creds_key, None)
+
+        return replaced_indices
+
     def replace_creds(self, old_creds_key: str, new_creds_key: str):
         if old_creds_key not in self.creds_keys:
             raise KeyError(f"Creds key {old_creds_key} does not exist")
         if new_creds_key in self.creds_keys:
-            raise ValueError(f"Creds key {new_creds_key} already exists")
+            return self._replace_with_existing_creds(old_creds_key, new_creds_key)
+        replaced_indices = []
         for i in range(len(self.creds_keys)):
             if self.creds_keys[i] == old_creds_key:
                 self.creds_keys[i] = new_creds_key
-                replaced_index = i
+                replaced_indices.append(i)
 
         if old_creds_key in self.creds_dict:
             self.creds_dict[new_creds_key] = self.creds_dict[old_creds_key]
             del self.creds_dict[old_creds_key]
 
         self.creds_mapping[new_creds_key] = self.creds_mapping[old_creds_key]
         del self.creds_mapping[old_creds_key]
@@ -167,15 +185,15 @@
             self.used_creds_keys.add(new_creds_key)
 
         if old_creds_key in self.storage_providers:
             self.storage_providers[new_creds_key] = self.storage_providers[
                 old_creds_key
             ]
             del self.storage_providers[old_creds_key]
-        return replaced_index
+        return replaced_indices
 
     def populate_creds(self, creds_key: str, creds):
         if creds_key not in self.creds_keys:
             raise MissingCredsError(f"Creds key {creds_key} does not exist")
         expires_in_to_expires_at(creds)
         self.creds_dict[creds_key] = creds
         self.storage_providers.pop(creds_key, None)
```

### Comparing `deeplake-3.6.1/deeplake/core/linked_chunk_engine.py` & `deeplake-3.6.2/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/linked_sample.py` & `deeplake-3.6.2/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/linked_tiled_sample.py` & `deeplake-3.6.2/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/lock.py` & `deeplake-3.6.2/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/meta/dataset_meta.py` & `deeplake-3.6.2/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.6.2/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.6.2/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.6.2/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/meta/encode/creds.py` & `deeplake-3.6.2/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/meta/encode/pad.py` & `deeplake-3.6.2/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/meta/encode/sequence.py` & `deeplake-3.6.2/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/meta/encode/shape.py` & `deeplake-3.6.2/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.6.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.6.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.6.2/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.6.2/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.6.2/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/meta/encode/tile.py` & `deeplake-3.6.2/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/meta/tensor_meta.py` & `deeplake-3.6.2/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/partial_reader.py` & `deeplake-3.6.2/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/partial_sample.py` & `deeplake-3.6.2/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/polygon.py` & `deeplake-3.6.2/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/query/autocomplete.py` & `deeplake-3.6.2/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/query/filter.py` & `deeplake-3.6.2/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/query/query.py` & `deeplake-3.6.2/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/sample.py` & `deeplake-3.6.2/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/serialize.py` & `deeplake-3.6.2/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/storage/azure.py` & `deeplake-3.6.2/deeplake/core/storage/azure.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.6.2/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/storage/gcs.py` & `deeplake-3.6.2/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/storage/google_drive.py` & `deeplake-3.6.2/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/storage/local.py` & `deeplake-3.6.2/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/storage/lru_cache.py` & `deeplake-3.6.2/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/storage/memory.py` & `deeplake-3.6.2/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/storage/provider.py` & `deeplake-3.6.2/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/storage/s3.py` & `deeplake-3.6.2/deeplake/core/storage/s3.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/tensor.py` & `deeplake-3.6.2/deeplake/core/tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/tensor_link.py` & `deeplake-3.6.2/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/test_serialize.py` & `deeplake-3.6.2/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/tests/test_compression.py` & `deeplake-3.6.2/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/tests/test_compute.py` & `deeplake-3.6.2/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/tests/test_deeplake_indra_dataset.py` & `deeplake-3.6.2/deeplake/core/tests/test_deeplake_indra_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/tests/test_io.py` & `deeplake-3.6.2/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/tests/test_locking.py` & `deeplake-3.6.2/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/tests/test_readonly.py` & `deeplake-3.6.2/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/tests/test_serialize.py` & `deeplake-3.6.2/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/tiling/deserialize.py` & `deeplake-3.6.2/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/tiling/optimizer.py` & `deeplake-3.6.2/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.6.2/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/tiling/serialize.py` & `deeplake-3.6.2/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.6.2/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/tiling/test_serialize.py` & `deeplake-3.6.2/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/transform/test_transform.py` & `deeplake-3.6.2/deeplake/core/transform/test_transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/transform/transform.py` & `deeplake-3.6.2/deeplake/core/transform/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/transform/transform_dataset.py` & `deeplake-3.6.2/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/transform/transform_tensor.py` & `deeplake-3.6.2/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/__init__.py` & `deeplake-3.6.2/deeplake/core/vectorstore/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/deeplake_vectorstore.py` & `deeplake-3.6.2/deeplake/core/vectorstore/deeplake_vectorstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,34 +322,34 @@
                 "embedding": True if embedding is not None else False,
                 "return_tensors": return_tensors,
                 "return_view": return_view,
             },
         )
 
         exec_option = exec_option or self.exec_option
-        embedding_function = embedding_function or self.embedding_function
 
         utils.parse_search_args(
             embedding_data=embedding_data,
             embedding_function=embedding_function,
+            initial_embedding_function=self.embedding_function,
             embedding=embedding,
             k=k,
             distance_metric=distance_metric,
             query=query,
             filter=filter,
             exec_option=exec_option,
             embedding_tensor=embedding_tensor,
             return_tensors=return_tensors,
         )
 
         # if embedding_function is not None or embedding is not None:
         query_emb = dataset_utils.get_embedding(
             embedding,
             embedding_data,
-            embedding_function=embedding_function,
+            embedding_function=embedding_function or self.embedding_function,
         )
 
         if not return_tensors:
             return_tensors = [
                 tensor for tensor in self.dataset.tensors if tensor != embedding_tensor
             ]
```

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/test_deeplake_vectorstore.py` & `deeplake-3.6.2/deeplake/core/vectorstore/test_deeplake_vectorstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 
 query_embedding = np.random.uniform(low=-10, high=10, size=(EMBEDDING_DIM)).astype(
     np.float32
 )
 
 
 def embedding_fn(text, embedding_dim=EMBEDDING_DIM):
-    pass  # pragma: no cover
+    return np.zeros(len(text), EMBEDDING_DIM)  # pragma: no cover
 
 
 def embedding_fn2(text, embedding_dim=EMBEDDING_DIM):
     pass  # pragma: no cover
 
 
 def embedding_fn3(text, embedding_dim=EMBEDDING_DIM):
     """Returns embedding in List[np.ndarray] format"""
     return [np.zeros(embedding_dim) for i in range(len(text))]
 
 
-def test_custom_tensors(hub_cloud_dev_token):
+def test_custom_tensors():
     # initialize vector store object:
     vector_store = DeepLakeVectorStore(
         path="./deeplake_vector_store",
         overwrite=True,
         tensor_params=[
             {"name": "texts_custom", "htype": "text"},
             {"name": "emb_custom", "htype": "embedding"},
@@ -261,14 +261,21 @@
     with pytest.raises(ValueError):
         data = vector_store.search(
             exec_option="compute_engine",
             query="select * where metadata == {'abcdefg': 28}",
             return_tensors=["metadata", "id"],
         )
 
+    vector_store = DeepLakeVectorStore(
+        path="mem://xyz", embedding_function=embedding_fn
+    )
+    vector_store.add(embedding=embeddings, text=texts, metadata=metadatas)
+    result = vector_store.search(embedding=np.zeros(1, EMBEDDING_DIM))
+    assert len(result) == 4
+
 
 @requires_libdeeplake
 @pytest.mark.parametrize("distance_metric", ["L1", "L2", "COS", "MAX"])
 def test_search_quantitative(distance_metric, hub_cloud_dev_token):
     """Test whether TQL and Python return the same results"""
 
     # initialize vector store object:
```

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/dataset/dataset.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/dataset/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -212,19 +212,14 @@
 
 
 def fetch_embeddings(view, embedding_tensor: str = "embedding"):
     return view[embedding_tensor].numpy()
 
 
 def get_embedding(embedding, embedding_data, embedding_function=None):
-    if embedding is not None and embedding_function:
-        always_warn(
-            "Both embedding data and embedding function were specified."
-            " Already computed `embedding` will be used."
-        )
     if embedding is None and embedding_function is not None:
         embedding = embedding_function(embedding_data)  # type: ignore
 
     if embedding is not None and (
         isinstance(embedding, list) or embedding.dtype != "float32"
     ):
         embedding = np.array(embedding, dtype=np.float32)
```

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/filter/filter.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/filter/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/filter/test_filter.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/filter/test_filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/indra/query.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/indra/test_indra.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/test_indra.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/indra/vector_search.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/python/search_algorithm.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/python/test_vector_search.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/test_vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/python/vector_search.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/utils.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from deeplake.constants import MB
 from deeplake.enterprise.util import raise_indra_installation_error
+from deeplake.util.warnings import always_warn
 
 import numpy as np
 
 import random
 import string
 from typing import Optional, List, Dict, Callable
 
@@ -95,19 +96,34 @@
         and kwargs["embedding"] is None
         and kwargs["query"] is None
         and kwargs["filter"] is None
     ):
         raise ValueError(
             f"Either an `embedding`, `embedding_function`, `filter`, or `query` must be specified."
         )
+
+    if kwargs["embedding"] is not None and kwargs["embedding_function"]:
+        always_warn(
+            "Both `embedding` and `embedding_function` were specified."
+            " Already computed `embedding` will be used."
+        )
     if kwargs["embedding_data"] is None and kwargs["embedding_function"] is not None:
         raise ValueError(
             f"When an `embedding_function` is specified, `embedding_data` must also be specified."
         )
 
+    if (
+        kwargs["embedding_data"] is not None
+        and kwargs["embedding_function"] is None
+        and kwargs["initial_embedding_function"] is None
+    ):
+        raise ValueError(
+            f"When an `embedding_data` is specified, `embedding_function` must also be specified."
+        )
+
     exec_option = kwargs["exec_option"]
     if exec_option == "python":
         if kwargs["query"] is not None:
             raise ValueError(
                 f"User-specified TQL queries are not support for exec_option={exec_option}."
             )
```

### Comparing `deeplake-3.6.1/deeplake/core/vectorstore/vector_search/vector_search.py` & `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.6.2/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/version_control/commit_diff.py` & `deeplake-3.6.2/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/version_control/commit_node.py` & `deeplake-3.6.2/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.6.2/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/version_control/test_merge.py` & `deeplake-3.6.2/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/core/version_control/test_version_control.py` & `deeplake-3.6.2/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.6.2/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/enterprise/dataloader.py` & `deeplake-3.6.2/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.6.2/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.6.2/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/enterprise/test_pytorch.py` & `deeplake-3.6.2/deeplake/enterprise/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/enterprise/test_query.py` & `deeplake-3.6.2/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.6.2/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/enterprise/util.py` & `deeplake-3.6.2/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/hooks.py` & `deeplake-3.6.2/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/htype.py` & `deeplake-3.6.2/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.6.2/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.6.2/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.6.2/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.6.2/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/integrations/pytorch/common.py` & `deeplake-3.6.2/deeplake/integrations/pytorch/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,23 @@
     elif isinstance(elem, (tuple, list)) and len(elem) > 0 and isinstance(elem[0], str):
         batch = [it[0] for it in batch]
     elif isinstance(elem, Polygons):
         batch = [it.numpy() for it in batch]
     elif isinstance(elem, list) and all(
         map(lambda e: isinstance(e, np.ndarray), elem)
     ):  # special case for video query api
-        if len(elem[0].shape) > 1 and elem[0].shape[1] not in [
-            2,
-            3,
-        ]:  # checking whether it is not a polygon
+        if (
+            len(elem) > 0
+            and len(elem[0].shape) > 1
+            and elem[0].shape[1]
+            not in [
+                2,
+                3,
+            ]
+        ):  # checking whether it is not a polygon
             elem_type = type(elem)
             return [
                 elem_type([torch.tensor(item) for item in sample]) for sample in batch
             ]
     return default_collate(batch)
```

### Comparing `deeplake-3.6.1/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.6.2/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.6.2/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.6.2/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/integrations/tf/common.py` & `deeplake-3.6.2/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.6.2/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.6.2/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/integrations/wandb/wandb.py` & `deeplake-3.6.2/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/tests/cache_fixtures.py` & `deeplake-3.6.2/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/tests/client_fixtures.py` & `deeplake-3.6.2/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/tests/common.py` & `deeplake-3.6.2/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/tests/dataset_fixtures.py` & `deeplake-3.6.2/deeplake/tests/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/tests/path_fixtures.py` & `deeplake-3.6.2/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/tests/storage_fixtures.py` & `deeplake-3.6.2/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/access_method.py` & `deeplake-3.6.2/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/agreement.py` & `deeplake-3.6.2/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/array_list.py` & `deeplake-3.6.2/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/assert_byte_indexes.py` & `deeplake-3.6.2/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/auto.py` & `deeplake-3.6.2/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/bugout_reporter.py` & `deeplake-3.6.2/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/cache_chain.py` & `deeplake-3.6.2/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/casting.py` & `deeplake-3.6.2/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/check_latest_version.py` & `deeplake-3.6.2/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/chunk_engine.py` & `deeplake-3.6.2/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/class_label.py` & `deeplake-3.6.2/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/compute.py` & `deeplake-3.6.2/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/connect_dataset.py` & `deeplake-3.6.2/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/dataset.py` & `deeplake-3.6.2/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/diff.py` & `deeplake-3.6.2/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/downsample.py` & `deeplake-3.6.2/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/encoder.py` & `deeplake-3.6.2/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/exceptions.py` & `deeplake-3.6.2/deeplake/util/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -864,20 +864,21 @@
     def __init__(self):
         super().__init__(
             "Token is invalid. Make sure the full token string is included and try again."
         )
 
 
 class TokenPermissionError(Exception):
-    def __init__(self):
-        message = (
-            "A dataset does not exist at the specified path, or you do not have "
-            "sufficient permissions to load or create one. Please check the dataset "
-            "path and make sure that you have sufficient permissions to the path."
-        )
+    def __init__(self, message=None):
+        if message is None:
+            message = (
+                "A dataset does not exist at the specified path, or you do not have "
+                "sufficient permissions to load or create one. Please check the dataset "
+                "path and make sure that you have sufficient permissions to the path."
+            )
         super().__init__(message)
 
 
 class SampleAppendingError(Exception):
     def __init__(self):
         message = """Cannot append sample because tensor(s) are not specified. Expected input to ds.append is a dictionary. To append samples, you need to either specify the tensors and append the samples as a dictionary, like: `ds.append({"image_tensor": sample, "label_tensor": sample})` or you need to call `append` method of the required tensor, like: `ds.image_tensor.append(sample)`"""
         super().__init__(message)
```

### Comparing `deeplake-3.6.1/deeplake/util/exif.py` & `deeplake-3.6.2/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/from_tfds.py` & `deeplake-3.6.2/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/htype.py` & `deeplake-3.6.2/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/image.py` & `deeplake-3.6.2/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/invalid_view_op.py` & `deeplake-3.6.2/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/iteration_warning.py` & `deeplake-3.6.2/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/json.py` & `deeplake-3.6.2/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/keys.py` & `deeplake-3.6.2/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/link.py` & `deeplake-3.6.2/deeplake/util/link.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from deeplake.core.lock import Lock
 from deeplake.core.storage.lru_cache import LRUCache
 from deeplake.util.keys import (
     get_dataset_linked_creds_key,
     get_dataset_linked_creds_lock_key,
 )
 from deeplake.util.remove_cache import get_base_storage
-from typing import Optional, Tuple
+from typing import Optional, Tuple, List
 
 
 def merge_link_creds(
     old_link_creds: LinkCreds,
     current_link_creds: LinkCreds,
-    replaced_index: Optional[int] = None,
+    replaced_indices: Optional[List[int]] = None,
     managed_info: Optional[Tuple] = None,
 ):
     num_common_keys = 0
-    if replaced_index is not None:
-        new_key = current_link_creds.creds_keys[replaced_index]
+    if replaced_indices is not None:
+        new_key = current_link_creds.creds_keys[replaced_indices[0]]
     for i, (key1, key2) in enumerate(
         zip(old_link_creds.creds_keys, current_link_creds.creds_keys)
     ):
-        if key1 == key2 or i == replaced_index:
+        if key1 == key2 or (replaced_indices is not None and i in replaced_indices):
             num_common_keys += 1
         else:
             break
     new_keys = current_link_creds.creds_keys[num_common_keys:]
     current_link_creds.creds_keys = old_link_creds.creds_keys
     current_link_creds.creds_mapping = old_link_creds.creds_mapping
     current_link_creds.managed_creds_keys = old_link_creds.managed_creds_keys.union(
@@ -34,16 +34,16 @@
     current_link_creds.used_creds_keys = old_link_creds.used_creds_keys.union(
         current_link_creds.used_creds_keys
     )
     for key in new_keys:
         if key not in current_link_creds.creds_mapping:
             managed = key in current_link_creds.managed_creds_keys
             current_link_creds.add_creds_key(key, managed)
-    if replaced_index is not None:
-        replaced_key = current_link_creds.creds_keys[replaced_index]
+    if replaced_indices is not None:
+        replaced_key = current_link_creds.creds_keys[replaced_indices[0]]
         current_link_creds.replace_creds(replaced_key, new_key)
     if managed_info is not None:
         is_managed = managed_info[0]
         managed_index = managed_info[1]
         key = current_link_creds.creds_keys[managed_index]
         if is_managed:
             current_link_creds.managed_creds_keys.add(key)
@@ -51,15 +51,15 @@
             current_link_creds.managed_creds_keys.discard(key)
     return current_link_creds
 
 
 def save_link_creds(
     current_link_creds: LinkCreds,
     storage: LRUCache,
-    replaced_index: Optional[int] = None,
+    replaced_indices: Optional[List[int]] = None,
     managed_info: Optional[Tuple] = None,
 ):
     """Saves the linked creds info to storage."""
     storage = get_base_storage(storage)
     lock = Lock(storage, get_dataset_linked_creds_lock_key())
     lock.acquire(timeout=10)
     key = get_dataset_linked_creds_key()
@@ -67,15 +67,15 @@
         data_bytes = storage[key]
     except KeyError:
         data_bytes = None
 
     if data_bytes is not None:
         old_link_creds = LinkCreds.frombuffer(data_bytes)
         new_link_creds = merge_link_creds(
-            old_link_creds, current_link_creds, replaced_index, managed_info
+            old_link_creds, current_link_creds, replaced_indices, managed_info
         )
     else:
         new_link_creds = current_link_creds
 
     storage[key] = new_link_creds.tobytes()
     lock.release()
```

### Comparing `deeplake-3.6.1/deeplake/util/logging.py` & `deeplake-3.6.2/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/merge.py` & `deeplake-3.6.2/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/modified.py` & `deeplake-3.6.2/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/notebook.py` & `deeplake-3.6.2/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/object_3d/mesh.py` & `deeplake-3.6.2/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.6.2/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.6.2/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.6.2/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.6.2/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.6.2/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.6.2/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.6.2/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.6.2/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.6.2/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/path.py` & `deeplake-3.6.2/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/pretty_print.py` & `deeplake-3.6.2/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/remove_cache.py` & `deeplake-3.6.2/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/scheduling.py` & `deeplake-3.6.2/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/shape_interval.py` & `deeplake-3.6.2/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/spinner.py` & `deeplake-3.6.2/deeplake/util/spinner.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/split.py` & `deeplake-3.6.2/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/storage.py` & `deeplake-3.6.2/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/tag.py` & `deeplake-3.6.2/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/tensor_db.py` & `deeplake-3.6.2/deeplake/util/tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/testing.py` & `deeplake-3.6.2/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/tests/test_auto.py` & `deeplake-3.6.2/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.6.2/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.6.2/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/tests/test_read.py` & `deeplake-3.6.2/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.6.2/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/tests/test_split.py` & `deeplake-3.6.2/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/tests/test_tensor_db.py` & `deeplake-3.6.2/deeplake/util/tests/test_tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/tests/test_version_control.py` & `deeplake-3.6.2/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/transform.py` & `deeplake-3.6.2/deeplake/util/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/version_control.py` & `deeplake-3.6.2/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/util/video.py` & `deeplake-3.6.2/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/visualizer/video_streaming.py` & `deeplake-3.6.2/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake/visualizer/visualizer.py` & `deeplake-3.6.2/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake.egg-info/PKG-INFO` & `deeplake-3.6.2/deeplake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.6.1
+Version: 3.6.2
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.6.1 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.6.2 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: azure
 Provides-Extra: dicom Provides-Extra: enterprise Provides-Extra: gcp Provides-
```

### Comparing `deeplake-3.6.1/deeplake.egg-info/SOURCES.txt` & `deeplake-3.6.2/deeplake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.1/deeplake.egg-info/requires.txt` & `deeplake-3.6.2/deeplake.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 azure-storage-blob
 flask
 google-api-python-client~=2.31.0
 google-auth-oauthlib~=0.4.5
 google-auth~=2.0.1
 google-cloud-storage~=1.42.0
 laspy
-libdeeplake==0.0.56
+libdeeplake==0.0.58
 nibabel
 oauth2client~=4.1.3
 pydicom
 
 [all:python_version >= "3.7" or sys_platform != "win32"]
 av>=8.1.0
 
@@ -47,15 +47,15 @@
 azure-storage-blob
 
 [dicom]
 nibabel
 pydicom
 
 [enterprise]
-libdeeplake==0.0.56
+libdeeplake==0.0.58
 pyjwt
 
 [gcp]
 google-auth-oauthlib~=0.4.5
 google-auth~=2.0.1
 google-cloud-storage~=1.42.0
```

### Comparing `deeplake-3.6.1/setup.py` & `deeplake-3.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 all_extras = {r for v in extras.values() for r in v}
 install_requires = [req_map[r] for r in req_map if r not in all_extras]
 extras_require = {k: [req_map[r] for r in v] for k, v in extras.items()}
 
 extras_require["all"] = [req_map[r] for r in all_extras]
 
 if libdeeplake_availabe():
-    libdeeplake = "libdeeplake==0.0.56"
+    libdeeplake = "libdeeplake==0.0.58"
     extras_require["enterprise"] = [libdeeplake, "pyjwt"]
     extras_require["all"].append(libdeeplake)
 
 init_file = os.path.join(project_name, "__init__.py")
 
 
 def get_property(prop):
```

