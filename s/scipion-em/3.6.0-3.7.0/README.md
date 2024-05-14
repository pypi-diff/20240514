# Comparing `tmp/scipion-em-3.6.0.tar.gz` & `tmp/scipion-em-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-3.6.0.tar", last modified: Fri Mar 15 12:54:45 2024, max compression
+gzip compressed data, was "scipion-em-3.7.0.tar", last modified: Tue May 14 08:22:10 2024, max compression
```

## Comparing `scipion-em-3.6.0.tar` & `scipion-em-3.7.0.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.094867 scipion-em-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-03-15 12:54:03.000000 scipion-em-3.6.0/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-15 12:54:03.000000 scipion-em-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-15 12:54:03.000000 scipion-em-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-15 12:54:45.094867 scipion-em-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-15 12:54:03.000000 scipion-em-3.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.062867 scipion-em-3.6.0/pwem/
--rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/bibtex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.062867 scipion-em-3.6.0/pwem/cmd/
--rwxr-xr-x   0 runner    (1001) docker     (127)      382 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/cmd/chimera_client.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4026 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/cmd/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/cmd/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     7697 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.066867 scipion-em-3.6.0/pwem/convert/
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45637 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/convert/atom_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    15221 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/convert/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/convert/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    51650 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/convert/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    65807 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/convert/transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/convert/trigonometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/convert/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.066867 scipion-em-3.6.0/pwem/emlib/
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/emlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29799 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/emlib/_libNone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.066867 scipion-em-3.6.0/pwem/emlib/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/emlib/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23362 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/emlib/image/image_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/emlib/image/image_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/emlib/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.066867 scipion-em-3.6.0/pwem/emlib/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/emlib/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11823 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/emlib/metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.066867 scipion-em-3.6.0/pwem/objects/
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    90731 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/objects/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/objects/data_flexhub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/objects/data_tiltpairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.074867 scipion-em-3.6.0/pwem/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    13585 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    33322 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_align_movies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_alignment_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_alignment_invertHand.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_base_flexhub.py
--rw-r--r--   0 runner    (1001) docker     (127)    29355 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_boxsize_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_boxsize_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_classes_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    18773 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_create_stream_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_ctf_assign.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.074867 scipion-em-3.6.0/pwem/protocols/protocol_export/
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16102 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_export/protocol_export_DB.py
--rw-r--r--   0 runner    (1001) docker     (127)    16631 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_extract_coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.074867 scipion-em-3.6.0/pwem/protocols/protocol_import/
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_import/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26667 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_import/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_import/ctfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_import/dataimport.py
--rw-r--r--   0 runner    (1001) docker     (127)    23705 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_import/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_import/masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    30655 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_import/micrographs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13977 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_import/particles.py
--rw-r--r--   0 runner    (1001) docker     (127)    26948 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_import/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    28278 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_import/volumes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_mathematical_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    31783 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_micrographs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_movie_eraser.py
--rw-r--r--   0 runner    (1001) docker     (127)    21511 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_movies.py
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_origin_sampling_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    25734 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_particles.py
--rw-r--r--   0 runner    (1001) docker     (127)    25337 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_particles_picking.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_pdf_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    18021 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_projection_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_set_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12652 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_set_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    36512 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    10282 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_tiltpairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols/protocol_wait.py
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/protocols.conf
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/scipion_icon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.074867 scipion-em-3.6.0/pwem/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/templates/demo.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.074867 scipion-em-3.6.0/pwem/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.082867 scipion-em-3.6.0/pwem/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  4875359 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/data/hexonAtomStruct.py
--rw-r--r--   0 runner    (1001) docker     (127)    41865 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/data/test_convert_atom_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    38585 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/data/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/data/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    49174 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/data/test_symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.086867 scipion-em-3.6.0/pwem/tests/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_angular_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_extract_particles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    60071 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_projection_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocol_alignment_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocol_boxsize_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocol_boxsize_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13968 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocol_export2DB.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocol_extract_coorinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocol_invert_Hand.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocol_mathematical_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocol_movie_eraser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11658 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocol_volume_homogenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocol_wait.py
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocols_assign_orig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_atomstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_ctfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_masks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_micrographs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_movies.py
--rw-r--r--   0 runner    (1001) docker     (127)    10826 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_particles.py
--rw-r--r--   0 runner    (1001) docker     (127)    25854 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    17661 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_volumes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocols_set_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocols_set_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    28741 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/protocols/test_protocols_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.086867 scipion-em-3.6.0/pwem/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17394 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/workflows/test_parallel_gpu_queue.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1299 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/workflows/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/workflows/test_workflow_initialvolume.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12779 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/workflows/test_workflow_mixed.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13571 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/workflows/test_workflow_mixed_large.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   123298 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/workflows/test_workflow_modeling.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11413 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/workflows/test_workflow_xmipp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4512 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/workflows/test_workflow_xmipp_assignment_tiltpairs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10427 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/workflows/test_workflow_xmipp_ctf_consensus.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5438 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/tests/workflows/test_workflow_xmipp_rct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.090867 scipion-em-3.6.0/pwem/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/filehandlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.090867 scipion-em-3.6.0/pwem/viewers/mdviewer/
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/mdviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25696 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/mdviewer/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/mdviewer/sqlite_dao.py
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/mdviewer/star_dao.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/mdviewer/viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14276 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/mdviewer/volumeViewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19553 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/showj.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/viewer_angular_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/viewer_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/viewer_chimera.py
--rw-r--r--   0 runner    (1001) docker     (127)    59344 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/viewer_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/viewer_fsc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19765 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/viewer_localres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/viewer_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/viewer_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/viewer_vmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/viewer_volumes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16064 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/viewers_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/viewers_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)    16273 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/viewers/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.090867 scipion-em-3.6.0/pwem/wizards/
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/wizards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55874 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/wizards/wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)    20253 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/wizards/wizards.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.090867 scipion-em-3.6.0/pwem/wizards/wizards_3d/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/wizards/wizards_3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/wizards/wizards_3d/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/wizards/wizards_3d/mask_structure_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-03-15 12:54:03.000000 scipion-em-3.6.0/pwem/wizards/wizards_3d/mask_volume_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-15 12:54:03.000000 scipion-em-3.6.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:45.094867 scipion-em-3.6.0/scipion_em.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-15 12:54:45.000000 scipion-em-3.6.0/scipion_em.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-03-15 12:54:45.000000 scipion-em-3.6.0/scipion_em.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 12:54:45.000000 scipion-em-3.6.0/scipion_em.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-15 12:54:45.000000 scipion-em-3.6.0/scipion_em.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-15 12:54:45.000000 scipion-em-3.6.0/scipion_em.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-15 12:54:45.000000 scipion-em-3.6.0/scipion_em.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 12:54:45.094867 scipion-em-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-03-15 12:54:03.000000 scipion-em-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.264281 scipion-em-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-05-14 08:21:02.000000 scipion-em-3.7.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-14 08:21:02.000000 scipion-em-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 08:21:02.000000 scipion-em-3.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-14 08:22:10.264281 scipion-em-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-14 08:21:02.000000 scipion-em-3.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.232281 scipion-em-3.7.0/pwem/
+-rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/bibtex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.236281 scipion-em-3.7.0/pwem/cmd/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      382 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/cmd/chimera_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4026 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/cmd/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/cmd/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7697 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.236281 scipion-em-3.7.0/pwem/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45637 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/convert/atom_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15221 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/convert/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/convert/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51650 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/convert/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65807 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/convert/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/convert/trigonometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/convert/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.236281 scipion-em-3.7.0/pwem/emlib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/emlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29799 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/emlib/_libNone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.236281 scipion-em-3.7.0/pwem/emlib/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/emlib/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23362 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/emlib/image/image_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/emlib/image/image_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/emlib/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.236281 scipion-em-3.7.0/pwem/emlib/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/emlib/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11823 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/emlib/metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.240281 scipion-em-3.7.0/pwem/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90823 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/objects/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/objects/data_flexhub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/objects/data_tiltpairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.244281 scipion-em-3.7.0/pwem/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13585 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33322 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_align_movies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_alignment_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_alignment_invertHand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_base_flexhub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29355 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_boxsize_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_boxsize_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_classes_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18773 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_create_stream_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_ctf_assign.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.244281 scipion-em-3.7.0/pwem/protocols/protocol_export/
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16102 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_export/protocol_export_DB.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16631 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_extract_coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.248281 scipion-em-3.7.0/pwem/protocols/protocol_import/
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12035 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_import/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27637 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_import/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_import/ctfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_import/dataimport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23705 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_import/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_import/masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31690 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_import/micrographs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13977 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_import/particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26948 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_import/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28278 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_import/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_mathematical_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31783 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_micrographs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_movie_eraser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21511 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_movies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_origin_sampling_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26127 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25337 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_particles_picking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_pdf_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18021 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_projection_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_set_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12652 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_set_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44330 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10282 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_tiltpairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols/protocol_wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/protocols.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/scipion_icon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.248281 scipion-em-3.7.0/pwem/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/templates/demo.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.248281 scipion-em-3.7.0/pwem/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.252281 scipion-em-3.7.0/pwem/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4875359 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/data/hexonAtomStruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41865 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/data/test_convert_atom_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38585 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/data/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/data/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49174 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/data/test_symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.256281 scipion-em-3.7.0/pwem/tests/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_angular_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_extract_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60071 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_projection_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocol_alignment_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocol_boxsize_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocol_boxsize_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13968 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocol_export2DB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocol_extract_coorinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocol_invert_Hand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocol_mathematical_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocol_movie_eraser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11658 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocol_volume_homogenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocol_wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocols_assign_orig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_atomstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_ctfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_micrographs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_movies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10826 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25854 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17661 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocols_set_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocols_set_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28741 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/protocols/test_protocols_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.260281 scipion-em-3.7.0/pwem/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17394 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/workflows/test_parallel_gpu_queue.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1299 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/workflows/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/workflows/test_workflow_initialvolume.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12779 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/workflows/test_workflow_mixed.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13571 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/workflows/test_workflow_mixed_large.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   123298 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/workflows/test_workflow_modeling.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11413 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/workflows/test_workflow_xmipp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4512 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/workflows/test_workflow_xmipp_assignment_tiltpairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10427 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/workflows/test_workflow_xmipp_ctf_consensus.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5438 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/tests/workflows/test_workflow_xmipp_rct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.260281 scipion-em-3.7.0/pwem/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/filehandlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.264281 scipion-em-3.7.0/pwem/viewers/mdviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/mdviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26527 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/mdviewer/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/mdviewer/sqlite_dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/mdviewer/star_dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/mdviewer/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14276 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/mdviewer/volumeViewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19553 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/showj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/viewer_angular_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/viewer_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20779 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/viewer_chimera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59096 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/viewer_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/viewer_fsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19750 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/viewer_localres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/viewer_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/viewer_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/viewer_vmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/viewer_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16064 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/viewers_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/viewers_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16273 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/viewers/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.264281 scipion-em-3.7.0/pwem/wizards/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/wizards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55889 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/wizards/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20253 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/wizards/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.264281 scipion-em-3.7.0/pwem/wizards/wizards_3d/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/wizards/wizards_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/wizards/wizards_3d/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/wizards/wizards_3d/mask_structure_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-14 08:21:02.000000 scipion-em-3.7.0/pwem/wizards/wizards_3d/mask_volume_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 08:21:02.000000 scipion-em-3.7.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:22:10.264281 scipion-em-3.7.0/scipion_em.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-14 08:22:10.000000 scipion-em-3.7.0/scipion_em.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-05-14 08:22:10.000000 scipion-em-3.7.0/scipion_em.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:22:10.000000 scipion-em-3.7.0/scipion_em.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-14 08:22:10.000000 scipion-em-3.7.0/scipion_em.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 08:22:10.000000 scipion-em-3.7.0/scipion_em.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 08:22:10.000000 scipion-em-3.7.0/scipion_em.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:22:10.264281 scipion-em-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-14 08:21:02.000000 scipion-em-3.7.0/setup.py
```

### Comparing `scipion-em-3.6.0/CHANGES.txt` & `scipion-em-3.7.0/CHANGES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+V3.7.0:
+  Users:
+     - Allowing drag and drop a coordinate when picking
+     - Allowing to create subsets from the selection in the metadataviewer plotter
+     - Fixing an error creating subset through new metadataviewer
+     - NEW PROTOCOL - Crossed subset protocol: Creates a subset of the main set based on a matching field in another set.
+     - ChimeraX resolution viewer compatible with WSL.
+     - Fix: Wizard for choosing a Mask radius returns integer.
+     - Describes better and register variables for the new GUI to edit variables
+     - NEW PROTOCOL - data summary: Aggregates (COUNT, MAX, MIN, AVG) any set data based on its fields
+     - Importing coordinates from cryoSPARC
+     - Fix: The coordinate viewer shows the complete list of micrographs when a subset has been generated and there are only coordinates for some micrographs in this subset
+     - Allows to run the whole workflow until 3D processing with trigger points
+     - Allowing the use of a pattern for the import of the gain file.
+
+Developers:
+     - Plugin._defineVar and _defineEmVar offers  description(str) and  varType(VarTypes) as optional arguments to better describe the variable devel
+     - Modify the finishing condition of the parent protocol "extract particles". Now, it checks if the input coords are closed and if all mics and CTFs have been processed.
+
 V3.6.0:
   Users:
      - Adapted to Sprites
      - Add a new 2D coordinate viewer
      - 2 level sets (like tilt series) copy enable flag in subitems when subsetting.
 
   Developers:
