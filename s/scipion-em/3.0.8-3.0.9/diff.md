# Comparing `tmp/scipion-em-3.0.8.tar.gz` & `tmp/scipion-em-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-3.0.8.tar", last modified: Fri Mar  5 10:02:15 2021, max compression
+gzip compressed data, was "scipion-em-3.0.9.tar", last modified: Tue Mar 30 10:37:19 2021, max compression
```

## Comparing `scipion-em-3.0.8.tar` & `scipion-em-3.0.9.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.481269 scipion-em-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-03-05 09:56:12.000000 scipion-em-3.0.8/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2021-03-05 09:56:12.000000 scipion-em-3.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-03-05 09:56:12.000000 scipion-em-3.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2021-03-05 10:02:15.481269 scipion-em-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-03-05 09:56:12.000000 scipion-em-3.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.465268 scipion-em-3.0.8/pwem/
--rw-r--r--   0 runner    (1001) docker     (121)     4916 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/bibtex.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.465268 scipion-em-3.0.8/pwem/cmd/
--rwxr-xr-x   0 runner    (1001) docker     (121)      382 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/cmd/chimera_client.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4026 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/cmd/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/cmd/program.py
--rw-r--r--   0 runner    (1001) docker     (121)     6375 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.465268 scipion-em-3.0.8/pwem/convert/
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    37562 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/convert/atom_struct.py
--rw-r--r--   0 runner    (1001) docker     (121)    14159 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/convert/headers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8688 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/convert/sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)    23840 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/convert/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (121)    65754 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/convert/transformations.py
--rw-r--r--   0 runner    (1001) docker     (121)     4547 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/convert/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.465268 scipion-em-3.0.8/pwem/emlib/
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/emlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29660 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/emlib/_libNone.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.465268 scipion-em-3.0.8/pwem/emlib/image/
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/emlib/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21780 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/emlib/image/image_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/emlib/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.465268 scipion-em-3.0.8/pwem/emlib/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/emlib/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11287 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/emlib/metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.465268 scipion-em-3.0.8/pwem/objects/
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    71469 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/objects/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     5562 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/objects/data_tiltpairs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.469268 scipion-em-3.0.8/pwem/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)     2454 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4142 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)    13672 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)     3902 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     3321 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_3d.py
--rw-r--r--   0 runner    (1001) docker     (121)    32581 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_align_movies.py
--rw-r--r--   0 runner    (1001) docker     (121)     7445 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_alignment_assign.py
--rw-r--r--   0 runner    (1001) docker     (121)     4553 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_alignment_invertHand.py
--rw-r--r--   0 runner    (1001) docker     (121)    24488 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_batch.py
--rw-r--r--   0 runner    (1001) docker     (121)     4585 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_classes_consensus.py
--rw-r--r--   0 runner    (1001) docker     (121)    15973 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_create_stream_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     8052 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_ctf_assign.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.469268 scipion-em-3.0.8/pwem/protocols/protocol_export/
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12107 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_export/protocol_export_DB.py
--rw-r--r--   0 runner    (1001) docker     (121)    16690 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_extract_coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.473268 scipion-em-3.0.8/pwem/protocols/protocol_import/
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12003 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_import/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    25865 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_import/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (121)    10122 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_import/ctfs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6057 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_import/dataimport.py
--rw-r--r--   0 runner    (1001) docker     (121)    23881 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_import/images.py
--rw-r--r--   0 runner    (1001) docker     (121)     3649 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_import/masks.py
--rw-r--r--   0 runner    (1001) docker     (121)    30302 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_import/micrographs.py
--rw-r--r--   0 runner    (1001) docker     (121)    13060 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_import/particles.py
--rw-r--r--   0 runner    (1001) docker     (121)    25590 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_import/sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)    22524 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_import/volumes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3201 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_metadata_editor.py
--rw-r--r--   0 runner    (1001) docker     (121)    31529 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_micrographs.py
--rw-r--r--   0 runner    (1001) docker     (121)    21203 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_movies.py
--rw-r--r--   0 runner    (1001) docker     (121)     7141 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_origin_sampling_volume.py
--rw-r--r--   0 runner    (1001) docker     (121)    25437 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_particles.py
--rw-r--r--   0 runner    (1001) docker     (121)    25045 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_particles_picking.py
--rw-r--r--   0 runner    (1001) docker     (121)     5259 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_pdf_report.py
--rw-r--r--   0 runner    (1001) docker     (121)    33673 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_sets.py
--rw-r--r--   0 runner    (1001) docker     (121)     7736 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)    10282 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/protocols/protocol_tiltpairs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.473268 scipion-em-3.0.8/pwem/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     6537 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/templates/demo.json.template
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.473268 scipion-em-3.0.8/pwem/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.473268 scipion-em-3.0.8/pwem/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    38693 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/data/test_convert_atom_struct.py
--rw-r--r--   0 runner    (1001) docker     (121)    35874 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/data/test_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3204 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/data/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    21174 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/data/test_symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.473268 scipion-em-3.0.8/pwem/tests/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8069 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_extract_particles.py
--rw-r--r--   0 runner    (1001) docker     (121)     6760 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     6500 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_protocol_alignment_assign.py
--rw-r--r--   0 runner    (1001) docker     (121)    13157 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_protocol_export2DB.py
--rw-r--r--   0 runner    (1001) docker     (121)     2248 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_protocol_extract_coorinates.py
--rw-r--r--   0 runner    (1001) docker     (121)     6065 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_protocol_invert_Hand.py
--rw-r--r--   0 runner    (1001) docker     (121)    11658 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_protocol_volume_homogenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     8404 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_protocols_assign_orig.py
--rw-r--r--   0 runner    (1001) docker     (121)     9190 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_coords.py
--rw-r--r--   0 runner    (1001) docker     (121)     6635 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_ctfs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2295 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_masks.py
--rw-r--r--   0 runner    (1001) docker     (121)     9168 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_micrographs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6488 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_movies.py
--rw-r--r--   0 runner    (1001) docker     (121)     9670 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_particles.py
--rw-r--r--   0 runner    (1001) docker     (121)    27671 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)    17661 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_volumes.py
--rw-r--r--   0 runner    (1001) docker     (121)    25634 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/protocols/test_protocols_sets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.477268 scipion-em-3.0.8/pwem/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17332 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/workflows/test_parallel_gpu_queue.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1299 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/workflows/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)    14023 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/workflows/test_workflow_initialvolume.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12648 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/workflows/test_workflow_mixed.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13743 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/workflows/test_workflow_mixed_large.py
--rwxr-xr-x   0 runner    (1001) docker     (121)   122820 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/workflows/test_workflow_modeling.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11926 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/workflows/test_workflow_xmipp.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4512 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/workflows/test_workflow_xmipp_assignment_tiltpairs.py
--rw-r--r--   0 runner    (1001) docker     (121)    10427 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/workflows/test_workflow_xmipp_ctf_consensus.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5438 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/tests/workflows/test_workflow_xmipp_rct.py
--rw-r--r--   0 runner    (1001) docker     (121)     3345 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.477268 scipion-em-3.0.8/pwem/viewers/
--rw-r--r--   0 runner    (1001) docker     (121)     2529 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6991 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/viewers/filehandlers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10409 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/viewers/plotter.py
--rw-r--r--   0 runner    (1001) docker     (121)    12570 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/viewers/showj.py
--rw-r--r--   0 runner    (1001) docker     (121)     5254 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/viewers/viewer_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    19582 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/viewers/viewer_chimera.py
--rw-r--r--   0 runner    (1001) docker     (121)     4770 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/viewers/viewer_fsc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4033 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/viewers/viewer_localres.py
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/viewers/viewer_pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3026 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/viewers/viewer_sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)     2893 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/viewers/viewer_vmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     7854 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/viewers/viewer_volumes.py
--rw-r--r--   0 runner    (1001) docker     (121)    10148 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/viewers/viewers_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/viewers/viewers_protocols.py
--rw-r--r--   0 runner    (1001) docker     (121)    16407 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/viewers/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.481269 scipion-em-3.0.8/pwem/wizards/
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/wizards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    49421 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/wizards/wizard.py
--rw-r--r--   0 runner    (1001) docker     (121)     9048 2021-03-05 09:56:12.000000 scipion-em-3.0.8/pwem/wizards/wizards.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-03-05 09:56:12.000000 scipion-em-3.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 10:02:15.481269 scipion-em-3.0.8/scipion_em.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2021-03-05 10:02:15.000000 scipion-em-3.0.8/scipion_em.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4460 2021-03-05 10:02:15.000000 scipion-em-3.0.8/scipion_em.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-05 10:02:15.000000 scipion-em-3.0.8/scipion_em.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      161 2021-03-05 10:02:15.000000 scipion-em-3.0.8/scipion_em.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-03-05 10:02:15.000000 scipion-em-3.0.8/scipion_em.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-03-05 10:02:15.000000 scipion-em-3.0.8/scipion_em.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-05 10:02:15.481269 scipion-em-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3168 2021-03-05 09:56:12.000000 scipion-em-3.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.989638 scipion-em-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2021-03-30 10:31:41.000000 scipion-em-3.0.9/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    35147 2021-03-30 10:31:41.000000 scipion-em-3.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-03-30 10:31:41.000000 scipion-em-3.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2257 2021-03-30 10:37:19.989638 scipion-em-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-03-30 10:31:41.000000 scipion-em-3.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.977636 scipion-em-3.0.9/pwem/
+-rw-r--r--   0 runner    (1001) docker     (121)     4916 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2113 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/bibtex.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.977636 scipion-em-3.0.9/pwem/cmd/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      382 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/cmd/chimera_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4026 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/cmd/convert.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1517 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/cmd/program.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6375 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.977636 scipion-em-3.0.9/pwem/convert/
+-rw-r--r--   0 runner    (1001) docker     (121)     1517 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37562 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/convert/atom_struct.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14159 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/convert/headers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8688 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/convert/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23840 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/convert/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    65754 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/convert/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4547 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/convert/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.977636 scipion-em-3.0.9/pwem/emlib/
+-rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/emlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29660 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/emlib/_libNone.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.977636 scipion-em-3.0.9/pwem/emlib/image/
+-rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/emlib/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21780 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/emlib/image/image_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/emlib/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.977636 scipion-em-3.0.9/pwem/emlib/metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/emlib/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11287 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/emlib/metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.977636 scipion-em-3.0.9/pwem/objects/
+-rw-r--r--   0 runner    (1001) docker     (121)     1205 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    71469 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/objects/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5562 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/objects/data_tiltpairs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.981637 scipion-em-3.0.9/pwem/protocols/
+-rw-r--r--   0 runner    (1001) docker     (121)     2454 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4142 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13672 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3902 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_2d.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3321 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_3d.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32873 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_align_movies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7445 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_alignment_assign.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4553 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_alignment_invertHand.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24488 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_batch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4585 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_classes_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15973 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_create_stream_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8052 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_ctf_assign.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.981637 scipion-em-3.0.9/pwem/protocols/protocol_export/
+-rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12107 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_export/protocol_export_DB.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16690 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_extract_coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.981637 scipion-em-3.0.9/pwem/protocols/protocol_import/
+-rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12003 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25865 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10122 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/ctfs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6057 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/dataimport.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23881 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/images.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3649 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/masks.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30302 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/micrographs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13060 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/particles.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25590 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22524 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3201 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_metadata_editor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31529 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_micrographs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21203 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_movies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7141 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_origin_sampling_volume.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25437 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_particles.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25045 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_particles_picking.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5259 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_pdf_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33673 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_sets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7736 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10282 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_tiltpairs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.981637 scipion-em-3.0.9/pwem/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     6537 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/templates/demo.json.template
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.981637 scipion-em-3.0.9/pwem/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.985637 scipion-em-3.0.9/pwem/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38693 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/data/test_convert_atom_struct.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35874 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/data/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3204 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/data/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21174 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/data/test_symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.985637 scipion-em-3.0.9/pwem/tests/protocols/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8069 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_extract_particles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6760 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6500 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocol_alignment_assign.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13157 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocol_export2DB.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2248 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocol_extract_coorinates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6065 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocol_invert_Hand.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11658 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocol_volume_homogenizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8404 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_assign_orig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9190 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_coords.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6635 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_ctfs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2295 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_masks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9168 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_micrographs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6488 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_movies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9670 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_particles.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27671 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17661 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25634 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_sets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2241 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.985637 scipion-em-3.0.9/pwem/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17332 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_parallel_gpu_queue.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1299 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14023 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_initialvolume.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12648 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_mixed.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    13743 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_mixed_large.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)   122820 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_modeling.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    11926 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4512 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp_assignment_tiltpairs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10427 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp_ctf_consensus.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5438 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp_rct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3345 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.989638 scipion-em-3.0.9/pwem/viewers/
+-rw-r--r--   0 runner    (1001) docker     (121)     2529 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6991 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/filehandlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10409 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12570 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/showj.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5254 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19582 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_chimera.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4770 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_fsc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4033 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_localres.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3026 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2893 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_vmd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7854 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10148 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewers_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2042 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewers_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16407 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.989638 scipion-em-3.0.9/pwem/wizards/
+-rw-r--r--   0 runner    (1001) docker     (121)     1200 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/wizards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49421 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/wizards/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9048 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/wizards/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2021-03-30 10:31:41.000000 scipion-em-3.0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.989638 scipion-em-3.0.9/scipion_em.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2257 2021-03-30 10:37:19.000000 scipion-em-3.0.9/scipion_em.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4460 2021-03-30 10:37:19.000000 scipion-em-3.0.9/scipion_em.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-30 10:37:19.000000 scipion-em-3.0.9/scipion_em.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2021-03-30 10:37:19.000000 scipion-em-3.0.9/scipion_em.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2021-03-30 10:37:19.000000 scipion-em-3.0.9/scipion_em.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-03-30 10:37:19.000000 scipion-em-3.0.9/scipion_em.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-30 10:37:19.989638 scipion-em-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3168 2021-03-30 10:31:41.000000 scipion-em-3.0.9/setup.py
```

### Comparing `scipion-em-3.0.8/LICENSE` & `scipion-em-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/PKG-INFO` & `scipion-em-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em
-Version: 3.0.8
+Version: 3.0.9
 Summary: This modules contains classes related with EM
 Home-page: https://github.com/scipion-em/scipion-em
 Author: J.M. De la Rosa Trevin, Roberto Marabini, Grigory Sharov, Josue Gomez Blanco, Pablo Conesa, Yunior Fonseca Reyna
 Author-email: delarosatrevin@scilifelab.se, roberto@cnb.csic.es, gsharov@mrc-lmb.cam.ac.uk, josue.gomez-blanco@mcgill.ca, pconesa@cnb.csic.es, fonsecareyna@cnb.csic.es
 License: UNKNOWN
 Description: ====
         pwem
