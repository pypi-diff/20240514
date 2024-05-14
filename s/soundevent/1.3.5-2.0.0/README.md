# Comparing `tmp/soundevent-1.3.5.tar.gz` & `tmp/soundevent-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundevent-1.3.5.tar", last modified: Fri Jan  5 11:52:12 2024, max compression
+gzip compressed data, was "soundevent-2.0.0.tar", last modified: Tue May 14 17:13:14 2024, max compression
```

## Comparing `soundevent-1.3.5.tar` & `soundevent-2.0.0.tar`

### file list

```diff
@@ -1,171 +1,297 @@
--rw-r--r--   0        0        0     1084 2024-01-05 11:51:57.329649 soundevent-1.3.5/LICENSE
--rw-r--r--   0        0        0     3790 2024-01-05 11:51:57.329649 soundevent-1.3.5/README.md
--rw-r--r--   0        0        0     2107 2024-01-05 11:52:12.573720 soundevent-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     1430 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/__init__.py
--rw-r--r--   0        0        0       60 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/__version__.py
--rw-r--r--   0        0        0      687 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/audio/__init__.py
--rw-r--r--   0        0        0     3255 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/audio/chunks.py
--rw-r--r--   0        0        0      555 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/audio/files.py
--rw-r--r--   0        0        0     3154 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/audio/filter.py
--rw-r--r--   0        0        0     6506 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/audio/io.py
--rw-r--r--   0        0        0     6577 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/audio/media_info.py
--rw-r--r--   0        0        0     3860 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/audio/raw.py
--rw-r--r--   0        0        0     2185 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/audio/resample.py
--rw-r--r--   0        0        0     3279 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/audio/scaling.py
--rw-r--r--   0        0        0     2720 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/audio/spectrograms.py
--rw-r--r--   0        0        0     5701 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/audio/spectrum.py
--rw-r--r--   0        0        0     2677 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/__init__.py
--rw-r--r--   0        0        0     1489 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/annotation_projects.py
--rw-r--r--   0        0        0      933 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/annotation_sets.py
--rw-r--r--   0        0        0     2340 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/annotation_tasks.py
--rw-r--r--   0        0        0     2123 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/clip_annotations.py
--rw-r--r--   0        0        0     4989 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/clip_evaluations.py
--rw-r--r--   0        0        0     3983 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/clip_predictions.py
--rw-r--r--   0        0        0     4217 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/clips.py
--rw-r--r--   0        0        0     1624 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/datasets.py
--rw-r--r--   0        0        0      410 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/evaluation_sets.py
--rw-r--r--   0        0        0     1093 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/evaluations.py
--rw-r--r--   0        0        0     4820 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/features.py
--rw-r--r--   0        0        0    31876 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/geometries.py
--rw-r--r--   0        0        0     4136 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/matches.py
--rw-r--r--   0        0        0      263 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/model_runs.py
--rw-r--r--   0        0        0     4552 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/notes.py
--rw-r--r--   0        0        0     2248 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/predicted_tags.py
--rw-r--r--   0        0        0     3007 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/prediction_sets.py
--rw-r--r--   0        0        0      428 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/recording_sets.py
--rw-r--r--   0        0        0     7154 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/recordings.py
--rw-r--r--   0        0        0     1240 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/sequence_annotations.py
--rw-r--r--   0        0        0      860 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/sequence_predictions.py
--rw-r--r--   0        0        0     3270 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/sequences.py
--rw-r--r--   0        0        0     5070 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/sound_event_annotations.py
--rw-r--r--   0        0        0     2214 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/sound_event_predictions.py
--rw-r--r--   0        0        0     2711 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/sound_events.py
--rw-r--r--   0        0        0     4513 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/tags.py
--rw-r--r--   0        0        0      355 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/data/users.py
--rw-r--r--   0        0        0      761 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/evaluation/__init__.py
--rw-r--r--   0        0        0     3815 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/evaluation/affinity.py
--rw-r--r--   0        0        0     8161 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/evaluation/encoding.py
--rw-r--r--   0        0        0     2833 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/evaluation/match.py
--rw-r--r--   0        0        0     5435 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/evaluation/metrics.py
--rw-r--r--   0        0        0      530 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/evaluation/tasks/__init__.py
--rw-r--r--   0        0        0     4689 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/evaluation/tasks/clip_classification.py
--rw-r--r--   0        0        0     4538 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/evaluation/tasks/clip_multilabel_classification.py
--rw-r--r--   0        0        0      576 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/evaluation/tasks/common.py
--rw-r--r--   0        0        0     5799 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/evaluation/tasks/sound_event_classification.py
--rw-r--r--   0        0        0     7600 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/evaluation/tasks/sound_event_detection.py
--rw-r--r--   0        0        0     1233 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/geometry/__init__.py
--rw-r--r--   0        0        0     4964 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/geometry/conversion.py
--rw-r--r--   0        0        0     8646 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/geometry/features.py
--rw-r--r--   0        0        0     3481 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/geometry/html.py
--rw-r--r--   0        0        0     5840 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/geometry/operations.py
--rw-r--r--   0        0        0      323 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/__init__.py
--rw-r--r--   0        0        0     6199 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/__init__.py
--rw-r--r--   0        0        0     4721 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/adapters.py
--rw-r--r--   0        0        0     3202 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/annotation_project.py
--rw-r--r--   0        0        0     6206 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/annotation_set.py
--rw-r--r--   0        0        0     2747 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/annotation_task.py
--rw-r--r--   0        0        0     1765 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/clip.py
--rw-r--r--   0        0        0     3803 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/clip_annotations.py
--rw-r--r--   0        0        0     2991 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/clip_evaluation.py
--rw-r--r--   0        0        0     3734 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/clip_predictions.py
--rw-r--r--   0        0        0     1237 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/dataset.py
--rw-r--r--   0        0        0    10222 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/evaluation.py
--rw-r--r--   0        0        0     2214 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/evaluation_set.py
--rw-r--r--   0        0        0     2582 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/match.py
--rw-r--r--   0        0        0     1579 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/model_run.py
--rw-r--r--   0        0        0     1344 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/note.py
--rw-r--r--   0        0        0     5828 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/prediction_set.py
--rw-r--r--   0        0        0     4085 2024-01-05 11:51:57.333649 soundevent-1.3.5/src/soundevent/io/aoef/recording.py
--rw-r--r--   0        0        0     2457 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/io/aoef/recording_set.py
--rw-r--r--   0        0        0     2041 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/io/aoef/sequence.py
--rw-r--r--   0        0        0     2725 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/io/aoef/sequence_annotation.py
--rw-r--r--   0        0        0     2018 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/io/aoef/sequence_prediction.py
--rw-r--r--   0        0        0     1754 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/io/aoef/sound_event.py
--rw-r--r--   0        0        0     2598 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/io/aoef/sound_event_annotation.py
--rw-r--r--   0        0        0     2134 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/io/aoef/sound_event_prediction.py
--rw-r--r--   0        0        0     1039 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/io/aoef/tag.py
--rw-r--r--   0        0        0     1008 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/io/aoef/user.py
--rw-r--r--   0        0        0      825 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/io/formats.py
--rw-r--r--   0        0        0     3754 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/io/loader.py
--rw-r--r--   0        0        0     1758 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/io/saver.py
--rw-r--r--   0        0        0     1487 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/io/types.py
--rw-r--r--   0        0        0      410 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/plot/__init__.py
--rw-r--r--   0        0        0     3264 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/plot/annotation.py
--rw-r--r--   0        0        0      535 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/plot/common.py
--rw-r--r--   0        0        0     1693 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/plot/geometries.py
--rw-r--r--   0        0        0        0 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/plot/sound_event.py
--rw-r--r--   0        0        0     1713 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/plot/spectrogram.py
--rw-r--r--   0        0        0     1645 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/plot/tags.py
--rw-r--r--   0        0        0        0 2024-01-05 11:51:57.337649 soundevent-1.3.5/src/soundevent/py.typed
--rw-r--r--   0        0        0        0 2024-01-05 11:51:57.337649 soundevent-1.3.5/tests/__init__.py
--rw-r--r--   0        0        0     3930 2024-01-05 11:51:57.337649 soundevent-1.3.5/tests/conftest.py
--rw-r--r--   0        0        0   154964 2024-01-05 11:51:57.337649 soundevent-1.3.5/tests/data/nips4b_dataset.json
--rw-r--r--   0        0        0  2513927 2024-01-05 11:51:57.345649 soundevent-1.3.5/tests/data/nips4b_evaluation_set.json
--rw-r--r--   0        0        0   469324 2024-01-05 11:51:57.357649 soundevent-1.3.5/tests/data/nips4b_model_run.json
--rw-r--r--   0        0        0  5587694 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_audio/24bitdepth.wav
--rw-r--r--   0        0        0        0 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_audio/__init__.py
--rw-r--r--   0        0        0      266 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_audio/conftest.py
--rw-r--r--   0        0        0     5726 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_audio/test_audio.py
--rw-r--r--   0        0        0      792 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_audio/test_files.py
--rw-r--r--   0        0        0     4128 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_audio/test_filter.py
--rw-r--r--   0        0        0     2125 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_audio/test_io.py
--rw-r--r--   0        0        0     1222 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_audio/test_media_info.py
--rw-r--r--   0        0        0     1593 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_audio/test_raw.py
--rw-r--r--   0        0        0     3695 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_audio/test_resample.py
--rw-r--r--   0        0        0     2416 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_audio/test_scaling.py
--rw-r--r--   0        0        0     2677 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_audio/test_spectrograms.py
--rw-r--r--   0        0        0        0 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_data/__init__.py
--rw-r--r--   0        0        0     3608 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_data/test_datasets.py
--rw-r--r--   0        0        0     4703 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_data/test_evaluated_samples.py
--rw-r--r--   0        0        0    11288 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_data/test_geometry.py
--rw-r--r--   0        0        0      600 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_data/test_tags.py
--rw-r--r--   0        0        0        0 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_evaluation/__init__.py
--rw-r--r--   0        0        0      681 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_evaluation/test_affinity.py
--rw-r--r--   0        0        0     7957 2024-01-05 11:51:57.381649 soundevent-1.3.5/tests/test_evaluation/test_clip_classification.py
--rw-r--r--   0        0        0     5011 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_evaluation/test_clip_multilabel_classification.py
--rw-r--r--   0        0        0     5308 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_evaluation/test_encode.py
--rw-r--r--   0        0        0     4637 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_evaluation/test_matching.py
--rw-r--r--   0        0        0     1442 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_evaluation/test_metrics.py
--rw-r--r--   0        0        0     1186 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_evaluation/test_sound_event_detection.py
--rw-r--r--   0        0        0        0 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_geometry/__init__.py
--rw-r--r--   0        0        0     1443 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_geometry/conftest.py
--rw-r--r--   0        0        0     3506 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_geometry/test_conversion.py
--rw-r--r--   0        0        0     5576 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_geometry/test_features.py
--rw-r--r--   0        0        0     2029 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_geometry/test_html.py
--rw-r--r--   0        0        0     5276 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_geometry/test_operations.py
--rw-r--r--   0        0        0        0 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/__init__.py
--rw-r--r--   0        0        0     7241 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/conftest.py
--rw-r--r--   0        0        0    16071 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_annotation_projects.py
--rw-r--r--   0        0        0      525 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_annotation_set.py
--rw-r--r--   0        0        0        0 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/__init__.py
--rw-r--r--   0        0        0    11681 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/conftest.py
--rw-r--r--   0        0        0      805 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_annotation_project.py
--rw-r--r--   0        0        0      721 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_annotation_set.py
--rw-r--r--   0        0        0      760 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_annotation_task.py
--rw-r--r--   0        0        0     2615 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_api.py
--rw-r--r--   0        0        0      599 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_clip.py
--rw-r--r--   0        0        0      757 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_clip_annotations.py
--rw-r--r--   0        0        0      858 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_clip_evaluation.py
--rw-r--r--   0        0        0      879 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_clip_predictions.py
--rw-r--r--   0        0        0      739 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_evaluation.py
--rw-r--r--   0        0        0      837 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_evaluation_set.py
--rw-r--r--   0        0        0      623 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_match.py
--rw-r--r--   0        0        0      708 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_model_run.py
--rw-r--r--   0        0        0      599 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_note.py
--rw-r--r--   0        0        0      835 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_prediction_set.py
--rw-r--r--   0        0        0     1484 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_recording.py
--rw-r--r--   0        0        0      812 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_recording_set.py
--rw-r--r--   0        0        0      718 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_sequence.py
--rw-r--r--   0        0        0      964 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_sequence_annotation.py
--rw-r--r--   0        0        0      964 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_sequence_prediction.py
--rw-r--r--   0        0        0      883 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_sound_event_annotation.py
--rw-r--r--   0        0        0     1012 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_sound_event_prediction.py
--rw-r--r--   0        0        0      576 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_tag.py
--rw-r--r--   0        0        0      599 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_aoef/test_user.py
--rw-r--r--   0        0        0    10576 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_datasets.py
--rw-r--r--   0        0        0      649 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_evaluation.py
--rw-r--r--   0        0        0      502 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_evaluation_set.py
--rw-r--r--   0        0        0     6906 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_model_runs.py
--rw-r--r--   0        0        0      494 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_io/test_recording_set.py
--rw-r--r--   0        0        0      183 2024-01-05 11:51:57.385649 soundevent-1.3.5/tests/test_soundevent.py
--rw-r--r--   0        0        0     4895 1970-01-01 00:00:00.000000 soundevent-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-05-14 17:12:59.002503 soundevent-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3790 2024-05-14 17:12:59.002503 soundevent-2.0.0/README.md
+-rw-r--r--   0        0        0     2326 2024-05-14 17:13:14.978563 soundevent-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1430 2024-05-14 17:12:59.006502 soundevent-2.0.0/src/soundevent/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-14 17:12:59.006502 soundevent-2.0.0/src/soundevent/__version__.py
+-rw-r--r--   0        0        0     1256 2024-05-14 17:12:59.006502 soundevent-2.0.0/src/soundevent/arrays/__init__.py
+-rw-r--r--   0        0        0     3640 2024-05-14 17:12:59.006502 soundevent-2.0.0/src/soundevent/arrays/attributes.py
+-rw-r--r--   0        0        0    19259 2024-05-14 17:12:59.006502 soundevent-2.0.0/src/soundevent/arrays/dimensions.py
+-rw-r--r--   0        0        0    15416 2024-05-14 17:12:59.006502 soundevent-2.0.0/src/soundevent/arrays/operations.py
+-rw-r--r--   0        0        0      586 2024-05-14 17:12:59.006502 soundevent-2.0.0/src/soundevent/audio/__init__.py
+-rw-r--r--   0        0        0      253 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/audio/attributes.py
+-rw-r--r--   0        0        0     4111 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/audio/files.py
+-rw-r--r--   0        0        0     5471 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/audio/io.py
+-rw-r--r--   0        0        0     4895 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/audio/media_info.py
+-rw-r--r--   0        0        0     8534 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/audio/operations.py
+-rw-r--r--   0        0        0     4312 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/audio/spectrograms.py
+-rw-r--r--   0        0        0     2677 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/__init__.py
+-rw-r--r--   0        0        0     1489 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/annotation_projects.py
+-rw-r--r--   0        0        0      933 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/annotation_sets.py
+-rw-r--r--   0        0        0     2340 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/annotation_tasks.py
+-rw-r--r--   0        0        0     2135 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/clip_annotations.py
+-rw-r--r--   0        0        0     4990 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/clip_evaluations.py
+-rw-r--r--   0        0        0     3984 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/clip_predictions.py
+-rw-r--r--   0        0        0     4359 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/clips.py
+-rw-r--r--   0        0        0     1624 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/datasets.py
+-rw-r--r--   0        0        0      410 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/evaluation_sets.py
+-rw-r--r--   0        0        0     1094 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/evaluations.py
+-rw-r--r--   0        0        0     4820 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/features.py
+-rw-r--r--   0        0        0    31881 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/geometries.py
+-rw-r--r--   0        0        0     4136 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/matches.py
+-rw-r--r--   0        0        0      262 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/model_runs.py
+-rw-r--r--   0        0        0     4552 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/notes.py
+-rw-r--r--   0        0        0     2249 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/predicted_tags.py
+-rw-r--r--   0        0        0     3008 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/prediction_sets.py
+-rw-r--r--   0        0        0      428 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/recording_sets.py
+-rw-r--r--   0        0        0     8259 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/recordings.py
+-rw-r--r--   0        0        0     1250 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/sequence_annotations.py
+-rw-r--r--   0        0        0      859 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/sequence_predictions.py
+-rw-r--r--   0        0        0     3271 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/sequences.py
+-rw-r--r--   0        0        0     5081 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/sound_event_annotations.py
+-rw-r--r--   0        0        0     2215 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/sound_event_predictions.py
+-rw-r--r--   0        0        0     2711 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/sound_events.py
+-rw-r--r--   0        0        0     4513 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/tags.py
+-rw-r--r--   0        0        0      355 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/data/users.py
+-rw-r--r--   0        0        0      762 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/evaluation/__init__.py
+-rw-r--r--   0        0        0     3813 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/evaluation/affinity.py
+-rw-r--r--   0        0        0     8319 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/evaluation/encoding.py
+-rw-r--r--   0        0        0     2832 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/evaluation/match.py
+-rw-r--r--   0        0        0     5426 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/evaluation/metrics.py
+-rw-r--r--   0        0        0      530 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/evaluation/tasks/__init__.py
+-rw-r--r--   0        0        0     4685 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/evaluation/tasks/clip_classification.py
+-rw-r--r--   0        0        0     4548 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/evaluation/tasks/clip_multilabel_classification.py
+-rw-r--r--   0        0        0      576 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/evaluation/tasks/common.py
+-rw-r--r--   0        0        0     5796 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/evaluation/tasks/sound_event_classification.py
+-rw-r--r--   0        0        0     7597 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/evaluation/tasks/sound_event_detection.py
+-rw-r--r--   0        0        0     1328 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/geometry/__init__.py
+-rw-r--r--   0        0        0     4987 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/geometry/conversion.py
+-rw-r--r--   0        0        0     8647 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/geometry/features.py
+-rw-r--r--   0        0        0     3578 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/geometry/html.py
+-rw-r--r--   0        0        0    12667 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/geometry/operations.py
+-rw-r--r--   0        0        0      324 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/__init__.py
+-rw-r--r--   0        0        0     6199 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/__init__.py
+-rw-r--r--   0        0        0     4697 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/adapters.py
+-rw-r--r--   0        0        0     3201 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/annotation_project.py
+-rw-r--r--   0        0        0     6205 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/annotation_set.py
+-rw-r--r--   0        0        0     2942 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/annotation_task.py
+-rw-r--r--   0        0        0     1868 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/clip.py
+-rw-r--r--   0        0        0     4032 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/clip_annotations.py
+-rw-r--r--   0        0        0     3098 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/clip_evaluation.py
+-rw-r--r--   0        0        0     3983 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/clip_predictions.py
+-rw-r--r--   0        0        0     1236 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/dataset.py
+-rw-r--r--   0        0        0    10277 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/evaluation.py
+-rw-r--r--   0        0        0     2281 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/evaluation_set.py
+-rw-r--r--   0        0        0     2621 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/match.py
+-rw-r--r--   0        0        0     1578 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/model_run.py
+-rw-r--r--   0        0        0     1343 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/note.py
+-rw-r--r--   0        0        0     5827 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/prediction_set.py
+-rw-r--r--   0        0        0     4140 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/recording.py
+-rw-r--r--   0        0        0     2456 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/recording_set.py
+-rw-r--r--   0        0        0     2079 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/sequence.py
+-rw-r--r--   0        0        0     2924 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/sequence_annotation.py
+-rw-r--r--   0        0        0     2077 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/sequence_prediction.py
+-rw-r--r--   0        0        0     1793 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/sound_event.py
+-rw-r--r--   0        0        0     2757 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/sound_event_annotation.py
+-rw-r--r--   0        0        0     2193 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/sound_event_prediction.py
+-rw-r--r--   0        0        0     1038 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/tag.py
+-rw-r--r--   0        0        0     1007 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/aoef/user.py
+-rw-r--r--   0        0        0     1043 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/crowsetta/__init__.py
+-rw-r--r--   0        0        0     8136 2024-05-14 17:12:59.010502 soundevent-2.0.0/src/soundevent/io/crowsetta/annotation.py
+-rw-r--r--   0        0        0     6194 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/io/crowsetta/bbox.py
+-rw-r--r--   0        0        0     8520 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/io/crowsetta/labels.py
+-rw-r--r--   0        0        0     7445 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/io/crowsetta/segment.py
+-rw-r--r--   0        0        0     4069 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/io/crowsetta/sequence.py
+-rw-r--r--   0        0        0      826 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/io/formats.py
+-rw-r--r--   0        0        0     3912 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/io/loader.py
+-rw-r--r--   0        0        0     1999 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/io/saver.py
+-rw-r--r--   0        0        0     1488 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/io/types.py
+-rw-r--r--   0        0        0      558 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/plot/__init__.py
+-rw-r--r--   0        0        0     2348 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/plot/annotation.py
+-rw-r--r--   0        0        0      536 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/plot/common.py
+-rw-r--r--   0        0        0     4075 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/plot/geometries.py
+-rw-r--r--   0        0        0     2517 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/plot/prediction.py
+-rw-r--r--   0        0        0     1686 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/plot/tags.py
+-rw-r--r--   0        0        0        0 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/py.typed
+-rw-r--r--   0        0        0     3008 2024-05-14 17:12:59.014503 soundevent-2.0.0/src/soundevent/types.py
+-rw-r--r--   0        0        0        0 2024-05-14 17:12:59.014503 soundevent-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     4104 2024-05-14 17:12:59.014503 soundevent-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0   154964 2024-05-14 17:12:59.014503 soundevent-2.0.0/tests/data/nips4b_dataset.json
+-rw-r--r--   0        0        0  2513927 2024-05-14 17:12:59.026502 soundevent-2.0.0/tests/data/nips4b_evaluation_set.json
+-rw-r--r--   0        0        0   469324 2024-05-14 17:12:59.034503 soundevent-2.0.0/tests/data/nips4b_model_run.json
+-rw-r--r--   0        0        0        0 2024-05-14 17:12:59.034503 soundevent-2.0.0/tests/test_array/__init__.py
+-rw-r--r--   0        0        0     6437 2024-05-14 17:12:59.034503 soundevent-2.0.0/tests/test_array/test_dimensions.py
+-rw-r--r--   0        0        0    14946 2024-05-14 17:12:59.034503 soundevent-2.0.0/tests/test_array/test_operations.py
+-rw-r--r--   0        0        0  5587694 2024-05-14 17:12:59.062503 soundevent-2.0.0/tests/test_audio/24bitdepth.wav
+-rw-r--r--   0        0        0        0 2024-05-14 17:12:59.062503 soundevent-2.0.0/tests/test_audio/__init__.py
+-rw-r--r--   0        0        0      267 2024-05-14 17:12:59.062503 soundevent-2.0.0/tests/test_audio/conftest.py
+-rw-r--r--   0        0        0    16072 2024-05-14 17:12:59.062503 soundevent-2.0.0/tests/test_audio/data/aiff_alaw.aiff
+-rw-r--r--   0        0        0   128096 2024-05-14 17:12:59.062503 soundevent-2.0.0/tests/test_audio/data/aiff_double.aiff
+-rw-r--r--   0        0        0    64096 2024-05-14 17:12:59.062503 soundevent-2.0.0/tests/test_audio/data/aiff_float.aiff
+-rw-r--r--   0        0        0     8572 2024-05-14 17:12:59.062503 soundevent-2.0.0/tests/test_audio/data/aiff_ima_adpcm.aiff
+-rw-r--r--   0        0        0    32054 2024-05-14 17:12:59.062503 soundevent-2.0.0/tests/test_audio/data/aiff_pcm_16.aiff
+-rw-r--r--   0        0        0    48054 2024-05-14 17:12:59.062503 soundevent-2.0.0/tests/test_audio/data/aiff_pcm_24.aiff
+-rw-r--r--   0        0        0    64054 2024-05-14 17:12:59.062503 soundevent-2.0.0/tests/test_audio/data/aiff_pcm_32.aiff
+-rw-r--r--   0        0        0    16054 2024-05-14 17:12:59.062503 soundevent-2.0.0/tests/test_audio/data/aiff_pcm_s8.aiff
+-rw-r--r--   0        0        0    16072 2024-05-14 17:12:59.062503 soundevent-2.0.0/tests/test_audio/data/aiff_pcm_u8.aiff
+-rw-r--r--   0        0        0    16072 2024-05-14 17:12:59.062503 soundevent-2.0.0/tests/test_audio/data/aiff_ulaw.aiff
+-rw-r--r--   0        0        0    16024 2024-05-14 17:12:59.062503 soundevent-2.0.0/tests/test_audio/data/au_alaw.au
+-rw-r--r--   0        0        0   128024 2024-05-14 17:12:59.062503 soundevent-2.0.0/tests/test_audio/data/au_double.au
+-rw-r--r--   0        0        0    64024 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/au_float.au
+-rw-r--r--   0        0        0    32024 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/au_pcm_16.au
+-rw-r--r--   0        0        0    48024 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/au_pcm_24.au
+-rw-r--r--   0        0        0    64024 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/au_pcm_32.au
+-rw-r--r--   0        0        0    16024 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/au_pcm_s8.au
+-rw-r--r--   0        0        0    16024 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/au_ulaw.au
+-rw-r--r--   0        0        0    32128 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/avr_pcm_16.avr
+-rw-r--r--   0        0        0    16128 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/avr_pcm_s8.avr
+-rw-r--r--   0        0        0    16128 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/avr_pcm_u8.avr
+-rw-r--r--   0        0        0    32168 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/caf_alac_16.caf
+-rw-r--r--   0        0        0    40168 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/caf_alac_20.caf
+-rw-r--r--   0        0        0    48168 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/caf_alac_24.caf
+-rw-r--r--   0        0        0    64172 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/caf_alac_32.caf
+-rw-r--r--   0        0        0    20096 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/caf_alaw.caf
+-rw-r--r--   0        0        0   132096 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/caf_double.caf
+-rw-r--r--   0        0        0    68096 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/caf_float.caf
+-rw-r--r--   0        0        0    36096 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/caf_pcm_16.caf
+-rw-r--r--   0        0        0    52096 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/caf_pcm_24.caf
+-rw-r--r--   0        0        0    68096 2024-05-14 17:12:59.066503 soundevent-2.0.0/tests/test_audio/data/caf_pcm_32.caf
+-rw-r--r--   0        0        0    20096 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/caf_pcm_s8.caf
+-rw-r--r--   0        0        0    20096 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/caf_ulaw.caf
+-rw-r--r--   0        0        0    31361 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/flac_pcm_16.flac
+-rw-r--r--   0        0        0    47375 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/flac_pcm_24.flac
+-rw-r--r--   0        0        0    15342 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/flac_pcm_s8.flac
+-rw-r--r--   0        0        0    32012 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/htk_pcm_16.htk
+-rw-r--r--   0        0        0    17024 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/ircam_alaw.ircam
+-rw-r--r--   0        0        0    65024 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/ircam_float.ircam
+-rw-r--r--   0        0        0    33024 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/ircam_pcm_16.ircam
+-rw-r--r--   0        0        0    65024 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/ircam_pcm_32.ircam
+-rw-r--r--   0        0        0    17024 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/ircam_ulaw.ircam
+-rw-r--r--   0        0        0   128068 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/mat4_double.mat4
+-rw-r--r--   0        0        0    64068 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/mat4_float.mat4
+-rw-r--r--   0        0        0    32068 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/mat4_pcm_16.mat4
+-rw-r--r--   0        0        0    64068 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/mat4_pcm_32.mat4
+-rw-r--r--   0        0        0   128264 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/mat5_double.mat5
+-rw-r--r--   0        0        0    64264 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/mat5_float.mat5
+-rw-r--r--   0        0        0    32264 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/mat5_pcm_16.mat5
+-rw-r--r--   0        0        0    64264 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/mat5_pcm_32.mat5
+-rw-r--r--   0        0        0    16264 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/mat5_pcm_u8.mat5
+-rw-r--r--   0        0        0     4968 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/mp3_mpeg_layer_iii.mp3
+-rw-r--r--   0        0        0    32042 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/mpc2k_pcm_16.mpc2k
+-rw-r--r--   0        0        0    17024 2024-05-14 17:12:59.070503 soundevent-2.0.0/tests/test_audio/data/nist_alaw.nist
+-rw-r--r--   0        0        0    33024 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/nist_pcm_16.nist
+-rw-r--r--   0        0        0    49024 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/nist_pcm_24.nist
+-rw-r--r--   0        0        0    65024 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/nist_pcm_32.nist
+-rw-r--r--   0        0        0    17024 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/nist_pcm_s8.nist
+-rw-r--r--   0        0        0    17024 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/nist_ulaw.nist
+-rw-r--r--   0        0        0     3901 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/ogg_opus.ogg
+-rw-r--r--   0        0        0     8614 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/ogg_vorbis.ogg
+-rw-r--r--   0        0        0    34048 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/paf_pcm_16.paf
+-rw-r--r--   0        0        0    53248 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/paf_pcm_24.paf
+-rw-r--r--   0        0        0    18048 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/paf_pcm_s8.paf
+-rw-r--r--   0        0        0    32016 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/pvf_pcm_16.pvf
+-rw-r--r--   0        0        0    64016 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/pvf_pcm_32.pvf
+-rw-r--r--   0        0        0    16015 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/pvf_pcm_s8.pvf
+-rw-r--r--   0        0        0    16104 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/rf64_alaw.rf64
+-rw-r--r--   0        0        0   128104 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/rf64_double.rf64
+-rw-r--r--   0        0        0    64104 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/rf64_float.rf64
+-rw-r--r--   0        0        0    32104 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/rf64_pcm_16.rf64
+-rw-r--r--   0        0        0    48104 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/rf64_pcm_24.rf64
+-rw-r--r--   0        0        0    64104 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/rf64_pcm_32.rf64
+-rw-r--r--   0        0        0    16104 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/rf64_pcm_u8.rf64
+-rw-r--r--   0        0        0    16104 2024-05-14 17:12:59.074503 soundevent-2.0.0/tests/test_audio/data/rf64_ulaw.rf64
+-rw-r--r--   0        0        0    50821 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/sds_pcm_16.sds
+-rw-r--r--   0        0        0    67839 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/sds_pcm_24.sds
+-rw-r--r--   0        0        0    33930 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/sds_pcm_s8.sds
+-rw-r--r--   0        0        0    32114 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/svx_pcm_16.svx
+-rw-r--r--   0        0        0    16114 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/svx_pcm_s8.svx
+-rw-r--r--   0        0        0    16043 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/voc_alaw.voc
+-rw-r--r--   0        0        0    32043 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/voc_pcm_16.voc
+-rw-r--r--   0        0        0    16033 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/voc_pcm_u8.voc
+-rw-r--r--   0        0        0    16043 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/voc_ulaw.voc
+-rw-r--r--   0        0        0    16136 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/w64_alaw.w64
+-rw-r--r--   0        0        0   128136 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/w64_double.w64
+-rw-r--r--   0        0        0    64136 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/w64_float.w64
+-rw-r--r--   0        0        0     8336 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/w64_ima_adpcm.w64
+-rw-r--r--   0        0        0     8368 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/w64_ms_adpcm.w64
+-rw-r--r--   0        0        0    32104 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/w64_pcm_16.w64
+-rw-r--r--   0        0        0    48104 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/w64_pcm_24.w64
+-rw-r--r--   0        0        0    64104 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/w64_pcm_32.w64
+-rw-r--r--   0        0        0    16104 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/w64_pcm_u8.w64
+-rw-r--r--   0        0        0    16136 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/w64_ulaw.w64
+-rw-r--r--   0        0        0    16058 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/wav_alaw.wav
+-rw-r--r--   0        0        0   128080 2024-05-14 17:12:59.078503 soundevent-2.0.0/tests/test_audio/data/wav_double.wav
+-rw-r--r--   0        0        0    64080 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wav_float.wav
+-rw-r--r--   0        0        0     8252 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wav_ima_adpcm.wav
+-rw-r--r--   0        0        0     8282 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wav_ms_adpcm.wav
+-rw-r--r--   0        0        0    32044 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wav_pcm_16.wav
+-rw-r--r--   0        0        0    48044 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wav_pcm_24.wav
+-rw-r--r--   0        0        0    64044 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wav_pcm_32.wav
+-rw-r--r--   0        0        0    16044 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wav_pcm_u8.wav
+-rw-r--r--   0        0        0    16058 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wav_ulaw.wav
+-rw-r--r--   0        0        0    16080 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wavex_alaw.wavex
+-rw-r--r--   0        0        0   128104 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wavex_double.wavex
+-rw-r--r--   0        0        0    64104 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wavex_float.wavex
+-rw-r--r--   0        0        0    32080 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wavex_pcm_16.wavex
+-rw-r--r--   0        0        0    48080 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wavex_pcm_24.wavex
+-rw-r--r--   0        0        0    64080 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wavex_pcm_32.wavex
+-rw-r--r--   0        0        0    16080 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wavex_pcm_u8.wavex
+-rw-r--r--   0        0        0    16080 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wavex_ulaw.wavex
+-rw-r--r--   0        0        0    16032 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/data/wve_alaw.wve
+-rw-r--r--   0        0        0    10217 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/test_audio.py
+-rw-r--r--   0        0        0     4896 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/test_files.py
+-rw-r--r--   0        0        0     2315 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/test_io.py
+-rw-r--r--   0        0        0     1665 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/test_media_info.py
+-rw-r--r--   0        0        0     7343 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/test_operations.py
+-rw-r--r--   0        0        0     3820 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_audio/test_spectrograms.py
+-rw-r--r--   0        0        0        0 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_data/__init__.py
+-rw-r--r--   0        0        0     3608 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_data/test_datasets.py
+-rw-r--r--   0        0        0     4703 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_data/test_evaluated_samples.py
+-rw-r--r--   0        0        0    11287 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_data/test_geometry.py
+-rw-r--r--   0        0        0      600 2024-05-14 17:12:59.082503 soundevent-2.0.0/tests/test_data/test_tags.py
+-rw-r--r--   0        0        0        0 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_evaluation/__init__.py
+-rw-r--r--   0        0        0      681 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_evaluation/test_affinity.py
+-rw-r--r--   0        0        0     7953 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_evaluation/test_clip_classification.py
+-rw-r--r--   0        0        0     5010 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_evaluation/test_clip_multilabel_classification.py
+-rw-r--r--   0        0        0     5308 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_evaluation/test_encode.py
+-rw-r--r--   0        0        0     4637 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_evaluation/test_matching.py
+-rw-r--r--   0        0        0     1442 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_evaluation/test_metrics.py
+-rw-r--r--   0        0        0     1187 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_evaluation/test_sound_event_detection.py
+-rw-r--r--   0        0        0        0 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_geometry/__init__.py
+-rw-r--r--   0        0        0     1443 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_geometry/conftest.py
+-rw-r--r--   0        0        0     3506 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_geometry/test_conversion.py
+-rw-r--r--   0        0        0     6031 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_geometry/test_features.py
+-rw-r--r--   0        0        0     2030 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_geometry/test_html.py
+-rw-r--r--   0        0        0    11565 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_geometry/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/__init__.py
+-rw-r--r--   0        0        0     7819 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/conftest.py
+-rw-r--r--   0        0        0    16071 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_annotation_projects.py
+-rw-r--r--   0        0        0      525 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_annotation_set.py
+-rw-r--r--   0        0        0        0 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/__init__.py
+-rw-r--r--   0        0        0    11681 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/conftest.py
+-rw-r--r--   0        0        0      805 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_annotation_project.py
+-rw-r--r--   0        0        0      721 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_annotation_set.py
+-rw-r--r--   0        0        0      760 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_annotation_task.py
+-rw-r--r--   0        0        0     2582 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_api.py
+-rw-r--r--   0        0        0      599 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_clip.py
+-rw-r--r--   0        0        0      757 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_clip_annotations.py
+-rw-r--r--   0        0        0      858 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_clip_evaluation.py
+-rw-r--r--   0        0        0      879 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_clip_predictions.py
+-rw-r--r--   0        0        0      739 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_evaluation.py
+-rw-r--r--   0        0        0      837 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_evaluation_set.py
+-rw-r--r--   0        0        0      622 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_match.py
+-rw-r--r--   0        0        0      707 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_model_run.py
+-rw-r--r--   0        0        0      599 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_note.py
+-rw-r--r--   0        0        0      835 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_prediction_set.py
+-rw-r--r--   0        0        0     1484 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_recording.py
+-rw-r--r--   0        0        0      812 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_recording_set.py
+-rw-r--r--   0        0        0      718 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_sequence.py
+-rw-r--r--   0        0        0      964 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_sequence_annotation.py
+-rw-r--r--   0        0        0      964 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_sequence_prediction.py
+-rw-r--r--   0        0        0      882 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_sound_event_annotation.py
+-rw-r--r--   0        0        0     1012 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_sound_event_prediction.py
+-rw-r--r--   0        0        0      576 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_tag.py
+-rw-r--r--   0        0        0      599 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_aoef/test_user.py
+-rw-r--r--   0        0        0        0 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_crowsetta/__init__.py
+-rw-r--r--   0        0        0     9996 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_crowsetta/test_annotation.py
+-rw-r--r--   0        0        0     5692 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_crowsetta/test_bbox.py
+-rw-r--r--   0        0        0     2049 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_crowsetta/test_import.py
+-rw-r--r--   0        0        0     6737 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_crowsetta/test_labels.py
+-rw-r--r--   0        0        0     5312 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_crowsetta/test_segments.py
+-rw-r--r--   0        0        0     5025 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_crowsetta/test_sequence.py
+-rw-r--r--   0        0        0    10576 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_datasets.py
+-rw-r--r--   0        0        0      649 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_evaluation.py
+-rw-r--r--   0        0        0      502 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_evaluation_set.py
+-rw-r--r--   0        0        0     6906 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_model_runs.py
+-rw-r--r--   0        0        0      494 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_io/test_recording_set.py
+-rw-r--r--   0        0        0      260 2024-05-14 17:12:59.086503 soundevent-2.0.0/tests/test_soundevent.py
+-rw-r--r--   0        0        0     5239 1970-01-01 00:00:00.000000 soundevent-2.0.0/PKG-INFO
```

### Comparing `soundevent-1.3.5/LICENSE` & `soundevent-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/README.md` & `soundevent-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/pyproject.toml` & `soundevent-2.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "soundevent"
-version = "1.3.5"
+version = "2.0.0"
 description = "soundevent is an open-source Python package for the computational biocoustic community, providing standardized tools for sound event analysis and data management."
 authors = [
     { name = "Santiago Martinez", email = "santiago.balvanera.20@ucl.ac.uk" },
 ]
 dependencies = [
     "pydantic>=2.0",
     "email-validator>=2.0",
@@ -26,88 +26,102 @@
     "soundfile>=0.12.1",
 ]
 evaluation = [
     "scikit-learn>=1.3.2",
 ]
 geometry = [
     "shapely>=2.0.1",
+    "rasterio>=1.3.10",
+    "xarray>=2023.1.0",
+]
+crowsetta = [
+    "crowsetta>=4.0.0.post2,<5.0",
+    "importlib-resources<6.0,>=5.0; python_version < \"3.9\"",
 ]
 all = [
     "soundevent[plot]",
     "soundevent[audio]",
     "soundevent[evaluation]",
     "soundevent[geometry]",
+    "soundevent[crowsetta]",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
-[tool.pdm.dev-dependencies]
-dev = [
+[tool.rye]
+dev-dependencies = [
+    "icecream>=2.1.3",
     "pytest>=7.4.0",
     "coverage[toml]>=7.3.2",
-    "black>=23.3.0",
-    "mypy>=1.4.1",
     "pytest-coverage>=0.0",
     "mkdocs>=1.2.4",
     "importlib-metadata>=4.3",
     "ruff>=0.0.276",
     "mkdocs-material>=9.1.18",
     "isort>=5.11.5",
     "mkdocstrings[python]>=0.22.0",
     "tox>=4.6.3",
     "hypothesis>=6.79.4",
     "mkdocs-gallery>=0.7.8",
     "memory-profiler>=0.61.0",
     "pytest-watch>=4.2.0",
     "pytest-testmon>=2.0.12",
     "html5lib>=1.1",
+    "pyright>=1.1.362",
+    "pytest-xdist>=3.6.1",
+    "ipykernel>=6.29.4",
 ]
 
-[tool.docformatter]
-style = "numpy"
-wrap-summaries = 79
-wrap-descriptions = 79
+[tool.pytest.ini_options]
+addopts = "-vv"
 
-[tool.black]
+[tool.ruff]
 line-length = 79
+target-version = "py38"
 
-[tool.pytest.ini_options]
-addopts = "-vv"
+[tool.ruff.format]
+docstring-code-format = true
+docstring-code-line-length = 60
+
+[tool.ruff.lint]
+select = [
+    "E4",
+    "E7",
+    "E9",
+    "F",
+    "B",
+    "Q",
+    "I",
+    "D",
+]
+ignore = [
+    "D1",
+]
+
+[tool.ruff.lint.pydocstyle]
+convention = "numpy"
+
+[tool.ruff.lint.isort]
+known-local-folder = [
+    "src",
+    "soundevent",
+]
 
 [tool.pyright]
 venvPath = "."
 venv = ".venv"
 include = [
     "src",
-    "tests",
 ]
 verboseOutput = true
 
-[tool.pydocstyle]
-convention = "numpy"
-match = "(?!test_).*\\.py"
-match_dir = "(?!tests).*"
-
-[tool.isort]
-profile = "black"
-
-[tool.mypy]
-ignore_missing_imports = true
-show_error_codes = true
-show_error_code_links = true
-disable_error_code = [
-    "call-overload",
-    "misc",
-    "override",
-]
-
 [tool.coverage.run]
 branch = true
 source = [
     "src/soundevent",
 ]
 command_line = "-m pytest"
 omit = [
```

### Comparing `soundevent-1.3.5/src/soundevent/__init__.py` & `soundevent-2.0.0/src/soundevent/__init__.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/src/soundevent/audio/__init__.py` & `soundevent-2.0.0/src/soundevent/audio/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 """Soundevent functions for handling audio files and arrays."""
 
-from .files import is_audio_file
-from .filter import filter_audio
+from .files import get_audio_files, is_audio_file
 from .io import load_audio, load_clip, load_recording
 from .media_info import MediaInfo, compute_md5_checksum, get_media_info
-from .resample import resample_audio
-from .scaling import clamp_amplitude, pcen, scale_amplitude
+from .operations import filter, pcen, resample
 from .spectrograms import compute_spectrogram
 
 __all__ = [
     "MediaInfo",
     "compute_spectrogram",
     "compute_md5_checksum",
     "get_media_info",
+    "get_audio_files",
     "load_audio",
     "load_clip",
     "load_recording",
     "is_audio_file",
-    "resample_audio",
-    "filter_audio",
-    "scale_amplitude",
-    "clamp_amplitude",
+    "resample",
+    "filter",
     "pcen",
 ]
```

### Comparing `soundevent-1.3.5/src/soundevent/audio/media_info.py` & `soundevent-2.0.0/src/soundevent/audio/media_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,68 @@
 """Functions for getting media information from WAV files."""
+
 import hashlib
 import struct
 from dataclasses import dataclass
-from typing import IO
 
-from soundevent.audio.chunks import Chunk, parse_into_chunks
+import soundfile as sf
+
 from soundevent.data.recordings import PathLike
 
 __all__ = [
     "MediaInfo",
     "get_media_info",
     "compute_md5_checksum",
+    "compute_sha2_checksum",
 ]
 
 
 @dataclass
-class FormatInfo:
-    """Information stored in the format chunk."""
-
-    audio_format: int
-    """Format code for the waveform audio data."""
-
-    bit_depth: int
-    """Bit depth."""
-
-    samplerate: int
-    """Sample rate in Hz."""
-
-    channels: int
-    """Number of channels."""
-
-    byte_rate: int
-    """Byte rate.
+class MediaInfo:
+    """MediaInfo Class.
 
-    byte_rate = samplerate * channels * bit_depth/8
+    Encapsulates essential metadata about audio data for processing and
+    analysis. The information stored in this dataclass can typically be
+    automatically extracted from the audio file itself.
     """
 
-    block_align: int
-    """Block align.
+    samplerate_hz: int
+    """The sampling rate of the audio, measured in Hertz (Hz). 
 
-    The number of bytes for one sample including all channels.
-    block_align = channels * bit_depth/8
+    This indicates the number of samples taken per second to represent the
+    analog audio signal.
     """
 
+    duration_s: float
+    """The total duration of the audio, measured in seconds (s).
 
-@dataclass
-class MediaInfo:
-    """MediaInfo Class.
-
-    MediaInfo encapsulates essential information about audio data, providing
-    key details necessary for processing and analysis. It includes format code,
-    bit depth, sample rate, duration, number of samples, and channel
-    information. The MediaInfo attributes can be automatically extracted from
-    the audio file itself.
-
-    Attributes
-    ----------
-    audio_format
-        Format code representing the waveform audio data format.
-    bit_depth
-        Bit depth, indicating the number of bits per sample.
-    samplerate_hz
-        Sample rate in Hertz (Hz), denoting the number of samples per second.
-    duration_s
-        Duration of the audio data in seconds.
-    samples
-        Total number of samples in the audio data.
-    channels
-        Number of audio channels, indicating whether the audio is mono, stereo,
-        or multichannel.
+    This represents the length of time the audio recording spans.
     """
 
-    audio_format: int
-    bit_depth: int
-    samplerate_hz: int
-    duration_s: float
     samples: int
+    """The total number of samples in the audio data."""
+
     channels: int
+    """The number of audio channels present in the data.
 
+    For example 1 for mono, 2 for stereo."""
 
-def extract_media_info_from_chunks(
-    fp: IO[bytes],
-    fmt_chunk: Chunk,
-) -> FormatInfo:
-    """Return the media information from the fmt chunk.
+    format: str
+    """A code representing the audio file format. 
 
-    Parameters
-    ----------
-    fp : BytesIO
-        File pointer to the WAV file.
-    chunk : Chunk
-        The fmt chunk.
+    For example "WAV", "MP3".
+    """
 
-    Returns
-    -------
-    MediaInfo
+    subtype: str
+    """A more specific subtype of the audio format. 
 
-    Notes
-    -----
-    The structure of the format chunk is described in
-    (WAV PCM soundfile format)[http://soundfile.sapp.org/doc/WaveFormat/].
+    For example "PCM_16", "A_LAW". These subtypes provide additional
+    information about the audio data, such as the bit depth for PCM encoded
+    audio, or encoding algorithm for compressed audio formats.
     """
-    # Go to the start of the fmt chunk after the chunk id and
-    # chunk size.
-    fp.seek(fmt_chunk.position + 8)
-
-    audio_format = int.from_bytes(fp.read(2), "little")
-    channels = int.from_bytes(fp.read(2), "little")
-    samplerate = int.from_bytes(fp.read(4), "little")
-    byte_rate = int.from_bytes(fp.read(4), "little")
-    block_align = int.from_bytes(fp.read(2), "little")
-    bit_depth = int.from_bytes(fp.read(2), "little")
-
-    return FormatInfo(
-        audio_format=audio_format,
-        bit_depth=bit_depth,
-        samplerate=samplerate,
-        channels=channels,
-        byte_rate=byte_rate,
-        block_align=block_align,
-    )
 
 
 def get_media_info(path: PathLike) -> MediaInfo:
     """Return the media information from the WAV file.
 
     The information extracted from the WAV file is the audio format,
     the bit depth, the sample rate, the duration, the number of
@@ -140,38 +79,23 @@
         Information about the WAV file.
 
     Raises
     ------
     ValueError
         If the WAV file is not PCM encoded.
     """
-    with open(path, "rb") as wav:
-        chunk = parse_into_chunks(wav)
-
-        # Get info from the fmt chunk
-        fmt = chunk.subchunks["fmt "]
-        fmt_info = extract_media_info_from_chunks(wav, fmt)
-
-        # Get size of data chunk. Notice that the size of the data
-        # chunk is the size of the data subchunk divided by the number
-        # of channels and the bit depth.
-        data_chunk = chunk.subchunks["data"]
-        samples = (
-            8 * data_chunk.size // (fmt_info.channels * fmt_info.bit_depth)
-        )
-        duration = samples / fmt_info.samplerate
-
-        return MediaInfo(
-            audio_format=fmt_info.audio_format,
-            bit_depth=fmt_info.bit_depth,
-            samplerate_hz=fmt_info.samplerate,
-            duration_s=duration,
-            samples=samples,
-            channels=fmt_info.channels,
-        )
+    info = sf.info(path)
+    return MediaInfo(
+        samplerate_hz=info.samplerate,
+        duration_s=info.duration,
+        samples=info.frames,
+        channels=info.channels,
+        format=info.format,
+        subtype=info.subtype,
+    )
 
 
 BUFFER_SIZE = 65536
 
 
 def compute_md5_checksum(path: PathLike) -> str:
     """Compute the MD5 checksum of a file.
@@ -191,14 +115,36 @@
         buffer = fp.read(BUFFER_SIZE)
         while len(buffer) > 0:
             md5.update(buffer)
             buffer = fp.read(BUFFER_SIZE)
     return md5.hexdigest()
 
 
+def compute_sha2_checksum(path: PathLike) -> str:
+    """Compute the SHA-256 checksum of a file.
+
+    Parameters
+    ----------
+    path
+        Path to the file.
+
+    Returns
+    -------
+    str
+        SHA-256 checksum of the file.
+    """
+    sha2 = hashlib.sha256()
+    with open(path, "rb") as fp:
+        buffer = fp.read(BUFFER_SIZE)
+        while len(buffer) > 0:
+            sha2.update(buffer)
+            buffer = fp.read(BUFFER_SIZE)
+    return sha2.hexdigest()
+
+
 def generate_wav_header(
     samplerate: int,
     channels: int,
     samples: int,
     bit_depth: int = 16,
 ) -> bytes:
     """Generate the data of a WAV header.
@@ -221,15 +167,14 @@
         The number of bits per sample. By default, it is 16 bits.
 
     Notes
     -----
     The structure of the WAV header is described in
     (WAV PCM soundfile format)[http://soundfile.sapp.org/doc/WaveFormat/].
     """
-
     data_size = samples * channels * bit_depth // 8
     byte_rate = samplerate * channels * bit_depth // 8
     block_align = channels * bit_depth // 8
 
     return struct.pack(
         "<4si4s4sihhiihh4si",  # Format string
         b"RIFF",  # RIFF chunk id
```

### Comparing `soundevent-1.3.5/src/soundevent/data/__init__.py` & `soundevent-2.0.0/src/soundevent/data/__init__.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/src/soundevent/data/annotation_projects.py` & `soundevent-2.0.0/src/soundevent/data/annotation_projects.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/src/soundevent/data/annotation_sets.py` & `soundevent-2.0.0/src/soundevent/data/annotation_sets.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/src/soundevent/data/annotation_tasks.py` & `soundevent-2.0.0/src/soundevent/data/annotation_tasks.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/src/soundevent/data/clip_annotations.py` & `soundevent-2.0.0/src/soundevent/data/clip_annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module for managing annotations related to audio clips.
 
 This module defines the `ClipAnnotations` class, representing a collection of
 annotations associated with a specific audio clip. It includes details about
 the clip, associated tags, annotations, status badges indicating the state of
 the annotation process, and any additional notes related to the annotations.
 """
+
 import datetime
 from typing import List
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel, Field
 
 from soundevent.data.clips import Clip
@@ -38,15 +39,17 @@
     clip
         The Clip instance representing the audio clip associated with these annotations.
     tags
         A list of Tag instances defining the set of tags associated with the clip.
     annotations
         A list of Annotation instances representing detailed annotations of
         sound events in the clip.
-    notes
+
+    Notes
+    -----
         A list of Note instances representing additional contextual
         information or remarks associated with the clip.
     """
 
     uuid: UUID = Field(default_factory=uuid4)
     clip: Clip
     sound_events: List[SoundEventAnnotation] = Field(default_factory=list)
```

### Comparing `soundevent-1.3.5/src/soundevent/data/clip_evaluations.py` & `soundevent-2.0.0/src/soundevent/data/clip_evaluations.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 The `EvaluatedExample` class within the `soundevent.data` package represents a
 specific example that has been evaluated by a machine learning model in the
 context of bioacoustic analysis. This class contains detailed information about
 the evaluation process, including the original `EvaluationExample`, the model's
 predictions (`ProcessedClip`), matches between predicted and ground truth
 annotations (`Match` instances), and computed evaluation metrics.
 """
+
 from typing import Optional, Sequence
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel, Field, model_validator
 
 from soundevent.data.clip_annotations import ClipAnnotation
 from soundevent.data.clip_predictions import ClipPrediction
```

### Comparing `soundevent-1.3.5/src/soundevent/data/clip_predictions.py` & `soundevent-2.0.0/src/soundevent/data/clip_predictions.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 ## Annotations and Additional Information
 
 The predicted sound events within the `ProcessedClip` object can be further
 enriched with tags and/or features associated with each predicted sound event.
 These annotations and additional information provide more detailed insights
 into the predicted events and aid in subsequent analysis and interpretation.
 """
+
 from typing import Sequence
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel, Field
 
 from soundevent.data.clips import Clip
 from soundevent.data.features import Feature
```

### Comparing `soundevent-1.3.5/src/soundevent/data/clips.py` & `soundevent-2.0.0/src/soundevent/data/clips.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,7 +94,12 @@
 
     @model_validator(mode="before")
     def _validate_times(cls, values):
         """Validate that start_time < end_time."""
         if values["start_time"] > values["end_time"]:
             raise ValueError("start_time must be less than end_time")
         return values
+
+    @property
+    def duration(self) -> float:
+        """Return the duration of the clip."""
+        return self.end_time - self.start_time
```

### Comparing `soundevent-1.3.5/src/soundevent/data/datasets.py` & `soundevent-2.0.0/src/soundevent/data/datasets.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/src/soundevent/data/evaluations.py` & `soundevent-2.0.0/src/soundevent/data/evaluations.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 The `Evaluation` class within the `soundevent.data` package encapsulates the
 core components of a bioacoustic evaluation process. This model is central to
 assessing the performance of machine learning models in bioacoustic tasks. The
 evaluation comprises an `EvaluationSet`, a specific `ModelRun`, computed
 metrics, and a set of `EvaluatedExample` instances.
 """
+
 import datetime
 from typing import Optional, Sequence
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel, Field
 
 from soundevent.data.clip_evaluations import ClipEvaluation
```

### Comparing `soundevent-1.3.5/src/soundevent/data/features.py` & `soundevent-2.0.0/src/soundevent/data/features.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/src/soundevent/data/geometries.py` & `soundevent-2.0.0/src/soundevent/data/geometries.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 * Multi-Polygon: Defines a collection of polygons, accommodating
 complex and overlapping sound event regions.
 
 By offering these geometry types, the soundevent package provides a
 comprehensive framework for accurately and flexibly describing the
 location and extent of sound events within a recording.
 """
+
 import json
 import sys
 from abc import ABC
 from typing import Dict, List, Type, Union
 
 from pydantic import BaseModel, Field, ValidationError, field_validator
 
@@ -903,15 +904,15 @@
             raise ValueError("Object must have a type key.")
 
         geom_type = obj["type"]
     else:
         if not hasattr(obj, "type"):
             raise ValueError(f"Object {obj} does not have a type attribute.")
 
-        geom_type = getattr(obj, "type")
+        geom_type = obj.type  # type: ignore
 
     if geom_type not in GEOMETRY_MAPPING:
         raise ValueError(f"Object {obj} does not have a geometry valid type.")
 
     geom_class = GEOMETRY_MAPPING[geom_type]
 
     try:
```

### Comparing `soundevent-1.3.5/src/soundevent/data/matches.py` & `soundevent-2.0.0/src/soundevent/data/matches.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/src/soundevent/data/notes.py` & `soundevent-2.0.0/src/soundevent/data/notes.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/src/soundevent/data/predicted_tags.py` & `soundevent-2.0.0/src/soundevent/data/predicted_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 By incorporating probability scores into predicted tags, machine
 learning-based audio analysis methods provide insights into the
 confidence level of the assigned tags. Researchers can leverage this
 information to assess the reliability and accuracy of the predicted
 tags, facilitating further analysis and evaluation of the audio data.
 """
+
 from pydantic import BaseModel, Field
 
 from soundevent.data.tags import Tag
 
 __all__ = [
     "PredictedTag",
 ]
```

### Comparing `soundevent-1.3.5/src/soundevent/data/prediction_sets.py` & `soundevent-2.0.0/src/soundevent/data/prediction_sets.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 ## Comparative Analysis and Evaluation
 
 `ModelRun` objects facilitate comparative analysis and evaluation of different
 processing methods or runs. Researchers can easily compare the results and
 performance of various models, algorithms, or parameter settings by examining
 the processed clips within each `ModelRun`.
 """
+
 import datetime
 from typing import List
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel, Field
 
 from soundevent.data.clip_predictions import ClipPrediction
```

### Comparing `soundevent-1.3.5/src/soundevent/data/recordings.py` & `soundevent-2.0.0/src/soundevent/data/recordings.py`

 * *Files 14% similar despite different names*

```diff
@@ -117,14 +117,35 @@
         A list of tags associated with the recording. Default is an empty list.
     features
         A list of features associated with the recording. Default is an empty
         list.
     notes : List[Note]
         A list of notes associated with the recording. Default is an empty
         list.
+
+    Notes
+    -----
+    When dealing with time-expanded recordings, adjustments are made to both
+    the duration and sample rate based on the time expansion factor. As a
+    result, the duration and sample rate stored in the Recording object may
+    deviate from the values derived from the file metadata.
+
+    A time-expanded recording is one that has been either slowed down or sped
+    up, typically to facilitate the playback and analysis of audio data. In
+    these cases, although the audio was originally captured at a specific
+    sample rate, the resulting audio file exhibits a different sample rate due
+    to the time expansion process. The time expansion factor represents the
+    ratio of the original sample rate to the sample rate of the time-expanded
+    recording.
+
+    Since the actual sample rate used to capture the audio differs from the
+    stored sample rate in the audio file, we have chosen to store the true
+    sample rate in the Recording object. This ensures that the Recording object
+    accurately reflects the sample rate at which the audio was originally
+    captured.
     """
 
     uuid: UUID = Field(default_factory=uuid4, repr=False)
     path: Path
     duration: float
     channels: int
     samplerate: int
```

### Comparing `soundevent-1.3.5/src/soundevent/data/sequence_annotations.py` & `soundevent-2.0.0/src/soundevent/data/sequence_annotations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Sequence Annotation Class."""
 
-
 import datetime
 from typing import List, Optional
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel, Field
 
 from soundevent.data.notes import Note
@@ -22,15 +21,17 @@
 
     Attributes
     ----------
     uuid
         A unique identifier for the annotation.
     sequence
         The sequence being annotated.
-    notes
+
+    Notes
+    -----
         A list of notes associated with the sequence.
     tags
         The tags attached to the sequence providing semantic information.
     created_on
         The date and time the annotation was created.
     created_by
         The user who created the annotation.
```

### Comparing `soundevent-1.3.5/src/soundevent/data/sequence_predictions.py` & `soundevent-2.0.0/src/soundevent/data/sequence_predictions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Sequence Prediction Class."""
 
-
 from typing import List
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel, Field
 
 from soundevent.data.predicted_tags import PredictedTag
 from soundevent.data.sequences import Sequence
```

### Comparing `soundevent-1.3.5/src/soundevent/data/sequences.py` & `soundevent-2.0.0/src/soundevent/data/sequences.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 By incorporating sequences into the analysis workflow, researchers gain a
 flexible and expressive framework to explore and study the intricacies of
 animal communication. The Sequence object, along with its associated tags,
 features, and hierarchical capabilities, provides a powerful tool for
 understanding the rich complexity of vocalization sequences.
 """
+
 from typing import List, Optional
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel, Field
 
 from soundevent.data.features import Feature
 from soundevent.data.sound_events import SoundEvent
```

### Comparing `soundevent-1.3.5/src/soundevent/data/sound_event_annotations.py` & `soundevent-2.0.0/src/soundevent/data/sound_event_annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,17 @@
         identity. This information is valuable for tracking and accountability within
         annotation projects.
     sound_event
         An instance of the `SoundEvent` class representing the specific sound event
         being annotated. Sound events define distinct audio occurrences, such as bird
         calls or animal vocalizations, and are essential for categorizing the content
         of the audio data.
-    notes
+
+    Notes
+    -----
         A list of `Note` instances representing additional contextual information or
         remarks associated with the annotation. Notes can provide insights into specific
         characteristics of the sound event, aiding in the comprehensive understanding
         of the annotated data.
     tags
         A list of `Tag` instances representing user-provided tags associated with the
         annotated sound event. These tags offer additional semantic context to the
```

### Comparing `soundevent-1.3.5/src/soundevent/data/sound_event_predictions.py` & `soundevent-2.0.0/src/soundevent/data/sound_event_predictions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Sound Event Predictions."""
+
 from typing import List
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel, Field
 
 from soundevent.data.predicted_tags import PredictedTag
 from soundevent.data.sound_events import SoundEvent
```

### Comparing `soundevent-1.3.5/src/soundevent/data/sound_events.py` & `soundevent-2.0.0/src/soundevent/data/sound_events.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/src/soundevent/data/tags.py` & `soundevent-2.0.0/src/soundevent/data/tags.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/src/soundevent/evaluation/__init__.py` & `soundevent-2.0.0/src/soundevent/evaluation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Evaluation functions."""
+
 from soundevent.evaluation.affinity import compute_affinity
 from soundevent.evaluation.encoding import (
     classification_encoding,
     create_tag_encoder,
     multilabel_encoding,
     prediction_encoding,
 )
```

### Comparing `soundevent-1.3.5/src/soundevent/evaluation/affinity.py` & `soundevent-2.0.0/src/soundevent/evaluation/affinity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Measures of affinity between sound events geometries."""
 
-
 from soundevent import data
 from soundevent.geometry import (
     buffer_geometry,
     compute_bounds,
     geometry_to_shapely,
 )
 
@@ -81,15 +80,14 @@
     ...     geometry2,
     ...     time_buffer=0.02,
     ...     freq_buffer=150,
     ... )
     >>> affinity
     0.75
     """
-
     geometry1 = _prepare_geometry(geometry1, time_buffer, freq_buffer)
     geometry2 = _prepare_geometry(geometry2, time_buffer, freq_buffer)
 
     if (
         geometry1.type in TIME_GEOMETRY_TYPES
         or geometry2.type in TIME_GEOMETRY_TYPES
     ):
```

### Comparing `soundevent-1.3.5/src/soundevent/evaluation/encoding.py` & `soundevent-2.0.0/src/soundevent/evaluation/encoding.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     return SimpleEncoder(tags)
 
 
 def classification_encoding(
     tags: Sequence[data.Tag],
     encoder: Encoder,
 ) -> Optional[int]:
-    """Encodes a list of tags into an integer value.
+    """Encode a list of tags into an integer value.
 
     This function is commonly used for mapping a list of tags to a compact
     integer representation, typically representing classes associated with
     objects like clips or sound events.
 
     Parameters
     ----------
@@ -138,18 +138,18 @@
         The encoded integer value representing the tags, or None if no
         encoding is available.
 
     Examples
     --------
     Consider the following set of tags:
 
-    >>> dog = data.Tag(key='animal', value='dog')
-    >>> cat = data.Tag(key='animal', value='cat')
-    >>> brown = data.Tag(key='color', value='brown')
-    >>> blue = data.Tag(key='color', value='blue')
+    >>> dog = data.Tag(key="animal", value="dog")
+    >>> cat = data.Tag(key="animal", value="cat")
+    >>> brown = data.Tag(key="color", value="brown")
+    >>> blue = data.Tag(key="color", value="blue")
 
     If we are interested in encoding only the 'dog' and 'brown' classes, the
     following examples demonstrate how the encoding works for tag list:
 
     >>> encoder = create_tag_encoder([dog, brown])
     >>> classification_encoding([brown], encoder)
     1
@@ -167,15 +167,15 @@
     return None
 
 
 def multilabel_encoding(
     tags: Sequence[data.Tag],
     encoder: Encoder,
 ) -> np.ndarray:
-    """Encodes a list of tags into a binary multilabel array.
+    """Encode a list of tags into a binary multilabel array.
 
     Parameters
     ----------
     tags
         A list of tags to be encoded.
     encoder
         A callable object that takes a data.Tag object as input and returns
@@ -189,18 +189,18 @@
         multilabel encoding for the input tags. Each index with a corresponding
         tag is set to 1, and the rest are 0.
 
     Examples
     --------
     Consider the following set of tags:
 
-    >>> dog = data.Tag(key='animal', value='dog')
-    >>> cat = data.Tag(key='animal', value='cat')
-    >>> brown = data.Tag(key='color', value='brown')
-    >>> blue = data.Tag(key='color', value='blue')
+    >>> dog = data.Tag(key="animal", value="dog")
+    >>> cat = data.Tag(key="animal", value="cat")
+    >>> brown = data.Tag(key="color", value="brown")
+    >>> blue = data.Tag(key="color", value="blue")
 
     And we are only interested in encoding the following two classes:
 
     >>> encoder = create_tag_encoder([dog, brown])
 
     Then the following examples show how the multilabel encoding works:
 
@@ -222,15 +222,15 @@
     return encoded
 
 
 def prediction_encoding(
     tags: Sequence[data.PredictedTag],
     encoder: Encoder,
 ) -> np.ndarray:
-    """Encodes a list of predicted tags into a floating-point array of scores.
+    """Encode a list of predicted tags into a floating-point array of scores.
 
     Parameters
     ----------
     tags
         A list of predicted tags to be encoded.
     encoder
         A callable object that takes a data.Tag object as input and returns
@@ -244,40 +244,51 @@
         predicted scores for each class. The array contains the scores for each
         class corresponding to the input predicted tags.
 
     Examples
     --------
     Consider the following set of tags:
 
-    >>> dog = data.Tag(key='animal', value='dog')
-    >>> cat = data.Tag(key='animal', value='cat')
-    >>> brown = data.Tag(key='color', value='brown')
-    >>> blue = data.Tag(key='color', value='blue')
+    >>> dog = data.Tag(key="animal", value="dog")
+    >>> cat = data.Tag(key="animal", value="cat")
+    >>> brown = data.Tag(key="color", value="brown")
+    >>> blue = data.Tag(key="color", value="blue")
 
     And we are only interested in encoding the following two classes:
 
     >>> encoder = create_tag_encoder([dog, brown])
 
     Then the following examples show how the encoding works for predicted tags:
 
-    >>> prediction_encoding([data.PredictedTag(tag=brown, score=0.5)], encoder)
+    >>> prediction_encoding(
+    ...     [data.PredictedTag(tag=brown, score=0.5)], encoder
+    ... )
     array([0, 0.5])
-    >>> multilabel_encoding([
-    ...    data.PredictedTag(tag=dog, score=0.2),
-    ...    data.PredictedTag(tag=blue, score=0.9),
-    ... ], encoder)
+    >>> multilabel_encoding(
+    ...     [
+    ...         data.PredictedTag(tag=dog, score=0.2),
+    ...         data.PredictedTag(tag=blue, score=0.9),
+    ...     ],
+    ...     encoder,
+    ... )
     array([0.2, 0])
-    >>> multilabel_encoding([
-    ...     data.PredictedTag(tag=dog, score=0.2),
-    ...     data.PredictedTag(tag=brown, score=0.5),
-    ... ], encoder)
+    >>> multilabel_encoding(
+    ...     [
+    ...         data.PredictedTag(tag=dog, score=0.2),
+    ...         data.PredictedTag(tag=brown, score=0.5),
+    ...     ],
+    ...     encoder,
+    ... )
     array([0.2, 0.5])
-    >>> classification_encoding([
-    ...     data.PredictedTag(tag=cat, score=0.7),
-    ... ], encoder)
+    >>> classification_encoding(
+    ...     [
+    ...         data.PredictedTag(tag=cat, score=0.7),
+    ...     ],
+    ...     encoder,
+    ... )
     array([0, 0])
     """
     encoded = np.zeros(encoder.num_classes, dtype=np.float32)
     for prediction in tags:
         index = encoder.encode(prediction.tag)
         if index is None:
             continue
```

### Comparing `soundevent-1.3.5/src/soundevent/evaluation/match.py` & `soundevent-2.0.0/src/soundevent/evaluation/match.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     Sequence[Tuple[Optional[int], Optional[int], float]]
         A sequence of matches. Each match is a tuple of the source index,
         target index and affinity. If a source geometry is not matched to
         any target geometry, the target index is None. If a target geometry
         is not matched to any source geometry, the source index is None.
         Every source and target geometry is matched exactly once.
     """
-
     # Compute the affinity between all pairs of geometries.
     cost_matrix = np.zeros(shape=(len(source), len(target)))
     for (index1, geometry1), (index2, geometry2) in product(
         enumerate(source), enumerate(target)
     ):
         cost_matrix[index1, index2] = compute_affinity(
             geometry1,
```

### Comparing `soundevent-1.3.5/src/soundevent/evaluation/metrics.py` & `soundevent-2.0.0/src/soundevent/evaluation/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,14 @@
     computes the Jaccard score for each sample and then averages over the
     samples.
 
     Note also that the y_score input is assumed to be an array of probabilities
     for each class. This function will convert the probabilities to binary
     predictions using the given threshold.
     """
-
     if y_true.ndim == 1:
         y_true = y_true[np.newaxis, :]
 
     if y_score.ndim == 1:
         y_score = y_score[np.newaxis, :]
 
     labels = np.arange(y_true.shape[1])
@@ -151,16 +150,15 @@
     )
 
 
 def average_precision(
     y_true: np.ndarray,
     y_score: np.ndarray,
 ) -> float:
-    """Compute the average precision score for the given true and predicted
-    labels.
+    """Compute the average precision score for the given true and predicted labels.
 
     Parameters
     ----------
     y_true
         True labels.
     y_score
         An array of predicted probabilities for each class.
@@ -186,16 +184,15 @@
     )
 
 
 def mean_average_precision(
     y_true: np.ndarray,
     y_score: np.ndarray,
 ) -> float:
-    """Compute the mean average precision score for the given true and
-    predicted labels.
+    """Compute the mean average precision score for the given true and predicted labels.
 
     Parameters
     ----------
     y_true
         True labels.
     y_score
         An array of predicted probabilities for each class.
```

### Comparing `soundevent-1.3.5/src/soundevent/evaluation/tasks/__init__.py` & `soundevent-2.0.0/src/soundevent/evaluation/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/src/soundevent/evaluation/tasks/clip_classification.py` & `soundevent-2.0.0/src/soundevent/evaluation/tasks/clip_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,16 +84,15 @@
         true_classes.append(true_class)
         predicted_classes_scores.append(predicted_class_scores)
 
     return evaluated_examples, true_classes, np.array(predicted_classes_scores)
 
 
 def _compute_overall_metrics(true_classes, predicted_classes_scores):
-    """Compute evaluation metrics based on true classes and predicted
-    scores."""
+    """Compute evaluation metrics based on true classes and predicted scores."""
     evaluation_metrics = [
         data.Feature(
             name=metric.__name__,
             value=metric(
                 y_true=true_classes,
                 y_score=predicted_classes_scores,
             ),
```

### Comparing `soundevent-1.3.5/src/soundevent/evaluation/tasks/clip_multilabel_classification.py` & `soundevent-2.0.0/src/soundevent/evaluation/tasks/clip_multilabel_classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,19 @@
     )
 
 
 def _evaluate_clips(
     clip_predictions: Sequence[data.ClipPrediction],
     clip_annotations: Sequence[data.ClipAnnotation],
     encoder: Encoder,
-) -> Tuple[List[data.ClipEvaluation], np.ndarray, np.ndarray,]:
+) -> Tuple[
+    List[data.ClipEvaluation],
+    np.ndarray,
+    np.ndarray,
+]:
     """Evaluate all examples in the given model run and evaluation set."""
     evaluated_clips = []
     true_classes = []
     predicted_classes_scores = []
 
     for annotations, predictions in iterate_over_valid_clips(
         clip_predictions=clip_predictions,
@@ -89,16 +93,15 @@
     )
 
 
 def _compute_overall_metrics(
     true_classes,
     predicted_classes_scores,
 ) -> List[data.Feature]:
-    """Compute evaluation metrics based on true classes and predicted
-    scores."""
+    """Compute evaluation metrics based on true classes and predicted scores."""
     return [
         data.Feature(
             name=metric.__name__,
             value=metric(
                 true_classes,
                 predicted_classes_scores,
             ),
```

### Comparing `soundevent-1.3.5/src/soundevent/evaluation/tasks/common.py` & `soundevent-2.0.0/src/soundevent/evaluation/tasks/common.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/src/soundevent/evaluation/tasks/sound_event_classification.py` & `soundevent-2.0.0/src/soundevent/evaluation/tasks/sound_event_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Sound event classification evaluation."""
+
 from typing import List, Optional, Sequence, Tuple
 
 import numpy as np
 
 from soundevent import data
 from soundevent.evaluation import metrics
 from soundevent.evaluation.encoding import (
@@ -83,16 +84,15 @@
         predicted_classes_scores.extend(predicted_classes)
         evaluated_clips.append(evaluated_clip)
 
     return evaluated_clips, true_classes, np.array(predicted_classes_scores)
 
 
 def _compute_overall_metrics(true_classes, predicted_classes_scores):
-    """Compute evaluation metrics based on true classes and predicted
-    scores."""
+    """Compute evaluation metrics based on true classes and predicted scores."""
     evaluation_metrics = [
         data.Feature(
             name=metric.__name__,
             value=metric(
                 true_classes,
                 predicted_classes_scores,
             ),
```

### Comparing `soundevent-1.3.5/src/soundevent/evaluation/tasks/sound_event_detection.py` & `soundevent-2.0.0/src/soundevent/evaluation/tasks/sound_event_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Sound event detection evaluation."""
+
 from typing import List, Optional, Sequence, Tuple
 
 import numpy as np
 
 from soundevent import data
 from soundevent.evaluation import metrics
 from soundevent.evaluation.encoding import (
@@ -83,16 +84,15 @@
         predicted_classes_scores.extend(predicted_classes)
         evaluated_clips.append(evaluated_clip)
 
     return evaluated_clips, true_classes, np.array(predicted_classes_scores)
 
 
 def compute_overall_metrics(true_classes, predicted_classes_scores):
-    """Compute evaluation metrics based on true classes and predicted
-    scores."""
+    """Compute evaluation metrics based on true classes and predicted scores."""
     evaluation_metrics = [
         data.Feature(
             name=metric.__name__,
             value=metric(
                 true_classes,
                 predicted_classes_scores,
             ),
```

### Comparing `soundevent-1.3.5/src/soundevent/geometry/__init__.py` & `soundevent-2.0.0/src/soundevent/geometry/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,17 +15,24 @@
 
 from soundevent.geometry.conversion import geometry_to_shapely
 from soundevent.geometry.features import (
     GeometricFeature,
     compute_geometric_features,
 )
 from soundevent.geometry.html import geometry_to_html
-from soundevent.geometry.operations import buffer_geometry, compute_bounds
+from soundevent.geometry.operations import (
+    buffer_geometry,
+    compute_bounds,
+    get_geometry_point,
+    rasterize,
+)
 
 __all__ = [
     "GeometricFeature",
     "buffer_geometry",
     "compute_bounds",
     "compute_geometric_features",
     "geometry_to_html",
     "geometry_to_shapely",
+    "get_geometry_point",
+    "rasterize",
 ]
```

### Comparing `soundevent-1.3.5/src/soundevent/geometry/conversion.py` & `soundevent-2.0.0/src/soundevent/geometry/conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,19 +19,19 @@
         The TimeStamp geometry to convert.
 
     Returns
     -------
     shapely.Geometry
         The converted shapely geometry.
     """
-    return geometry.box(
-        geom.coordinates,
-        0,
-        geom.coordinates,
-        data.MAX_FREQUENCY,
+    return shapely.linestrings(
+        [
+            [geom.coordinates, 0],
+            [geom.coordinates, data.MAX_FREQUENCY],
+        ]
     )
 
 
 def time_interval_to_shapely(geom: data.TimeInterval) -> shapely.Geometry:
     """Convert a TimeInterval to a shapely geometry.
 
     Parameters
```

### Comparing `soundevent-1.3.5/src/soundevent/geometry/features.py` & `soundevent-2.0.0/src/soundevent/geometry/features.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 ... )
 >>> features.compute_geometric_features(geometry)
 [Feature(name='duration', value=1),
     Feature(name='low_freq', value=0),
     Feature(name='high_freq', value=1000),
     Feature(name='bandwidth', value=1000)]
 """
+
 from enum import Enum
 from typing import Any, Callable, Dict, List
 
 from soundevent.data import Feature, geometries
 from soundevent.geometry.conversion import geometry_to_shapely
 
 __all__ = [
```

### Comparing `soundevent-1.3.5/src/soundevent/geometry/html.py` & `soundevent-2.0.0/src/soundevent/geometry/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """HTML representation of geometries."""
+
 import shapely
 
 from soundevent import data
 from soundevent.geometry.conversion import geometry_to_shapely
 
 
 def timestamp_to_html(geom: data.TimeStamp) -> str:
@@ -89,26 +90,30 @@
         axis: str = "time",
     ) -> str:
         outer_style = "; ".join(
             [
                 "position: absolute",
                 "top: 0; " if top else "bottom: 0",
                 "left: 0; " if left else "right: 0",
-                "transform: translate(-105%, 0)"
-                if axis == "freq"
-                else "transform: translate(0, 100%)",
+                (
+                    "transform: translate(-105%, 0)"
+                    if axis == "freq"
+                    else "transform: translate(0, 100%)"
+                ),
             ]
         )
 
         inner_style = "; ".join(
             [
                 "display: inline",
-                "vertical-align: top"
-                if axis == "time"
-                else "vertical-align: bottom",
+                (
+                    "vertical-align: top"
+                    if axis == "time"
+                    else "vertical-align: bottom"
+                ),
             ]
         )
 
         label_str = f"{label:.2f}" if axis == "time" else f"{label:.0f}"
 
         return (
             f'<div style="{outer_style}">'
@@ -136,11 +141,11 @@
         The geometry to represent as HTML.
 
     Returns
     -------
     str
         The HTML representation of the geometry.
     """
-    if geom.type == "timestamp":
+    if geom.type == "TimeStamp":
         return timestamp_to_html(geom)
     else:
         return shapely_to_html(geometry_to_shapely(geom))
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/__init__.py` & `soundevent-2.0.0/src/soundevent/io/aoef/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,34 +20,34 @@
 data objects across different platforms and systems.
 
 * Validation and Data Integrity: The schema validation provided by Pydantic
 ensures that the data objects conform to the specified structure, reducing the
 risk of errors and inconsistencies.
 
 """
+
 import datetime
 from pathlib import Path
 from typing import Any, Dict, Optional, Set, TypeVar, Union
 
 from pydantic import BaseModel, Field
 
-from soundevent import data
-from soundevent.io.types import DataCollections, DataType
-
 from .annotation_project import (
     AnnotationProjectAdapter,
     AnnotationProjectObject,
 )
 from .annotation_set import AnnotationSetAdapter, AnnotationSetObject
 from .dataset import DatasetAdapter, DatasetObject
 from .evaluation import EvaluationAdapter, EvaluationObject
 from .evaluation_set import EvaluationSetAdapter, EvaluationSetObject
 from .model_run import ModelRunAdapter, ModelRunObject
 from .prediction_set import PredictionSetAdapter, PredictionSetObject
 from .recording_set import RecordingSetAdapter, RecordingSetObject
+from soundevent import data
+from soundevent.io.types import DataCollections, DataType
 
 __all__ = [
     "is_json",
     "load",
     "save",
     "to_aeof",
     "to_soundevent",
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/adapters.py` & `soundevent-2.0.0/src/soundevent/io/aoef/adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,22 +36,19 @@
 D = TypeVar("D", bound=BaseModel)
 
 
 class AdapterProtocol(Protocol, Generic[C, D]):
     def __init__(
         self,
         audio_dir: Optional[data.PathLike] = None,
-    ):
-        ...
+    ): ...
 
-    def to_aoef(self, obj: C) -> D:
-        ...
+    def to_aoef(self, obj: C) -> D: ...
 
-    def to_soundevent(self, obj: D) -> C:
-        ...
+    def to_soundevent(self, obj: D) -> C: ...
 
 
 class DataAdapter(
     ABC, Generic[SoundEventObject, AOEFObject, SoundEventKey, AOEFKey]
 ):
     """Base class for data adapters.
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/annotation_project.py` & `soundevent-2.0.0/src/soundevent/io/aoef/annotation_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import List, Literal, Optional
 
-from soundevent import data
-
 from .annotation_set import AnnotationSetAdapter, AnnotationSetObject
 from .annotation_task import AnnotationTaskAdapter, AnnotationTaskObject
+from soundevent import data
 
 ColType = Literal["annotation_project"]
 
 
 class AnnotationProjectObject(AnnotationSetObject):
     """Schema definition for an annotation project object in AOEF format."""
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/annotation_set.py` & `soundevent-2.0.0/src/soundevent/io/aoef/annotation_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import datetime
 from typing import List, Literal, Optional
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .clip import ClipAdapter, ClipObject
 from .clip_annotations import ClipAnnotationsAdapter, ClipAnnotationsObject
 from .note import NoteAdapter
 from .recording import RecordingAdapter, RecordingObject
 from .sequence import SequenceAdapter, SequenceObject
 from .sequence_annotation import (
     SequenceAnnotationAdapter,
@@ -18,14 +16,15 @@
 from .sound_event import SoundEventAdapter, SoundEventObject
 from .sound_event_annotation import (
     SoundEventAnnotationAdapter,
     SoundEventAnnotationObject,
 )
 from .tag import TagAdapter, TagObject
 from .user import UserAdapter, UserObject
+from soundevent import data
 
 
 class AnnotationSetObject(BaseModel):
     uuid: UUID
     collection_type: Literal["annotation_set"] = "annotation_set"
     users: Optional[List[UserObject]] = None
     tags: Optional[List[TagObject]] = None
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/annotation_task.py` & `soundevent-2.0.0/src/soundevent/io/aoef/annotation_task.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import datetime
 from typing import List, Optional
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .adapters import DataAdapter
 from .clip import ClipAdapter
 from .user import UserAdapter
+from soundevent import data
 
 
 class StatusBadgeObject(BaseModel):
     """Schema definition for a status badge object in AOEF format."""
 
     state: data.AnnotationState
     owner: Optional[UUID] = None
@@ -48,26 +47,30 @@
         for badge in obj.status_badges or []:
             if badge.owner is not None:
                 self.user_adapter.to_aoef(badge.owner)
 
         return AnnotationTaskObject(
             uuid=obj.uuid,
             clip=self.clip_adapter.to_aoef(obj.clip).uuid,
-            status_badges=[
-                StatusBadgeObject(
-                    state=badge.state,
-                    owner=self.user_adapter.to_aoef(badge.owner).uuid
-                    if badge.owner is not None
-                    else None,
-                    created_on=badge.created_on,
-                )
-                for badge in obj.status_badges
-            ]
-            if obj.status_badges
-            else None,
+            status_badges=(
+                [
+                    StatusBadgeObject(
+                        state=badge.state,
+                        owner=(
+                            self.user_adapter.to_aoef(badge.owner).uuid
+                            if badge.owner is not None
+                            else None
+                        ),
+                        created_on=badge.created_on,
+                    )
+                    for badge in obj.status_badges
+                ]
+                if obj.status_badges
+                else None
+            ),
             created_on=obj.created_on,
         )
 
     def assemble_soundevent(
         self,
         obj: AnnotationTaskObject,
     ) -> data.AnnotationTask:
@@ -78,16 +81,18 @@
 
         return data.AnnotationTask(
             uuid=obj.uuid or uuid4(),
             clip=clip,
             status_badges=[
                 data.StatusBadge(
                     state=badge.state,
-                    owner=self.user_adapter.from_id(badge.owner)
-                    if badge.owner is not None
-                    else None,
+                    owner=(
+                        self.user_adapter.from_id(badge.owner)
+                        if badge.owner is not None
+                        else None
+                    ),
                     created_on=badge.created_on or datetime.datetime.now(),
                 )
                 for badge in obj.status_badges or []
             ],
             created_on=obj.created_on or datetime.datetime.now(),
         )
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/clip.py` & `soundevent-2.0.0/src/soundevent/io/aoef/clip.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Dict, Optional
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .adapters import DataAdapter
 from .recording import RecordingAdapter
+from soundevent import data
 
 
 class ClipObject(BaseModel):
     """Schema definition for a clip object in AOEF format."""
 
     uuid: UUID
     recording: UUID
@@ -29,17 +28,19 @@
 
     def assemble_aoef(self, obj: data.Clip, obj_id: UUID) -> ClipObject:
         return ClipObject(
             recording=self.recording_adapter.to_aoef(obj.recording).uuid,
             start_time=obj.start_time,
             end_time=obj.end_time,
             uuid=obj.uuid,
-            features={feature.name: feature.value for feature in obj.features}
-            if obj.features
-            else None,
+            features=(
+                {feature.name: feature.value for feature in obj.features}
+                if obj.features
+                else None
+            ),
         )
 
     def assemble_soundevent(
         self,
         obj: ClipObject,
     ) -> data.Clip:
         recording = self.recording_adapter.from_id(obj.recording)
@@ -48,17 +49,19 @@
             raise ValueError(f"Recording with ID {obj.recording} not found.")
 
         return data.Clip(
             recording=recording,
             start_time=obj.start_time,
             end_time=obj.end_time,
             uuid=obj.uuid or uuid4(),
-            features=[
-                data.Feature(
-                    name=name,
-                    value=value,
-                )
-                for name, value in obj.features.items()
-            ]
-            if obj.features
-            else [],
+            features=(
+                [
+                    data.Feature(
+                        name=name,
+                        value=value,
+                    )
+                    for name, value in obj.features.items()
+                ]
+                if obj.features
+                else []
+            ),
         )
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/clip_annotations.py` & `soundevent-2.0.0/src/soundevent/io/aoef/clip_annotations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import datetime
 from typing import List, Optional
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .adapters import DataAdapter
 from .clip import ClipAdapter
 from .note import NoteAdapter, NoteObject
 from .sequence_annotation import SequenceAnnotationAdapter
 from .sound_event_annotation import SoundEventAnnotationAdapter
 from .tag import TagAdapter
+from soundevent import data
 
 
 class ClipAnnotationsObject(BaseModel):
     """Schema definition for the clip annotations object in AOEF format."""
 
     uuid: UUID
     clip: UUID
@@ -48,32 +47,42 @@
         self,
         obj: data.ClipAnnotation,
         obj_id: UUID,
     ) -> ClipAnnotationsObject:
         return ClipAnnotationsObject(
             uuid=obj.uuid,
             clip=self.clip_adapter.to_aoef(obj.clip).uuid,
-            tags=[self.tag_adapter.to_aoef(tag).id for tag in obj.tags]
-            if obj.tags
-            else None,
-            sound_events=[
-                self.sound_event_annotation_adapter.to_aoef(annotation).uuid
-                for annotation in obj.sound_events
-            ]
-            if obj.sound_events
-            else None,
-            sequences=[
-                self.sequence_annotation_adapter.to_aoef(annotation).uuid
-                for annotation in obj.sequences
-            ]
-            if obj.sequences
-            else None,
-            notes=[self.note_adapter.to_aoef(note) for note in obj.notes]
-            if obj.notes
-            else None,
+            tags=(
+                [self.tag_adapter.to_aoef(tag).id for tag in obj.tags]
+                if obj.tags
+                else None
+            ),
+            sound_events=(
+                [
+                    self.sound_event_annotation_adapter.to_aoef(
+                        annotation
+                    ).uuid
+                    for annotation in obj.sound_events
+                ]
+                if obj.sound_events
+                else None
+            ),
+            sequences=(
+                [
+                    self.sequence_annotation_adapter.to_aoef(annotation).uuid
+                    for annotation in obj.sequences
+                ]
+                if obj.sequences
+                else None
+            ),
+            notes=(
+                [self.note_adapter.to_aoef(note) for note in obj.notes]
+                if obj.notes
+                else None
+            ),
             created_on=obj.created_on,
         )
 
     def assemble_soundevent(
         self,
         obj: ClipAnnotationsObject,
     ) -> data.ClipAnnotation:
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/clip_evaluation.py` & `soundevent-2.0.0/src/soundevent/io/aoef/clip_evaluation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import Dict, List, Optional
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .adapters import DataAdapter
 from .clip_annotations import ClipAnnotationsAdapter
 from .clip_predictions import ClipPredictionsAdapter
 from .match import MatchAdapter
 from .note import NoteAdapter
+from soundevent import data
 
 
 class ClipEvaluationObject(BaseModel):
     uuid: UUID
     annotations: UUID
     predictions: UUID
     matches: Optional[List[UUID]] = None
@@ -45,22 +44,27 @@
         annotations = self.clip_annotations_adapter.to_aoef(obj.annotations)
         predictions = self.clip_predictions_adapter.to_aoef(obj.predictions)
 
         return ClipEvaluationObject(
             uuid=obj.uuid,
             annotations=annotations.uuid,
             predictions=predictions.uuid,
-            matches=[
-                self.match_adapter.to_aoef(match).uuid for match in obj.matches
-            ]
-            if obj.matches
-            else None,
-            metrics={metrics.name: metrics.value for metrics in obj.metrics}
-            if obj.metrics
-            else None,
+            matches=(
+                [
+                    self.match_adapter.to_aoef(match).uuid
+                    for match in obj.matches
+                ]
+                if obj.matches
+                else None
+            ),
+            metrics=(
+                {metrics.name: metrics.value for metrics in obj.metrics}
+                if obj.metrics
+                else None
+            ),
             score=obj.score,
         )
 
     def assemble_soundevent(
         self,
         obj: ClipEvaluationObject,
     ) -> data.ClipEvaluation:
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/clip_predictions.py` & `soundevent-2.0.0/src/soundevent/io/aoef/clip_predictions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import Dict, List, Optional, Tuple
 from uuid import UUID
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .adapters import DataAdapter
 from .clip import ClipAdapter
 from .sequence_prediction import SequencePredictionAdapter
 from .sound_event_prediction import SoundEventPredictionAdapter
 from .tag import TagAdapter
+from soundevent import data
 
 
 class ClipPredictionsObject(BaseModel):
     uuid: UUID
     clip: UUID
     sound_events: Optional[List[UUID]] = None
     sequences: Optional[List[UUID]] = None
@@ -41,37 +40,47 @@
         self,
         obj: data.ClipPrediction,
         obj_id: UUID,
     ) -> ClipPredictionsObject:
         return ClipPredictionsObject(
             uuid=obj.uuid,
             clip=self.clip_adapter.to_aoef(obj.clip).uuid,
-            sound_events=[
-                self.sound_event_prediction_adapter.to_aoef(sound_event).uuid
-                for sound_event in obj.sound_events
-            ]
-            if obj.sound_events
-            else None,
-            sequences=[
-                self.sequence_prediction_adapter.to_aoef(sequence).uuid
-                for sequence in obj.sequences
-            ]
-            if obj.sequences
-            else None,
-            tags=[
-                (tag.id, predicted_tag.score)
-                for predicted_tag in obj.tags
-                if (tag := self.tag_adapter.to_aoef(predicted_tag.tag))
-                is not None
-            ]
-            if obj.tags
-            else None,
-            features={feature.name: feature.value for feature in obj.features}
-            if obj.features is not None
-            else None,
+            sound_events=(
+                [
+                    self.sound_event_prediction_adapter.to_aoef(
+                        sound_event
+                    ).uuid
+                    for sound_event in obj.sound_events
+                ]
+                if obj.sound_events
+                else None
+            ),
+            sequences=(
+                [
+                    self.sequence_prediction_adapter.to_aoef(sequence).uuid
+                    for sequence in obj.sequences
+                ]
+                if obj.sequences
+                else None
+            ),
+            tags=(
+                [
+                    (tag.id, predicted_tag.score)
+                    for predicted_tag in obj.tags
+                    if (tag := self.tag_adapter.to_aoef(predicted_tag.tag))
+                    is not None
+                ]
+                if obj.tags
+                else None
+            ),
+            features=(
+                {feature.name: feature.value for feature in obj.features}
+                if obj.features is not None
+                else None
+            ),
         )
 
     def assemble_soundevent(
         self,
         obj: ClipPredictionsObject,
     ) -> data.ClipPrediction:
         clip = self.clip_adapter.from_id(obj.clip)
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/dataset.py` & `soundevent-2.0.0/src/soundevent/io/aoef/dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Literal, Optional
 
-from soundevent import data
-
 from .recording_set import RecordingSetAdapter, RecordingSetObject
+from soundevent import data
 
 
 class DatasetObject(RecordingSetObject):
     """Schema definition for a dataset object in AOEF format."""
 
     collection_type: Literal["dataset"] = "dataset"  # type: ignore
     name: str
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/evaluation.py` & `soundevent-2.0.0/src/soundevent/io/aoef/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import datetime
 from typing import Dict, List, Literal, Optional
 from uuid import UUID
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .clip import ClipAdapter, ClipObject
 from .clip_annotations import ClipAnnotationsAdapter, ClipAnnotationsObject
 from .clip_evaluation import ClipEvaluationAdapter, ClipEvaluationObject
 from .clip_predictions import ClipPredictionsAdapter, ClipPredictionsObject
 from .match import MatchAdapter, MatchObject
 from .note import NoteAdapter
 from .recording import RecordingAdapter, RecordingObject
@@ -29,14 +27,15 @@
 )
 from .sound_event_prediction import (
     SoundEventPredictionAdapter,
     SoundEventPredictionObject,
 )
 from .tag import TagAdapter, TagObject
 from .user import UserAdapter, UserObject
+from soundevent import data
 
 
 class EvaluationObject(BaseModel):
     uuid: UUID
     collection_type: Literal["evaluation"] = "evaluation"
     created_on: Optional[datetime.datetime] = None
     evaluation_task: str
@@ -185,21 +184,23 @@
             sound_event_annotations=self.sound_event_annotation_adapter.values(),
             sequence_annotations=self.sequence_annotation_adapter.values(),
             clip_annotations=self.clip_annotations_adapter.values(),
             sound_event_predictions=self.sound_event_prediction_adapter.values(),
             sequence_predictions=self.sequence_prediction_adapter.values(),
             clip_predictions=self.clip_predictions_adapter.values(),
             clip_evaluations=self.clip_evaluation_adapter.values(),
-            metrics={
-                metric.name: metric.value
-                for metric in obj.metrics
-                if metric.value is not None
-            }
-            if obj.metrics
-            else None,
+            metrics=(
+                {
+                    metric.name: metric.value
+                    for metric in obj.metrics
+                    if metric.value is not None
+                }
+                if obj.metrics
+                else None
+            ),
             score=obj.score,
             matches=self.match_adapter.values(),
         )
 
     def to_soundevent(
         self,
         obj: EvaluationObject,
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/evaluation_set.py` & `soundevent-2.0.0/src/soundevent/io/aoef/evaluation_set.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import List, Literal, Optional
 
-from soundevent import data
-
 from .annotation_set import AnnotationSetAdapter, AnnotationSetObject
+from soundevent import data
 
 
 class EvaluationSetObject(AnnotationSetObject):
     """Schema definition for an evaluation set object in AOEF format."""
 
     collection_type: Literal["evaluation_set"] = "evaluation_set"  # type: ignore
     name: str
@@ -30,19 +29,22 @@
             clips=self.clip_adapter.values(),
             sound_event_annotations=self.sound_event_annotations_adapter.values(),
             sequence_annotations=self.sequence_annotations_adapter.values(),
             clip_annotations=annotation_set.clip_annotations,
             created_on=obj.created_on,
             name=obj.name,
             description=obj.description,
-            evaluation_tags=[
-                self.tag_adapter.to_aoef(tag).id for tag in obj.evaluation_tags
-            ]
-            if obj.evaluation_tags
-            else None,
+            evaluation_tags=(
+                [
+                    self.tag_adapter.to_aoef(tag).id
+                    for tag in obj.evaluation_tags
+                ]
+                if obj.evaluation_tags
+                else None
+            ),
         )
 
     def to_soundevent(  # type: ignore
         self,
         obj: EvaluationSetObject,  # type: ignore
     ) -> data.EvaluationSet:
         annotation_set = super().to_soundevent(obj)
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/match.py` & `soundevent-2.0.0/src/soundevent/io/aoef/match.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import Dict, Optional
 from uuid import UUID
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .adapters import DataAdapter
 from .sound_event_annotation import SoundEventAnnotationAdapter
 from .sound_event_prediction import SoundEventPredictionAdapter
+from soundevent import data
 
 
 class MatchObject(BaseModel):
     uuid: UUID
     source: Optional[UUID] = None
     target: Optional[UUID] = None
     affinity: float
@@ -50,17 +49,19 @@
 
         return MatchObject(
             uuid=obj.uuid,
             source=source,
             target=target,
             affinity=obj.affinity,
             score=obj.score,
-            metrics={metrics.name: metrics.value for metrics in obj.metrics}
-            if obj.metrics
-            else None,
+            metrics=(
+                {metrics.name: metrics.value for metrics in obj.metrics}
+                if obj.metrics
+                else None
+            ),
         )
 
     def assemble_soundevent(
         self,
         obj: MatchObject,
     ) -> data.Match:
         source = None
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/model_run.py` & `soundevent-2.0.0/src/soundevent/io/aoef/model_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Literal, Optional
 
-from soundevent import data
-
 from .prediction_set import PredictionSetAdapter, PredictionSetObject
+from soundevent import data
 
 
 class ModelRunObject(PredictionSetObject):
     collection_type: Literal["model_run"] = "model_run"  # type: ignore
     name: str
     version: Optional[str] = None
     description: Optional[str] = None
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/note.py` & `soundevent-2.0.0/src/soundevent/io/aoef/note.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import datetime
 from typing import Optional
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .user import UserAdapter
+from soundevent import data
 
 
 class NoteObject(BaseModel):
     """Schema definition for a note object in AOEF format."""
 
     uuid: UUID
     message: str
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/prediction_set.py` & `soundevent-2.0.0/src/soundevent/io/aoef/prediction_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import datetime
 from typing import List, Literal, Optional
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .clip import ClipAdapter, ClipObject
 from .clip_predictions import ClipPredictionsAdapter, ClipPredictionsObject
 from .note import NoteAdapter
 from .recording import RecordingAdapter, RecordingObject
 from .sequence import SequenceAdapter, SequenceObject
 from .sequence_prediction import (
     SequencePredictionAdapter,
@@ -18,14 +16,15 @@
 from .sound_event import SoundEventAdapter, SoundEventObject
 from .sound_event_prediction import (
     SoundEventPredictionAdapter,
     SoundEventPredictionObject,
 )
 from .tag import TagAdapter, TagObject
 from .user import UserAdapter, UserObject
+from soundevent import data
 
 
 class PredictionSetObject(BaseModel):
     uuid: UUID
     created_on: Optional[datetime.datetime] = None
     collection_type: Literal["prediction_set"] = "prediction_set"
     users: Optional[List[UserObject]] = None
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/recording.py` & `soundevent-2.0.0/src/soundevent/io/aoef/recording.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import datetime
 from pathlib import Path
 from typing import Dict, List, Optional
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .adapters import DataAdapter
 from .note import NoteAdapter, NoteObject
 from .tag import TagAdapter
 from .user import UserAdapter
+from soundevent import data
 
 
 class RecordingObject(BaseModel):
     """Schema definition for a recording object in AOEF format."""
 
     uuid: UUID
     path: Path
@@ -70,26 +69,28 @@
 
         return RecordingObject(
             uuid=obj.uuid,
             path=path,
             duration=obj.duration,
             channels=obj.channels,
             samplerate=obj.samplerate,
-            time_expansion=obj.time_expansion
-            if obj.time_expansion != 1.0
-            else None,
+            time_expansion=(
+                obj.time_expansion if obj.time_expansion != 1.0 else None
+            ),
             hash=obj.hash,
             date=obj.date,
             time=obj.time,
             latitude=obj.latitude,
             longitude=obj.longitude,
             tags=tag_ids if tag_ids else None,
-            features={feature.name: feature.value for feature in obj.features}
-            if obj.features
-            else None,
+            features=(
+                {feature.name: feature.value for feature in obj.features}
+                if obj.features
+                else None
+            ),
             notes=notes if notes else None,
             owners=owners,
             rights=obj.rights,
         )
 
     def assemble_soundevent(self, obj: RecordingObject) -> data.Recording:
         tags = [
@@ -115,17 +116,17 @@
 
         return data.Recording(
             uuid=obj.uuid or uuid4(),
             path=path,
             duration=obj.duration,
             channels=obj.channels,
             samplerate=obj.samplerate,
-            time_expansion=obj.time_expansion
-            if obj.time_expansion is not None
-            else 1.0,
+            time_expansion=(
+                obj.time_expansion if obj.time_expansion is not None else 1.0
+            ),
             hash=obj.hash,
             date=obj.date,
             time=obj.time,
             latitude=obj.latitude,
             longitude=obj.longitude,
             tags=tags,
             features=[
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/recording_set.py` & `soundevent-2.0.0/src/soundevent/io/aoef/recording_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import datetime
 from typing import List, Literal, Optional
 from uuid import UUID
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .note import NoteAdapter
 from .recording import RecordingAdapter, RecordingObject
 from .tag import TagAdapter, TagObject
 from .user import UserAdapter, UserObject
+from soundevent import data
 
 
 class RecordingSetObject(BaseModel):
     """Schema definition for a dataset object in AOEF format."""
 
     uuid: UUID
     collection_type: Literal["recording_set"] = "recording_set"
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/sequence.py` & `soundevent-2.0.0/src/soundevent/io/aoef/sequence.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """Sequence object in AOEF format."""
 
-
 from typing import Dict, List, Optional
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .adapters import DataAdapter
 from .sound_event import SoundEventAdapter
+from soundevent import data
 
 
 class SequenceObject(BaseModel):
     """Schema definition for a sound event object in AOEF format."""
 
     uuid: UUID
     sound_events: List[UUID]
@@ -41,17 +39,19 @@
             for sound_event in obj.sound_events
         ]
 
         return SequenceObject(
             uuid=obj.uuid,
             sound_events=sound_events,
             parent=parent,
-            features={feature.name: feature.value for feature in obj.features}
-            if obj.features
-            else None,
+            features=(
+                {feature.name: feature.value for feature in obj.features}
+                if obj.features
+                else None
+            ),
         )
 
     def assemble_soundevent(
         self,
         obj: SequenceObject,
     ) -> data.Sequence:
         sound_events = [
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/sequence_annotation.py` & `soundevent-2.0.0/src/soundevent/io/aoef/sequence_annotation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import datetime
 from typing import List, Optional
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .adapters import DataAdapter
 from .note import NoteAdapter, NoteObject
 from .sequence import SequenceAdapter
 from .tag import TagAdapter
 from .user import UserAdapter
+from soundevent import data
 
 
 class SequenceAnnotationObject(BaseModel):
     """Schema definition for a sequence annotation object in AOEF format."""
 
     uuid: UUID
     sequence: UUID
@@ -43,24 +42,30 @@
     def assemble_aoef(
         self,
         obj: data.SequenceAnnotation,
         obj_id: UUID,
     ) -> SequenceAnnotationObject:
         return SequenceAnnotationObject(
             sequence=self.sequence_adapter.to_aoef(obj.sequence).uuid,
-            notes=[self.note_adapter.to_aoef(note) for note in obj.notes]
-            if obj.notes
-            else None,
-            tags=[self.tag_adapter.to_aoef(tag).id for tag in obj.tags]
-            if obj.tags
-            else None,
+            notes=(
+                [self.note_adapter.to_aoef(note) for note in obj.notes]
+                if obj.notes
+                else None
+            ),
+            tags=(
+                [self.tag_adapter.to_aoef(tag).id for tag in obj.tags]
+                if obj.tags
+                else None
+            ),
             uuid=obj.uuid,
-            created_by=self.user_adapter.to_aoef(obj.created_by).uuid
-            if obj.created_by
-            else None,
+            created_by=(
+                self.user_adapter.to_aoef(obj.created_by).uuid
+                if obj.created_by
+                else None
+            ),
             created_on=obj.created_on,
         )
 
     def assemble_soundevent(
         self,
         obj: SequenceAnnotationObject,
     ) -> data.SequenceAnnotation:
@@ -68,20 +73,24 @@
 
         if sequence is None:
             raise ValueError(f"Sequence with ID {obj.sequence} not found.")
 
         return data.SequenceAnnotation(
             uuid=obj.uuid or uuid4(),
             sequence=sequence,
-            notes=[self.note_adapter.to_soundevent(note) for note in obj.notes]
-            if obj.notes
-            else [],
+            notes=(
+                [self.note_adapter.to_soundevent(note) for note in obj.notes]
+                if obj.notes
+                else []
+            ),
             tags=[
                 tag
                 for tag_id in obj.tags or []
                 if (tag := self.tag_adapter.from_id(tag_id)) is not None
             ],
-            created_by=self.user_adapter.from_id(obj.created_by)
-            if obj.created_by is not None
-            else None,
+            created_by=(
+                self.user_adapter.from_id(obj.created_by)
+                if obj.created_by is not None
+                else None
+            ),
             created_on=obj.created_on or datetime.datetime.now(),
         )
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/sequence_prediction.py` & `soundevent-2.0.0/src/soundevent/io/aoef/sequence_prediction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import List, Optional, Tuple
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .adapters import DataAdapter
 from .sequence import SequenceAdapter
 from .tag import TagAdapter
+from soundevent import data
 
 
 class SequencePredictionObject(BaseModel):
     uuid: UUID
     sequence: UUID
     score: float
     tags: Optional[List[Tuple[int, float]]] = None
@@ -34,22 +33,24 @@
         obj: data.SequencePrediction,
         obj_id: UUID,
     ) -> SequencePredictionObject:
         return SequencePredictionObject(
             sequence=self.sequence_adapter.to_aoef(obj.sequence).uuid,
             uuid=obj.uuid,
             score=obj.score,
-            tags=[
-                (tag.id, predicted_tag.score)
-                for predicted_tag in obj.tags
-                if (tag := self.tag_adapter.to_aoef(predicted_tag.tag))
-                is not None
-            ]
-            if obj.tags
-            else None,
+            tags=(
+                [
+                    (tag.id, predicted_tag.score)
+                    for predicted_tag in obj.tags
+                    if (tag := self.tag_adapter.to_aoef(predicted_tag.tag))
+                    is not None
+                ]
+                if obj.tags
+                else None
+            ),
         )
 
     def assemble_soundevent(
         self,
         obj: SequencePredictionObject,
     ) -> data.SequencePrediction:
         sequence = self.sequence_adapter.from_id(obj.sequence)
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/sound_event.py` & `soundevent-2.0.0/src/soundevent/io/aoef/sound_event.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Dict, Optional
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .adapters import DataAdapter
 from .recording import RecordingAdapter
+from soundevent import data
 
 
 class SoundEventObject(BaseModel):
     """Schema definition for a sound event object in AOEF format."""
 
     uuid: UUID
     recording: UUID
@@ -33,17 +32,19 @@
         obj: data.SoundEvent,
         obj_id: UUID,
     ) -> SoundEventObject:
         return SoundEventObject(
             geometry=obj.geometry,
             uuid=obj.uuid,
             recording=self.recording_adapter.to_aoef(obj.recording).uuid,
-            features={feature.name: feature.value for feature in obj.features}
-            if obj.features
-            else None,
+            features=(
+                {feature.name: feature.value for feature in obj.features}
+                if obj.features
+                else None
+            ),
         )
 
     def assemble_soundevent(
         self,
         obj: SoundEventObject,
     ) -> data.SoundEvent:
         recording = self.recording_adapter.from_id(obj.recording)
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/sound_event_annotation.py` & `soundevent-2.0.0/src/soundevent/io/aoef/sound_event_annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import datetime
 from typing import List, Optional
 from uuid import UUID
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .adapters import DataAdapter
 from .note import NoteObject
+from soundevent import data
 
 
 class SoundEventAnnotationObject(BaseModel):
     """Schema definition for an annotation object in AOEF format."""
 
     uuid: UUID
     sound_event: UUID
@@ -42,22 +41,26 @@
     def assemble_aoef(
         self,
         obj: data.SoundEventAnnotation,
         obj_id: UUID,
     ) -> SoundEventAnnotationObject:
         return SoundEventAnnotationObject(
             sound_event=self.sound_event_adapter.to_aoef(obj.sound_event).uuid,
-            notes=[self.note_adapter.to_aoef(note) for note in obj.notes]
-            if obj.notes
-            else None,
+            notes=(
+                [self.note_adapter.to_aoef(note) for note in obj.notes]
+                if obj.notes
+                else None
+            ),
             tags=[self.tag_adapter.to_aoef(tag).id for tag in obj.tags],
             uuid=obj.uuid,
-            created_by=self.user_adapter.to_aoef(obj.created_by).uuid
-            if obj.created_by
-            else None,
+            created_by=(
+                self.user_adapter.to_aoef(obj.created_by).uuid
+                if obj.created_by
+                else None
+            ),
             created_on=obj.created_on,
         )
 
     def assemble_soundevent(
         self,
         obj: SoundEventAnnotationObject,
     ) -> data.SoundEventAnnotation:
@@ -67,20 +70,24 @@
             raise ValueError(
                 f"Sound event with ID {obj.sound_event} not found."
             )
 
         return data.SoundEventAnnotation(
             uuid=obj.uuid,
             sound_event=sound_event,
-            notes=[self.note_adapter.to_soundevent(note) for note in obj.notes]
-            if obj.notes
-            else [],
+            notes=(
+                [self.note_adapter.to_soundevent(note) for note in obj.notes]
+                if obj.notes
+                else []
+            ),
             tags=[
                 tag
                 for tag_id in obj.tags or []
                 if (tag := self.tag_adapter.from_id(tag_id)) is not None
             ],
-            created_by=self.user_adapter.from_id(obj.created_by)
-            if obj.created_by is not None
-            else None,
+            created_by=(
+                self.user_adapter.from_id(obj.created_by)
+                if obj.created_by is not None
+                else None
+            ),
             created_on=obj.created_on or datetime.datetime.now(),
         )
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/sound_event_prediction.py` & `soundevent-2.0.0/src/soundevent/io/aoef/sound_event_prediction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import List, Optional, Tuple
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .adapters import DataAdapter
 from .sound_event import SoundEventAdapter
 from .tag import TagAdapter
+from soundevent import data
 
 
 class SoundEventPredictionObject(BaseModel):
     uuid: UUID
     sound_event: UUID
     score: float
     tags: Optional[List[Tuple[int, float]]] = None
@@ -36,22 +35,24 @@
         obj: data.SoundEventPrediction,
         obj_id: UUID,
     ) -> SoundEventPredictionObject:
         return SoundEventPredictionObject(
             sound_event=self.sound_event_adapter.to_aoef(obj.sound_event).uuid,
             uuid=obj.uuid,
             score=obj.score,
-            tags=[
-                (tag.id, predicted_tag.score)
-                for predicted_tag in obj.tags
-                if (tag := self.tag_adapter.to_aoef(predicted_tag.tag))
-                is not None
-            ]
-            if obj.tags
-            else None,
+            tags=(
+                [
+                    (tag.id, predicted_tag.score)
+                    for predicted_tag in obj.tags
+                    if (tag := self.tag_adapter.to_aoef(predicted_tag.tag))
+                    is not None
+                ]
+                if obj.tags
+                else None
+            ),
         )
 
     def assemble_soundevent(
         self,
         obj: SoundEventPredictionObject,
     ) -> data.SoundEventPrediction:
         sound_event = self.sound_event_adapter.from_id(obj.sound_event)
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/tag.py` & `soundevent-2.0.0/src/soundevent/io/aoef/tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Tuple
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .adapters import DataAdapter
+from soundevent import data
 
 __all__ = ["TagObject"]
 
 
 class TagObject(BaseModel):
     """Schema definition for a tag object in AOEF format."""
```

### Comparing `soundevent-1.3.5/src/soundevent/io/aoef/user.py` & `soundevent-2.0.0/src/soundevent/io/aoef/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Optional
 from uuid import UUID, uuid4
 
 from pydantic import BaseModel
 
-from soundevent import data
-
 from .adapters import DataAdapter
+from soundevent import data
 
 
 class UserObject(BaseModel):
     """Schema definition for a user object in AOEF format."""
 
     uuid: UUID
     username: Optional[str] = None
```

### Comparing `soundevent-1.3.5/src/soundevent/io/formats.py` & `soundevent-2.0.0/src/soundevent/io/formats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Storage formats for soundevent objects."""
+
 from typing import Callable, Dict
 
 from soundevent.data import PathLike
 from soundevent.io.aoef import is_json
 
 __all__ = [
     "infer_format",
```

### Comparing `soundevent-1.3.5/src/soundevent/io/loader.py` & `soundevent-2.0.0/src/soundevent/io/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""Module for loading sound event data in various formats.
+
+This module provides a flexible `load` function to load different types of sound
+event data.
+"""
+
 import sys
 from typing import Dict, Optional, overload
 
 from soundevent import data
 from soundevent.io import aoef
 from soundevent.io.formats import infer_format
 from soundevent.io.types import DataCollections, DataType, Loader
```

### Comparing `soundevent-1.3.5/src/soundevent/io/saver.py` & `soundevent-2.0.0/src/soundevent/io/saver.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Module for saving sound event data in various formats.
+
+This module provides a versatile `save` function for storing different types of
+sound event data. Data can be saved in formats compatible with the
+`soundevent.io.load` function.
+"""
+
 from typing import Dict, Optional
 
 from soundevent import data
 from soundevent.io.aoef import save as aoef_save
 from soundevent.io.formats import infer_format
 from soundevent.io.types import DataCollections, Saver
 
@@ -38,15 +45,14 @@
         All path to audio files will be stored relative to this directory.
         This is useful to avoid storing absolute paths which are not portable.
         If `None`, audio paths will be stored as absolute paths.
     format
         Format to save the data in. If `None`, the format will be inferred
         from the file extension.
     """
-
     if format is None:
         format = infer_format(path)
 
     saver = SAVERS.get(format)
     if saver is None:
         raise ValueError(f"Unknown format {format}")
```

### Comparing `soundevent-1.3.5/src/soundevent/io/types.py` & `soundevent-2.0.0/src/soundevent/io/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Submodule of io module containing type definitions."""
+
 import sys
 from typing import Generic, Optional, TypeVar, Union
 
 from soundevent import data
 
 if sys.version_info < (3, 8):
     from typing_extensions import Literal, Protocol  # pragma: no cover
```

### Comparing `soundevent-1.3.5/src/soundevent/plot/common.py` & `soundevent-2.0.0/src/soundevent/plot/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Common utilities for plotting."""
+
 from typing import Optional, Tuple
 
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
 
 __all__ = ["create_axes"]
```

### Comparing `soundevent-1.3.5/src/soundevent/plot/tags.py` & `soundevent-2.0.0/src/soundevent/plot/tags.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Functions for plotting tags."""
 
 from itertools import cycle
 from typing import Dict, Optional
 
 import numpy as np
+from matplotlib import colormaps
 from matplotlib.axes import Axes
-from matplotlib.cm import get_cmap
 
 from soundevent import data
 from soundevent.plot.common import create_axes
 
 __all__ = [
     "plot_tag",
     "add_tags_legend",
@@ -24,23 +24,23 @@
         self,
         cmap: str = "tab20",
         num_colors: int = 20,
     ):
         """Initialize color mapper."""
         self._tags: Dict[data.Tag, str] = {}
 
-        colormap = get_cmap(cmap)
+        colormap = colormaps.get_cmap(cmap)
         self._colors = cycle(
             [colormap(x) for x in np.linspace(0, 1, num_colors)]
         )
 
     def get_color(self, tag: data.Tag) -> str:
         """Get color for tag."""
         if tag not in self._tags:
-            self._tags[tag] = next(self._colors)
+            self._tags[tag] = next(self._colors)  # type: ignore
 
         return self._tags[tag]
 
 
 def plot_tag(
     time: float,
     frequency: float,
@@ -71,12 +71,12 @@
     """Add a legend for tags."""
     handles = []
     labels = []
 
     for tag in color_mapper._tags:
         color = color_mapper.get_color(tag)
         handles.append(ax.scatter([], [], color=color))
-        labels.append(str(tag))
+        labels.append(f"{tag.key}: {tag.value}")
 
     ax.legend(handles, labels, loc="upper right")
 
     return ax
```

### Comparing `soundevent-1.3.5/tests/conftest.py` & `soundevent-2.0.0/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """Pytest fixtures for the audio tests."""
+
 import random
 import string
+import sys
 from pathlib import Path
 from typing import Optional
 from uuid import uuid4
 
 import numpy as np
 import pytest
 import soundfile as sf
 
 from soundevent import data
 
+if sys.version_info < (3, 9):
+    # NOTE: Crowsetta is not supported in Python 3.8
+    collect_ignore_glob = ["test_io/test_crowsetta/*.py"]  # pragma: no cover
+
 
 def get_random_string(length):
     """Generate a random string of fixed length."""
     letters = string.ascii_lowercase
     return "".join(random.choice(letters) for _ in range(length))
```

### Comparing `soundevent-1.3.5/tests/data/nips4b_dataset.json` & `soundevent-2.0.0/tests/data/nips4b_dataset.json`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/data/nips4b_evaluation_set.json` & `soundevent-2.0.0/tests/data/nips4b_evaluation_set.json`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/data/nips4b_model_run.json` & `soundevent-2.0.0/tests/data/nips4b_model_run.json`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_audio/24bitdepth.wav` & `soundevent-2.0.0/tests/test_audio/24bitdepth.wav`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_audio/test_io.py` & `soundevent-2.0.0/tests/test_audio/test_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Optional
 from pathlib import Path
+from typing import Optional
 
 import numpy as np
 import pytest
 
 from soundevent.audio.io import audio_to_bytes, load_audio
 
 
@@ -63,7 +63,13 @@
 
     if samples is None:
         total_samples = int(duration * samplerate)
         assert array.shape == (total_samples - offset, channels)
 
     else:
         assert array.shape == (samples, channels)
+
+
+def test_audio_to_bytes_fails_with_invalid_bit_depth():
+    array = np.random.random(size=[1024, 2])
+    with pytest.raises(ValueError):
+        audio_to_bytes(array, 16000, bit_depth=12)
```

### Comparing `soundevent-1.3.5/tests/test_audio/test_spectrograms.py` & `soundevent-2.0.0/tests/test_audio/test_spectrograms.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Test suite for spectrograms functions."""
 
 import numpy as np
 import xarray as xr
 
-from soundevent import audio, data
+from soundevent import arrays, audio, data
 
 
 def test_compute_spectrograms_from_recordings(random_wav):
     """Test computing spectrograms from a random recording."""
     # Arrange
     samplerate = 16000
     window_size = 1024 / samplerate
@@ -23,33 +23,28 @@
         window_size=window_size,
         hop_size=hop_size,
     )
 
     # Assert
     # Is correct type
     assert isinstance(spectrogram, xr.DataArray)
-    assert spectrogram.dtype == np.float32
+    assert spectrogram.dtype == np.float64
 
     # Has correct dimensions
     assert spectrogram.dims == ("frequency", "time", "channel")
-    assert spectrogram.shape == (513, 30, 1)
+    assert spectrogram.shape == (513, 33, 1)
 
     # Has correct metadata
-    assert spectrogram.attrs["samplerate"] == samplerate
     assert spectrogram.attrs["window_size"] == window_size
     assert spectrogram.attrs["hop_size"] == hop_size
     assert spectrogram.attrs["window_type"] == "hann"
 
     # Has correct coordinates
     assert spectrogram.time.data[0] == 0.0
-    assert np.isclose(
-        spectrogram.time.data[-1],
-        1.0 - window_size,
-        atol=hop_size / 4,
-    )
+    assert np.abs(spectrogram.time.data[-1] - 1.0) < hop_size
     assert spectrogram.frequency.data[0] == 0.0
     assert spectrogram.frequency.data[-1] == samplerate / 2
 
 
 def test_compute_spectrograms_from_clip(random_wav):
     """Test computing spectrograms from a random clip."""
     # Arrange
@@ -70,22 +65,64 @@
     )
 
     # Assert
     assert isinstance(spectrogram, xr.DataArray)
 
     # Has correct dimensions
     assert spectrogram.dims == ("frequency", "time", "channel")
-    assert spectrogram.shape == (513, 24, 1)
+    assert spectrogram.shape == (513, 26, 1)
 
     # Has correct metadata
-    assert spectrogram.attrs["samplerate"] == samplerate
     assert spectrogram.attrs["window_size"] == window_size
     assert spectrogram.attrs["hop_size"] == hop_size
     assert spectrogram.attrs["window_type"] == "hann"
 
     # Has correct coordinates
     assert spectrogram.time.data[0] == 0.1
-    assert np.isclose(
-        spectrogram.time.data[-1],
-        0.9 - window_size,
-        atol=hop_size / 4,
+    assert np.abs(spectrogram.time.data[-1] - 0.9) < hop_size
+
+
+def test_spectrogram_has_correct_time_step(random_wav):
+    # Arrange
+    samplerate = 16000
+    window_size = 1024 / samplerate
+    hop_size = 512 / samplerate
+
+    path = random_wav(samplerate=samplerate, duration=0.2)
+    recording = data.Recording.from_file(path)
+    clip = data.Clip(recording=recording, start_time=0.1, end_time=0.9)
+    waveform = audio.load_clip(clip)
+
+    # Act
+    spectrogram = audio.compute_spectrogram(
+        waveform,
+        window_size=window_size,
+        hop_size=hop_size,
     )
+
+    step = arrays.estimate_dim_step(spectrogram.time)
+    assert step == hop_size
+    assert spectrogram.time.attrs["step"] == hop_size
+
+
+def test_spectrogram_has_correct_frequency_step(random_wav):
+    # Arrange
+    samplerate = 16000
+    nfft = 1024
+    window_size = nfft / samplerate
+    hop_size = 512 / samplerate
+
+    path = random_wav(samplerate=samplerate, duration=0.2)
+    recording = data.Recording.from_file(path)
+    clip = data.Clip(recording=recording, start_time=0.1, end_time=0.9)
+    waveform = audio.load_clip(clip)
+
+    # Act
+    spectrogram = audio.compute_spectrogram(
+        waveform,
+        window_size=window_size,
+        hop_size=hop_size,
+    )
+
+    step = arrays.estimate_dim_step(spectrogram.frequency)
+    assert step == samplerate / 1024
+    assert spectrogram.frequency.attrs["step"] == samplerate / 1024
```

### Comparing `soundevent-1.3.5/tests/test_data/test_datasets.py` & `soundevent-2.0.0/tests/test_data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_data/test_evaluated_samples.py` & `soundevent-2.0.0/tests/test_data/test_evaluated_samples.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_data/test_geometry.py` & `soundevent-2.0.0/tests/test_data/test_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,14 @@
     # No unsorted time
     with pytest.raises(ValueError):
         data.TimeInterval(coordinates=[2, 1])
 
 
 def test_invalid_bounding_box_fails():
     """Test that an invalid bounds fails."""
-
     # No negative time
     with pytest.raises(ValueError):
         data.BoundingBox(coordinates=[-1, 0, 0, 1])
 
     # No negative frequencies
     with pytest.raises(ValueError):
         data.BoundingBox(coordinates=[0, -200, 0, 1])
```

### Comparing `soundevent-1.3.5/tests/test_data/test_tags.py` & `soundevent-2.0.0/tests/test_data/test_tags.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_evaluation/test_affinity.py` & `soundevent-2.0.0/tests/test_evaluation/test_affinity.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_evaluation/test_clip_classification.py` & `soundevent-2.0.0/tests/test_evaluation/test_clip_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,16 +211,15 @@
 
 
 def test_overall_score_is_the_mean_of_the_scores_of_all_evaluated_clips(
     annotation_set: data.AnnotationSet,
     prediction_set: data.PredictionSet,
     evaluation_tags: List[data.Tag],
 ):
-    """Test that the overall score is the mean of the scores of all evaluated
-    examples."""
+    """Test that the overall score is the mean of the scores of all evaluated examples."""
     evaluation = clip_classification(
         clip_annotations=annotation_set.clip_annotations,
         clip_predictions=prediction_set.clip_predictions,
         tags=evaluation_tags,
     )
 
     assert evaluation.score is not None
```

### Comparing `soundevent-1.3.5/tests/test_evaluation/test_clip_multilabel_classification.py` & `soundevent-2.0.0/tests/test_evaluation/test_clip_multilabel_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Test suite of the Clip Multi-Label Classification module."""
 
-
 from typing import List
 
 import pytest
 
 from soundevent import data
 from soundevent.evaluation import clip_multilabel_classification
```

### Comparing `soundevent-1.3.5/tests/test_evaluation/test_encode.py` & `soundevent-2.0.0/tests/test_evaluation/test_encode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test suite for the soundevent.evaluation.ecoding module."""
+
 from typing import Callable, Sequence
 
 import numpy as np
 import pytest
 
 from soundevent import data
 from soundevent.evaluation import (
@@ -12,35 +13,34 @@
     prediction_encoding,
 )
 from soundevent.evaluation.encoding import Encoder
 
 
 @pytest.fixture
 def tags(
-    random_tags: Callable[[int], Sequence[data.Tag]]
+    random_tags: Callable[[int], Sequence[data.Tag]],
 ) -> Sequence[data.Tag]:
     """Tags for testing."""
     return random_tags(10)
 
 
 @pytest.fixture
 def encoder(
     tags: Sequence[data.Tag],
 ) -> Encoder:
-    """Encoder for testing."""
+    """Encode for testing."""
     target_tags = tags[:5]
     return create_tag_encoder(target_tags)
 
 
 def test_classification_encoding(
     tags: Sequence[data.Tag],
     encoder: Encoder,
 ):
     """Test encoding objects with tags."""
-
     encoded = classification_encoding(
         tags=[tags[3]],
         encoder=encoder,
     )
 
     assert encoded == 3
```

### Comparing `soundevent-1.3.5/tests/test_evaluation/test_matching.py` & `soundevent-2.0.0/tests/test_evaluation/test_matching.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_evaluation/test_metrics.py` & `soundevent-2.0.0/tests/test_evaluation/test_metrics.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_evaluation/test_sound_event_detection.py` & `soundevent-2.0.0/tests/test_evaluation/test_sound_event_detection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test suite for sound event detection evaluation."""
+
 from pathlib import Path
 
 from soundevent import data, io
 from soundevent.evaluation import sound_event_detection
 
 TEST_DATA = Path(__file__).parent.parent / "data"
```

### Comparing `soundevent-1.3.5/tests/test_geometry/conftest.py` & `soundevent-2.0.0/tests/test_geometry/conftest.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_geometry/test_conversion.py` & `soundevent-2.0.0/tests/test_geometry/test_conversion.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_geometry/test_features.py` & `soundevent-2.0.0/tests/test_geometry/test_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Test suite for functions computing the geometric features."""
 
+import pytest
+
 from soundevent.data import geometries
 from soundevent.geometry import GeometricFeature, compute_geometric_features
 
 
 def test_compute_time_stamp_features():
     """Test that the duration of a TimeStamp is 0."""
     time_stamp = geometries.TimeStamp(coordinates=0)
@@ -131,7 +133,20 @@
     assert features[1].value == 0
     assert features[2].name == GeometricFeature.HIGH_FREQ
     assert features[2].value == 5
     assert features[3].name == GeometricFeature.BANDWIDTH
     assert features[3].value == 5
     assert features[4].name == GeometricFeature.NUM_SEGMENTS
     assert features[4].value == 2
+
+
+def test_compute_geometry_features_fails_on_unrecognized_geometry():
+    """Test that an error is raised when an unrecognized geometry is passed."""
+
+    class UnrecognizedGeometry(geometries.BaseGeometry):
+        type: str = "unrecognized"
+
+        coordinates: list
+
+    geometry = UnrecognizedGeometry(coordinates=[0, 1, 2, 3])
+    with pytest.raises(NotImplementedError):
+        compute_geometric_features(geometry)  # type: ignore
```

### Comparing `soundevent-1.3.5/tests/test_geometry/test_html.py` & `soundevent-2.0.0/tests/test_geometry/test_html.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test that geometries get converted to HTML."""
+
 import html5lib
 
 from soundevent import data
 from soundevent.geometry.html import geometry_to_html
 
 
 def test_can_generate_time_stamp_html(time_stamp: data.TimeStamp) -> None:
```

### Comparing `soundevent-1.3.5/tests/test_io/conftest.py` & `soundevent-2.0.0/tests/test_io/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,39 @@
         features=[
             data.Feature(name="MaxAmp", value=23.3),
         ],
     )
 
 
 @pytest.fixture
+def time_expanded_recording(
+    random_wav: Callable[[], Path],
+    user: data.User,
+    tags: List[data.Tag],
+    note: data.Note,
+) -> data.Recording:
+    path = random_wav()
+    return data.Recording.from_file(
+        path,
+        date=datetime.date(2020, 1, 1),
+        time=datetime.time(12, 0, 0),
+        time_expansion=10,
+        latitude=1.0,
+        longitude=2.0,
+        owners=[user],
+        rights="CC BY 4.0",
+        tags=tags,
+        notes=[note],
+        features=[
+            data.Feature(name="MaxAmp", value=23.3),
+        ],
+    )
+
+
+@pytest.fixture
 def recording_set(recording: data.Recording) -> data.RecordingSet:
     return data.RecordingSet(recordings=[recording])
 
 
 @pytest.fixture
 def dataset(
     recording: data.Recording,
```

### Comparing `soundevent-1.3.5/tests/test_io/test_annotation_projects.py` & `soundevent-2.0.0/tests/test_io/test_annotation_projects.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_annotation_set.py` & `soundevent-2.0.0/tests/test_io/test_annotation_set.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/conftest.py` & `soundevent-2.0.0/tests/test_io/test_aoef/conftest.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_annotation_project.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_annotation_project.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_annotation_set.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_annotation_set.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_annotation_task.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_annotation_task.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_api.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Test the basic API of the io functions."""
+
 import datetime
 import json
 from pathlib import Path
 
 import pytest
 
-from soundevent import data
-from soundevent import io
+from soundevent import data, io
 
 
 def test_load_fails_if_file_does_not_exist():
     """Test that the load function fails if the file does not exist."""
     # Arrange
     path = "non_existing_file.json"
 
@@ -27,16 +27,15 @@
 
     # Act and assert
     with pytest.raises(ValueError):
         io.load(path)
 
 
 def test_load_fails_if_collection_type_is_not_supported(tmp_path):
-    """Test that the load function fails if the collection type is not
-    supported."""
+    """Test that the load function fails if the collection type is not supported."""
     # Arrange
     path = tmp_path / "collection_type_not_supported.json"
     path.write_text(
         json.dumps(
             {
                 "version": 1,
                 "created_on": datetime.datetime.now().isoformat(),
@@ -47,16 +46,15 @@
 
     # Act and assert
     with pytest.raises(ValueError):
         io.load(path)
 
 
 def test_load_fails_if_aoef_version_is_not_supported(tmp_path):
-    """Test that the load function fails if the aoef version is not
-    supported."""
+    """Test that the load function fails if the aoef version is not supported."""
     # Arrange
     path = tmp_path / "aoef_version_not_supported.json"
     path.write_text(
         json.dumps(
             {
                 "version": 999,
                 "created_on": datetime.datetime.now().isoformat(),
@@ -87,15 +85,14 @@
     assert path.exists()
 
 
 def test_save_fails_if_trying_to_save_unsupported_collection_type(
     tmp_path: Path,
     clip_evaluation: data.ClipEvaluation,
 ):
-    """Test that the save function fails if trying to save an unsupported
-    collection type."""
+    """Test that the save function fails if trying to save an unsupported collection type."""
     # Arrange
     path = tmp_path / "unsupported_collection_type.json"
 
     # Act and assert
     with pytest.raises(NotImplementedError):
         io.save(clip_evaluation, path)  # type: ignore
```

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_clip.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_clip.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_clip_annotations.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_clip_annotations.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_clip_evaluation.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_clip_evaluation.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_clip_predictions.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_clip_predictions.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_evaluation.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_evaluation_set.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_evaluation_set.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_match.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_match.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Test suite for AOEF Match Adapter."""
 
-
 from soundevent import data
 from soundevent.io.aoef.match import MatchAdapter, MatchObject
 
 
 def test_match_can_be_converted_to_aoef(
     match: data.Match,
     match_adapter: MatchAdapter,
```

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_model_run.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_model_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Test suite for AOEF Model Run Adapter."""
 
-
 from soundevent import data
 from soundevent.io.aoef.model_run import ModelRunAdapter, ModelRunObject
 
 
 def test_model_run_can_be_converted_to_aoef(
     model_run: data.ModelRun,
     model_run_adapter: ModelRunAdapter,
```

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_note.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_note.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_prediction_set.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_prediction_set.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_recording.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_recording.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_recording_set.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_recording_set.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_sequence.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_sequence.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_sequence_annotation.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_sequence_annotation.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_sequence_prediction.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_sequence_prediction.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_sound_event_annotation.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_sound_event_annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Test suite for AOEF sound event annotation adapter."""
 
-
 from soundevent import data
 from soundevent.io.aoef.sound_event_annotation import (
     SoundEventAnnotationAdapter,
     SoundEventAnnotationObject,
 )
```

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_sound_event_prediction.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_sound_event_prediction.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_tag.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_tag.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_aoef/test_user.py` & `soundevent-2.0.0/tests/test_io/test_aoef/test_user.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_datasets.py` & `soundevent-2.0.0/tests/test_io/test_datasets.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_evaluation.py` & `soundevent-2.0.0/tests/test_io/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/tests/test_io/test_model_runs.py` & `soundevent-2.0.0/tests/test_io/test_model_runs.py`

 * *Files identical despite different names*

### Comparing `soundevent-1.3.5/PKG-INFO` & `soundevent-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: soundevent
-Version: 1.3.5
+Version: 2.0.0
 Summary: soundevent is an open-source Python package for the computational biocoustic community, providing standardized tools for sound event analysis and data management.
 Author-Email: Santiago Martinez <santiago.balvanera.20@ucl.ac.uk>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: pydantic>=2.0
 Requires-Dist: email-validator>=2.0
 Requires-Dist: matplotlib>=3.7.3; extra == "plot"
 Requires-Dist: scipy>=1.6.1; extra == "audio"
 Requires-Dist: xarray>=0.20.2; extra == "audio"
 Requires-Dist: cython>=0.29.36; extra == "audio"
 Requires-Dist: soundfile>=0.12.1; extra == "audio"
 Requires-Dist: scikit-learn>=1.3.2; extra == "evaluation"
 Requires-Dist: shapely>=2.0.1; extra == "geometry"
+Requires-Dist: rasterio>=1.3.10; extra == "geometry"
+Requires-Dist: xarray>=2023.1.0; extra == "geometry"
+Requires-Dist: crowsetta<5.0,>=4.0.0.post2; extra == "crowsetta"
+Requires-Dist: importlib-resources<6.0,>=5.0; python_version < "3.9" and extra == "crowsetta"
 Requires-Dist: soundevent[plot]; extra == "all"
 Requires-Dist: soundevent[audio]; extra == "all"
 Requires-Dist: soundevent[evaluation]; extra == "all"
 Requires-Dist: soundevent[geometry]; extra == "all"
+Requires-Dist: soundevent[crowsetta]; extra == "all"
 Provides-Extra: plot
 Provides-Extra: audio
 Provides-Extra: evaluation
 Provides-Extra: geometry
+Provides-Extra: crowsetta
 Provides-Extra: all
 Description-Content-Type: text/markdown
 
 # soundevent
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/soundevent.svg)](https://badge.fury.io/py/soundevent)
```