```

### Comparing `scipion-em-3.6.0/LICENSE` & `scipion-em-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/PKG-INFO` & `scipion-em-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em
-Version: 3.6.0
+Version: 3.7.0
 Summary: This modules contains classes related with EM
 Home-page: https://github.com/scipion-em/scipion-em
 Author: J.M. De la Rosa Trevin, Roberto Marabini, Grigory Sharov, Josue Gomez Blanco, Pablo Conesa, Yunior Fonseca Reyna
 Author-email: delarosatrevin@scilifelab.se, roberto@cnb.csic.es, gsharov@mrc-lmb.cam.ac.uk, josue.gomez-blanco@mcgill.ca, pconesa@cnb.csic.es, fonsecareyna@cnb.csic.es
 License: UNKNOWN
 Description: .. image:: https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg
           :width: 200
```

### Comparing `scipion-em-3.6.0/README.rst` & `scipion-em-3.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/__init__.py` & `scipion-em-3.7.0/pwem/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 """
 This module contains classes related with EM
 """
 import logging
+
+from pyworkflow import VarTypes
+
 logger = logging.getLogger(__name__)
 import os
 import re
 from pkg_resources import parse_version
 
 import pyworkflow as pw
 from pyworkflow.protocol import Protocol
@@ -40,49 +43,55 @@
 import pyworkflow.plugin
 
 from .constants import *
 from .objects import EMObject
 from .tests import defineDatasets
 from .utils import *
 
-__version__ = '3.6.0'
+__version__ = '3.7.0'
 NO_VERSION_FOUND_STR = "0.0"
 CUDA_LIB_VAR = 'CUDA_LIB'
 
 _logo = "scipion_icon.png"
 _references = ["delaRosaTrevin201693"]
 
 
 class Config(pw.Config):
     _get = pw.Config._get
     _join = pw.Config._join
 
     EM_ROOT = _join(_get(EM_ROOT_VAR, _join(pw.Config.SCIPION_SOFTWARE, 'em')))
 
     # Default XMIPP_HOME: needed here for ShowJ viewers
-    XMIPP_HOME = _join(_get('XMIPP_HOME', os.path.join(EM_ROOT, 'xmipp')))
+    XMIPP_HOME = _join(_get('XMIPP_HOME', _join(EM_ROOT, 'xmipp'),
+                            description="Path where XMIPP is installed.",
+                            var_type=VarTypes.FOLDER,
+                            source="pwem"))
 
     # Get java home, we might need to provide correct default value. Use SCIPION_JAVA_HOME to force it when there is other JAVA_HOME you don't want/cant to change: e.g. pycharm debugging.
-    JAVA_HOME = _get('SCIPION_JAVA_HOME', _get('JAVA_HOME', ''))
-    JAVA_MAX_MEMORY = _get('JAVA_MAX_MEMORY', '4')
+    JAVA_HOME = _get('SCIPION_JAVA_HOME', _get('JAVA_HOME', ''),
+                     description="Path where JAVA is located.", var_type=VarTypes.FOLDER, source="pwem")
+    JAVA_MAX_MEMORY = _get('JAVA_MAX_MEMORY', '4', description="Memory (in GB) to use in java processes. For movies it will be increased. Used in Xmipp viewer.", var_type=VarTypes.INTEGER, source="pwem")
 
     # MPI
     MPI_LIBDIR = _get('MPI_LIBDIR', '/usr/lib64/mpi/gcc/openmpi/lib')
     MPI_BINDIR = _get('MPI_BINDIR', '/usr/lib64/mpi/gcc/openmpi/bin')
 
     # CUDA
     CUDA_LIB = _get(CUDA_LIB_VAR, '/usr/local/cuda/lib64')
     CUDA_BIN = _get('CUDA_BIN', '/usr/local/cuda/bin')
-    MAX_PREVIEW_FILE_SIZE = float(_get("MAX_PREVIEW_FILE_SIZE", DEFAULT_MAX_PREVIEW_FILE_SIZE))
+
+
+    MAX_PREVIEW_FILE_SIZE = float(_get("MAX_PREVIEW_FILE_SIZE", DEFAULT_MAX_PREVIEW_FILE_SIZE, description="Maximum size (MB) of files to visualize in the file browser preview."))
 
     # OLD CHIMERA variable
-    CHIMERA_OLD_BINARY_PATH = _get("CHIMERA_OLD_BINARY_PATH",'')
+    CHIMERA_OLD_BINARY_PATH = _get("CHIMERA_OLD_BINARY_PATH",'',description="Path to the Chimera OLD binary program (not the folder). Will only be used a viewer. None of the chimera scripts will work.", var_type=VarTypes.PATH, source="pwem")
 
     # Path to either ImageJ or Fiji binary program
-    IMAGEJ_BINARY_PATH = _get("IMAGEJ_BINARY_PATH",'')
+    IMAGEJ_BINARY_PATH = _get("IMAGEJ_BINARY_PATH",'',description="Path to the IMAGEJ or FIJI program.", var_type=VarTypes.PATH, source="pwem")
 
 
 class Domain(pyworkflow.plugin.Domain):
     _name = __name__
     _objectClass = EMObject
     _protocolClass = Protocol
     _viewerClass = Viewer
@@ -90,50 +99,64 @@
     _baseClasses = getSubclasses(EMObject, globals())
 
 
 class Plugin(pyworkflow.plugin.Plugin):
     _url = URL
 
     @classmethod
-    def _defineEmVar(cls, varName, defaultValue):
+    def _defineEmVar(cls, varName, defaultValue, description="Missing", var_type:VarTypes=None):
         """ Shortcut method to define variables prepending EM_ROOT if variable is not absolute"""
 
         # Get the value, either whatever is in the environment or a join of EM_ROOT + defaultValue
-        value = os.environ.get(varName, os.path.join(Config.EM_ROOT, defaultValue))
+        defaultValueWithEM= os.path.join(Config.EM_ROOT,defaultValue)
+
+        value = os.environ.get(varName, defaultValueWithEM)
+
+        def expand(value):
+
+
+            # CASE-1 : Users might have used ~ and that has to be expanded
+            value = os.path.expanduser(value)
+
+            # CASE-2 :Old configs 2.0 will likely have:
+            # EM_ROOT = software/em
+            # CHIMERA_HOME = %(EM_ROOT)s/chimera-13.0.1
+            #  ...
+            #
+            # this end up in the environment resolved like: software/em/chimera-13.0.1
+            # whereas as default values will come as absolute:
+            # /<scipion_home>/software/em/chimera-13.0.1
+            # In any case we join it (absolute paths will not join)
+            value = os.path.join(pw.Config.SCIPION_HOME, value)
+
+            return value
 
-        # CASE-1 : Users might have used ~ and that has to be expanded
-        value = os.path.expanduser(value)
+        value=expand(value)
 
-        # CASE-2 :Old configs 2.0 will likely have:
-        # EM_ROOT = software/em
-        # CHIMERA_HOME = %(EM_ROOT)s/chimera-13.0.1
-        #  ...
-        #
-        # this end up in the environment resolved like: software/em/chimera-13.0.1
-        # whereas as default values will come as absolute:
-        # /<scipion_home>/software/em/chimera-13.0.1
-        # In any case we join it (absolute paths will not join)
-        value = os.path.join(pw.Config.SCIPION_HOME, value)
+        if varName in os.environ:
+            defaultValue= expand(defaultValueWithEM)
+        else:
+            defaultValue=value
 
-        cls._addVar(varName, value)
+        cls._addVar(varName, value, defaultValue, description=description, var_type=var_type)
 
     @classmethod
     def getMaxitHome(cls):
         return cls.getVar(MAXIT_HOME)
 
     @classmethod
     def getMaxitBin(cls):
         return os.path.join(cls.getMaxitHome(), 'bin', MAXIT)
 
     @classmethod
     def _defineVariables(cls):
         # Avoid defining variables from children that does not define variables.
         if cls == Plugin:
             cls._defineVar(EM_ROOT_VAR, pwem.Config.EM_ROOT)
-            cls._defineEmVar(MAXIT_HOME, 'maxit-10.1')
+            cls._defineEmVar(MAXIT_HOME, 'maxit-10.1', description="Path where maxit is installed.", var_type=VarTypes.FOLDER)
 
             # Take this initialization event to define own datasets
             defineDatasets()
             # Register filehandlers too
             cls._registerFileHandlers()
 
     @classmethod
```

### Comparing `scipion-em-3.6.0/pwem/bibtex.py` & `scipion-em-3.7.0/pwem/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/cmd/convert.py` & `scipion-em-3.7.0/pwem/cmd/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/cmd/program.py` & `scipion-em-3.7.0/pwem/cmd/program.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/constants.py` & `scipion-em-3.7.0/pwem/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/convert/__init__.py` & `scipion-em-3.7.0/pwem/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/convert/atom_struct.py` & `scipion-em-3.7.0/pwem/convert/atom_struct.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/convert/headers.py` & `scipion-em-3.7.0/pwem/convert/headers.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/convert/sequence.py` & `scipion-em-3.7.0/pwem/convert/sequence.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/convert/symmetry.py` & `scipion-em-3.7.0/pwem/convert/symmetry.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/convert/transformations.py` & `scipion-em-3.7.0/pwem/convert/transformations.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/convert/trigonometry.py` & `scipion-em-3.7.0/pwem/convert/trigonometry.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/convert/utils.py` & `scipion-em-3.7.0/pwem/convert/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/emlib/__init__.py` & `scipion-em-3.7.0/pwem/emlib/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/emlib/_libNone.py` & `scipion-em-3.7.0/pwem/emlib/_libNone.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/emlib/image/__init__.py` & `scipion-em-3.7.0/pwem/emlib/image/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/emlib/image/image_handler.py` & `scipion-em-3.7.0/pwem/emlib/image/image_handler.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/emlib/image/image_readers.py` & `scipion-em-3.7.0/pwem/emlib/image/image_readers.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/emlib/lib.py` & `scipion-em-3.7.0/pwem/emlib/lib.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/emlib/metadata/__init__.py` & `scipion-em-3.7.0/pwem/emlib/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/emlib/metadata/utils.py` & `scipion-em-3.7.0/pwem/emlib/metadata/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/objects/__init__.py` & `scipion-em-3.7.0/pwem/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/objects/data.py` & `scipion-em-3.7.0/pwem/objects/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1619,15 +1619,15 @@
         return self._coordsPointer.get()
     def getIsSubparticles(self):
         return self._isSubParticles
     def setIsSubparticles(self, value):
         self._isSubParticles = Boolean(value)
 
     def setCoordinates(self, coordinates):