```

### Comparing `scipion-em-3.0.8/README.rst` & `scipion-em-3.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/__init__.py` & `scipion-em-3.0.9/pwem/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from pyworkflow.wizard import Wizard
 import pyworkflow.plugin
 
 from .constants import *
 from .objects import EMObject
 from .utils import *
 
-__version__ = '3.0.8'
+__version__ = '3.0.9'
 _logo = "scipion_icon.gif"
 _references = ["delaRosaTrevin201693"]
 
 
 class Config(pw.Config):
     _get = pw.Config._get
     _join = pw.Config._join
```

### Comparing `scipion-em-3.0.8/pwem/bibtex.py` & `scipion-em-3.0.9/pwem/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/cmd/convert.py` & `scipion-em-3.0.9/pwem/cmd/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/cmd/program.py` & `scipion-em-3.0.9/pwem/cmd/program.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/constants.py` & `scipion-em-3.0.9/pwem/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/convert/__init__.py` & `scipion-em-3.0.9/pwem/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/convert/atom_struct.py` & `scipion-em-3.0.9/pwem/convert/atom_struct.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/convert/headers.py` & `scipion-em-3.0.9/pwem/convert/headers.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/convert/sequence.py` & `scipion-em-3.0.9/pwem/convert/sequence.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/convert/symmetry.py` & `scipion-em-3.0.9/pwem/convert/symmetry.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/convert/transformations.py` & `scipion-em-3.0.9/pwem/convert/transformations.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/convert/utils.py` & `scipion-em-3.0.9/pwem/convert/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/emlib/__init__.py` & `scipion-em-3.0.9/pwem/emlib/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/emlib/_libNone.py` & `scipion-em-3.0.9/pwem/emlib/_libNone.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/emlib/image/__init__.py` & `scipion-em-3.0.9/pwem/emlib/image/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/emlib/image/image_handler.py` & `scipion-em-3.0.9/pwem/emlib/image/image_handler.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/emlib/lib.py` & `scipion-em-3.0.9/pwem/emlib/lib.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/emlib/metadata/__init__.py` & `scipion-em-3.0.9/pwem/emlib/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/emlib/metadata/utils.py` & `scipion-em-3.0.9/pwem/emlib/metadata/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/objects/__init__.py` & `scipion-em-3.0.9/pwem/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/objects/data.py` & `scipion-em-3.0.9/pwem/objects/data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/objects/data_tiltpairs.py` & `scipion-em-3.0.9/pwem/objects/data_tiltpairs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/__init__.py` & `scipion-em-3.0.9/pwem/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/parallel.py` & `scipion-em-3.0.9/pwem/protocols/parallel.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol.py` & `scipion-em-3.0.9/pwem/protocols/protocol.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_2d.py` & `scipion-em-3.0.9/pwem/protocols/protocol_2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_3d.py` & `scipion-em-3.0.9/pwem/protocols/protocol_3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_align_movies.py` & `scipion-em-3.0.9/pwem/protocols/protocol_align_movies.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,22 @@
                 extraMicFn = self._getExtraPath(getOutputMicName(movie))
                 mic.setFileName(extraMicFn)
                 if not os.path.exists(extraMicFn):
                     print(pwutils.yellowStr("WARNING: Micrograph %s was not generated, "
                                             "can't add it to output set." % extraMicFn))
                     doneFailed.append(movie)
                     continue