-        """ Set the SetOfCoordinates associates with
+        """ Set the SetOfCoordinates associated with
         this set of particles.
          """
         if coordinates.isPointer():
             self._coordsPointer.copy(coordinates)
         else:
             self._coordsPointer.set(coordinates)
 
@@ -2676,7 +2676,11 @@
         resolution = below_res - ((threshold-below_fsc)/(above_fsc-below_fsc) * (below_res-above_res))
         return "{0:.1f}".format(1/resolution)
 
 
 class SetOfFSCs(EMSet):
     """Represents a set of FSCs"""
     ITEM_TYPE = FSC
+
+class SetOfStats(EMSet):
+    """Represents lines of data elements"""
+    ITEM_TYPE = Object
```

### Comparing `scipion-em-3.6.0/pwem/objects/data_flexhub.py` & `scipion-em-3.7.0/pwem/objects/data_flexhub.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/objects/data_tiltpairs.py` & `scipion-em-3.7.0/pwem/objects/data_tiltpairs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/__init__.py` & `scipion-em-3.7.0/pwem/protocols/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 from .protocol_pdf_report import *
 from .protocol_tiltpairs import *
 from .protocol_ctf_assign import ProtCTFAssign
 from .protocol_alignment_assign import ProtAlignmentAssign
 from .protocol_alignment_invertHand import ProtAlignmentInvertHand
 from .protocol_batch import *
 from .protocol_extract_coordinates import ProtExtractCoords
-#from .protocol_extract_subparticles_coordinates import ProtExtractSubparticlesCoords
 
 from .protocol_create_stream_data import ProtCreateStreamData
 from .parallel import ProtTestParallel
 from .protocol_create_stream_data import SET_OF_RANDOM_MICROGRAPHS
 
 from .protocol_import import *
```

### Comparing `scipion-em-3.6.0/pwem/protocols/parallel.py` & `scipion-em-3.7.0/pwem/protocols/parallel.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol.py` & `scipion-em-3.7.0/pwem/protocols/protocol.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_2d.py` & `scipion-em-3.7.0/pwem/protocols/protocol_2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_3d.py` & `scipion-em-3.7.0/pwem/protocols/protocol_3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_align_movies.py` & `scipion-em-3.7.0/pwem/protocols/protocol_align_movies.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_alignment_assign.py` & `scipion-em-3.7.0/pwem/protocols/protocol_alignment_assign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_alignment_invertHand.py` & `scipion-em-3.7.0/pwem/protocols/protocol_alignment_invertHand.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_base_flexhub.py` & `scipion-em-3.7.0/pwem/protocols/protocol_base_flexhub.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_batch.py` & `scipion-em-3.7.0/pwem/protocols/protocol_batch.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_boxsize_checkpoint.py` & `scipion-em-3.7.0/pwem/protocols/protocol_boxsize_checkpoint.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_boxsize_parameters.py` & `scipion-em-3.7.0/pwem/protocols/protocol_boxsize_parameters.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_classes_selector.py` & `scipion-em-3.7.0/pwem/protocols/protocol_classes_selector.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_create_stream_data.py` & `scipion-em-3.7.0/pwem/protocols/protocol_create_stream_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_ctf_assign.py` & `scipion-em-3.7.0/pwem/protocols/protocol_ctf_assign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_export/__init__.py` & `scipion-em-3.7.0/pwem/protocols/protocol_export/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_export/protocol_export_DB.py` & `scipion-em-3.7.0/pwem/protocols/protocol_export/protocol_export_DB.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_extract_coordinates.py` & `scipion-em-3.7.0/pwem/protocols/protocol_extract_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_import/__init__.py` & `scipion-em-3.7.0/pwem/protocols/protocol_import/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_import/base.py` & `scipion-em-3.7.0/pwem/protocols/protocol_import/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from os.path import join
 from glob import glob
 import re
 from datetime import datetime
 
 import pyworkflow.utils as pwutils
 import pyworkflow.protocol.params as params
+from pwem import getMatchingFiles
 
 from pwem.protocols import EMProtocol
 
 
 class ProtImport(EMProtocol):
     """ Base class for other all Import protocols. """
 
@@ -223,16 +224,15 @@
     def getMatchFiles(self, pattern=None):
         """ Return a sorted list with the paths of files that
         matched the pattern.
         """
         if pattern is None:
             pattern = self.getPattern()
 
-        filePaths = glob(pattern)
-        filePaths.sort()
+        filePaths = getMatchingFiles(pattern, sort=True)
         self.numberOfFiles = len(filePaths)
 
         return filePaths
 
     def getCopyOrLink(self):
         # Set a function to copyFile or createLink
         # depending in the user selected option
```

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_import/coordinates.py` & `scipion-em-3.7.0/pwem/protocols/protocol_import/coordinates.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,23 +52,24 @@
 
     IMPORT_FROM_AUTO = 0
     IMPORT_FROM_XMIPP = 1
     IMPORT_FROM_RELION = 2
     IMPORT_FROM_EMAN = 3
     IMPORT_FROM_DOGPICKER = 4
     IMPORT_FROM_SCIPION = 5
+    IMPORT_FROM_CRYOSPARC = 6
 
     OUTPUT_NAME='outputCoordinates'
 
     def _getImportChoices(self):
         """ Return a list of possible choices
         from which the import can be done.
         (usually packages formats such as: xmipp3, eman2, relion...etc.
         """
-        return ['auto', 'xmipp', 'relion', 'eman', 'dogpicker', 'scipion']
+        return ['auto', 'xmipp', 'relion', 'eman', 'dogpicker', 'scipion', 'cryosparc']
 
     def _getDefaultChoice(self):
         return self.IMPORT_FROM_AUTO
 
     def _getFilesCondition(self):
         """ Return an string representing the condition
         when to display the files path and pattern to grab
@@ -100,28 +101,37 @@
                       condition='importFrom!=%d' % self.IMPORT_FROM_SCIPION,
                       label='Invert Y',
                       help='Invert Y for EMAN coordinates taken on dm3 or'
                            ' tif micrographs')
 
     # ------------------- INSERT steps functions ------------------------------
     def _insertAllSteps(self):
-        importFrom = self.importFrom.get()
-        self._insertFunctionStep('createOutputStep', importFrom,
+        self._insertFunctionStep(self.createOutputStep,
+                                 self.getImportFrom(),
                                  self.filesPath.get())
 
     # ------------------ STEPS functions --------------------------------------
     def createOutputStep(self, importFrom, *args):
 
         # scipion imports have a predefined format (see dataimport)
         if importFrom == self.IMPORT_FROM_SCIPION:
             from .dataimport import ScipionImport
             self.importFilePath = self.filesPath.get('').strip()
             sImport = ScipionImport(self, self.importFilePath)
             # this function defines outputs and relations
             sImport.importCoordinates(self.inputMicrographs)
+
+        elif importFrom in [self.IMPORT_FROM_CRYOSPARC,
+                            self.IMPORT_FROM_RELION]:
+            ci = self.getImportClass()
+            coordsSet = ci.importCoordinates()
+            coordsSet.setBoxSize(self.boxSize.get())
+            self._defineOutputs(**{self.OUTPUT_NAME: coordsSet})
+            self._defineSourceRelation(self.inputMicrographs, coordsSet)
+
         else:
             # Pass the pointer with extended.
             coordsSet = self._createSetOfCoordinates(self.inputMicrographs)
             coordsSet.setBoxSize(self.boxSize.get())
             ci = self.getImportClass()
             for coordFile, fileId in self.iterFiles():
                 mic = self.getMatchingMic(coordFile, fileId)
@@ -189,14 +199,21 @@
         elif importFrom == self.IMPORT_FROM_DOGPICKER:
             DogpickerImport = Domain.importFromPlugin('appion.convert', 'DogpickerImport',
                                                       errorMsg='appion plugin is needed to import '
                                                                'dogpicker files',
                                                       doRaise=True)
             return DogpickerImport(self)
 
+        elif importFrom == self.IMPORT_FROM_CRYOSPARC:
+            cryoSPARCImport = Domain.importFromPlugin('cryosparc2.convert', 'cryoSPARCImport',
+                                                      'cryoSPARC is needed to import .cs files',
+                                                      doRaise=True)
+            self.importFilePath = self.filesPath.get('').strip()
+            return cryoSPARCImport(self, self.importFilePath)
+
         else:
             self.importFilePath = ''
             return None
 
     def getImportFrom(self):
         importFrom = self.importFrom.get()
         if importFrom == self.IMPORT_FROM_AUTO:
@@ -207,14 +224,16 @@
         for coordFile, _ in self.iterFiles():
             if coordFile.endswith('.pos'):
                 return self.IMPORT_FROM_XMIPP
             if coordFile.endswith('.star'):
                 return self.IMPORT_FROM_RELION
             if coordFile.endswith('.json') or coordFile.endswith('.box'):
                 return self.IMPORT_FROM_EMAN
+            if coordFile.endswith('.cs'):
+                return self.IMPORT_FROM_CRYOSPARC
         return -1
 
     def getInputMicrographs(self):
         return self.inputMicrographs.get()
 
     def getMatchingMic(self, coordFile, fileId):
         """ Given a coordinates file check if there is a micrograph
```

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_import/ctfs.py` & `scipion-em-3.7.0/pwem/protocols/protocol_import/ctfs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_import/dataimport.py` & `scipion-em-3.7.0/pwem/protocols/protocol_import/dataimport.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_import/images.py` & `scipion-em-3.7.0/pwem/protocols/protocol_import/images.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_import/masks.py` & `scipion-em-3.7.0/pwem/protocols/protocol_import/masks.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_import/micrographs.py` & `scipion-em-3.7.0/pwem/protocols/protocol_import/micrographs.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,21 @@
 # *
 # **************************************************************************
 import enum
 import os
 from os.path import join, basename
 import re
 from datetime import timedelta, datetime
+import logging
+logger = logging.getLogger(__name__)
 
 import pyworkflow.utils as pwutils
 import pyworkflow.protocol.params as params
 
-from pwem import Domain
+from pwem import Domain, getMatchingFiles
 from pwem.emlib.image import ImageHandler
 import pwem.constants as emcts
 
 from .images import ProtImportImages
 from ...objects import SetOfMicrographs, SetOfMovies
 
 
@@ -442,14 +444,16 @@
     _possibleOutputs = ImportMoviesOutput
     _outputClassName = ImportMoviesOutput.outputMovies.value.__name__
 
     def __init__(self, **kwargs):
         ProtImportMicBase.__init__(self, **kwargs)
         self.serverSocket = None
         self.connectionList = None
+        self.gain = -1
+        self.dark = -1
 
     def _getBlacklistSetClass(self):
         """ Returns the class to be blacklisted by this protocol.
         """
         return "SetOfMovies"
 
     def _defineAcquisitionParams(self, form):
@@ -554,25 +558,54 @@
 
         errors = ProtImportMicBase._validate(self)
         if self.inputIndividualFrames and not self.stackFrames:
             errors.append("Scipion does not support individual frames. "
                           "You must set to Yes *Create movie stacks?* "
                           "parameter.")
 
-        if not self.gainFile.empty() and not os.path.exists(self.gainFile.get()):
-            errors.append("Gain file not found in " + str(self.gainFile.get()))
-        if not self.darkFile.empty() and not os.path.exists(self.darkFile.get()):
-            errors.append("Dark file not found in " + str(self.gainFile.get()))
+        #  Using getMatchFile to find a file that matches with the given pattern.In case it is empty, the
+        #  validation fails, otherwise the first file that matches is returned.
+        if not self.gainFile.empty():
+            if not self.getGain():
+                errors.append("There is no file that corresponds to the gain file " + str(self.gainFile.get()))
+            else:
+                logger.info("It has been used as a gain file: %s" % self.getGain())
+
+        if not self.darkFile.empty():
+
+            if not self.getDark():
+                errors.append("There is no file that corresponds to the dark file " + str(self.darkFile.get()))
+            else:
+               logger.info("It has been used as a dark file: %s" % self.getDark())
+
         return errors
 
+    def getGain(self):
+        if self.gain == -1:
+            self.gain = self.getGainOrDark(self.gainFile)
+        return self.gain
+
+    def getDark(self):
+        if self.dark == -1:
+            self.dark = self.getGainOrDark(self.darkFile)
+        return self.dark
+
+    def getGainOrDark(self, path):
+        if path.empty():
+            return None
+        matchinFiles = getMatchingFiles(path.get())
+        if not matchinFiles:
+            return None
+        return matchinFiles[0]
+
     # --------------------------- UTILS functions ------------------------------
     def setSamplingRate(self, movieSet):
         ProtImportMicBase.setSamplingRate(self, movieSet)
-        movieSet.setGain(self.gainFile.get())
-        movieSet.setDark(self.darkFile.get())
+        movieSet.setGain(self.getGain())
+        movieSet.setDark(self.getDark())
         acq = movieSet.getAcquisition()
         acq.setDoseInitial(self.doseInitial.get())
         acq.setDosePerFrame(self.dosePerFrame.get())
 
     def _setupFirstImage(self, movie, imgSet):
         # Create a movie object to read dimensions
         dimMovie = movie.clone()
```

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_import/particles.py` & `scipion-em-3.7.0/pwem/protocols/protocol_import/particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_import/sequence.py` & `scipion-em-3.7.0/pwem/protocols/protocol_import/sequence.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_import/volumes.py` & `scipion-em-3.7.0/pwem/protocols/protocol_import/volumes.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_mathematical_operator.py` & `scipion-em-3.7.0/pwem/protocols/protocol_mathematical_operator.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_micrographs.py` & `scipion-em-3.7.0/pwem/protocols/protocol_micrographs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_movie_eraser.py` & `scipion-em-3.7.0/pwem/protocols/protocol_movie_eraser.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_movies.py` & `scipion-em-3.7.0/pwem/protocols/protocol_movies.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_origin_sampling_volume.py` & `scipion-em-3.7.0/pwem/protocols/protocol_origin_sampling_volume.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_particles.py` & `scipion-em-3.7.0/pwem/protocols/protocol_particles.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,15 +309,24 @@
         particles.
          Should be implemented in derived classes.
         """
         return False
 
     # ------ Methods for Streaming extraction --------------
     def _isStreamClosed(self):
-        return self.micsClosed and self.ctfsClosed and self.coordsClosed
+        return self.coordsClosed
+
+    def _areAllMicsProcessed(self):
+        """
+        This condition determines if the processing is complete when all the micrographs associated
+        with the input coordinates have been processed.
+        """
+        currentPicsMics = self.inputCoordinates.get().getUniqueValues("_micName")
+
+        return len(self.micDict) == len(currentPicsMics)
 
     def _stepsCheck(self):
         # To allow streaming picking we need to detect:
         #   1) new micrographs ready to be picked
         #   2) new output coordinates that have been produced and add then
         #      to the output set.
         self._checkNewInput()
@@ -515,15 +524,16 @@
                    % (inputLen, len(doneList), len(newDone)))
 
         firstTime = len(doneList) == 0
         allDone = len(doneList) + len(newDone)
         # We have finished when there is not more input mics (stream closed)
         # and the number of processed mics is equal to the number of inputs
         streamClosed = self._isStreamClosed()
-        self.finished = streamClosed and allDone == inputLen
+        allMicsProcessed = self._areAllMicsProcessed()
+        self.finished = streamClosed and allDone == inputLen and allMicsProcessed
         self.debug(' is finished? %s ' % self.finished)
         self.debug(' is stream closed? %s ' % streamClosed)
         streamMode = pwobj.Set.STREAM_CLOSED if self.finished else pwobj.Set.STREAM_OPEN
 
         if newDone:
             self._updateOutputPartSet(newDone, streamMode)
             self._writeDoneList(newDone)
```

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_particles_picking.py` & `scipion-em-3.7.0/pwem/protocols/protocol_particles_picking.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_pdf_report.py` & `scipion-em-3.7.0/pwem/protocols/protocol_pdf_report.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_projection_edit.py` & `scipion-em-3.7.0/pwem/protocols/protocol_projection_edit.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_set_editor.py` & `scipion-em-3.7.0/pwem/protocols/protocol_set_editor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_set_filter.py` & `scipion-em-3.7.0/pwem/protocols/protocol_set_filter.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_sets.py` & `scipion-em-3.7.0/pwem/protocols/protocol_sets.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,19 +31,18 @@
 ... etc
 """
 
 import random
 import sys
 
 import pyworkflow.protocol as pwprot
-import pyworkflow.object as pwobj
+from pyworkflow.object import Object,Float, Integer, String
 
-import pwem.objects as emobj
 from pwem.protocols import EMProtocol
-from pwem.objects import Volume, EMSet
+from pwem.objects import Volume, EMSet, SetOfClasses, SetOfStats
 from pyworkflow.utils import ProgressBar, getListFromRangeString
 
 
 class ProtSets(EMProtocol):
     """ Base class for all protocols related to subsets. """
 
     def _append(self, outputSet, item, sourceItem=None):
@@ -313,15 +312,15 @@
     # -------------------------- INFO functions -------------------------------
     def _validate(self):
         # Are all inputSets from the same class?
         classes = {x.get().getClassName() for x in self.inputSets}
         if len(classes) > 1:
             return ["All objects should have the same type.",
                     "Types of objects found: %s" % ", ".join(classes)]
-        if issubclass(type(self.inputSets[0].get()), emobj.SetOfClasses):
+        if issubclass(type(self.inputSets[0].get()), SetOfClasses):
             return ["Is not possible to join different sets of classes.\n"
                     "If you want to join different representative, extract them "
                     "with the viewer and them run this protocol with the "
                     "resulting averages."]
 
         # Validate attributes like sampling rate or dimensions
         return self._checkSetsCompatibility()
@@ -387,15 +386,15 @@
                                 "attributes:" % index)
                 for attr in lostAttributes:
                     warnings.append(attr)
 
         if len(warnings):
             warnings.append("Your input sets have different attributes. "
                             "We will keep only the common ones. This may "
-                            "cause the lost of important data like CFT, "
+                            "cause the lost of important data like CTF, "
                             "alignment information,...")
 
         return  warnings
 
     def _summary(self):
         if not hasattr(self, 'outputSet'):
             return ["Protocol has not finished yet."]
@@ -866,7 +865,206 @@
             summary = ["Protocol has not finished yet."]
         else:
             summary = ['A subset of *%d* particles is made from a total of *%d*'
                        ' particles.' % (self.outputParticles.getSize(),
                                         self.inputParticles.get().getSize())]
         return summary
 
+class ProtCrossSubSet(ProtSets):
+    """
+    Create a subset of the main set based on a matching field in another set. e.g.: Use _micName field (in both fields)
+    to select micrographs (main set) present in a set of coordinates (secondary set)
+    """
+    _label = 'Crossed subset'
+
+    # --------------------------- DEFINE param functions ----------------------
+    def _defineParams(self, form):
+        form.addSection(label='Input')
+
+        add = form.addParam  # short notation
+        add('mainSet', pwprot.params.PointerParam,
+            pointerClass='EMSet', label="Main set",
+            help='Set to be reduced')
+
+        add('mainSetField', pwprot.params.StringParam,
+            label='Main field', default="id",
+            help='Field in the main set that contains the values in common with the secondary set. Use any of the metadata viewers to find the field name.')
+
+        add('secSet', pwprot.params.PointerParam,
+            pointerClass='EMSet', label="Secondary set",
+            help='Set holding the matching field. e.g: Set of Coordinates hold the micName that can be used to filter a set of micrographs (main set)')
+
+        add('secSetField', pwprot.params.StringParam,
+            label='Secondary field', default="id",
+            help='Field in the secondary set that contains the values in common with the main set. Use any of the metadata viewers to find the field name.')
+
+
+    # --------------------------- INSERT steps functions ----------------------
+    def _insertAllSteps(self):
+        # These arguments are mainly for skipping the step if they are the same in the resume execution.
+        self._insertFunctionStep(self.createOutputStep,
+                                 self.mainSet.getObjId(),
+                                 self.secSet.getObjId(),
+                                 self.mainSetField.get(),
+                                 self.secSetField.get())
+
+    # --------------------------- STEPS functions -----------------------------
+    def createOutputStep(self, mainId, secId, mainSetField, secSetField):
+        mainSet = self.mainSet.get()
+        secSet = self.secSet.get()
+
+        # Instantiate and copy main properties
+        outputSet = mainSet.create(self.getPath())
+        outputSet.copyInfo(mainSet)
+
+        # Get unique values of secfield in secset
+        uniqueValuesinSec = secSet.getUniqueValues(secSetField)
+        uniqueValuesinSec ={value:None for value in uniqueValuesinSec}
+
+        pb = ProgressBar(mainSet.getSize(), fmt=ProgressBar.FULL)
+        pb.start()
+
+        for item in mainSet:
+            valueInMain=getattr(item,self.getMainSetField(pythonName=True))
+            if valueInMain.get() in uniqueValuesinSec:
+                self._append(outputSet,item)
+            pb.increase()
+
+        pb.finish()
+
+        self._defineOutputs(subset=outputSet)
+        self._defineTransformRelation(mainSet, outputSet)
+
+    def getMainSetField(self, pythonName=False):
+        if pythonName:
+            return self._normalizeSpecialFields(self.mainSetField.get())
+        else:
+            return self.mainSetField.get()
+
+    def getSecSetField(self, pythonName=False):
+        if pythonName:
+            return self._normalizeSpecialFields(self.secSetField.get())
+        else:
+            return self.secSetField.get()
+
+    def _normalizeSpecialFields(self, field):
+        if field == "id":
+            return "_objId"
+        else:
+            return field
+    # --------------------------- INFO functions ------------------------------
+    def _validate(self):
+        """Make sure the input data make sense"""
+        errors=[]
+        if not hasattr(self.mainSet.get().getFirstItem(), self.getMainSetField(pythonName=True)):
+            errors.append('The main set does not have the field %s' % self.mainSetField.get())
+
+        if not hasattr(self.secSet.get().getFirstItem(), self.getSecSetField(pythonName=True)):
+            errors.append('The secondary set does not have the field %s' % self.secSetField.get())
+
+        return errors
+    def _summary(self):
+
+        summary = ["Items in the main set where %s=%s of items in the secondary set where selected." % (self.mainSetField.get(), self.secSetField.get())]
+
+        if hasattr(self, "subset"):
+            summary.append('*%d* items matched the criteria' % self.subset.getSize())
+
+        return summary
+
+
+class ProtSetAggregate(EMProtocol):
+    """ Aggregates any set data based on its fields"""
+    _label = "data summary"
+    def _defineParams(self, form):
+        form.addSection(label='Input')
+
+        add = form.addParam  # short notation
+        add('inputSet', pwprot.params.PointerParam,
+            pointerClass='EMSet', label="Any set",
+            help='Set with the dta to be aggregated')
+
+        add('operations', pwprot.params.StringParam,
+            label='Summary operations',default="COUNT",
+            help='Summary operations to apply to all fields in Fields parameter. e.g: MIN MAX AVG. Possible values are MIN, MAX, COUNT, '
+                 'AVG, SUM, TOTAL, GROUP_CONCAT. For more technical information see: https://www.sqlite.org/lang_aggfunc.html')
+
+        add('fields', pwprot.params.StringParam,
+            label='Fields', default="id",
+            help='Fields to apply operations on. Fields can be found in the metadata viewers.'
+                  ' The header of the columns are valid names. e.g: _samplingRate id. Fields listed here should '
+                 'support the operations specified: DO NOT add literal fields.',
+            )
+
+        add('groupby', pwprot.params.StringParam,
+            label='Group by',
+            help='Fields to make the group. An empty value will summarize the whole dataset.',
+            )
+
+    def _insertAllSteps(self):
+        self._insertFunctionStep(self.aggregateSet, self.operations.get(), self.fields.get(), self.groupby.get())
+
+    def aggregateSet(self, *args):
+
+        mainSet = self.inputSet.get()
+
+        # Instantiate and copy main properties
+        outputSet = SetOfStats.create(self.getPath())
+
+        # Run the aggregation method
+        operations = self.operations.getListFromValues(caster=str)
+        self.info("Operations: %s" % operations)
+
+        fields = self.fields.getListFromValues(caster=str)
+        self.info("Fields: %s" % fields)
+
+
+        if self.groupby.get():
+            groupBy = self.groupby.getListFromValues(caster=str)
+            self.info("Grouping by: %s" % groupBy)
+        else:
+            groupBy = None
+            self.info("No grouping fields.")
+
+
+        result = mainSet.aggregate(operations,
+                                   fields, groupBy)
+
+        pb = ProgressBar(len(result), fmt=ProgressBar.FULL)
+        pb.start()
+
+        # Dictionary to hold the scipion data type based on the key
+        scipionTypes ={}
+
+        def getScipionType(fieldName:str):
+
+            if fieldName not in scipionTypes:
+
+                if fieldName.startswith("COUNT"):
+                    scipionType=Integer
+                elif fieldName.startswith(("MIN","MAX","AVG", "SUM","TOTAL")):
+                    scipionType=Float
+                else:
+                    scipionType=String
+
+                self.info("Scipion type for %s is %s" %(key, scipionType.getClassName()))
+                scipionTypes[key] = scipionType
+            return scipionTypes[key]
+
+        # Fill the set
+        for line in result:
+            newItem = Object()
+            for key in line.keys():
+                scipionType = getScipionType(key)
+                value =line[key]
+                setattr(newItem, key, scipionType(value))
+
+            outputSet.append(newItem)
+            pb.increase()
+
+        pb.finish()
+
+        self._defineOutputs(aggregate=outputSet)
+        self._defineTransformRelation(mainSet, outputSet)
+
+
+
```

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_tests.py` & `scipion-em-3.7.0/pwem/protocols/protocol_tests.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_tiltpairs.py` & `scipion-em-3.7.0/pwem/protocols/protocol_tiltpairs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_tools.py` & `scipion-em-3.7.0/pwem/protocols/protocol_tools.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols/protocol_wait.py` & `scipion-em-3.7.0/pwem/protocols/protocol_wait.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/protocols.conf` & `scipion-em-3.7.0/pwem/protocols.conf`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,19 @@
 	]},
     {"tag": "section", "text": "Tools", "openItem": "False", "children": [
 	  {"tag": "protocol_group", "text": "Sets", "openItem": "False", "children": [
         {"tag": "protocol", "value": "ProtSubSet",   "text": "default"},
         {"tag": "protocol", "value": "ProtUnionSet", "text": "default"},
         {"tag": "protocol", "value": "ProtSplitSet", "text": "default"},
 	    {"tag": "protocol", "value": "ProtSetFilter", "text": "default"},
-	    {"tag": "protocol", "value": "ProtClassesSelector", "text": "default"}
+	    {"tag": "protocol", "value": "ProtClassesSelector", "text": "default"},
+	    {"tag": "protocol", "value": "ProtSubSetByCoord", "text": "default"},
+	    {"tag": "protocol", "value": "ProtSubSetByMic", "text": "default"},
+	    {"tag": "protocol", "value": "ProtCrossSubSet", "text": "default"},
+	    {"tag": "protocol", "value": "ProtSetAggregate", "text": "default"}
 	  ]},
 	  {"tag": "protocol_group", "text": "Calculators", "openItem": "False", "children": [
 	    {"tag": "protocol", "value": "ProtBoxSizeParameters", "text": "default"},
         {"tag": "protocol", "value": "ProtMathematicalOperator", "text": "default"},
         {"tag": "protocol", "value": "ProtBoxSizeCheckpoint", "text": "default"}
 	  ]}
 	]},
```