-                self._preprocessOutputMicrograph(mic, movie)
+                # Tolerate errors here. Usually here some plots are generated.
+                try:
+                    self._preprocessOutputMicrograph(mic, movie)
+                except Exception as e:
+                    self.error("Couldn't prepare output details: %s" % e)
+                    doneFailed.append(movie)
+                    continue
+
                 micSet.append(mic)
 
             self._updateOutputSet(outputName, micSet, streamMode)
             if doneFailed:
                 self._writeFailedList(doneFailed)
 
             if firstTime:
```

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_alignment_assign.py` & `scipion-em-3.0.9/pwem/protocols/protocol_alignment_assign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_alignment_invertHand.py` & `scipion-em-3.0.9/pwem/protocols/protocol_alignment_invertHand.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_batch.py` & `scipion-em-3.0.9/pwem/protocols/protocol_batch.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_classes_consensus.py` & `scipion-em-3.0.9/pwem/protocols/protocol_classes_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_create_stream_data.py` & `scipion-em-3.0.9/pwem/protocols/protocol_create_stream_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_ctf_assign.py` & `scipion-em-3.0.9/pwem/protocols/protocol_ctf_assign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_export/__init__.py` & `scipion-em-3.0.9/pwem/protocols/protocol_export/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_export/protocol_export_DB.py` & `scipion-em-3.0.9/pwem/protocols/protocol_export/protocol_export_DB.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_extract_coordinates.py` & `scipion-em-3.0.9/pwem/protocols/protocol_extract_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_import/__init__.py` & `scipion-em-3.0.9/pwem/protocols/protocol_import/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_import/base.py` & `scipion-em-3.0.9/pwem/protocols/protocol_import/base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_import/coordinates.py` & `scipion-em-3.0.9/pwem/protocols/protocol_import/coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_import/ctfs.py` & `scipion-em-3.0.9/pwem/protocols/protocol_import/ctfs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_import/dataimport.py` & `scipion-em-3.0.9/pwem/protocols/protocol_import/dataimport.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_import/images.py` & `scipion-em-3.0.9/pwem/protocols/protocol_import/images.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_import/masks.py` & `scipion-em-3.0.9/pwem/protocols/protocol_import/masks.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_import/micrographs.py` & `scipion-em-3.0.9/pwem/protocols/protocol_import/micrographs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_import/particles.py` & `scipion-em-3.0.9/pwem/protocols/protocol_import/particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_import/sequence.py` & `scipion-em-3.0.9/pwem/protocols/protocol_import/sequence.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_import/volumes.py` & `scipion-em-3.0.9/pwem/protocols/protocol_import/volumes.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_metadata_editor.py` & `scipion-em-3.0.9/pwem/protocols/protocol_metadata_editor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_micrographs.py` & `scipion-em-3.0.9/pwem/protocols/protocol_micrographs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_movies.py` & `scipion-em-3.0.9/pwem/protocols/protocol_movies.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_origin_sampling_volume.py` & `scipion-em-3.0.9/pwem/protocols/protocol_origin_sampling_volume.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_particles.py` & `scipion-em-3.0.9/pwem/protocols/protocol_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_particles_picking.py` & `scipion-em-3.0.9/pwem/protocols/protocol_particles_picking.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_pdf_report.py` & `scipion-em-3.0.9/pwem/protocols/protocol_pdf_report.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_sets.py` & `scipion-em-3.0.9/pwem/protocols/protocol_sets.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_tests.py` & `scipion-em-3.0.9/pwem/protocols/protocol_tests.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/protocols/protocol_tiltpairs.py` & `scipion-em-3.0.9/pwem/protocols/protocol_tiltpairs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/templates/demo.json.template` & `scipion-em-3.0.9/pwem/templates/demo.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/__init__.py` & `scipion-em-3.0.9/pwem/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/data/test_convert_atom_struct.py` & `scipion-em-3.0.9/pwem/tests/data/test_convert_atom_struct.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/data/test_data.py` & `scipion-em-3.0.9/pwem/tests/data/test_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/data/test_metadata.py` & `scipion-em-3.0.9/pwem/tests/data/test_metadata.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/data/test_symmetry.py` & `scipion-em-3.0.9/pwem/tests/data/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_extract_particles.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_extract_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_notifier.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_notifier.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_protocol_alignment_assign.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_protocol_alignment_assign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_protocol_export2DB.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_protocol_export2DB.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_protocol_extract_coorinates.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_protocol_extract_coorinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_protocol_invert_Hand.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_protocol_invert_Hand.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_protocol_volume_homogenizer.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_protocol_volume_homogenizer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_protocols_assign_orig.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_assign_orig.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_coords.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_coords.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_ctfs.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_ctfs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_masks.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_masks.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_micrographs.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_micrographs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_movies.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_movies.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_particles.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_sequence.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_sequence.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_protocols_import_volumes.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_volumes.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/protocols/test_protocols_sets.py` & `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_sets.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/utils.py` & `scipion-em-3.0.9/pwem/tests/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/workflows/test_parallel_gpu_queue.py` & `scipion-em-3.0.9/pwem/tests/workflows/test_parallel_gpu_queue.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/workflows/test_workflow.py` & `scipion-em-3.0.9/pwem/tests/workflows/test_workflow.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/workflows/test_workflow_initialvolume.py` & `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_initialvolume.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/workflows/test_workflow_mixed.py` & `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_mixed.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/workflows/test_workflow_mixed_large.py` & `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_mixed_large.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/workflows/test_workflow_modeling.py` & `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_modeling.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/workflows/test_workflow_xmipp.py` & `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/workflows/test_workflow_xmipp_assignment_tiltpairs.py` & `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp_assignment_tiltpairs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/workflows/test_workflow_xmipp_ctf_consensus.py` & `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp_ctf_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/tests/workflows/test_workflow_xmipp_rct.py` & `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp_rct.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/utils.py` & `scipion-em-3.0.9/pwem/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/viewers/__init__.py` & `scipion-em-3.0.9/pwem/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/viewers/filehandlers.py` & `scipion-em-3.0.9/pwem/viewers/filehandlers.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/viewers/plotter.py` & `scipion-em-3.0.9/pwem/viewers/plotter.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/viewers/showj.py` & `scipion-em-3.0.9/pwem/viewers/showj.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/viewers/viewer_base.py` & `scipion-em-3.0.9/pwem/viewers/viewer_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/viewers/viewer_chimera.py` & `scipion-em-3.0.9/pwem/viewers/viewer_chimera.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/viewers/viewer_fsc.py` & `scipion-em-3.0.9/pwem/viewers/viewer_fsc.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/viewers/viewer_localres.py` & `scipion-em-3.0.9/pwem/viewers/viewer_localres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/viewers/viewer_pdf.py` & `scipion-em-3.0.9/pwem/viewers/viewer_pdf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/viewers/viewer_sequence.py` & `scipion-em-3.0.9/pwem/viewers/viewer_sequence.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/viewers/viewer_vmd.py` & `scipion-em-3.0.9/pwem/viewers/viewer_vmd.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/viewers/viewer_volumes.py` & `scipion-em-3.0.9/pwem/viewers/viewer_volumes.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/viewers/viewers_data.py` & `scipion-em-3.0.9/pwem/viewers/viewers_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/viewers/viewers_protocols.py` & `scipion-em-3.0.9/pwem/viewers/viewers_protocols.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/viewers/views.py` & `scipion-em-3.0.9/pwem/viewers/views.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/wizards/__init__.py` & `scipion-em-3.0.9/pwem/wizards/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/wizards/wizard.py` & `scipion-em-3.0.9/pwem/wizards/wizard.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/pwem/wizards/wizards.py` & `scipion-em-3.0.9/pwem/wizards/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/scipion_em.egg-info/PKG-INFO` & `scipion-em-3.0.9/scipion_em.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em
-Version: 3.0.8
+Version: 3.0.9
 Summary: This modules contains classes related with EM
 Home-page: https://github.com/scipion-em/scipion-em
 Author: J.M. De la Rosa Trevin, Roberto Marabini, Grigory Sharov, Josue Gomez Blanco, Pablo Conesa, Yunior Fonseca Reyna
 Author-email: delarosatrevin@scilifelab.se, roberto@cnb.csic.es, gsharov@mrc-lmb.cam.ac.uk, josue.gomez-blanco@mcgill.ca, pconesa@cnb.csic.es, fonsecareyna@cnb.csic.es
 License: UNKNOWN
 Description: ====
         pwem
```

### Comparing `scipion-em-3.0.8/scipion_em.egg-info/SOURCES.txt` & `scipion-em-3.0.9/scipion_em.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.8/setup.py` & `scipion-em-3.0.9/setup.py`

 * *Files identical despite different names*