### Comparing `scipion-em-3.6.0/pwem/scipion_icon.png` & `scipion-em-3.7.0/pwem/scipion_icon.png`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/templates/demo.json.template` & `scipion-em-3.7.0/pwem/templates/demo.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/__init__.py` & `scipion-em-3.7.0/pwem/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,18 @@
                 'volumes': 'volumes/*.spi',
                 'averages': 'averages/averages.stk'})
 
     DataSet(name='nma', folder='nma',
             files={'pdb': 'pdb/AK.pdb'})
 
     DataSet(name='relion_tutorial', folder='relion_tutorial',
-            files={'allMics': 'micrographs/*.mrc'})
+            files={'allMics': 'micrographs/*.mrc',
+                   'boxingDir': 'pickingEman',
+                   'posAllDir': 'pickingXmipp',
+                   'volume': 'volumes/reference.mrc'})
 
     DataSet(name='relion30_tutorial', folder='relion30_tutorial', files={})
 
     DataSet(name='ribo_movies', folder='ribo_movies',
             files={
                 'movies': 'movies/1??_*.mrcs',
                 'posAllDir': 'pickingXmipp',
```

### Comparing `scipion-em-3.6.0/pwem/tests/data/hexonAtomStruct.py` & `scipion-em-3.7.0/pwem/tests/data/hexonAtomStruct.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/data/test_convert_atom_struct.py` & `scipion-em-3.7.0/pwem/tests/data/test_convert_atom_struct.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/data/test_data.py` & `scipion-em-3.7.0/pwem/tests/data/test_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/data/test_metadata.py` & `scipion-em-3.7.0/pwem/tests/data/test_metadata.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/data/test_symmetry.py` & `scipion-em-3.7.0/pwem/tests/data/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_angular_distribution.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_angular_distribution.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_extract_particles.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_extract_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_notifier.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_notifier.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_plugin.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_plugin.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_projection_edit.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_projection_edit.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocol_alignment_assign.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocol_alignment_assign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocol_boxsize_checkpoint.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocol_boxsize_checkpoint.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocol_boxsize_parameters.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocol_boxsize_parameters.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocol_export2DB.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocol_export2DB.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocol_extract_coorinates.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocol_extract_coorinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocol_invert_Hand.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocol_invert_Hand.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocol_mathematical_operator.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocol_mathematical_operator.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocol_movie_eraser.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocol_movie_eraser.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocol_volume_homogenizer.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocol_volume_homogenizer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocol_wait.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocol_wait.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocols_assign_orig.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocols_assign_orig.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_atomstruct.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_atomstruct.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_coords.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_coords.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_ctfs.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_ctfs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_masks.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_masks.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_micrographs.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_micrographs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_movies.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_movies.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_particles.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_sequence.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_sequence.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocols_import_volumes.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocols_import_volumes.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocols_set_editor.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocols_set_editor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocols_set_filter.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocols_set_filter.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/protocols/test_protocols_sets.py` & `scipion-em-3.7.0/pwem/tests/protocols/test_protocols_sets.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/utils.py` & `scipion-em-3.7.0/pwem/tests/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/workflows/test_parallel_gpu_queue.py` & `scipion-em-3.7.0/pwem/tests/workflows/test_parallel_gpu_queue.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/workflows/test_workflow.py` & `scipion-em-3.7.0/pwem/tests/workflows/test_workflow.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/workflows/test_workflow_initialvolume.py` & `scipion-em-3.7.0/pwem/tests/workflows/test_workflow_initialvolume.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/workflows/test_workflow_mixed.py` & `scipion-em-3.7.0/pwem/tests/workflows/test_workflow_mixed.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/workflows/test_workflow_mixed_large.py` & `scipion-em-3.7.0/pwem/tests/workflows/test_workflow_mixed_large.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/workflows/test_workflow_modeling.py` & `scipion-em-3.7.0/pwem/tests/workflows/test_workflow_modeling.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/workflows/test_workflow_xmipp.py` & `scipion-em-3.7.0/pwem/tests/workflows/test_workflow_xmipp.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/workflows/test_workflow_xmipp_assignment_tiltpairs.py` & `scipion-em-3.7.0/pwem/tests/workflows/test_workflow_xmipp_assignment_tiltpairs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/workflows/test_workflow_xmipp_ctf_consensus.py` & `scipion-em-3.7.0/pwem/tests/workflows/test_workflow_xmipp_ctf_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/tests/workflows/test_workflow_xmipp_rct.py` & `scipion-em-3.7.0/pwem/tests/workflows/test_workflow_xmipp_rct.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/utils.py` & `scipion-em-3.7.0/pwem/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+from glob import glob
 from os.path import join, dirname, basename
 import logging
 logger = logging.getLogger(__name__)
 import pyworkflow.utils as pwutils
 import pwem
 
 
@@ -104,14 +105,15 @@
     for step in range(0, splitNum):
         rangeList.append(round(minValue + step * inter, roundTo))
     return rangeList
 
 
 PROBLEMATIC_SHELL_CHARS = ";<>?\"()|*\\'&"
 
+
 def cleanFileName(fn, warn=True):
     """ Cleans any character that later on might cause shell parsing errors like "(", ")", " "
     and warns about it if warn is true.
 
     :param fn: file to be cleaned
     :param warn: Optional (True). Logs """
 
@@ -123,17 +125,25 @@
                 logger.info("Warning!. Problematic character (%s) found in file %s. "
                             "Any of these characters will be removed: %s" % (bannedChar, fn, PROBLEMATIC_SHELL_CHARS))
             fn = fn.replace(bannedChar, '')
             cleaned = True
 
     return fn, cleaned
 
+
 def round_to_nearest(number, base):
     """ Rounds number to the nearest integer: E.g: pass base=5 to round to the nearest
      number multiple of 5
 
     :param number: number to be rounded
     :param base: integer to limit the rounding to
     """
 
     return base * round(number/base)
 
+
+def getMatchingFiles(path, sort=False):
+    filePaths = glob(path)
+    if sort:
+        filePaths.sort()
+    return filePaths
+
```

### Comparing `scipion-em-3.6.0/pwem/viewers/__init__.py` & `scipion-em-3.7.0/pwem/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/filehandlers.py` & `scipion-em-3.7.0/pwem/viewers/filehandlers.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/mdviewer/__init__.py` & `scipion-em-3.7.0/pwem/viewers/mdviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/mdviewer/readers.py` & `scipion-em-3.7.0/pwem/viewers/mdviewer/readers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,23 @@
 
 import pyworkflow as pw
 import metadataviewer
 from metadataviewer.dao.model import IDAO
 from metadataviewer.model import Table, Column, BoolRenderer, ImageRenderer, StrRenderer
 from metadataviewer.model.renderers import ImageReader, Action
 
-
 SCIPION_OBJECT_ID = "SCIPION_OBJECT_ID"
 SCIPION_PORT = "SCIPION_PORT"
 
 
 class ScipionImageReader(ImageReader):
     @classmethod
     def getCompatibleFileTypes(cls) -> list:
         return list(ImageReadersRegistry._readers.keys())
 
-
     @classmethod
     @lru_cache
     def open(cls, path):
         ext = path.split('.')[-1]
         imageReader = ImageReadersRegistry._readers[ext]
         return imageReader.open(path)
 
@@ -120,15 +118,15 @@
         if tableName != PROPERTIES_TABLE:
             firstRow = self.getTableRow(tableName, 0)
             className = firstRow['class_name']
             if tableName.__contains__('_'):
                 tableSplit = tableName.split('_')
                 lenTableSplit = len(tableSplit)
                 if lenTableSplit > 1:
-                    alias = tableName.replace(tableSplit[-1],'') + className
+                    alias = tableName.replace(tableSplit[-1], '') + className
             else:
                 alias = className
         else:
             alias = PROPERTIES_TABLE
         return alias
 
     def getTableNames(self):
@@ -153,15 +151,15 @@
                 for key, value in firstRow.items():
                     if key not in EXCLUDED_COLUMNS:
                         labelsTypes.append(_guessType(value))
                 self._labelsTypes[tableName] = labelsTypes
 
             self.composeObjectType()
 
-        if len(self._tables) > 2: # Assuming that there are more tables than just Object and Properties
+        if len(self._tables) > 2:  # Assuming that there are more tables than just Object and Properties
             self._tableWithAdditionalInfo = OBJECT_TABLE
         endTime = time.time()
         logging.info("GetTableNames: %f" % (endTime - initTime))
         return self._names
 
     def findColbyName(self, colNames, colName):
         """Return a column index given a column name"""
@@ -200,21 +198,25 @@
             objectTypes = list(self._objectsType.values())
             aliasSplit = alias.split('_')
             if alias.startswith('Class') and len(aliasSplit) == 1:
 
                 table.addAction(labels[0], lambda: self.createSubsetCallback(table, objectTypes[0], objectManager))
                 table.addAction(labels[1], lambda: self.createSubsetCallback(table, objectTypes[1], objectManager))
                 if alias == 'Class2D':
-                    table.addAction('Averages', lambda: self.createSubsetCallback(table, 'SetOfAverages', objectManager))
+                    table.addAction('Averages',
+                                    lambda: self.createSubsetCallback(table, 'SetOfAverages', objectManager))
                 else:
-                    table.addAction('Volumes', lambda: self.createSubsetCallback(table, 'SetOfVolumes',  objectManager))
+                    table.addAction('Volumes', lambda: self.createSubsetCallback(table, 'SetOfVolumes', objectManager))
             elif alias.startswith('Class'):
-                    table.addAction(aliasSplit[1], lambda: self.createSubsetCallback(table, self._objectsType[aliasSplit[1]], objectManager))
+                table.addAction(aliasSplit[1],
+                                lambda: self.createSubsetCallback(table, self._objectsType[aliasSplit[1]],
+                                                                  objectManager))
             elif alias in self._objectsType and self._objectsType[alias].startswith('SetOf'):
-                table.addAction(alias, lambda: self.createSubsetCallback(table, self._objectsType[alias], objectManager))
+                table.addAction(alias,
+                                lambda: self.createSubsetCallback(table, self._objectsType[alias], objectManager))
 
     def fillTable(self, table, objectManager):
         """Create the table structure (columns) and set the table alias"""
         initTime = time.time()
         tableName = table.getName()
         colNames = self._labels[tableName]
         self.updateExtendColumn(table)
@@ -236,15 +238,18 @@
                 renderer = table.guessRenderer(str(values[index]))
                 if isinstance(renderer, ImageRenderer):
                     imageExt = str(values[index]).split('.')[-1]
                     self.addExternalProgram(renderer, imageExt)
 
             newCol = Column(colName, renderer)
             newCol.setIsSorteable(True)
-            newCol.setIsVisible(objectManager.isLabelVisible(colName))
+            if (tableName == OBJECT_TABLE):
+                newCol.setIsVisible(objectManager.isLabelVisible(colName))
+            else:
+                newCol.setIsVisible(True)
             table.addColumn(newCol)
 
             if isFileNameCol:
                 logger.debug("Creating an extended column: %s" % EXTENDED_COLUMN_NAME)
                 imageExt = str(values[index]).split('.')[-1]
                 if values[index] is not None and ImageRenderer().getImageReader(values[index]) is not None:
                     renderer = ImageRenderer()
@@ -284,15 +289,15 @@
     def addImageJ(self, renderer: ImageRenderer):
         imageJPath = os.environ.get('IMAGEJ_BINARY_PATH', None)
         if imageJPath is not None:
             icon = pw.findResource('Imagej.png')
 
             def openImageJCallback(imagePath):
                 imageSplit = imagePath.split('@')
-                if len(imageSplit)>1:
+                if len(imageSplit) > 1:
                     selectedSlice = int(imageSplit[0])
                 else:
                     selectedSlice = 0
                 path = imageSplit[-1]
                 program = os.path.join(imageJPath)
                 macro = r"""
 path = "%s";
@@ -308,15 +313,15 @@
                 cmd = program + ' -macro %s' % macroPath
                 Popen(cmd, shell=True, cwd=os.getcwd())
 
             renderer.addAction(Action('IJ', icon, 'Open with ImageJ',
                                       openImageJCallback))
 
     def addImageViewer(self, renderer: ImageRenderer, imageExt: str):
-        icon = os.path.join(pw.getResourcesPath(),'file_vol.png')
+        icon = os.path.join(pw.getResourcesPath(), 'file_vol.png')
 
         def openImageViewerCallback(imagePath):
             path = imagePath.split('@')[-1]
 
             pythonPath = sys.executable
             program = '%s -m pwem.viewers.mdviewer.volumeViewer' % pythonPath
             cmd = program + ' "%s"' % path
@@ -339,16 +344,16 @@
         limit = pageSize
 
         column = self._labels[tableName][actualColumn]
         mode = 'ASC' if orderAsc else 'DESC'
         self.updateExtendColumn(page.getTable())
 
         for rowcount, row in enumerate(self.iterTable(tableName, start=firstRow, limit=limit,
-                                       classes=self._tables[tableName],
-                                       orderBy=column, mode=mode)):
+                                                      classes=self._tables[tableName],
+                                                      orderBy=column, mode=mode)):
             if row:
                 values = [value for key, value in row.items() if key not in EXCLUDED_COLUMNS]
                 if 'id' in row.keys():
                     id = row['id']
                 else:
                     id = rowcount
 
@@ -362,15 +367,15 @@
 
                 page.addRow((int(id), values))
         endTime = time.time()
         logging.info("Fill the page: %f" % (endTime - initTime))
 
     def getRowsCount(self, tableName):
         """ Return the number of elements in the given table. """
-        logger.debug("Reading the table %s" %tableName)
+        logger.debug("Reading the table %s" % tableName)
         if tableName == OBJECT_TABLE:
             size = int(self._con.execute(f"SELECT * FROM {PROPERTIES_TABLE} WHERE key='_size'").fetchall()[0]['value'])
             return size
         return self._con.execute(f"SELECT COUNT(*) FROM {tableName}").fetchone()['COUNT(*)']
 
     def getTableRowCount(self, tableName):
         if tableName not in self._tableCount:
@@ -380,62 +385,66 @@
             logging.info("Table count: %f" % (endTime - initTime))
         return self._tableCount[tableName]
 
     def getSelectedRangeRowsIds(self, tableName, startRow, numberOfRows, column, reverse=True):
         """Return a range of rows starting at 'startRow' an amount
            of 'numberOfRows' """
 
-        logger.debug("Reading the table %s and selected a range of rows %d - %d" % (tableName,startRow, numberOfRows + 1))
+        logger.debug(
+            "Reading the table %s and selected a range of rows %d - %d" % (tableName, startRow, numberOfRows + 1))
         mode = 'ASC' if reverse else 'DESC'
         col = self._getColumnMap(tableName, column)
         if col == None:
             col = column
-        query = "SELECT id FROM %s ORDER BY %s %s LIMIT %d , %d" % (tableName, col, mode, startRow - 1, numberOfRows + 1)
+        query = "SELECT id FROM %s ORDER BY %s %s LIMIT %d , %d" % (
+        tableName, col, mode, startRow - 1, numberOfRows + 1)
         rowsList = self._con.execute(query).fetchall()
         rowsIds = [row['id'] for row in rowsList]
         return rowsIds
 
     def getColumnsValues(self, tableName, columns, xAxis, selection, limit,
                          useSelection, reverse=True):
         """Get the values of the selected columns in order to plot them"""
 
         logger.debug("Reading the table %s and selected some columns values...")
-        cols = columns
+        cols = [colName for colName in columns]
         if xAxis and xAxis not in cols:
             cols.append(xAxis)
         columnNames = []
         for column in cols:
             col = self._getColumnMap(tableName, column) or column
             columnNames.append(col)
-
+        if 'id' not in cols:
+            columnNames.append('id')  # Always retrieve the id values to create subsets
+            cols.append('id')
         columnNames = ", ".join(columnNames)
 
         col = self._getColumnMap(tableName, xAxis)
         if col is not None:
             xAxis = col
 
         mode = 'ASC' if reverse else 'DESC'
         orderBy = ' ORDER BY %s %s' % (xAxis, mode) if xAxis else ''
         limit = ' LIMIT %d' % limit if limit is not None else ''
         where = f" WHERE id in ({', '.join(map(str, selection.getSelection().keys()))})" if selection.getCount() > 1 and useSelection else ''
 
         query = "SELECT %s FROM %s %s %s %s" % (columnNames, tableName, where,
-                                                 orderBy, limit)
+                                                orderBy, limit)
         selectedColumns = self._con.execute(query).fetchall()
 
         columnsValues = {}
 
         firstValue = selectedColumns[0]
-        for colName in columns:
+        for colName in cols:
             col = self._getColumnMap(tableName, colName) or colName
             columnsValues[colName] = [firstValue[col]]
 
         for pos, value in enumerate(selectedColumns):
             if pos > 0:
-                for colName in columns:
+                for colName in cols:
                     col = self._getColumnMap(tableName, colName) or colName
                     columnsValues[colName].append((value[col]))
 
         return columnsValues
 
     def iterTable(self, tableName, **kwargs):
         """
@@ -473,21 +482,24 @@
 
         if 'classes' not in kwargs or kwargs['classes'] == PROPERTIES_TABLE:
             res = self._con.execute(query)
             while row := res.fetchone():
                 yield row
         else:  # Mapping the column names and  including only the allowed columns
             self._columnsMap[tableName] = {row['column_name']: row['label_property']
-                          for row in self.iterTable(kwargs['classes']) if row['class_name'] in ALLOWED_COLUMNS_TYPES}
+                                           for row in self.iterTable(kwargs['classes']) if
+                                           row['class_name'] in ALLOWED_COLUMNS_TYPES}
             self._excludedColumns = {row['column_name']: row['label_property']
-                          for row in self.iterTable(kwargs['classes']) if row['class_name'] not in ALLOWED_COLUMNS_TYPES}
+                                     for row in self.iterTable(kwargs['classes']) if
+                                     row['class_name'] not in ALLOWED_COLUMNS_TYPES}
 
             def _row_factory(cursor, row):
                 fields = [column[0] for column in cursor.description]
-                rowFact = {self._columnsMap[tableName].get(k, k): v for k, v in zip(fields, row) if k not in self._excludedColumns}
+                rowFact = {self._columnsMap[tableName].get(k, k): v for k, v in zip(fields, row) if
+                           k not in self._excludedColumns}
                 return rowFact
 
             # Modify row factory to modify column names
             self._con.row_factory = _row_factory
             res = self._con.execute(query)
             while row := res.fetchone():
                 yield row
@@ -521,24 +533,27 @@
     def createSubsetCallback(self, table: Table, objectType: str, objectManager):
         """Create a subset"""
         selection = table.getSelection().getSelection()
         tableName = table.getName()
         elementsCount = len(selection)
         if not elementsCount:
             elementsCount = self._tableCount[tableName]
+            objectManager.getSelectedRangeRowsIds(tableName,
+                                                  1, self._tableCount[tableName],
+                                                  'id', 'ASC')
         subsetName = objectManager.getGui().getSubsetName(objectType, elementsCount)
         if subsetName:
             format = '%Y%m%d%H%M%S'
             now = datetime.now()
             timestamp = now.strftime(format)
             path = 'Logs/selection_%s.txt' % timestamp
             self.writeSelection(table, path)
             path += ","  # Always add a comma, it is expected by the user subset protocol
             if tableName != OBJECT_TABLE:
-                path += tableName.split(OBJECT_TABLE)[0]
+                path += tableName.split('_Objects')[0]
 
             self.sendSubsetCreationMessage(path, objectType, subsetName)
 
     def sendSubsetCreationMessage(self, selectionFile, outputClassName, label):
 
         import socket
 
@@ -551,29 +566,28 @@
         # We should create this message:
         # run protocol ProtUserSubSet inputObject=380 sqliteFile='...','' outputClassName=SetOfTiltSeries other='' label='create subset'
         data = f"run protocol ProtUserSubSet inputObject={self.getScipionObjectId()} " \
                f"sqliteFile='{selectionFile}' outputClassName='{outputClassName}' other='' label='{label}'"
 
         clientSocket.send(data.encode())
 
-
     def getScipionPort(self):
         """ Returns Scipion port or None if not in the environment"""
         return os.getenv(SCIPION_PORT, '1300')
 
     def getScipionObjectId(self):
         """ Returns Scipion object id"""
         return os.getenv(SCIPION_OBJECT_ID)
 
     def writeSelection(self, table: Table, path):
         """ Create a file with the selected rows ids"""
         tableName = table.getName()
         rowsIds = table.getSelection().getSelection().keys()
         if not rowsIds:
-            rowsIds = [i+1 for i in range(self._tableCount[tableName])]
+            rowsIds = [i + 1 for i in range(self._tableCount[tableName])]
         try:
             with open(path, 'w') as file:
                 for rowId in rowsIds:
                     file.write(str(rowId) + ' ')
                 file.close()
             logger.debug(f"The file: {path} was created correctly.")
         except Exception as e:
@@ -612,11 +626,11 @@
         try:
             float(strValue)
             return float
         except ValueError:
             return str
 
 
-def extendMDViewer(om:metadataviewer.model.ObjectManager):
+def extendMDViewer(om: metadataviewer.model.ObjectManager):
     """ Function to extend the object manager with DAOs and readers"""
     om.registerDAO(SqliteFile)
     om.registerReader(ScipionImageReader)
```

### Comparing `scipion-em-3.6.0/pwem/viewers/mdviewer/sqlite_dao.py` & `scipion-em-3.7.0/pwem/viewers/mdviewer/sqlite_dao.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/mdviewer/star_dao.py` & `scipion-em-3.7.0/pwem/viewers/mdviewer/star_dao.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/mdviewer/viewer.py` & `scipion-em-3.7.0/pwem/viewers/mdviewer/viewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,26 +41,26 @@
         self.protocol = protocol
         self.port = port
 
     def show(self):
         env = os.environ
         env[SCIPION_PORT] = str(self.port)
         env[SCIPION_OBJECT_ID] = str(self._emSet.getObjId())
-        visibleLabels = self.getVisibleLabels()
-
+        config = self.getVisibleAndOrderLabels()
+        visibleLabels, orderLabels = config[0], config[1]
         subprocess.Popen(
             [PYTHON, "-m", "metadataviewer", "--extensionpath", os.path.join(os.path.dirname(__file__), "readers.py"),
-            self._emSet.getFileName(), "--visiblelabels", visibleLabels])
+            self._emSet.getFileName(), "--visiblelabels", visibleLabels, "--orderlabels", orderLabels])
 
-    def getVisibleLabels(self):
-        from pwem.viewers import VISIBLE
+    def getVisibleAndOrderLabels(self):
+        from pwem.viewers import VISIBLE, ORDER
         config = RegistryViewerConfig.getConfig(type(self._emSet))
-        if config is not None and VISIBLE in config:
-            return config[VISIBLE]
-        return ''
+        visible = config[VISIBLE] if VISIBLE in config else ''
+        order = config[ORDER] if ORDER in config else ''
+        return visible, order
 
 
 class MDViewer(Viewer):
     _name = 'Scipion'
     _targets = [EMSet]
 
     def _visualize(self, obj, **kwargs):
```

### Comparing `scipion-em-3.6.0/pwem/viewers/mdviewer/volumeViewer.py` & `scipion-em-3.7.0/pwem/viewers/mdviewer/volumeViewer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/plotter.py` & `scipion-em-3.7.0/pwem/viewers/plotter.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/showj.py` & `scipion-em-3.7.0/pwem/viewers/showj.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/viewer_angular_dist.py` & `scipion-em-3.7.0/pwem/viewers/viewer_angular_dist.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/viewer_base.py` & `scipion-em-3.7.0/pwem/viewers/viewer_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,17 +109,15 @@
                 for projection in projectionList:
                     if (abs(projection[0] - angleRot) <= 0.5 and
                             abs(projection[1] - angleTilt) <= 0.5):
                         return projection
                 return None
 
             weight = 1. / numberOfParticles
-            print("RELION-ROT\tRELION-TILT")
             for angleRot, angleTilt in itemDataIterator:
-                print("%s\t%s" % (angleRot, angleTilt))
                 projection = getCloseProjection(angleRot, angleTilt)
                 if projection is None:
                     projectionList.append([angleRot, angleTilt, weight])
                 else:
                     projection[2] = projection[2] + weight
 
             mdProj = md.MetaData()
```

### Comparing `scipion-em-3.6.0/pwem/viewers/viewer_chimera.py` & `scipion-em-3.7.0/pwem/viewers/viewer_chimera.py`

 * *Files 3% similar despite different names*

```diff
@@ -438,25 +438,33 @@
                         showAxis=True,
                         fontSize=12):  # default chimera font size
     """ colors surface of volume 'displayVolFileName' using values from
     'mapVolFikeName'. A colorkey is created using the values in stepColors
     and the color in colorList. """
     scriptFile = scriptFileName
     fhCmd = open(scriptFile, 'w')
+    fhCmd.write("# -*- coding: utf-8 -*-\n")
     fhCmd.write("from chimerax.core.commands import run\n")
     fhCmd.write("run(session, 'set bgColor %s')\n" % bgColorImage)
 
     chimeraVolId = 1
 
     bildFileName = scriptFile.replace(".py", ".bild")
     Chimera.createCoordinateAxisFile(voldim[0],
                                      bildFileName=bildFileName,
                                      sampling=sampling)
+
+    # Convert paths to WSL is apply:
+    if OS.isWSL():
+        bildFileName=OS.WLSfile2Windows(bildFileName)
+        mapVolFileName=OS.WLSfile2Windows(mapVolFileName)
+        displayVolFileName=OS.WLSfile2Windows(displayVolFileName)
+
     # axis
-    fhCmd.write("run(session, 'open %s')\n" % bildFileName)
+    fhCmd.write("run(session, r'open %s')\n" % bildFileName)
     if not showAxis:
         fhCmd.write("run(session, 'hide #1')\n")
 
     fhCmd.write("run(session, 'cofr 0,0,0')\n")  # set center of coordinates
 
     chimeraVolId += 1
 
@@ -468,26 +476,26 @@
         z = -voldim[2] * sampling // 2
     else:
         # TODO, not sure about sign
         x = volOrigin[0]
         y = volOrigin[1]
         z = volOrigin[2]
 
-    fhCmd.write("run(session, 'open %s')\n" % displayVolFileName)
+    fhCmd.write("run(session, r'open %s')\n" % displayVolFileName)
     if step == -1:
         fhCmd.write("run(session, 'volume #%d voxelSize %s')\n" %
                     (chimeraVolId, str(sampling)))
     else:
         fhCmd.write("run(session, 'volume #%d voxelSize %s step %d')\n" %
                     (chimeraVolId, str(sampling), step))
     fhCmd.write("run(session, 'volume #%d origin %0.2f,%0.2f,%0.2f')\n"
                 % (chimeraVolId, x, y, z))
     # second volume
     chimeraVolId += 1
-    fhCmd.write("run(session, 'open %s')\n" % mapVolFileName)
+    fhCmd.write("run(session, r'open %s')\n" % mapVolFileName)
     # TODO: Why no step here?
     fhCmd.write("run(session, 'volume #%d voxelSize %f')\n" % (chimeraVolId, sampling))
     fhCmd.write("run(session, 'volume #%d origin %0.2f,%0.2f,%0.2f')\n"
                 % (chimeraVolId, x, y, z))
     fhCmd.write("run(session, 'vol #%d hide')\n" % chimeraVolId)
 
     # replace scolor + colorkey which has been discontinued in chimerax
```

### Comparing `scipion-em-3.6.0/pwem/viewers/viewer_coordinates.py` & `scipion-em-3.7.0/pwem/viewers/viewer_coordinates.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 from tkinter import filedialog, messagebox
 
 from PIL import ImageOps, ImageFilter, ImageEnhance, ImageTk
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 
 import logging
+
+from matplotlib.widgets import RangeSlider
+
 from pwem.emlib.image.image_readers import ImageReadersRegistry
 from pwem.objects import EMSet, SetOfCoordinates, SetOfMicrographs
 from pyworkflow.gui import getImage, ToolTip
 from pyworkflow.utils import Icon
 from pyworkflow.viewer import View, Viewer
 
 logger = logging.getLogger()
@@ -300,30 +303,30 @@
             self.eraserAction.configure(relief=tk.GROOVE)
             self.dragButton.configure(relief=tk.GROOVE)
             self.filamentPickerAction.configure(relief=tk.GROOVE)
             self.root.config(cursor='')
             self.picking = True
             self.eraser = False
             self.filament = False
-            self.drag = False
+            self.drag = True
 
     def eraserActivate(self):
         """ Recovering some actions when eraser button is pressed """
         if self.eraser:
             self.eraserAction.configure(relief=tk.GROOVE)
             self.eraser = False
         else:
             self.pickerAction.configure(relief=tk.GROOVE)
             self.filamentPickerAction.configure(relief=tk.GROOVE)
             self.dragButton.configure(relief=tk.GROOVE)
             self.eraserAction.configure(relief=tk.SUNKEN)
             self.picking = False
             self.filament = False
             self.eraser = True
-            self.drag = False
+            self.drag = True
 
     def filamentActivate(self):
         """ Recovering some actions when filament button is pressed """
         if self.filament:
             self.filamentPickerAction.configure(relief=tk.GROOVE)
             self.filament = False
         else:
@@ -407,39 +410,40 @@
             self.showCoordinates()
             if self.particlesWindowVisible:
                 self.extractImages()
 
     def _createTable(self):
         """Create a table on the left side to display information"""
         columns = ('Index', 'File', 'Particles', 'Updated')
-        data = []
+        data = {}
 
         setOfMicrographs = self.setOfCoordinate.getMicrographs()
         for micrograph in setOfMicrographs.iterItems():
             micId = str(micrograph.getObjId())
             self.coordinatesDict[micId] = {}
             self.oldCoordinatesDict[micId] = {}
             self.deletedCoordinates[micId] = {}
             self.movedCoordinates[micId] = {}
             self.newCoordinates[micId] = {}
             self.micrographPathDict[micId] = (micrograph.getFileName(), micrograph.getObjId())
+            data[micId] = (micrograph.getObjId(), micrograph.getMicName(), 0, 'No')
 
         label = '_micName' if isinstance(setOfMicrographs, SetOfMicrographs) else '_micId'
         for micAgg in self.setOfCoordinate.aggregate(["count"], label, [label, "_micId"]):
             micName = micAgg[label]
-            data.append((micAgg['_micId'], micName, micAgg['count'], 'No'))
+            data[str(micAgg['_micId'])] = (micAgg['_micId'], micName, micAgg['count'], 'No')
 
         self.table = ttk.Treeview(self.contentFrame, columns=columns, show="headings")
         self.table.bind("<Enter>", self.recoveryPointer)
         self.table.bind("<ButtonRelease-1>", self.onTableClick)  # Bind event for table click
         for col, width in zip(columns, (50, 300, 100, 100)):
             self.table.heading(col, text=col, anchor="center")
             self.table.column(col, anchor="center", width=width)
 
-        for row in data:
+        for row in data.values():
             self.table.insert("", tk.END, values=row)
 
         y_scrollbar = ttk.Scrollbar(self.contentFrame, orient="vertical", command=self.table.yview)
         self.table.configure(yscrollcommand=y_scrollbar.set)
 
         self.table.grid(row=0, column=0, sticky='nsew')
         y_scrollbar.grid(row=0, column=1, sticky="ns")
@@ -467,15 +471,15 @@
                 self.showCoordinates()
                 if self.particlesWindowVisible:
                     self.extractImages()
 
     def loadCoordinates(self, micrograph):
         """Load the coordinate for a given micrograph """
         micId = micrograph[0]
-        if not self.coordinatesDict[self.micId]:
+        if not self.coordinatesDict[self.micId] and micrograph[2] != 0:
             for index, coordinate in enumerate(self.setOfCoordinate.iterCoordinates(int(micId))):
                 self.coordinatesDict[self.micId][index+2] = (coordinate.getX(), coordinate.getY(), coordinate.getObjId())
                 self.oldCoordinatesDict[self.micId][index+2] = (coordinate.getX(), coordinate.getY(), coordinate.getObjId())
 
     def _createImageFrame(self):
         """Create the image frame on the right side to display micrographs and associated coordinates"""
         self.imageFrame = ttk.Frame(self.contentFrame)
@@ -726,15 +730,15 @@
                                                                (y - self.yOffset) * self.scale / self.zoomFactor,
                                                                None)
                     self.newCoordinates[self.micId][shape] = self.coordinatesDict[self.micId][shape]
                     self.totalCoordinates += 1
                     self.totalPickButton.configure(text=f"Total picks: {self.totalCoordinates}")
                     self.hasChanges[self.micId] = True
 
-                elif self.drag:  # Move coordinate or drag all image
+                elif self.drag or (self.picking and not self.canPick(event)):  # Move coordinate or drag all image
                     if self.selectedCoordinate:
                         index, coords = self.selectedCoordinate, self.shapes[self.selectedCoordinate]
                         self.root.config(cursor='hand2')
                         indexesToMove = self.nearCoordinates(index)
                         newX = self.root.winfo_pointerx() - self.root.winfo_rootx() - self.coordX
                         newY = self.root.winfo_pointery() - self.root.winfo_rooty() - self.coordY
 
@@ -853,52 +857,47 @@
 
                 self.scaledImage = self.imagePIL.resize((int(dpiWidth), int(dpiHeight)))
                 self.imageTk = ImageTk.PhotoImage(self.scaledImage)
 
                 # self.quadtree = Index(bbox=[0, 0, self.imagePIL.size[0], self.imagePIL.size[1]])
                 self.imageCanvas.delete("all")
                 self.image = self.imageCanvas.create_image(0, 0, anchor=tk.NW, image=self.imageTk, tags='image')
+                self.zoomFactor = 1
                 self.drawCoordinates(self.micId)
 
             except Exception as e:
                 logger.error(f"Error loading image '{self.micId}': {e}")
         else:
             logger.error("Unable to upload the file %s. Make sure the path is correct." % imagePath)
 
     def applyPowerHistogram(self):
         """ Create the histogram and the plot"""
         self.histWindow = tk.Toplevel(self.root)
         self.histWindow.title('Power histogram')
         self.histWindow.resizable(False, False)
-        figure, axes = plt.subplots(figsize=(6, 4))
-        self.plotHistogram(axes)
-        histCanvas = FigureCanvasTkAgg(figure, master=self.histWindow)
+        self.figure, self.axes = plt.subplots(figsize=(6, 4))
+        self.plotHistogram(self.axes)
+        histCanvas = FigureCanvasTkAgg(self.figure, master=self.histWindow)
         histCanvasWidget = histCanvas.get_tk_widget()
         histCanvasWidget.grid(row=0, column=0, sticky="news", padx=10, pady=10)
 
-        # Create the sliders
-        sliderFrame = tk.Frame(self.histWindow)
-        sliderFrame.grid(row=2, column=0, sticky="w", pady=10)
-
-        lowerValueLabel = ttk.Label(sliderFrame, text="Lower value:")
-        lowerValueLabel.grid(row=0, column=0, padx=10, pady=5, sticky="w")
-        self.powerSlider1 = ttk.Scale(sliderFrame, from_=0, to=255, length=430,
-                                      orient=tk.HORIZONTAL, command=self.filterCoordinates)
-        self.powerSlider1.grid(row=0, column=1, sticky="e", padx=5, pady=5)
-
-        upperValueLabel = ttk.Label(sliderFrame, text="Upper value:")
-        upperValueLabel.grid(row=1, column=0, padx=10, pady=5, sticky="w")
-        self.powerSlider2 = ttk.Scale(sliderFrame, from_=0, to=255, length=430,
-                                      orient=tk.HORIZONTAL, command=self.filterCoordinates)
-        self.powerSlider2.grid(row=1, column=1, sticky="e", padx=5, pady=5)
-        self.powerSlider2.set(self.powerSlider2['to'])
+        def update(val):
+            minValue, maxValue = self.rangeSlider.val
+            self.drawRangeLines(self.axes, minValue, maxValue)
+            plt.draw()
+            self.removeCoordinates(minValue, maxValue)
+
+        self.rangeLines = []
+        ax_slider = plt.axes([0.2, 0.05, 0.65, 0.03], facecolor='lightgoldenrodyellow')
+        self.rangeSlider = RangeSlider(ax_slider, '', 0, 256, valinit=(0, 256), valstep=1, valfmt='%d')
+
+        self.rangeSlider.on_changed(update)
 
         buttonsFrame = tk.Frame(self.histWindow)
         buttonsFrame.grid(row=3, column=0, sticky="e", pady=10)
-
         # Close button
         closeButton = tk.Button(buttonsFrame, text='Close', command=self.histWindowClose, font=('Helvetica', 10, 'bold'),
                                 image=getImage(Icon.BUTTON_CANCEL), compound=tk.LEFT)
         closeButton.grid(row=3, column=0, sticky="e", padx=5)
 
         # Save button
         saveButton = tk.Button(buttonsFrame, text='Save & Close', command=self.histWindowSaveClose, fg='white',
@@ -927,29 +926,14 @@
                 self.totalCoordinates -= 1
 
         for i in range(len(shapeToDelete)):
             self.shapes.pop(shapeToDelete[i])
 
         self.histWindowClose()
 
-    def filterCoordinates(self, value):
-        """Handle the range of pixel values that will be removed """
-        slider1Value = self.powerSlider1.get()
-        slider2Value = self.powerSlider2.get()
-        if slider1Value + 20 >= slider2Value:
-            slider2Value += 1
-            if slider2Value < 255:
-                self.powerSlider2.set(slider2Value)
-        if slider2Value - 20 <= slider1Value:
-            slider1Value -= 1
-            if slider1Value > 0:
-                self.powerSlider1.set(slider1Value)
-
-        self.removeCoordinates(slider1Value, slider2Value)
-
     def removeCoordinates(self, value1, value2):
         """Remove the coordinate taking into account the pixel values"""
         pixelRange = (round(float(value1)), round(float(value2)))
         for index, coords in self.shapes.items():
             pixelValue = self.calculateAveragePixel(coords[0], coords[1])
             new_state = "normal"
             if int(pixelValue) < pixelRange[0] or int(pixelValue) > pixelRange[1]:
@@ -968,34 +952,47 @@
         return averagePixel
 
     def extractRegion(self, x, y):
         """Take the particle region"""
         return self.scaledImage.crop((x - self.shapeRadius,  y - self.shapeRadius,
                                      x + self.shapeRadius, y + self.shapeRadius))
 
-    def plotHistogram(self, ejes):
+    def plotHistogram(self, axes):
         """Plot the micrograph histogram"""
         img_array = np.array(self.imagePIL)
         # Apply the power transformation
         img_power = np.power(img_array / 255.0, 2.0) * 255.0
         hist_power, bins_power = np.histogram(img_power.flatten(), bins=256, range=[0, 256])
 
         # Plot histogram
-        ejes.clear()
-        ejes.plot(hist_power)
-        ejes.set_xlabel("Pixel Value")
-        ejes.set_ylabel("Frequency")
+        axes.clear()
+        axes.plot(hist_power)
+        axes.set_xlabel("Pixel Value")
+        axes.set_ylabel("Frequency")
+        plt.subplots_adjust(bottom=0.2)
+
+    def drawRangeLines(self, ax, minVal, maxVal):
+        """Draw vertical lines to represent the selected range"""
+        # Remove old lines
+        for line in self.rangeLines:
+            line.remove()
+        # Draw the new vertical lines
+        lineMin = ax.axvline(minVal, color='red', linestyle='--', linewidth=1)
+        lineMax = ax.axvline(maxVal, color='red', linestyle='--', linewidth=1)
+        # Store the new vertical lines
+        self.rangeLines = [lineMin, lineMax]
 
     def resetMicrograph(self):
         """Remove all coordinates from current micrograph"""
         result = messagebox.askquestion("Confirmation", "Are you sure you want to reset the micrograph?",
                                         icon='warning', **{'parent': self.root})
         if result == messagebox.YES:
             self.totalCoordinates -= len(self.coordinatesDict[self.micId])
             self.coordinatesDict[self.micId] = {}
+            self.shapes.clear()
             self.totalPickButton.configure(text=f"Total picks: {self.totalCoordinates}")
             self.table.set(self.table.selection(), column="Particles", value=0)
             self.imageCanvas.delete("shape")
             self.table.set(self.table.selection(), column='Updated', value='Yes')
             self.hasChanges[self.micId] = True
             if self.particlesWindowVisible:
                 self.onParticlesWindowClosing()
```

### Comparing `scipion-em-3.6.0/pwem/viewers/viewer_fsc.py` & `scipion-em-3.7.0/pwem/viewers/viewer_fsc.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/viewer_localres.py` & `scipion-em-3.7.0/pwem/viewers/viewer_localres.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,14 +289,15 @@
           else:
               f.write("run(session, 'open %s')\n" % cifFile)
               defAttrFile = self.createAttributesFile(cifFile, strId)
               f.write("run(session, 'open %s')\n" % defAttrFile)
               attrColorName = attrName
 
           stepColors, colorList = self.getColors()
+          colorList.reverse(), stepColors.reverse()
           scolorStr = ''
           for step, color in zip(stepColors, colorList):
             scolorStr += '%s,%s:' % (step, color)
           scolorStr = scolorStr[:-1]
 
           average = ''
           if getStructureRecipient(cifDic, attrName=attrName) == 'atoms' and self.residuesAverages:
@@ -332,37 +333,35 @@
       n = 5
       mult = 10 ** n
       stepSize = int(round((high-low) / self.intervals.get(), n) * mult)
       bins = [i / mult for i in range(int(low * mult), int(high * mult), stepSize)]
       _, _, bars = a.hist(attrValues, bins=bins, linewidth=1, label="Map", rwidth=0.9)
 
       colorSteps, colorList = self.getColors()
-      colorList.reverse()
       for bar, colorS, color in zip(bars, colorSteps, colorList):
           bar.set_facecolor(color)
 
       a.grid(True)
       return [self.plotter]
 
     ###################### UTILS #########################
     def getValuesRange(self):
         if self.lowest.get() != self.highest.get():
             return self.lowest.get(), self.highest.get()
         else:
             attrname = self.getEnumText('attrName')
             cifDic = AtomicStructHandler().readLowLevel(self.getAtomStructObject().getFileName())
             names, values = np.array(cifDic[NAME]), np.array(cifDic[VALUE])
-            recipient = cifDic[RECIP][0]
             attrValues = values[names == attrname]
             attrValues = list(map(float, attrValues))
             return min(attrValues), max(attrValues)
 
     def getColors(self):
       low, high = self.getValuesRange()
-      stepColors = splitRange(high, low, splitNum=self.intervals.get())
+      stepColors = splitRange(low, high, splitNum=self.intervals.get())
       colorList = plotter.getHexColorList(len(stepColors), self.colorMap.get())
       return stepColors, colorList
 
     def createAttributesFile(self, cifFile, chiEleId):
         cifDic = AtomicStructHandler().readLowLevel(cifFile)
 
         attrName = self.getEnumText('attrName')
```

### Comparing `scipion-em-3.6.0/pwem/viewers/viewer_pdf.py` & `scipion-em-3.7.0/pwem/viewers/viewer_pdf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/viewer_sequence.py` & `scipion-em-3.7.0/pwem/viewers/viewer_sequence.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/viewer_vmd.py` & `scipion-em-3.7.0/pwem/viewers/viewer_vmd.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/viewer_volumes.py` & `scipion-em-3.7.0/pwem/viewers/viewer_volumes.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/viewers_data.py` & `scipion-em-3.7.0/pwem/viewers/viewers_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/viewers_protocols.py` & `scipion-em-3.7.0/pwem/viewers/viewers_protocols.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/viewers/views.py` & `scipion-em-3.7.0/pwem/viewers/views.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/wizards/__init__.py` & `scipion-em-3.7.0/pwem/wizards/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/wizards/wizard.py` & `scipion-em-3.7.0/pwem/wizards/wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
                                   provider,
                                   maskRadius=value,
                                   unit=units)
             if d.resultYes():
                 if units == emcts.UNIT_ANGSTROM:
                     value = round(d.getRadiusAngstroms(d.radiusSlider))  # Must be an integer
                 else:
-                    value = d.getRadius(d.radiusSlider)
+                    value = int(d.getRadius(d.radiusSlider))
                 self.setVar(form, label, value)
         else:
             dialog.showWarning("Empty input", "Select elements first", form.root)
 
     def setVar(self, form, label, value):
         form.setVar(label, value)
 
@@ -273,16 +273,16 @@
                                        outerRadius=value[1],
                                        unit=units)
             if d.resultYes():
                 if units == emcts.UNIT_ANGSTROM:
                     form.setVar(label[0], d.getRadiusAngstroms(d.radiusSliderIn))
                     form.setVar(label[1], d.getRadiusAngstroms(d.radiusSliderOut))
                 else:
-                    form.setVar(label[0], d.getRadius(d.radiusSliderIn))
-                    form.setVar(label[1], d.getRadius(d.radiusSliderOut))
+                    form.setVar(label[0], int(d.getRadius(d.radiusSliderIn)))
+                    form.setVar(label[1], int(d.getRadius(d.radiusSliderOut)))
         else:
             dialog.showWarning("Empty input", "Select elements first", form.root)
 
     @classmethod
     def getView(self):
         return "wiz_volume_mask_radii"
```

### Comparing `scipion-em-3.6.0/pwem/wizards/wizards.py` & `scipion-em-3.7.0/pwem/wizards/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/wizards/wizards_3d/__init__.py` & `scipion-em-3.7.0/pwem/wizards/wizards_3d/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/wizards/wizards_3d/callbacks.py` & `scipion-em-3.7.0/pwem/wizards/wizards_3d/callbacks.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/wizards/wizards_3d/mask_structure_wizard.py` & `scipion-em-3.7.0/pwem/wizards/wizards_3d/mask_structure_wizard.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/pwem/wizards/wizards_3d/mask_volume_wizard.py` & `scipion-em-3.7.0/pwem/wizards/wizards_3d/mask_volume_wizard.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/scipion_em.egg-info/PKG-INFO` & `scipion-em-3.7.0/scipion_em.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em
-Version: 3.6.0
+Version: 3.7.0
 Summary: This modules contains classes related with EM
 Home-page: https://github.com/scipion-em/scipion-em
 Author: J.M. De la Rosa Trevin, Roberto Marabini, Grigory Sharov, Josue Gomez Blanco, Pablo Conesa, Yunior Fonseca Reyna
 Author-email: delarosatrevin@scilifelab.se, roberto@cnb.csic.es, gsharov@mrc-lmb.cam.ac.uk, josue.gomez-blanco@mcgill.ca, pconesa@cnb.csic.es, fonsecareyna@cnb.csic.es
 License: UNKNOWN
 Description: .. image:: https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg
           :width: 200
```

### Comparing `scipion-em-3.6.0/scipion_em.egg-info/SOURCES.txt` & `scipion-em-3.7.0/scipion_em.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-3.6.0/setup.py` & `scipion-em-3.7.0/setup.py`

 * *Files identical despite different names*

