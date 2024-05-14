# Comparing `tmp/whylogs-1.4.0.tar.gz` & `tmp/whylogs-1.4.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylogs-1.4.0.tar", max compression
+gzip compressed data, was "whylogs-1.4.0rc0.tar", max compression
```

## Comparing `whylogs-1.4.0.tar` & `whylogs-1.4.0rc0.tar`

### file list

```diff
@@ -1,250 +1,252 @@
--rw-r--r--   0        0        0     3166 2024-05-13 20:41:30.719503 whylogs-1.4.0/DESCRIPTION.md
--rw-r--r--   0        0        0     6646 2024-05-13 20:41:30.859971 whylogs-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1801 2024-05-13 20:41:30.907000 whylogs-1.4.0/whylogs/__init__.py
--rw-r--r--   0        0        0      347 2024-05-13 20:41:30.907352 whylogs-1.4.0/whylogs/api/__init__.py
--rw-r--r--   0        0        0      590 2024-05-13 20:41:30.907525 whylogs-1.4.0/whylogs/api/annotations.py
--rw-r--r--   0        0        0      168 2024-05-13 20:41:30.907751 whylogs-1.4.0/whylogs/api/fugue/__init__.py
--rw-r--r--   0        0        0     4840 2024-05-13 20:41:30.907985 whylogs-1.4.0/whylogs/api/fugue/profiler.py
--rw-r--r--   0        0        0     1997 2024-05-13 20:41:30.908136 whylogs-1.4.0/whylogs/api/fugue/registry.py
--rw-r--r--   0        0        0    12819 2024-05-13 20:41:30.908467 whylogs-1.4.0/whylogs/api/logger/__init__.py
--rw-r--r--   0        0        0      101 2024-05-13 20:41:30.908686 whylogs-1.4.0/whylogs/api/logger/events/__init__.py
--rw-r--r--   0        0        0     5621 2024-05-13 20:41:30.908950 whylogs-1.4.0/whylogs/api/logger/events/event.py
--rw-r--r--   0        0        0      750 2024-05-13 20:41:30.909958 whylogs-1.4.0/whylogs/api/logger/events/file_name.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.910300 whylogs-1.4.0/whylogs/api/logger/experimental/logger/__init__.py
--rw-r--r--   0        0        0     7953 2024-05-13 20:41:30.910669 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/actor.py
--rw-r--r--   0        0        0     2614 2024-05-13 20:41:30.910850 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/data_logger.py
--rw-r--r--   0        0        0     1607 2024-05-13 20:41:30.911008 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py
--rw-r--r--   0        0        0     1557 2024-05-13 20:41:30.911170 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/future_util.py
--rw-r--r--   0        0        0     1282 2024-05-13 20:41:30.911337 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/list_util.py
--rw-r--r--   0        0        0     1638 2024-05-13 20:41:30.911582 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py
--rw-r--r--   0        0        0     5181 2024-05-13 20:41:30.911910 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/pipe_signaler.py
--rw-r--r--   0        0        0      281 2024-05-13 20:41:30.912206 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/proc_error_message.py
--rw-r--r--   0        0        0     5476 2024-05-13 20:41:30.912493 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/process_actor.py
--rw-r--r--   0        0        0    18881 2024-05-13 20:41:30.912846 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py
--rw-r--r--   0        0        0     9034 2024-05-13 20:41:30.913261 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py
--rw-r--r--   0        0        0      486 2024-05-13 20:41:30.913499 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/signal_util.py
--rw-r--r--   0        0        0      641 2024-05-13 20:41:30.913745 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/string_util.py
--rw-r--r--   0        0        0     3010 2024-05-13 20:41:30.913978 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/thread_actor.py
--rw-r--r--   0        0        0    18936 2024-05-13 20:41:30.914261 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py
--rw-r--r--   0        0        0     4225 2024-05-13 20:41:30.914591 whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/time_util.py
--rw-r--r--   0        0        0     5777 2024-05-13 20:41:30.914912 whylogs-1.4.0/whylogs/api/logger/logger.py
--rw-r--r--   0        0        0    22351 2024-05-13 20:41:30.915199 whylogs-1.4.0/whylogs/api/logger/result_set.py
--rw-r--r--   0        0        0     9549 2024-05-13 20:41:30.915622 whylogs-1.4.0/whylogs/api/logger/rolling.py
--rw-r--r--   0        0        0     2113 2024-05-13 20:41:30.915893 whylogs-1.4.0/whylogs/api/logger/segment_cache.py
--rw-r--r--   0        0        0     7090 2024-05-13 20:41:30.916267 whylogs-1.4.0/whylogs/api/logger/segment_processing.py
--rw-r--r--   0        0        0      687 2024-05-13 20:41:30.916520 whylogs-1.4.0/whylogs/api/logger/transient.py
--rw-r--r--   0        0        0      406 2024-05-13 20:41:30.917022 whylogs-1.4.0/whylogs/api/pyspark/experimental/__init__.py
--rw-r--r--   0        0        0     6178 2024-05-13 20:41:30.917370 whylogs-1.4.0/whylogs/api/pyspark/experimental/profiler.py
--rw-r--r--   0        0        0     7673 2024-05-13 20:41:30.917928 whylogs-1.4.0/whylogs/api/pyspark/experimental/segmented_profiler.py
--rw-r--r--   0        0        0      465 2024-05-13 20:41:30.918356 whylogs-1.4.0/whylogs/api/reader/__init__.py
--rw-r--r--   0        0        0      645 2024-05-13 20:41:30.918577 whylogs-1.4.0/whylogs/api/reader/local.py
--rw-r--r--   0        0        0      617 2024-05-13 20:41:30.918825 whylogs-1.4.0/whylogs/api/reader/reader.py
--rw-r--r--   0        0        0     2073 2024-05-13 20:41:30.919109 whylogs-1.4.0/whylogs/api/reader/s3.py
--rw-r--r--   0        0        0      237 2024-05-13 20:41:30.919586 whylogs-1.4.0/whylogs/api/store/__init__.py
--rw-r--r--   0        0        0     4566 2024-05-13 20:41:30.919946 whylogs-1.4.0/whylogs/api/store/local_store.py
--rw-r--r--   0        0        0     1208 2024-05-13 20:41:30.920220 whylogs-1.4.0/whylogs/api/store/profile_store.py
--rw-r--r--   0        0        0      672 2024-05-13 20:41:30.920477 whylogs-1.4.0/whylogs/api/store/query.py
--rw-r--r--   0        0        0     5350 2024-05-13 20:41:30.920840 whylogs-1.4.0/whylogs/api/store/sqlite_store.py
--rw-r--r--   0        0        0     6128 2024-05-13 20:41:30.921341 whylogs-1.4.0/whylogs/api/usage_stats/__init__.py
--rw-r--r--   0        0        0       79 2024-05-13 20:41:30.921727 whylogs-1.4.0/whylogs/api/whylabs/__init__.py
--rw-r--r--   0        0        0    18270 2024-05-13 20:41:30.922239 whylogs-1.4.0/whylogs/api/whylabs/session/config.py
--rw-r--r--   0        0        0      354 2024-05-13 20:41:30.922431 whylogs-1.4.0/whylogs/api/whylabs/session/lazy.py
--rw-r--r--   0        0        0      442 2024-05-13 20:41:30.922716 whylogs-1.4.0/whylogs/api/whylabs/session/notebook_check.py
--rw-r--r--   0        0        0     3893 2024-05-13 20:41:30.922952 whylogs-1.4.0/whylogs/api/whylabs/session/notebook_logger.py
--rw-r--r--   0        0        0     2823 2024-05-13 20:41:30.923189 whylogs-1.4.0/whylogs/api/whylabs/session/prompts.py
--rw-r--r--   0        0        0    13613 2024-05-13 20:41:30.923686 whylogs-1.4.0/whylogs/api/whylabs/session/session.py
--rw-r--r--   0        0        0     6940 2024-05-13 20:41:30.923985 whylogs-1.4.0/whylogs/api/whylabs/session/session_manager.py
--rw-r--r--   0        0        0     5142 2024-05-13 20:41:30.924237 whylogs-1.4.0/whylogs/api/whylabs/session/session_types.py
--rw-r--r--   0        0        0      278 2024-05-13 20:41:30.924455 whylogs-1.4.0/whylogs/api/whylabs/session/why_init.py
--rw-r--r--   0        0        0     6581 2024-05-13 20:41:30.924726 whylogs-1.4.0/whylogs/api/whylabs/session/whylabs_client_cache.py
--rw-r--r--   0        0        0      152 2024-05-13 20:41:30.925032 whylogs-1.4.0/whylogs/api/writer/__init__.py
--rw-r--r--   0        0        0     3498 2024-05-13 20:41:30.925288 whylogs-1.4.0/whylogs/api/writer/gcs.py
--rw-r--r--   0        0        0     2300 2024-05-13 20:41:30.925512 whylogs-1.4.0/whylogs/api/writer/local.py
--rw-r--r--   0        0        0     2421 2024-05-13 20:41:30.925673 whylogs-1.4.0/whylogs/api/writer/mlflow.py
--rw-r--r--   0        0        0     4021 2024-05-13 20:41:30.925836 whylogs-1.4.0/whylogs/api/writer/s3.py
--rw-r--r--   0        0        0    11074 2024-05-13 20:41:30.926073 whylogs-1.4.0/whylogs/api/writer/whylabs.py
--rw-r--r--   0        0        0    10271 2024-05-13 20:41:30.926311 whylogs-1.4.0/whylogs/api/writer/whylabs_base.py
--rw-r--r--   0        0        0     6668 2024-05-13 20:41:30.926551 whylogs-1.4.0/whylogs/api/writer/whylabs_batch_writer.py
--rw-r--r--   0        0        0    39735 2024-05-13 20:41:30.926792 whylogs-1.4.0/whylogs/api/writer/whylabs_client.py
--rw-r--r--   0        0        0     4167 2024-05-13 20:41:30.927025 whylogs-1.4.0/whylogs/api/writer/whylabs_estimation_result_writer.py
--rw-r--r--   0        0        0     6713 2024-05-13 20:41:30.927310 whylogs-1.4.0/whylogs/api/writer/whylabs_reference_writer.py
--rw-r--r--   0        0        0     6789 2024-05-13 20:41:30.927510 whylogs-1.4.0/whylogs/api/writer/whylabs_transaction_writer.py
--rw-r--r--   0        0        0     5433 2024-05-13 20:41:30.927736 whylogs-1.4.0/whylogs/api/writer/writer.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.927915 whylogs-1.4.0/whylogs/context/__init__.py
--rw-r--r--   0        0        0      302 2024-05-13 20:41:30.928076 whylogs-1.4.0/whylogs/context/environ.py
--rw-r--r--   0        0        0      516 2024-05-13 20:41:30.928216 whylogs-1.4.0/whylogs/context/version.py
--rw-r--r--   0        0        0     1090 2024-05-13 20:41:30.928921 whylogs-1.4.0/whylogs/core/__init__.py
--rw-r--r--   0        0        0     3575 2024-05-13 20:41:30.929096 whylogs-1.4.0/whylogs/core/column_profile.py
--rw-r--r--   0        0        0      208 2024-05-13 20:41:30.929270 whylogs-1.4.0/whylogs/core/common.py
--rw-r--r--   0        0        0     1589 2024-05-13 20:41:30.929429 whylogs-1.4.0/whylogs/core/configs.py
--rw-r--r--   0        0        0      455 2024-05-13 20:41:30.929662 whylogs-1.4.0/whylogs/core/constraints/__init__.py
--rw-r--r--   0        0        0     1798 2024-05-13 20:41:30.929899 whylogs-1.4.0/whylogs/core/constraints/factories/__init__.py
--rw-r--r--   0        0        0     1103 2024-05-13 20:41:30.930056 whylogs-1.4.0/whylogs/core/constraints/factories/cardinality_metrics.py
--rw-r--r--   0        0        0     2049 2024-05-13 20:41:30.930215 whylogs-1.4.0/whylogs/core/constraints/factories/condition_counts.py
--rw-r--r--   0        0        0     2601 2024-05-13 20:41:30.931005 whylogs-1.4.0/whylogs/core/constraints/factories/count_metrics.py
--rw-r--r--   0        0        0     7063 2024-05-13 20:41:30.931353 whylogs-1.4.0/whylogs/core/constraints/factories/distribution_metrics.py
--rw-r--r--   0        0        0     2083 2024-05-13 20:41:30.931575 whylogs-1.4.0/whylogs/core/constraints/factories/frequent_items.py
--rw-r--r--   0        0        0      737 2024-05-13 20:41:30.931751 whylogs-1.4.0/whylogs/core/constraints/factories/multi_metrics.py
--rw-r--r--   0        0        0     3199 2024-05-13 20:41:30.931922 whylogs-1.4.0/whylogs/core/constraints/factories/types_metrics.py
--rw-r--r--   0        0        0    30661 2024-05-13 20:41:30.932293 whylogs-1.4.0/whylogs/core/constraints/metric_constraints.py
--rw-r--r--   0        0        0    11321 2024-05-13 20:41:30.932713 whylogs-1.4.0/whylogs/core/dataset_profile.py
--rw-r--r--   0        0        0     4230 2024-05-13 20:41:30.933105 whylogs-1.4.0/whylogs/core/datatypes.py
--rw-r--r--   0        0        0      518 2024-05-13 20:41:30.933342 whylogs-1.4.0/whylogs/core/errors.py
--rw-r--r--   0        0        0     1400 2024-05-13 20:41:30.933596 whylogs-1.4.0/whylogs/core/feature_weights.py
--rw-r--r--   0        0        0      806 2024-05-13 20:41:30.933808 whylogs-1.4.0/whylogs/core/input_resolver.py
--rw-r--r--   0        0        0     2987 2024-05-13 20:41:30.934024 whylogs-1.4.0/whylogs/core/metadata.py
--rw-r--r--   0        0        0     1740 2024-05-13 20:41:30.934222 whylogs-1.4.0/whylogs/core/metric_getters.py
--rw-r--r--   0        0        0      984 2024-05-13 20:41:30.934991 whylogs-1.4.0/whylogs/core/metrics/__init__.py
--rw-r--r--   0        0        0     4085 2024-05-13 20:41:30.935290 whylogs-1.4.0/whylogs/core/metrics/aggregators.py
--rw-r--r--   0        0        0     5031 2024-05-13 20:41:30.935564 whylogs-1.4.0/whylogs/core/metrics/column_metrics.py
--rw-r--r--   0        0        0     6481 2024-05-13 20:41:30.935923 whylogs-1.4.0/whylogs/core/metrics/compound_metric.py
--rw-r--r--   0        0        0    10678 2024-05-13 20:41:30.936222 whylogs-1.4.0/whylogs/core/metrics/condition_count_metric.py
--rw-r--r--   0        0        0     1597 2024-05-13 20:41:30.936404 whylogs-1.4.0/whylogs/core/metrics/decorators.py
--rw-r--r--   0        0        0     4840 2024-05-13 20:41:30.936738 whylogs-1.4.0/whylogs/core/metrics/deserializers.py
--rw-r--r--   0        0        0     1361 2024-05-13 20:41:30.936912 whylogs-1.4.0/whylogs/core/metrics/maths.py
--rw-r--r--   0        0        0     6053 2024-05-13 20:41:30.937166 whylogs-1.4.0/whylogs/core/metrics/metric_components.py
--rw-r--r--   0        0        0    21749 2024-05-13 20:41:30.937492 whylogs-1.4.0/whylogs/core/metrics/metrics.py
--rw-r--r--   0        0        0     8016 2024-05-13 20:41:30.937745 whylogs-1.4.0/whylogs/core/metrics/multimetric.py
--rw-r--r--   0        0        0     4517 2024-05-13 20:41:30.938071 whylogs-1.4.0/whylogs/core/metrics/serializers.py
--rw-r--r--   0        0        0     5504 2024-05-13 20:41:30.938345 whylogs-1.4.0/whylogs/core/metrics/unicode_range.py
--rw-r--r--   0        0        0      107 2024-05-13 20:41:30.938605 whylogs-1.4.0/whylogs/core/model_performance_metrics/__init__.py
--rw-r--r--   0        0        0    10663 2024-05-13 20:41:30.938862 whylogs-1.4.0/whylogs/core/model_performance_metrics/confusion_matrix.py
--rw-r--r--   0        0        0     7445 2024-05-13 20:41:30.939106 whylogs-1.4.0/whylogs/core/model_performance_metrics/model_performance_metrics.py
--rw-r--r--   0        0        0     2837 2024-05-13 20:41:30.939268 whylogs-1.4.0/whylogs/core/model_performance_metrics/regression_metrics.py
--rw-r--r--   0        0        0     5499 2024-05-13 20:41:30.939524 whylogs-1.4.0/whylogs/core/predicate_parser.py
--rw-r--r--   0        0        0    14608 2024-05-13 20:41:30.939849 whylogs-1.4.0/whylogs/core/preprocessing.py
--rw-r--r--   0        0        0      335 2024-05-13 20:41:30.940059 whylogs-1.4.0/whylogs/core/projectors.py
--rw-r--r--   0        0        0      183 2024-05-13 20:41:30.940367 whylogs-1.4.0/whylogs/core/proto/__init__.py
--rw-r--r--   0        0        0      242 2024-05-13 20:41:30.940631 whylogs-1.4.0/whylogs/core/proto/v0/__init__.py
--rw-r--r--   0        0        0    12534 2024-05-13 20:45:59.654100 whylogs-1.4.0/whylogs/core/proto/v0/v0_constraints_pb2.py
--rw-r--r--   0        0        0    20212 2024-05-13 20:45:58.520466 whylogs-1.4.0/whylogs/core/proto/v0/v0_constraints_pb2.pyi
--rw-r--r--   0        0        0    21343 2024-05-13 20:45:58.522424 whylogs-1.4.0/whylogs/core/proto/v0/v0_messages_pb2.py
--rw-r--r--   0        0        0    29724 2024-05-13 20:45:58.523979 whylogs-1.4.0/whylogs/core/proto/v0/v0_messages_pb2.pyi
--rw-r--r--   0        0        0    18521 2024-05-13 20:45:59.901235 whylogs-1.4.0/whylogs/core/proto/v0/v0_summaries_pb2.py
--rw-r--r--   0        0        0    24739 2024-05-13 20:45:58.527203 whylogs-1.4.0/whylogs/core/proto/v0/v0_summaries_pb2.pyi
--rw-r--r--   0        0        0    18571 2024-05-13 20:45:58.256704 whylogs-1.4.0/whylogs/core/proto/whylogs_messages_pb2.py
--rw-r--r--   0        0        0    21840 2024-05-13 20:45:58.258143 whylogs-1.4.0/whylogs/core/proto/whylogs_messages_pb2.pyi
--rw-r--r--   0        0        0     7350 2024-05-13 20:41:30.940879 whylogs-1.4.0/whylogs/core/relations.py
--rw-r--r--   0        0        0    11357 2024-05-13 20:41:30.941200 whylogs-1.4.0/whylogs/core/resolvers.py
--rw-r--r--   0        0        0    10754 2024-05-13 20:41:30.941456 whylogs-1.4.0/whylogs/core/schema.py
--rw-r--r--   0        0        0      144 2024-05-13 20:41:30.941607 whylogs-1.4.0/whylogs/core/segment.py
--rw-r--r--   0        0        0     2343 2024-05-13 20:41:30.941773 whylogs-1.4.0/whylogs/core/segmentation_partition.py
--rw-r--r--   0        0        0      826 2024-05-13 20:41:30.941963 whylogs-1.4.0/whylogs/core/specialized_resolvers.py
--rw-r--r--   0        0        0     2118 2024-05-13 20:41:30.942176 whylogs-1.4.0/whylogs/core/stubs.py
--rw-r--r--   0        0        0      486 2024-05-13 20:41:30.942405 whylogs-1.4.0/whylogs/core/utils/__init__.py
--rw-r--r--   0        0        0     3603 2024-05-13 20:41:30.942560 whylogs-1.4.0/whylogs/core/utils/protobuf_utils.py
--rw-r--r--   0        0        0     2569 2024-05-13 20:41:30.942700 whylogs-1.4.0/whylogs/core/utils/stats_calculations.py
--rw-r--r--   0        0        0      130 2024-05-13 20:41:30.942853 whylogs-1.4.0/whylogs/core/utils/timestamp_calculations.py
--rw-r--r--   0        0        0     2004 2024-05-13 20:41:30.943026 whylogs-1.4.0/whylogs/core/utils/utils.py
--rw-r--r--   0        0        0      281 2024-05-13 20:41:30.943287 whylogs-1.4.0/whylogs/core/validators/__init__.py
--rw-r--r--   0        0        0     4823 2024-05-13 20:41:30.943558 whylogs-1.4.0/whylogs/core/validators/condition_validator.py
--rw-r--r--   0        0        0     1329 2024-05-13 20:41:30.943778 whylogs-1.4.0/whylogs/core/validators/validator.py
--rw-r--r--   0        0        0      214 2024-05-13 20:41:30.944297 whylogs-1.4.0/whylogs/core/view/__init__.py
--rw-r--r--   0        0        0     6157 2024-05-13 20:41:30.944676 whylogs-1.4.0/whylogs/core/view/column_profile_view.py
--rw-r--r--   0        0        0    18600 2024-05-13 20:41:30.945021 whylogs-1.4.0/whylogs/core/view/dataset_profile_view.py
--rw-r--r--   0        0        0     9474 2024-05-13 20:41:30.945420 whylogs-1.4.0/whylogs/core/view/segmented_dataset_profile_view.py
--rw-r--r--   0        0        0      211 2024-05-13 20:41:30.945789 whylogs-1.4.0/whylogs/datasets/__init__.py
--rw-r--r--   0        0        0     5813 2024-05-13 20:41:30.946183 whylogs-1.4.0/whylogs/datasets/base.py
--rw-r--r--   0        0        0     6087 2024-05-13 20:41:30.946534 whylogs-1.4.0/whylogs/datasets/configs.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.946810 whylogs-1.4.0/whylogs/datasets/descr/__init__.py
--rw-r--r--   0        0        0     6397 2024-05-13 20:41:30.947195 whylogs-1.4.0/whylogs/datasets/descr/ecommerce.rst
--rw-r--r--   0        0        0     3506 2024-05-13 20:41:30.947472 whylogs-1.4.0/whylogs/datasets/descr/employee.rst
--rw-r--r--   0        0        0    11285 2024-05-13 20:41:30.948164 whylogs-1.4.0/whylogs/datasets/descr/weather.rst
--rw-r--r--   0        0        0    10688 2024-05-13 20:41:30.949324 whylogs-1.4.0/whylogs/datasets/ecommerce.py
--rw-r--r--   0        0        0    10981 2024-05-13 20:41:30.950641 whylogs-1.4.0/whylogs/datasets/employee.py
--rw-r--r--   0        0        0     2349 2024-05-13 20:41:30.950920 whylogs-1.4.0/whylogs/datasets/utils.py
--rw-r--r--   0        0        0    11476 2024-05-13 20:41:30.951685 whylogs-1.4.0/whylogs/datasets/weather.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.952010 whylogs-1.4.0/whylogs/experimental/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.952250 whylogs-1.4.0/whylogs/experimental/api/__init__.py
--rw-r--r--   0        0        0    16453 2024-05-13 20:41:30.952578 whylogs-1.4.0/whylogs/experimental/api/logger/__init__.py
--rw-r--r--   0        0        0     3770 2024-05-13 20:41:30.952889 whylogs-1.4.0/whylogs/experimental/constraints_generation/__init__.py
--rw-r--r--   0        0        0     1105 2024-05-13 20:41:30.953055 whylogs-1.4.0/whylogs/experimental/constraints_generation/condition_counts.py
--rw-r--r--   0        0        0      846 2024-05-13 20:41:30.953221 whylogs-1.4.0/whylogs/experimental/constraints_generation/count_metrics.py
--rw-r--r--   0        0        0     1554 2024-05-13 20:41:30.953384 whylogs-1.4.0/whylogs/experimental/constraints_generation/distribution_metrics.py
--rw-r--r--   0        0        0     1011 2024-05-13 20:41:30.953622 whylogs-1.4.0/whylogs/experimental/constraints_generation/frequent_items.py
--rw-r--r--   0        0        0      685 2024-05-13 20:41:30.954215 whylogs-1.4.0/whylogs/experimental/constraints_generation/multi_metrics.py
--rw-r--r--   0        0        0      973 2024-05-13 20:41:30.954467 whylogs-1.4.0/whylogs/experimental/constraints_generation/types_metrics.py
--rw-r--r--   0        0        0    19692 2024-05-13 20:41:30.955051 whylogs-1.4.0/whylogs/experimental/core/metrics/udf_metric.py
--rw-r--r--   0        0        0    19154 2024-05-13 20:41:30.955300 whylogs-1.4.0/whylogs/experimental/core/udf_schema.py
--rw-r--r--   0        0        0      299 2024-05-13 20:41:30.955597 whylogs-1.4.0/whylogs/experimental/core/validators/__init__.py
--rw-r--r--   0        0        0     1218 2024-05-13 20:41:30.955843 whylogs-1.4.0/whylogs/experimental/core/validators/condition_validator.py
--rw-r--r--   0        0        0     1698 2024-05-13 20:41:30.956083 whylogs-1.4.0/whylogs/experimental/core/validators/validator.py
--rw-r--r--   0        0        0     8861 2024-05-13 20:41:30.956579 whylogs-1.4.0/whylogs/experimental/extras/embedding_metric.py
--rw-r--r--   0        0        0      939 2024-05-13 20:41:30.956884 whylogs-1.4.0/whylogs/experimental/extras/matrix_component.py
--rwxr-xr-x   0        0        0    16737 2024-05-13 20:41:30.957168 whylogs-1.4.0/whylogs/experimental/extras/nlp_metric.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.957460 whylogs-1.4.0/whylogs/experimental/performance_estimation/__init__.py
--rw-r--r--   0        0        0     1280 2024-05-13 20:41:30.957765 whylogs-1.4.0/whylogs/experimental/performance_estimation/estimation_results.py
--rw-r--r--   0        0        0     8872 2024-05-13 20:41:30.958548 whylogs-1.4.0/whylogs/experimental/performance_estimation/estimators.py
--rw-r--r--   0        0        0     3777 2024-05-13 20:41:30.959073 whylogs-1.4.0/whylogs/experimental/preprocess/embeddings/selectors.py
--rw-r--r--   0        0        0    11126 2024-05-13 20:41:30.959737 whylogs-1.4.0/whylogs/extras/image_metric.py
--rw-r--r--   0        0        0       52 2024-05-13 20:41:30.960137 whylogs-1.4.0/whylogs/migration/__init__.py
--rw-r--r--   0        0        0    15564 2024-05-13 20:41:30.960577 whylogs-1.4.0/whylogs/migration/converters.py
--rw-r--r--   0        0        0     7662 2024-05-13 20:41:30.960903 whylogs-1.4.0/whylogs/migration/uncompound.py
--rw-r--r--   0        0        0      296 2024-05-13 20:41:30.961302 whylogs-1.4.0/whylogs/viz/__init__.py
--rw-r--r--   0        0        0      168 2024-05-13 20:41:30.961582 whylogs-1.4.0/whylogs/viz/configs.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.961990 whylogs-1.4.0/whylogs/viz/drift/__init__.py
--rw-r--r--   0        0        0    22069 2024-05-13 20:41:30.962393 whylogs-1.4.0/whylogs/viz/drift/column_drift_algorithms.py
--rw-r--r--   0        0        0     1366 2024-05-13 20:41:30.962713 whylogs-1.4.0/whylogs/viz/drift/configs.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.962986 whylogs-1.4.0/whylogs/viz/enums/__init__.py
--rw-r--r--   0        0        0      901 2024-05-13 20:41:30.963500 whylogs-1.4.0/whylogs/viz/enums/enums.py
--rw-r--r--   0        0        0        0 2024-05-13 20:41:30.963787 whylogs-1.4.0/whylogs/viz/extensions/__init__.py
--rw-r--r--   0        0        0      114 2024-05-13 20:41:30.964141 whylogs-1.4.0/whylogs/viz/extensions/reports/constraints.py
--rw-r--r--   0        0        0      272 2024-05-13 20:41:30.964338 whylogs-1.4.0/whylogs/viz/extensions/reports/histograms.py
--rw-r--r--   0        0        0     2171 2024-05-13 20:41:30.964563 whylogs-1.4.0/whylogs/viz/extensions/reports/html_report.py
--rw-r--r--   0        0        0      975 2024-05-13 20:41:30.965593 whylogs-1.4.0/whylogs/viz/extensions/reports/profile_summary.py
--rw-r--r--   0        0        0     3218 2024-05-13 20:41:30.965806 whylogs-1.4.0/whylogs/viz/extensions/reports/summary_drift.py
--rw-r--r--   0        0        0       38 2024-05-13 20:41:30.966035 whylogs-1.4.0/whylogs/viz/html/.prettierignore
--rw-r--r--   0        0        0      135 2024-05-13 20:41:30.966197 whylogs-1.4.0/whylogs/viz/html/.prettierrc.yaml
--rw-r--r--   0        0        0   155568 2024-05-13 20:41:30.966896 whylogs-1.4.0/whylogs/viz/html/css/bootstrap.min.css
--rw-r--r--   0        0        0    22747 2024-05-13 20:41:30.967298 whylogs-1.4.0/whylogs/viz/html/css/whylogs-styles.css
--rw-r--r--   0        0        0   160788 2024-05-13 20:41:30.968459 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Bold.ttf
--rw-r--r--   0        0        0    50888 2024-05-13 20:41:30.969346 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Bold.woff
--rw-r--r--   0        0        0    32180 2024-05-13 20:41:30.970143 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Bold.woff2
--rw-r--r--   0        0        0   172144 2024-05-13 20:41:30.971247 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
--rw-r--r--   0        0        0    55560 2024-05-13 20:41:30.971901 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-BoldItalic.woff
--rw-r--r--   0        0        0    35476 2024-05-13 20:41:30.972211 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
--rw-r--r--   0        0        0   172188 2024-05-13 20:41:30.973349 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Italic.ttf
--rw-r--r--   0        0        0    55728 2024-05-13 20:41:30.973892 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Italic.woff
--rw-r--r--   0        0        0    35144 2024-05-13 20:41:30.975202 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Italic.woff2
--rw-r--r--   0        0        0   161212 2024-05-13 20:41:30.976031 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Medium.ttf
--rw-r--r--   0        0        0    53244 2024-05-13 20:41:30.977239 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Medium.woff
--rw-r--r--   0        0        0    34516 2024-05-13 20:41:30.977969 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Medium.woff2
--rw-r--r--   0        0        0   172380 2024-05-13 20:41:30.978839 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
--rw-r--r--   0        0        0    59012 2024-05-13 20:41:30.979722 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-MediumItalic.woff
--rw-r--r--   0        0        0    38404 2024-05-13 20:41:30.980137 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
--rw-r--r--   0        0        0   161220 2024-05-13 20:41:30.980848 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Regular.ttf
--rw-r--r--   0        0        0    50936 2024-05-13 20:41:30.981667 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Regular.woff
--rw-r--r--   0        0        0    32192 2024-05-13 20:41:30.981990 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Regular.woff2
--rw-r--r--   0        0        0   161152 2024-05-13 20:41:30.982756 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-SemiBold.ttf
--rw-r--r--   0        0        0    53296 2024-05-13 20:41:30.983725 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-SemiBold.woff
--rw-r--r--   0        0        0    34744 2024-05-13 20:41:30.984109 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-SemiBold.woff2
--rw-r--r--   0        0        0   172396 2024-05-13 20:41:30.984873 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
--rw-r--r--   0        0        0    58892 2024-05-13 20:41:30.985612 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
--rw-r--r--   0        0        0    38500 2024-05-13 20:41:30.985962 whylogs-1.4.0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
--rw-r--r--   0        0        0     3156 2024-05-13 20:41:30.986354 whylogs-1.4.0/whylogs/viz/html/images/placement-chart.png
--rw-r--r--   0        0        0     9649 2024-05-13 20:41:30.986744 whylogs-1.4.0/whylogs/viz/html/images/whylabs-favicon.png
--rw-r--r--   0        0        0   270687 2024-05-13 20:41:30.988999 whylogs-1.4.0/whylogs/viz/html/js/d3.min.js
--rw-r--r--   0        0        0    12606 2024-05-13 20:41:30.989496 whylogs-1.4.0/whylogs/viz/html/js/handlebars.js
--rw-r--r--   0        0        0    89501 2024-05-13 20:41:30.990082 whylogs-1.4.0/whylogs/viz/html/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0    55927 2024-05-13 20:41:30.990502 whylogs-1.4.0/whylogs/viz/html/js/whylogs-script.js
--rw-r--r--   0        0        0    52663 2024-05-13 20:41:30.991128 whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
--rw-r--r--   0        0        0    14235 2024-05-13 20:41:30.991614 whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
--rw-r--r--   0        0        0    26825 2024-05-13 20:41:30.992038 whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
--rw-r--r--   0        0        0    14144 2024-05-13 20:41:30.992470 whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
--rw-r--r--   0        0        0    15177 2024-05-13 20:41:30.992839 whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
--rw-r--r--   0        0        0    18298 2024-05-13 20:41:30.993104 whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
--rw-r--r--   0        0        0    41933 2024-05-13 20:41:30.993447 whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
--rw-r--r--   0        0        0    98500 2024-05-13 20:41:30.995992 whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
--rw-r--r--   0        0        0   752494 2024-05-13 20:41:30.997043 whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-library-all-in.html
--rw-r--r--   0        0        0    25371 2024-05-13 20:41:30.998284 whylogs-1.4.0/whylogs/viz/html/templates/index-hbs.html
--rw-r--r--   0        0        0    26014 2024-05-13 20:41:30.998658 whylogs-1.4.0/whylogs/viz/html/templates/index.html
--rw-r--r--   0        0        0    22429 2024-05-13 20:41:30.998983 whylogs-1.4.0/whylogs/viz/notebook_profile_viz.py
--rw-r--r--   0        0        0      410 2024-05-13 20:41:30.999513 whylogs-1.4.0/whylogs/viz/utils/__init__.py
--rw-r--r--   0        0        0     2466 2024-05-13 20:41:30.999780 whylogs-1.4.0/whylogs/viz/utils/descriptive_stats.py
--rw-r--r--   0        0        0    12576 2024-05-13 20:41:31.000214 whylogs-1.4.0/whylogs/viz/utils/drift_calculations.py
--rw-r--r--   0        0        0     3561 2024-05-13 20:41:31.000477 whylogs-1.4.0/whylogs/viz/utils/frequent_items_calculations.py
--rw-r--r--   0        0        0     2747 2024-05-13 20:41:31.000760 whylogs-1.4.0/whylogs/viz/utils/histogram_calculations.py
--rw-r--r--   0        0        0     1128 2024-05-13 20:41:31.000999 whylogs-1.4.0/whylogs/viz/utils/html_template_utils.py
--rw-r--r--   0        0        0    14298 2024-05-13 20:41:31.001387 whylogs-1.4.0/whylogs/viz/utils/profile_viz_calculations.py
--rw-r--r--   0        0        0     3581 2024-05-13 20:41:31.001651 whylogs-1.4.0/whylogs/viz/utils/quantile_stats.py
--rw-r--r--   0        0        0     7004 1970-01-01 00:00:00.000000 whylogs-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3166 2024-04-26 21:02:29.946175 whylogs-1.4.0rc0/DESCRIPTION.md
+-rw-r--r--   0        0        0     6650 2024-04-27 00:02:55.944051 whylogs-1.4.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     1801 2024-04-26 21:02:30.063493 whylogs-1.4.0rc0/whylogs/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-26 21:02:30.063708 whylogs-1.4.0rc0/whylogs/api/__init__.py
+-rw-r--r--   0        0        0      590 2024-04-26 21:02:30.063845 whylogs-1.4.0rc0/whylogs/api/annotations.py
+-rw-r--r--   0        0        0      168 2024-04-26 21:02:30.064133 whylogs-1.4.0rc0/whylogs/api/fugue/__init__.py
+-rw-r--r--   0        0        0     4840 2024-04-26 21:02:30.064351 whylogs-1.4.0rc0/whylogs/api/fugue/profiler.py
+-rw-r--r--   0        0        0     1997 2024-04-26 21:02:30.064518 whylogs-1.4.0rc0/whylogs/api/fugue/registry.py
+-rw-r--r--   0        0        0    12819 2024-04-26 21:02:57.083873 whylogs-1.4.0rc0/whylogs/api/logger/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-26 21:02:30.066009 whylogs-1.4.0rc0/whylogs/api/logger/events/__init__.py
+-rw-r--r--   0        0        0     5621 2024-04-26 21:02:30.066189 whylogs-1.4.0rc0/whylogs/api/logger/events/event.py
+-rw-r--r--   0        0        0      750 2024-04-26 21:02:30.066765 whylogs-1.4.0rc0/whylogs/api/logger/events/file_name.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.067049 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/__init__.py
+-rw-r--r--   0        0        0     7953 2024-04-26 21:02:30.068170 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/actor.py
+-rw-r--r--   0        0        0     2614 2024-04-26 21:02:30.068350 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/data_logger.py
+-rw-r--r--   0        0        0     1607 2024-04-26 21:02:30.068507 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py
+-rw-r--r--   0        0        0     1557 2024-04-26 21:02:30.068753 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/future_util.py
+-rw-r--r--   0        0        0     1282 2024-04-26 21:02:30.068996 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/list_util.py
+-rw-r--r--   0        0        0     1638 2024-04-26 21:02:30.069153 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py
+-rw-r--r--   0        0        0     5181 2024-04-26 21:02:30.069309 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/pipe_signaler.py
+-rw-r--r--   0        0        0      281 2024-04-26 21:02:30.069434 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/proc_error_message.py
+-rw-r--r--   0        0        0     5476 2024-04-26 21:02:30.069598 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_actor.py
+-rw-r--r--   0        0        0    18881 2024-04-26 21:02:57.084243 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py
+-rw-r--r--   0        0        0     9034 2024-04-26 21:02:30.074524 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py
+-rw-r--r--   0        0        0      486 2024-04-26 21:02:30.074679 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/signal_util.py
+-rw-r--r--   0        0        0      641 2024-04-26 21:02:30.075590 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/string_util.py
+-rw-r--r--   0        0        0     3010 2024-04-26 21:02:30.076218 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/thread_actor.py
+-rw-r--r--   0        0        0    18936 2024-04-26 21:02:30.076557 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py
+-rw-r--r--   0        0        0     4225 2024-04-26 21:02:30.076782 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/time_util.py
+-rw-r--r--   0        0        0     5777 2024-04-26 21:02:30.077041 whylogs-1.4.0rc0/whylogs/api/logger/logger.py
+-rw-r--r--   0        0        0    22351 2024-04-26 21:02:57.084889 whylogs-1.4.0rc0/whylogs/api/logger/result_set.py
+-rw-r--r--   0        0        0     9549 2024-04-26 21:02:30.077787 whylogs-1.4.0rc0/whylogs/api/logger/rolling.py
+-rw-r--r--   0        0        0     2113 2024-04-26 21:02:30.078010 whylogs-1.4.0rc0/whylogs/api/logger/segment_cache.py
+-rw-r--r--   0        0        0     7090 2024-04-26 21:02:30.079019 whylogs-1.4.0rc0/whylogs/api/logger/segment_processing.py
+-rw-r--r--   0        0        0      687 2024-04-26 21:02:30.079308 whylogs-1.4.0rc0/whylogs/api/logger/transient.py
+-rw-r--r--   0        0        0      406 2024-04-26 21:02:30.079668 whylogs-1.4.0rc0/whylogs/api/pyspark/experimental/__init__.py
+-rw-r--r--   0        0        0     6178 2024-04-26 21:02:30.079867 whylogs-1.4.0rc0/whylogs/api/pyspark/experimental/profiler.py
+-rw-r--r--   0        0        0     7673 2024-04-26 21:02:30.080008 whylogs-1.4.0rc0/whylogs/api/pyspark/experimental/segmented_profiler.py
+-rw-r--r--   0        0        0      465 2024-04-26 21:02:30.080255 whylogs-1.4.0rc0/whylogs/api/reader/__init__.py
+-rw-r--r--   0        0        0      645 2024-04-26 21:02:30.080389 whylogs-1.4.0rc0/whylogs/api/reader/local.py
+-rw-r--r--   0        0        0      617 2024-04-26 21:02:30.080528 whylogs-1.4.0rc0/whylogs/api/reader/reader.py
+-rw-r--r--   0        0        0     2073 2024-04-26 21:02:30.081205 whylogs-1.4.0rc0/whylogs/api/reader/s3.py
+-rw-r--r--   0        0        0      237 2024-04-26 21:02:30.081559 whylogs-1.4.0rc0/whylogs/api/store/__init__.py
+-rw-r--r--   0        0        0     4566 2024-04-26 21:02:30.081764 whylogs-1.4.0rc0/whylogs/api/store/local_store.py
+-rw-r--r--   0        0        0     1208 2024-04-26 21:02:30.082376 whylogs-1.4.0rc0/whylogs/api/store/profile_store.py
+-rw-r--r--   0        0        0      672 2024-04-26 21:02:30.082644 whylogs-1.4.0rc0/whylogs/api/store/query.py
+-rw-r--r--   0        0        0     5350 2024-04-26 21:02:30.083354 whylogs-1.4.0rc0/whylogs/api/store/sqlite_store.py
+-rw-r--r--   0        0        0     6128 2024-04-26 21:02:30.083784 whylogs-1.4.0rc0/whylogs/api/usage_stats/__init__.py
+-rw-r--r--   0        0        0       79 2024-04-26 21:02:30.084259 whylogs-1.4.0rc0/whylogs/api/whylabs/__init__.py
+-rw-r--r--   0        0        0    18270 2024-04-26 21:02:30.084747 whylogs-1.4.0rc0/whylogs/api/whylabs/session/config.py
+-rw-r--r--   0        0        0      354 2024-04-26 21:02:30.084948 whylogs-1.4.0rc0/whylogs/api/whylabs/session/lazy.py
+-rw-r--r--   0        0        0      442 2024-04-26 21:02:30.085192 whylogs-1.4.0rc0/whylogs/api/whylabs/session/notebook_check.py
+-rw-r--r--   0        0        0     3893 2024-04-26 21:02:30.085442 whylogs-1.4.0rc0/whylogs/api/whylabs/session/notebook_logger.py
+-rw-r--r--   0        0        0     2823 2024-04-26 21:02:30.085705 whylogs-1.4.0rc0/whylogs/api/whylabs/session/prompts.py
+-rw-r--r--   0        0        0    13613 2024-04-26 21:02:30.086301 whylogs-1.4.0rc0/whylogs/api/whylabs/session/session.py
+-rw-r--r--   0        0        0     6940 2024-04-26 21:02:30.086995 whylogs-1.4.0rc0/whylogs/api/whylabs/session/session_manager.py
+-rw-r--r--   0        0        0     5142 2024-04-26 21:02:30.087545 whylogs-1.4.0rc0/whylogs/api/whylabs/session/session_types.py
+-rw-r--r--   0        0        0      278 2024-04-26 21:02:30.087706 whylogs-1.4.0rc0/whylogs/api/whylabs/session/why_init.py
+-rw-r--r--   0        0        0     6581 2024-04-26 21:02:30.087863 whylogs-1.4.0rc0/whylogs/api/whylabs/session/whylabs_client_cache.py
+-rw-r--r--   0        0        0     6622 2024-04-26 21:18:13.863456 whylogs-1.4.0rc0/whylogs/api/writer/#whylabs_batch_writer.py#
+-rw-r--r--   0        0        0      152 2024-04-26 21:02:57.085198 whylogs-1.4.0rc0/whylogs/api/writer/__init__.py
+-rw-r--r--   0        0        0     3498 2024-04-26 21:02:57.085563 whylogs-1.4.0rc0/whylogs/api/writer/gcs.py
+-rw-r--r--   0        0        0     2300 2024-04-26 21:02:57.085930 whylogs-1.4.0rc0/whylogs/api/writer/local.py
+-rw-r--r--   0        0        0     2421 2024-04-26 21:02:57.086194 whylogs-1.4.0rc0/whylogs/api/writer/mlflow.py
+-rw-r--r--   0        0        0        0 2024-04-27 00:05:16.106073 whylogs-1.4.0rc0/whylogs/api/writer/richard@richards-MacBook-Pro.26122
+-rw-r--r--   0        0        0     4021 2024-04-26 21:02:57.086609 whylogs-1.4.0rc0/whylogs/api/writer/s3.py
+-rw-r--r--   0        0        0    11074 2024-04-26 22:54:01.723581 whylogs-1.4.0rc0/whylogs/api/writer/whylabs.py
+-rw-r--r--   0        0        0    10110 2024-04-26 21:02:57.087536 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_base.py
+-rw-r--r--   0        0        0     6633 2024-04-26 21:16:43.382854 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_batch_writer.py
+-rw-r--r--   0        0        0    38861 2024-04-26 21:02:57.088060 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_client.py
+-rw-r--r--   0        0        0     4167 2024-04-26 21:02:57.088290 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_estimation_result_writer.py
+-rw-r--r--   0        0        0     6678 2024-04-26 21:18:33.755656 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_reference_writer.py
+-rw-r--r--   0        0        0     6755 2024-04-26 22:35:16.271359 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_transaction_writer.py
+-rw-r--r--   0        0        0     5433 2024-04-26 21:02:57.089133 whylogs-1.4.0rc0/whylogs/api/writer/writer.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.089202 whylogs-1.4.0rc0/whylogs/context/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-26 21:02:30.089357 whylogs-1.4.0rc0/whylogs/context/environ.py
+-rw-r--r--   0        0        0      516 2024-04-26 21:02:30.090077 whylogs-1.4.0rc0/whylogs/context/version.py
+-rw-r--r--   0        0        0     1090 2024-04-26 21:02:30.090383 whylogs-1.4.0rc0/whylogs/core/__init__.py
+-rw-r--r--   0        0        0     3575 2024-04-26 21:02:30.090535 whylogs-1.4.0rc0/whylogs/core/column_profile.py
+-rw-r--r--   0        0        0      208 2024-04-26 21:02:30.090670 whylogs-1.4.0rc0/whylogs/core/common.py
+-rw-r--r--   0        0        0     1589 2024-04-26 21:02:30.090879 whylogs-1.4.0rc0/whylogs/core/configs.py
+-rw-r--r--   0        0        0      455 2024-04-26 21:02:30.091165 whylogs-1.4.0rc0/whylogs/core/constraints/__init__.py
+-rw-r--r--   0        0        0     1798 2024-04-26 21:02:30.091993 whylogs-1.4.0rc0/whylogs/core/constraints/factories/__init__.py
+-rw-r--r--   0        0        0     1103 2024-04-26 21:02:30.092239 whylogs-1.4.0rc0/whylogs/core/constraints/factories/cardinality_metrics.py
+-rw-r--r--   0        0        0     2049 2024-04-26 21:02:30.092453 whylogs-1.4.0rc0/whylogs/core/constraints/factories/condition_counts.py
+-rw-r--r--   0        0        0     2601 2024-04-26 21:02:30.092612 whylogs-1.4.0rc0/whylogs/core/constraints/factories/count_metrics.py
+-rw-r--r--   0        0        0     7063 2024-04-26 21:02:30.092764 whylogs-1.4.0rc0/whylogs/core/constraints/factories/distribution_metrics.py
+-rw-r--r--   0        0        0     2083 2024-04-26 21:02:30.092928 whylogs-1.4.0rc0/whylogs/core/constraints/factories/frequent_items.py
+-rw-r--r--   0        0        0      737 2024-04-26 21:02:30.093167 whylogs-1.4.0rc0/whylogs/core/constraints/factories/multi_metrics.py
+-rw-r--r--   0        0        0     3199 2024-04-26 21:02:30.093863 whylogs-1.4.0rc0/whylogs/core/constraints/factories/types_metrics.py
+-rw-r--r--   0        0        0    30661 2024-04-26 21:02:30.094241 whylogs-1.4.0rc0/whylogs/core/constraints/metric_constraints.py
+-rw-r--r--   0        0        0    11321 2024-04-26 21:02:57.089842 whylogs-1.4.0rc0/whylogs/core/dataset_profile.py
+-rw-r--r--   0        0        0     4230 2024-04-26 21:02:30.095454 whylogs-1.4.0rc0/whylogs/core/datatypes.py
+-rw-r--r--   0        0        0      518 2024-04-26 21:02:30.096077 whylogs-1.4.0rc0/whylogs/core/errors.py
+-rw-r--r--   0        0        0     1400 2024-04-26 21:02:57.090158 whylogs-1.4.0rc0/whylogs/core/feature_weights.py
+-rw-r--r--   0        0        0      806 2024-04-26 21:02:30.096562 whylogs-1.4.0rc0/whylogs/core/input_resolver.py
+-rw-r--r--   0        0        0     2987 2024-04-26 21:02:30.096782 whylogs-1.4.0rc0/whylogs/core/metadata.py
+-rw-r--r--   0        0        0     1740 2024-04-26 21:02:30.096939 whylogs-1.4.0rc0/whylogs/core/metric_getters.py
+-rw-r--r--   0        0        0      984 2024-04-26 21:02:30.097220 whylogs-1.4.0rc0/whylogs/core/metrics/__init__.py
+-rw-r--r--   0        0        0     4085 2024-04-26 21:02:30.097456 whylogs-1.4.0rc0/whylogs/core/metrics/aggregators.py
+-rw-r--r--   0        0        0     5031 2024-04-26 21:02:30.097696 whylogs-1.4.0rc0/whylogs/core/metrics/column_metrics.py
+-rw-r--r--   0        0        0     6481 2024-04-26 21:02:30.098380 whylogs-1.4.0rc0/whylogs/core/metrics/compound_metric.py
+-rw-r--r--   0        0        0    10678 2024-04-26 21:02:30.098841 whylogs-1.4.0rc0/whylogs/core/metrics/condition_count_metric.py
+-rw-r--r--   0        0        0     1597 2024-04-26 21:02:30.099685 whylogs-1.4.0rc0/whylogs/core/metrics/decorators.py
+-rw-r--r--   0        0        0     4840 2024-04-26 21:02:30.099997 whylogs-1.4.0rc0/whylogs/core/metrics/deserializers.py
+-rw-r--r--   0        0        0     1361 2024-04-26 21:02:30.100234 whylogs-1.4.0rc0/whylogs/core/metrics/maths.py
+-rw-r--r--   0        0        0     6053 2024-04-26 21:02:30.101104 whylogs-1.4.0rc0/whylogs/core/metrics/metric_components.py
+-rw-r--r--   0        0        0    21749 2024-04-26 21:02:30.101553 whylogs-1.4.0rc0/whylogs/core/metrics/metrics.py
+-rw-r--r--   0        0        0     8016 2024-04-26 21:02:30.101832 whylogs-1.4.0rc0/whylogs/core/metrics/multimetric.py
+-rw-r--r--   0        0        0     4517 2024-04-26 21:02:30.102576 whylogs-1.4.0rc0/whylogs/core/metrics/serializers.py
+-rw-r--r--   0        0        0     5504 2024-04-26 21:02:30.102850 whylogs-1.4.0rc0/whylogs/core/metrics/unicode_range.py
+-rw-r--r--   0        0        0      107 2024-04-26 21:02:30.103687 whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/__init__.py
+-rw-r--r--   0        0        0    10663 2024-04-26 21:02:30.104196 whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     7445 2024-04-26 21:02:30.104467 whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/model_performance_metrics.py
+-rw-r--r--   0        0        0     2837 2024-04-26 21:02:30.104746 whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/regression_metrics.py
+-rw-r--r--   0        0        0     5499 2024-04-26 21:02:30.105006 whylogs-1.4.0rc0/whylogs/core/predicate_parser.py
+-rw-r--r--   0        0        0    14608 2024-04-26 21:02:30.105755 whylogs-1.4.0rc0/whylogs/core/preprocessing.py
+-rw-r--r--   0        0        0      335 2024-04-26 21:02:30.105951 whylogs-1.4.0rc0/whylogs/core/projectors.py
+-rw-r--r--   0        0        0      183 2024-04-26 21:02:30.106363 whylogs-1.4.0rc0/whylogs/core/proto/__init__.py
+-rw-r--r--   0        0        0      242 2024-04-26 21:02:30.106838 whylogs-1.4.0rc0/whylogs/core/proto/v0/__init__.py
+-rw-r--r--   0        0        0    12534 2024-04-26 23:53:13.202845 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_constraints_pb2.py
+-rw-r--r--   0        0        0    20212 2024-04-26 23:53:12.021184 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_constraints_pb2.pyi
+-rw-r--r--   0        0        0    21343 2024-04-26 23:53:12.023238 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_messages_pb2.py
+-rw-r--r--   0        0        0    29724 2024-04-26 23:53:12.027712 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_messages_pb2.pyi
+-rw-r--r--   0        0        0    18521 2024-04-26 23:53:13.448691 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_summaries_pb2.py
+-rw-r--r--   0        0        0    24739 2024-04-26 23:53:12.032451 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_summaries_pb2.pyi
+-rw-r--r--   0        0        0    18571 2024-04-26 23:53:11.785488 whylogs-1.4.0rc0/whylogs/core/proto/whylogs_messages_pb2.py
+-rw-r--r--   0        0        0    21840 2024-04-26 23:53:11.788864 whylogs-1.4.0rc0/whylogs/core/proto/whylogs_messages_pb2.pyi
+-rw-r--r--   0        0        0     7350 2024-04-26 21:02:30.107160 whylogs-1.4.0rc0/whylogs/core/relations.py
+-rw-r--r--   0        0        0    11357 2024-04-26 21:02:30.107626 whylogs-1.4.0rc0/whylogs/core/resolvers.py
+-rw-r--r--   0        0        0    10754 2024-04-26 21:02:30.107983 whylogs-1.4.0rc0/whylogs/core/schema.py
+-rw-r--r--   0        0        0      144 2024-04-26 21:02:30.108593 whylogs-1.4.0rc0/whylogs/core/segment.py
+-rw-r--r--   0        0        0     2343 2024-04-26 21:02:30.108833 whylogs-1.4.0rc0/whylogs/core/segmentation_partition.py
+-rw-r--r--   0        0        0      826 2024-04-26 21:02:30.109060 whylogs-1.4.0rc0/whylogs/core/specialized_resolvers.py
+-rw-r--r--   0        0        0     2118 2024-04-26 21:02:30.109644 whylogs-1.4.0rc0/whylogs/core/stubs.py
+-rw-r--r--   0        0        0      486 2024-04-26 21:02:30.110010 whylogs-1.4.0rc0/whylogs/core/utils/__init__.py
+-rw-r--r--   0        0        0     3603 2024-04-26 21:02:30.110216 whylogs-1.4.0rc0/whylogs/core/utils/protobuf_utils.py
+-rw-r--r--   0        0        0     2569 2024-04-26 21:02:30.110377 whylogs-1.4.0rc0/whylogs/core/utils/stats_calculations.py
+-rw-r--r--   0        0        0      130 2024-04-26 21:02:30.110574 whylogs-1.4.0rc0/whylogs/core/utils/timestamp_calculations.py
+-rw-r--r--   0        0        0     2004 2024-04-26 21:02:30.110740 whylogs-1.4.0rc0/whylogs/core/utils/utils.py
+-rw-r--r--   0        0        0      281 2024-04-26 21:02:30.110948 whylogs-1.4.0rc0/whylogs/core/validators/__init__.py
+-rw-r--r--   0        0        0     4823 2024-04-26 21:02:30.111113 whylogs-1.4.0rc0/whylogs/core/validators/condition_validator.py
+-rw-r--r--   0        0        0     1329 2024-04-26 21:02:30.111610 whylogs-1.4.0rc0/whylogs/core/validators/validator.py
+-rw-r--r--   0        0        0      214 2024-04-26 21:02:30.111979 whylogs-1.4.0rc0/whylogs/core/view/__init__.py
+-rw-r--r--   0        0        0     6157 2024-04-26 21:02:30.112333 whylogs-1.4.0rc0/whylogs/core/view/column_profile_view.py
+-rw-r--r--   0        0        0    18600 2024-04-26 21:02:57.090538 whylogs-1.4.0rc0/whylogs/core/view/dataset_profile_view.py
+-rw-r--r--   0        0        0     9474 2024-04-26 21:02:57.091117 whylogs-1.4.0rc0/whylogs/core/view/segmented_dataset_profile_view.py
+-rw-r--r--   0        0        0      211 2024-04-26 21:02:30.113593 whylogs-1.4.0rc0/whylogs/datasets/__init__.py
+-rw-r--r--   0        0        0     5813 2024-04-26 21:02:30.113832 whylogs-1.4.0rc0/whylogs/datasets/base.py
+-rw-r--r--   0        0        0     6087 2024-04-26 21:02:30.114504 whylogs-1.4.0rc0/whylogs/datasets/configs.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.114862 whylogs-1.4.0rc0/whylogs/datasets/descr/__init__.py
+-rw-r--r--   0        0        0     6397 2024-04-26 21:02:30.115167 whylogs-1.4.0rc0/whylogs/datasets/descr/ecommerce.rst
+-rw-r--r--   0        0        0     3506 2024-04-26 21:02:30.116132 whylogs-1.4.0rc0/whylogs/datasets/descr/employee.rst
+-rw-r--r--   0        0        0    11285 2024-04-26 21:02:30.116732 whylogs-1.4.0rc0/whylogs/datasets/descr/weather.rst
+-rw-r--r--   0        0        0    10688 2024-04-26 21:02:30.117401 whylogs-1.4.0rc0/whylogs/datasets/ecommerce.py
+-rw-r--r--   0        0        0    10981 2024-04-26 21:02:30.117969 whylogs-1.4.0rc0/whylogs/datasets/employee.py
+-rw-r--r--   0        0        0     2349 2024-04-26 21:02:30.118208 whylogs-1.4.0rc0/whylogs/datasets/utils.py
+-rw-r--r--   0        0        0    11476 2024-04-26 21:02:30.118700 whylogs-1.4.0rc0/whylogs/datasets/weather.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.118942 whylogs-1.4.0rc0/whylogs/experimental/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.119221 whylogs-1.4.0rc0/whylogs/experimental/api/__init__.py
+-rw-r--r--   0        0        0    15177 2024-04-26 21:02:30.119905 whylogs-1.4.0rc0/whylogs/experimental/api/logger/__init__.py
+-rw-r--r--   0        0        0     3770 2024-04-26 21:02:30.120168 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/__init__.py
+-rw-r--r--   0        0        0     1105 2024-04-26 21:02:30.120422 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/condition_counts.py
+-rw-r--r--   0        0        0      846 2024-04-26 21:02:30.120686 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/count_metrics.py
+-rw-r--r--   0        0        0     1554 2024-04-26 21:02:30.120930 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/distribution_metrics.py
+-rw-r--r--   0        0        0     1011 2024-04-26 21:02:30.121140 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/frequent_items.py
+-rw-r--r--   0        0        0      685 2024-04-26 21:02:30.121327 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/multi_metrics.py
+-rw-r--r--   0        0        0      973 2024-04-26 21:02:30.121539 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/types_metrics.py
+-rw-r--r--   0        0        0    19692 2024-04-26 21:02:30.122243 whylogs-1.4.0rc0/whylogs/experimental/core/metrics/udf_metric.py
+-rw-r--r--   0        0        0    19154 2024-04-26 21:02:30.122535 whylogs-1.4.0rc0/whylogs/experimental/core/udf_schema.py
+-rw-r--r--   0        0        0      299 2024-04-26 21:02:30.122823 whylogs-1.4.0rc0/whylogs/experimental/core/validators/__init__.py
+-rw-r--r--   0        0        0     1218 2024-04-26 21:02:30.122974 whylogs-1.4.0rc0/whylogs/experimental/core/validators/condition_validator.py
+-rw-r--r--   0        0        0     1698 2024-04-26 21:02:30.123128 whylogs-1.4.0rc0/whylogs/experimental/core/validators/validator.py
+-rw-r--r--   0        0        0     8861 2024-04-26 21:02:30.123654 whylogs-1.4.0rc0/whylogs/experimental/extras/embedding_metric.py
+-rw-r--r--   0        0        0      939 2024-04-26 21:02:30.123862 whylogs-1.4.0rc0/whylogs/experimental/extras/matrix_component.py
+-rwxr-xr-x   0        0        0    16737 2024-04-26 21:02:30.124080 whylogs-1.4.0rc0/whylogs/experimental/extras/nlp_metric.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.124365 whylogs-1.4.0rc0/whylogs/experimental/performance_estimation/__init__.py
+-rw-r--r--   0        0        0     1280 2024-04-26 21:02:57.091490 whylogs-1.4.0rc0/whylogs/experimental/performance_estimation/estimation_results.py
+-rw-r--r--   0        0        0     8872 2024-04-26 21:02:30.126148 whylogs-1.4.0rc0/whylogs/experimental/performance_estimation/estimators.py
+-rw-r--r--   0        0        0     3777 2024-04-26 21:02:30.128009 whylogs-1.4.0rc0/whylogs/experimental/preprocess/embeddings/selectors.py
+-rw-r--r--   0        0        0    11126 2024-04-26 21:02:30.128727 whylogs-1.4.0rc0/whylogs/extras/image_metric.py
+-rw-r--r--   0        0        0       52 2024-04-26 21:02:30.129427 whylogs-1.4.0rc0/whylogs/migration/__init__.py
+-rw-r--r--   0        0        0    15564 2024-04-26 21:02:30.130625 whylogs-1.4.0rc0/whylogs/migration/converters.py
+-rw-r--r--   0        0        0     7662 2024-04-26 21:02:30.130849 whylogs-1.4.0rc0/whylogs/migration/uncompound.py
+-rw-r--r--   0        0        0      296 2024-04-26 21:02:30.131116 whylogs-1.4.0rc0/whylogs/viz/__init__.py
+-rw-r--r--   0        0        0      168 2024-04-26 21:02:30.131338 whylogs-1.4.0rc0/whylogs/viz/configs.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.131523 whylogs-1.4.0rc0/whylogs/viz/drift/__init__.py
+-rw-r--r--   0        0        0    22069 2024-04-26 21:02:30.132305 whylogs-1.4.0rc0/whylogs/viz/drift/column_drift_algorithms.py
+-rw-r--r--   0        0        0     1366 2024-04-26 21:02:30.132487 whylogs-1.4.0rc0/whylogs/viz/drift/configs.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.132653 whylogs-1.4.0rc0/whylogs/viz/enums/__init__.py
+-rw-r--r--   0        0        0      901 2024-04-26 21:02:30.132892 whylogs-1.4.0rc0/whylogs/viz/enums/enums.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.133697 whylogs-1.4.0rc0/whylogs/viz/extensions/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-26 21:02:30.133973 whylogs-1.4.0rc0/whylogs/viz/extensions/reports/constraints.py
+-rw-r--r--   0        0        0      272 2024-04-26 21:02:30.134163 whylogs-1.4.0rc0/whylogs/viz/extensions/reports/histograms.py
+-rw-r--r--   0        0        0     2171 2024-04-26 21:02:57.091852 whylogs-1.4.0rc0/whylogs/viz/extensions/reports/html_report.py
+-rw-r--r--   0        0        0      975 2024-04-26 21:02:30.135017 whylogs-1.4.0rc0/whylogs/viz/extensions/reports/profile_summary.py
+-rw-r--r--   0        0        0     3218 2024-04-26 21:02:30.135259 whylogs-1.4.0rc0/whylogs/viz/extensions/reports/summary_drift.py
+-rw-r--r--   0        0        0       38 2024-04-26 21:02:30.135605 whylogs-1.4.0rc0/whylogs/viz/html/.prettierignore
+-rw-r--r--   0        0        0      135 2024-04-26 21:02:30.135825 whylogs-1.4.0rc0/whylogs/viz/html/.prettierrc.yaml
+-rw-r--r--   0        0        0   155568 2024-04-26 21:02:30.136368 whylogs-1.4.0rc0/whylogs/viz/html/css/bootstrap.min.css
+-rw-r--r--   0        0        0    22747 2024-04-26 21:02:30.136699 whylogs-1.4.0rc0/whylogs/viz/html/css/whylogs-styles.css
+-rw-r--r--   0        0        0   160788 2024-04-26 21:02:30.137324 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.ttf
+-rw-r--r--   0        0        0    50888 2024-04-26 21:02:30.137795 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.woff
+-rw-r--r--   0        0        0    32180 2024-04-26 21:02:30.163153 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.woff2
+-rw-r--r--   0        0        0   172144 2024-04-26 21:02:30.163664 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
+-rw-r--r--   0        0        0    55560 2024-04-26 21:02:30.164714 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff
+-rw-r--r--   0        0        0    35476 2024-04-26 21:02:30.165330 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
+-rw-r--r--   0        0        0   172188 2024-04-26 21:02:30.165793 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.ttf
+-rw-r--r--   0        0        0    55728 2024-04-26 21:02:30.166103 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.woff
+-rw-r--r--   0        0        0    35144 2024-04-26 21:02:30.166288 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.woff2
+-rw-r--r--   0        0        0   161212 2024-04-26 21:02:30.166714 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.ttf
+-rw-r--r--   0        0        0    53244 2024-04-26 21:02:30.167040 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.woff
+-rw-r--r--   0        0        0    34516 2024-04-26 21:02:30.167237 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.woff2
+-rw-r--r--   0        0        0   172380 2024-04-26 21:02:30.167700 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
+-rw-r--r--   0        0        0    59012 2024-04-26 21:02:30.168007 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff
+-rw-r--r--   0        0        0    38404 2024-04-26 21:02:30.168227 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
+-rw-r--r--   0        0        0   161220 2024-04-26 21:02:30.168656 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.ttf
+-rw-r--r--   0        0        0    50936 2024-04-26 21:02:30.169371 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.woff
+-rw-r--r--   0        0        0    32192 2024-04-26 21:02:30.169558 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.woff2
+-rw-r--r--   0        0        0   161152 2024-04-26 21:02:30.170475 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.ttf
+-rw-r--r--   0        0        0    53296 2024-04-26 21:02:30.170829 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff
+-rw-r--r--   0        0        0    34744 2024-04-26 21:02:30.171479 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff2
+-rw-r--r--   0        0        0   172396 2024-04-26 21:02:30.171957 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0        0        0    58892 2024-04-26 21:02:30.172659 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
+-rw-r--r--   0        0        0    38500 2024-04-26 21:02:30.173258 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
+-rw-r--r--   0        0        0     3156 2024-04-26 21:02:30.173506 whylogs-1.4.0rc0/whylogs/viz/html/images/placement-chart.png
+-rw-r--r--   0        0        0     9649 2024-04-26 21:02:30.173841 whylogs-1.4.0rc0/whylogs/viz/html/images/whylabs-favicon.png
+-rw-r--r--   0        0        0   270687 2024-04-26 21:02:30.174623 whylogs-1.4.0rc0/whylogs/viz/html/js/d3.min.js
+-rw-r--r--   0        0        0    12606 2024-04-26 21:02:30.175451 whylogs-1.4.0rc0/whylogs/viz/html/js/handlebars.js
+-rw-r--r--   0        0        0    89501 2024-04-26 21:02:30.175796 whylogs-1.4.0rc0/whylogs/viz/html/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0    55927 2024-04-26 21:02:30.176016 whylogs-1.4.0rc0/whylogs/viz/html/js/whylogs-script.js
+-rw-r--r--   0        0        0    52663 2024-04-26 21:02:30.176733 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
+-rw-r--r--   0        0        0    14235 2024-04-26 21:02:30.177157 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
+-rw-r--r--   0        0        0    26825 2024-04-26 21:02:30.177379 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
+-rw-r--r--   0        0        0    14144 2024-04-26 21:02:30.177724 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
+-rw-r--r--   0        0        0    15177 2024-04-26 21:02:30.178049 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
+-rw-r--r--   0        0        0    18298 2024-04-26 21:02:30.178223 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
+-rw-r--r--   0        0        0    41933 2024-04-26 21:02:30.178408 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
+-rw-r--r--   0        0        0    98500 2024-04-26 21:02:30.179832 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
+-rw-r--r--   0        0        0   752494 2024-04-26 21:02:30.180443 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-library-all-in.html
+-rw-r--r--   0        0        0    25371 2024-04-26 21:02:30.180710 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs.html
+-rw-r--r--   0        0        0    26014 2024-04-26 21:02:30.180899 whylogs-1.4.0rc0/whylogs/viz/html/templates/index.html
+-rw-r--r--   0        0        0    22429 2024-04-26 21:02:30.181067 whylogs-1.4.0rc0/whylogs/viz/notebook_profile_viz.py
+-rw-r--r--   0        0        0      410 2024-04-26 21:02:30.181325 whylogs-1.4.0rc0/whylogs/viz/utils/__init__.py
+-rw-r--r--   0        0        0     2466 2024-04-26 21:02:30.181455 whylogs-1.4.0rc0/whylogs/viz/utils/descriptive_stats.py
+-rw-r--r--   0        0        0    12576 2024-04-26 21:02:30.182816 whylogs-1.4.0rc0/whylogs/viz/utils/drift_calculations.py
+-rw-r--r--   0        0        0     3561 2024-04-26 21:02:30.182997 whylogs-1.4.0rc0/whylogs/viz/utils/frequent_items_calculations.py
+-rw-r--r--   0        0        0     2747 2024-04-26 21:02:30.186179 whylogs-1.4.0rc0/whylogs/viz/utils/histogram_calculations.py
+-rw-r--r--   0        0        0     1128 2024-04-26 21:02:30.186828 whylogs-1.4.0rc0/whylogs/viz/utils/html_template_utils.py
+-rw-r--r--   0        0        0    14298 2024-04-26 21:02:30.193627 whylogs-1.4.0rc0/whylogs/viz/utils/profile_viz_calculations.py
+-rw-r--r--   0        0        0     3581 2024-04-26 21:02:30.193953 whylogs-1.4.0rc0/whylogs/viz/utils/quantile_stats.py
+-rw-r--r--   0        0        0     7007 1970-01-01 00:00:00.000000 whylogs-1.4.0rc0/PKG-INFO
```

### Comparing `whylogs-1.4.0/DESCRIPTION.md` & `whylogs-1.4.0rc0/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/pyproject.toml` & `whylogs-1.4.0rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylogs"
-version = "1.4.0"
+version = "1.4.0-rc0"
 description = "Profile and monitor your ML data pipeline end-to-end"
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 homepage = "https://docs.whylabs.ai"
 readme = "DESCRIPTION.md"
 include = ["whylogs/core/proto/v0/*.py*", "whylogs/core/proto/*.py*"]
```

### Comparing `whylogs-1.4.0/whylogs/__init__.py` & `whylogs-1.4.0rc0/whylogs/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/annotations.py` & `whylogs-1.4.0rc0/whylogs/api/annotations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/fugue/profiler.py` & `whylogs-1.4.0rc0/whylogs/api/fugue/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/fugue/registry.py` & `whylogs-1.4.0rc0/whylogs/api/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/__init__.py` & `whylogs-1.4.0rc0/whylogs/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/events/event.py` & `whylogs-1.4.0rc0/whylogs/api/logger/events/event.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/events/file_name.py` & `whylogs-1.4.0rc0/whylogs/api/logger/events/file_name.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/actor.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/actor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/data_logger.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/data_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/future_util.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/future_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/list_util.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/list_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/pipe_signaler.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/pipe_signaler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/process_actor.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_actor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/string_util.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/string_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/thread_actor.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/thread_actor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/experimental/logger/actor/time_util.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/time_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/logger.py` & `whylogs-1.4.0rc0/whylogs/api/logger/logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/result_set.py` & `whylogs-1.4.0rc0/whylogs/api/logger/result_set.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/rolling.py` & `whylogs-1.4.0rc0/whylogs/api/logger/rolling.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/segment_cache.py` & `whylogs-1.4.0rc0/whylogs/api/logger/segment_cache.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/segment_processing.py` & `whylogs-1.4.0rc0/whylogs/api/logger/segment_processing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/logger/transient.py` & `whylogs-1.4.0rc0/whylogs/api/logger/transient.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/pyspark/experimental/profiler.py` & `whylogs-1.4.0rc0/whylogs/api/pyspark/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/pyspark/experimental/segmented_profiler.py` & `whylogs-1.4.0rc0/whylogs/api/pyspark/experimental/segmented_profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/reader/local.py` & `whylogs-1.4.0rc0/whylogs/api/reader/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/reader/reader.py` & `whylogs-1.4.0rc0/whylogs/api/reader/reader.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/reader/s3.py` & `whylogs-1.4.0rc0/whylogs/api/reader/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/store/local_store.py` & `whylogs-1.4.0rc0/whylogs/api/store/local_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/store/profile_store.py` & `whylogs-1.4.0rc0/whylogs/api/store/profile_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/store/query.py` & `whylogs-1.4.0rc0/whylogs/api/store/query.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/store/sqlite_store.py` & `whylogs-1.4.0rc0/whylogs/api/store/sqlite_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/usage_stats/__init__.py` & `whylogs-1.4.0rc0/whylogs/api/usage_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/whylabs/session/config.py` & `whylogs-1.4.0rc0/whylogs/api/whylabs/session/config.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/whylabs/session/notebook_logger.py` & `whylogs-1.4.0rc0/whylogs/api/whylabs/session/notebook_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/whylabs/session/prompts.py` & `whylogs-1.4.0rc0/whylogs/api/whylabs/session/prompts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/whylabs/session/session.py` & `whylogs-1.4.0rc0/whylogs/api/whylabs/session/session.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/whylabs/session/session_manager.py` & `whylogs-1.4.0rc0/whylogs/api/whylabs/session/session_manager.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/whylabs/session/session_types.py` & `whylogs-1.4.0rc0/whylogs/api/whylabs/session/session_types.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/whylabs/session/whylabs_client_cache.py` & `whylogs-1.4.0rc0/whylogs/api/whylabs/session/whylabs_client_cache.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/writer/gcs.py` & `whylogs-1.4.0rc0/whylogs/api/writer/gcs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/writer/local.py` & `whylogs-1.4.0rc0/whylogs/api/writer/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/writer/mlflow.py` & `whylogs-1.4.0rc0/whylogs/api/writer/mlflow.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/writer/s3.py` & `whylogs-1.4.0rc0/whylogs/api/writer/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/writer/whylabs.py` & `whylogs-1.4.0rc0/whylogs/api/writer/whylabs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/writer/whylabs_base.py` & `whylogs-1.4.0rc0/whylogs/api/writer/whylabs_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import tempfile
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import requests  # type: ignore
 from whylabs_client import ApiClient
 from whylabs_client.model.segment_tag import SegmentTag
 
-from whylogs.api.logger.result_set import ProfileResultSet, ResultSet, ViewResultSet
+from whylogs.api.logger.result_set import ProfileResultSet, ViewResultSet
 from whylogs.api.whylabs.session.session_manager import default_init
 from whylogs.api.writer.whylabs_client import WhyLabsClient
 from whylogs.api.writer.writer import Writable, Writer
 from whylogs.core import DatasetProfileView
 from whylogs.core.dataset_profile import DatasetProfile
 from whylogs.core.errors import BadConfigError
 from whylogs.core.view.segmented_dataset_profile_view import SegmentedDatasetProfileView
@@ -173,27 +173,24 @@
             logger.error(
                 f"Profiles should have timestamps greater than 0, but found a timestamp of {stamp}"
                 f" and current timestamp is {utc_now.timestamp()}, this is likely an error."
             )
 
         return int(stamp * 1000)
 
-    def _custom_tagging(
-        self,
-        view: Union[DatasetProfile, DatasetProfileView, SegmentedDatasetProfileView, ResultSet],
-    ) -> None:
-        self._whylabs_client._tag_custom_perf_metrics(view)
-        self._whylabs_client._tag_custom_output_metrics(view)
-
     def _prepare_view_for_upload(
         self,
         view: Union[DatasetProfileView, SegmentedDatasetProfileView],
     ) -> Union[DatasetProfileView, SegmentedDatasetProfileView]:
         view_is_a_segment = isinstance(view, SegmentedDatasetProfileView)
+        self._whylabs_client._tag_custom_perf_metrics(view)
+        self._whylabs_client._tag_custom_output_metrics(view)
+
         flags = FeatureFlags(_check_whylabs_condition_count_uncompound())
+
         if _uncompound_metric_feature_flag():
             if view_is_a_segment:
                 updated_profile_view = _uncompound_dataset_profile(view.profile_view, flags)
                 view = SegmentedDatasetProfileView(
                     profile_view=updated_profile_view, segment=view._segment, partition=view._partition
                 )
```

### Comparing `whylogs-1.4.0/whylogs/api/writer/whylabs_batch_writer.py` & `whylogs-1.4.0rc0/whylogs/api/writer/#whylabs_batch_writer.py#`

 * *Files 1% similar despite different names*

```diff
@@ -131,19 +131,17 @@
         return self._upload_view(view, profile_id, upload_url, dataset_timestamp_epoch, **kwargs)
 
     @deprecated_alias(profile="file")
     def write(
         self, file: Writable, dest: Optional[str] = None, **kwargs: Any
     ) -> Tuple[bool, Union[str, List[Tuple[bool, str]]]]:
         self._whylabs_client = self._whylabs_client.option(**kwargs)  # type: ignore
-        self._custom_tagging(file)
 
         if isinstance(file, SegmentedResultSet):
-            # TODO: force zip if the number of segemtns is large
-            if kwargs.get("zip"):
+            if kwargs.get("zip"):  # TODO: force zip if the number of segemtns is large
                 return self._write_segmented_result_set_zip(file, **kwargs)
             else:
                 return self._write_segmented_result_set(file, **kwargs)
 
         # file represents a single profile/segment, extract a view of it
         view = self._get_view_of_writable(file)
         return self._write_view(view, **kwargs)
```

### Comparing `whylogs-1.4.0/whylogs/api/writer/whylabs_client.py` & `whylogs-1.4.0rc0/whylogs/api/writer/whylabs_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 import pprint
-from typing import IO, Any, Dict, List, Optional, Set, Tuple, Union
+from typing import IO, Any, Dict, List, Optional, Tuple, Union
 from urllib.parse import urlparse
 
 import requests  # type: ignore
 from urllib3 import PoolManager, ProxyManager
 from whylabs_client import ApiClient, Configuration  # type: ignore
 from whylabs_client.api.dataset_profile_api import DatasetProfileApi  # type: ignore
 from whylabs_client.api.feature_weights_api import FeatureWeightsApi  # type: ignore
@@ -28,24 +28,23 @@
 from whylabs_client.model.segment import Segment  # type: ignore
 from whylabs_client.model.segment_tag import SegmentTag  # type: ignore
 from whylabs_client.model.transaction_commit_request import TransactionCommitRequest
 from whylabs_client.model.transaction_log_request import TransactionLogRequest
 from whylabs_client.model.transaction_start_request import TransactionStartRequest
 from whylabs_client.rest import ForbiddenException  # type: ignore
 
-from whylogs.api.logger.result_set import ResultSet, SegmentedResultSet
 from whylogs.api.whylabs.session.session_manager import INIT_DOCS, default_init
 from whylogs.api.whylabs.session.whylabs_client_cache import (
     ClientCacheConfig,
     EnvironmentKeyRefresher,
     KeyRefresher,
     WhylabsClientCache,
 )
 from whylogs.context.environ import read_bool_env_var
-from whylogs.core import DatasetProfile, DatasetProfileView
+from whylogs.core import DatasetProfileView
 from whylogs.core.feature_weights import FeatureWeights
 from whylogs.core.utils.utils import get_auth_headers
 from whylogs.core.view.segmented_dataset_profile_view import SegmentedDatasetProfileView
 
 FIVE_MINUTES_IN_SECONDS = 60 * 5
 DAY_IN_SECONDS = 60 * 60 * 24
 FIVE_YEARS_IN_SECONDS = DAY_IN_SECONDS * 365 * 5
@@ -79,36 +78,14 @@
     "top_rank": ("integral", "continuous"),
     "average_precision_k_": ("fractional", "continuous"),
     "norm_dis_cumul_gain_k_": ("fractional", "continuous"),
     "sum_gain_k_": ("fractional", "continuous"),
 }
 
 
-def _get_column_names(x: Union[DatasetProfile, DatasetProfileView, SegmentedDatasetProfileView, ResultSet]) -> Set[str]:
-    if isinstance(x, DatasetProfile):
-        return _get_column_names(x.view())
-    elif isinstance(x, DatasetProfileView):
-        return set(x.get_columns().keys())
-    elif isinstance(x, SegmentedDatasetProfileView):
-        return _get_column_names(x._profile_view)
-    elif isinstance(x, SegmentedResultSet):
-        maps = x._segments.values()
-        if not maps:
-            return set()
-        segments = list(maps)[0].values()
-        if not segments:
-            return set()
-        segment = list(segments)[0]
-        view = segment if isinstance(segment, DatasetProfileView) else segment.view()
-        return _get_column_names(view)
-
-    assert isinstance(x, ResultSet)
-    return _get_column_names(x.view())
-
-
 class TransactionAbortedException(Exception):
     pass
 
 
 class WhyLabsClient:
     f"""
     An interface for interacting with the WhyLabs platform.
@@ -487,37 +464,35 @@
                 f"Failed to set column outputs {self._org_id}/{self._dataset_id} for column name: ("
                 f"{column_name}) "
                 f"{self.whylabs_api_endpoint}"
                 f" with API token ID: {self.key_id}"
             )
             raise e
 
-    def _tag_custom_output_metrics(
-        self, view: Union[DatasetProfile, DatasetProfileView, SegmentedDatasetProfileView, ResultSet]
-    ) -> None:
-        column_names = _get_column_names(view)
-        for column_name in column_names:
-            for perf_col in KNOWN_CUSTOM_OUTPUT_METRICS:
-                if column_name.startswith(perf_col):
-                    data_type = KNOWN_CUSTOM_OUTPUT_METRICS[perf_col][0]
-                    discreteness = KNOWN_CUSTOM_OUTPUT_METRICS[perf_col][1]
-                    column_schema: ColumnSchema = ColumnSchema(
-                        classifier="output", data_type=data_type, discreteness=discreteness  # type: ignore
-                    )
-                    self._set_column_schema(column_name, column_schema=column_schema)
-
-    def _tag_custom_perf_metrics(
-        self, view: Union[DatasetProfile, DatasetProfileView, SegmentedDatasetProfileView, ResultSet]
-    ) -> None:
-        column_names = _get_column_names(view)
-        for column_name in column_names:
-            for perf_col in KNOWN_CUSTOM_PERFORMANCE_METRICS:
-                if column_name.startswith(perf_col):
-                    metric = KNOWN_CUSTOM_PERFORMANCE_METRICS[perf_col]
-                    self.tag_custom_performance_column(column_name, default_metric=metric)
+    def _tag_custom_output_metrics(self, view: Union[DatasetProfileView, SegmentedDatasetProfileView]):
+        if isinstance(view, DatasetProfileView):
+            column_names = view.get_columns().keys()
+            for column_name in column_names:
+                for perf_col in KNOWN_CUSTOM_OUTPUT_METRICS:
+                    if column_name.startswith(perf_col):
+                        data_type = KNOWN_CUSTOM_OUTPUT_METRICS[perf_col][0]
+                        discreteness = KNOWN_CUSTOM_OUTPUT_METRICS[perf_col][1]
+                        column_schema: ColumnSchema = ColumnSchema(
+                            classifier="output", data_type=data_type, discreteness=discreteness  # type: ignore
+                        )
+                        self._set_column_schema(column_name, column_schema=column_schema)
+
+    def _tag_custom_perf_metrics(self, view: Union[DatasetProfileView, SegmentedDatasetProfileView]):
+        if isinstance(view, DatasetProfileView):
+            column_names = view.get_columns().keys()
+            for column_name in column_names:
+                for perf_col in KNOWN_CUSTOM_PERFORMANCE_METRICS:
+                    if column_name.startswith(perf_col):
+                        metric = KNOWN_CUSTOM_PERFORMANCE_METRICS[perf_col]
+                        self.tag_custom_performance_column(column_name, default_metric=metric)
 
     def _do_get_feature_weights(self):
         """Get latest version for the feature weights for the specified dataset
 
         Returns
         -------
             Response of the GET request, with segmentWeights and metadata.
```

### Comparing `whylogs-1.4.0/whylogs/api/writer/whylabs_estimation_result_writer.py` & `whylogs-1.4.0rc0/whylogs/api/writer/whylabs_estimation_result_writer.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/api/writer/whylabs_reference_writer.py` & `whylogs-1.4.0rc0/whylogs/api/writer/whylabs_reference_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,14 @@
 
     @deprecated_alias(profile="file")
     def write(
         self, file: Writable, dest: Optional[str] = None, **kwargs: Any
     ) -> Tuple[bool, Union[str, List[Tuple[bool, str]]]]:
         self.option(**kwargs)
         self._whylabs_client = self._whylabs_client.option(**kwargs)  # type: ignore
-        self._custom_tagging(file)
 
         if isinstance(file, SegmentedResultSet):
             if kwargs.get("zip"):  # TODO: force zip if the number of segemtns is large
                 return self._write_segmented_result_set_zip(file, **kwargs)
             else:
                 return self._write_segmented_result_set(file, **kwargs)
```

### Comparing `whylogs-1.4.0/whylogs/api/writer/whylabs_transaction_writer.py` & `whylogs-1.4.0rc0/whylogs/api/writer/whylabs_transaction_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             return False, f"Transaction {self.transaction_id} was aborted"
 
         transaction_id = kwargs.get("transaction_id") or self.transaction_id
         if not transaction_id:
             raise ValueError("Missing transaction id")
 
         self._whylabs_client = self._whylabs_client.option(**kwargs)  # type: ignore
-        self._custom_tagging(file)
+
         if isinstance(file, SegmentedResultSet):
             return self._write_segmented_result_set(file, **kwargs)
 
         # file represents a single profile/segment, extract a view of it
         view = self._get_view_of_writable(file)
         return self._write_view(view, **kwargs)
```

### Comparing `whylogs-1.4.0/whylogs/api/writer/writer.py` & `whylogs-1.4.0rc0/whylogs/api/writer/writer.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/context/version.py` & `whylogs-1.4.0rc0/whylogs/context/version.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/__init__.py` & `whylogs-1.4.0rc0/whylogs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/column_profile.py` & `whylogs-1.4.0rc0/whylogs/core/column_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/configs.py` & `whylogs-1.4.0rc0/whylogs/core/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/constraints/factories/__init__.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/constraints/factories/cardinality_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/cardinality_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/constraints/factories/condition_counts.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/constraints/factories/count_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/constraints/factories/distribution_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/constraints/factories/frequent_items.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/constraints/factories/multi_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/constraints/factories/types_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/constraints/metric_constraints.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/metric_constraints.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/dataset_profile.py` & `whylogs-1.4.0rc0/whylogs/core/dataset_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/datatypes.py` & `whylogs-1.4.0rc0/whylogs/core/datatypes.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/errors.py` & `whylogs-1.4.0rc0/whylogs/core/errors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/feature_weights.py` & `whylogs-1.4.0rc0/whylogs/core/feature_weights.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/input_resolver.py` & `whylogs-1.4.0rc0/whylogs/core/input_resolver.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/metadata.py` & `whylogs-1.4.0rc0/whylogs/core/metadata.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/metric_getters.py` & `whylogs-1.4.0rc0/whylogs/core/metric_getters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/metrics/__init__.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/metrics/aggregators.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/aggregators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/metrics/column_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/column_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/metrics/compound_metric.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/compound_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/metrics/condition_count_metric.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/condition_count_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/metrics/decorators.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/decorators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/metrics/deserializers.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/deserializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/metrics/maths.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/maths.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/metrics/metric_components.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/metric_components.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/metrics/metrics.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/metrics/multimetric.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/multimetric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/metrics/serializers.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/serializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/metrics/unicode_range.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/unicode_range.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/model_performance_metrics/confusion_matrix.py` & `whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/model_performance_metrics/model_performance_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/model_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/model_performance_metrics/regression_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/predicate_parser.py` & `whylogs-1.4.0rc0/whylogs/core/predicate_parser.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/preprocessing.py` & `whylogs-1.4.0rc0/whylogs/core/preprocessing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/proto/v0/v0_constraints_pb2.py` & `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/proto/v0/v0_constraints_pb2.pyi` & `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_constraints_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/proto/v0/v0_messages_pb2.py` & `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/proto/v0/v0_messages_pb2.pyi` & `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/proto/v0/v0_summaries_pb2.py` & `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_summaries_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/proto/v0/v0_summaries_pb2.pyi` & `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_summaries_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/proto/whylogs_messages_pb2.py` & `whylogs-1.4.0rc0/whylogs/core/proto/whylogs_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/proto/whylogs_messages_pb2.pyi` & `whylogs-1.4.0rc0/whylogs/core/proto/whylogs_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/relations.py` & `whylogs-1.4.0rc0/whylogs/core/relations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/resolvers.py` & `whylogs-1.4.0rc0/whylogs/core/resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/schema.py` & `whylogs-1.4.0rc0/whylogs/core/schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/segmentation_partition.py` & `whylogs-1.4.0rc0/whylogs/core/segmentation_partition.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/specialized_resolvers.py` & `whylogs-1.4.0rc0/whylogs/core/specialized_resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/stubs.py` & `whylogs-1.4.0rc0/whylogs/core/stubs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/utils/protobuf_utils.py` & `whylogs-1.4.0rc0/whylogs/core/utils/protobuf_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/utils/stats_calculations.py` & `whylogs-1.4.0rc0/whylogs/core/utils/stats_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/utils/utils.py` & `whylogs-1.4.0rc0/whylogs/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/validators/condition_validator.py` & `whylogs-1.4.0rc0/whylogs/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/validators/validator.py` & `whylogs-1.4.0rc0/whylogs/core/validators/validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/view/column_profile_view.py` & `whylogs-1.4.0rc0/whylogs/core/view/column_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/view/dataset_profile_view.py` & `whylogs-1.4.0rc0/whylogs/core/view/dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/core/view/segmented_dataset_profile_view.py` & `whylogs-1.4.0rc0/whylogs/core/view/segmented_dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/datasets/base.py` & `whylogs-1.4.0rc0/whylogs/datasets/base.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/datasets/configs.py` & `whylogs-1.4.0rc0/whylogs/datasets/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/datasets/descr/ecommerce.rst` & `whylogs-1.4.0rc0/whylogs/datasets/descr/ecommerce.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/datasets/descr/employee.rst` & `whylogs-1.4.0rc0/whylogs/datasets/descr/employee.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/datasets/descr/weather.rst` & `whylogs-1.4.0rc0/whylogs/datasets/descr/weather.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/datasets/ecommerce.py` & `whylogs-1.4.0rc0/whylogs/datasets/ecommerce.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/datasets/employee.py` & `whylogs-1.4.0rc0/whylogs/datasets/employee.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/datasets/utils.py` & `whylogs-1.4.0rc0/whylogs/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/datasets/weather.py` & `whylogs-1.4.0rc0/whylogs/datasets/weather.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/api/logger/__init__.py` & `whylogs-1.4.0rc0/whylogs/experimental/api/logger/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import math
-from typing import List, Optional, Set, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 from whylogs.api.logger import log
-from whylogs.api.logger.result_set import SegmentedResultSet, ViewResultSet
+from whylogs.api.logger.result_set import ViewResultSet
 from whylogs.core import DatasetSchema
 from whylogs.core.stubs import np, pd
 
 diagnostic_logger = logging.getLogger(__name__)
 
 
 def _convert_to_int_if_bool(data: pd.core.frame.DataFrame, *columns: str) -> pd.core.frame.DataFrame:
@@ -131,34 +131,14 @@
     return averages
 
 
 def _all_strings(data: pd.Series) -> bool:
     return all([all([isinstance(y, str) for y in x]) for x in data])
 
 
-def _get_segment_columns(schema: DatasetSchema, data: pd.DataFrame) -> List[str]:
-    columns: Set[str] = set()
-    for partition_name, partition in schema.segments.items():
-        if partition.filter:
-            raise ValueError("Filters are not supported for segmented ranking metrics")  # Filters are deprecated
-        if partition.mapper:
-            columns = columns.union(set(partition.mapper.col_names))
-
-    return list(columns)
-
-
-def _drop_non_output_columns(result: SegmentedResultSet, keep_columns: Set[str]) -> SegmentedResultSet:
-    for partition in result._segments.values():
-        for segment in partition.values():
-            for column in {column for column in segment._columns.keys() if column not in keep_columns}:
-                segment._columns.pop(column)
-
-    return result
-
-
 def log_batch_ranking_metrics(
     data: pd.core.frame.DataFrame,
     prediction_column: Optional[str] = None,
     target_column: Optional[str] = None,
     score_column: Optional[str] = None,
     k: Optional[int] = None,
     schema: Union[DatasetSchema, None] = None,
@@ -346,29 +326,22 @@
         formatted_data, target_column, prediction_column, convert_non_numeric=convert_non_numeric, k=k  # type: ignore
     )
 
     output_data["norm_dis_cumul_gain" + ("_k_" + str(k) if k else "")] = formatted_data.apply(
         row_wise_functions.calculate_row_ndcg, args=(k,), axis=1
     )
     output_data[f"sum_gain_k_{k}"] = formatted_data.apply(row_wise_functions.sum_gains, args=(k,), axis=1)
+    hit_ratio = formatted_data["count_at_k"].apply(lambda x: bool(x)).sum() / len(formatted_data)
     mrr = (1 / formatted_data["top_rank"]).replace([np.inf, np.nan], 0)
     output_data["reciprocal_rank"] = mrr
-
-    if schema and schema.segments:
-        original_columns = set(data.columns)
-        for column in set(formatted_data.columns):
-            if column not in original_columns:
-                formatted_data = formatted_data.drop(column, axis=1)
-
-        if log_full_data:
-            return log(pandas=pd.concat([formatted_data, output_data], axis=1), schema=schema)
-        else:
-            segment_columns = _get_segment_columns(schema, formatted_data)
-            segmentable_data = formatted_data[segment_columns]
-            result = log(pandas=pd.concat([segmentable_data, output_data], axis=1), schema=schema)
-            result = _drop_non_output_columns(result, set(output_data.columns))
-            return result
-
     result = log(pandas=output_data, schema=schema)
+    result = result.merge(
+        log(
+            row={
+                "accuracy" + ("_k_" + str(k) if k else ""): hit_ratio,
+            },
+            schema=schema,
+        )
+    )
     if log_full_data:
         result = result.merge(log(pandas=data, schema=schema))
     return result
```

### Comparing `whylogs-1.4.0/whylogs/experimental/constraints_generation/__init__.py` & `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/constraints_generation/condition_counts.py` & `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/constraints_generation/count_metrics.py` & `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/constraints_generation/distribution_metrics.py` & `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/constraints_generation/frequent_items.py` & `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/constraints_generation/multi_metrics.py` & `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/constraints_generation/types_metrics.py` & `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/core/metrics/udf_metric.py` & `whylogs-1.4.0rc0/whylogs/experimental/core/metrics/udf_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/core/udf_schema.py` & `whylogs-1.4.0rc0/whylogs/experimental/core/udf_schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/core/validators/condition_validator.py` & `whylogs-1.4.0rc0/whylogs/experimental/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/core/validators/validator.py` & `whylogs-1.4.0rc0/whylogs/experimental/core/validators/validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/extras/embedding_metric.py` & `whylogs-1.4.0rc0/whylogs/experimental/extras/embedding_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/extras/matrix_component.py` & `whylogs-1.4.0rc0/whylogs/experimental/extras/matrix_component.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/extras/nlp_metric.py` & `whylogs-1.4.0rc0/whylogs/experimental/extras/nlp_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/performance_estimation/estimation_results.py` & `whylogs-1.4.0rc0/whylogs/experimental/performance_estimation/estimation_results.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/performance_estimation/estimators.py` & `whylogs-1.4.0rc0/whylogs/experimental/performance_estimation/estimators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/experimental/preprocess/embeddings/selectors.py` & `whylogs-1.4.0rc0/whylogs/experimental/preprocess/embeddings/selectors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/extras/image_metric.py` & `whylogs-1.4.0rc0/whylogs/extras/image_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/migration/converters.py` & `whylogs-1.4.0rc0/whylogs/migration/converters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/migration/uncompound.py` & `whylogs-1.4.0rc0/whylogs/migration/uncompound.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/drift/column_drift_algorithms.py` & `whylogs-1.4.0rc0/whylogs/viz/drift/column_drift_algorithms.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/drift/configs.py` & `whylogs-1.4.0rc0/whylogs/viz/drift/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/enums/enums.py` & `whylogs-1.4.0rc0/whylogs/viz/enums/enums.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/extensions/reports/html_report.py` & `whylogs-1.4.0rc0/whylogs/viz/extensions/reports/html_report.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/extensions/reports/profile_summary.py` & `whylogs-1.4.0rc0/whylogs/viz/extensions/reports/profile_summary.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/extensions/reports/summary_drift.py` & `whylogs-1.4.0rc0/whylogs/viz/extensions/reports/summary_drift.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/css/bootstrap.min.css` & `whylogs-1.4.0rc0/whylogs/viz/html/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/css/whylogs-styles.css` & `whylogs-1.4.0rc0/whylogs/viz/html/css/whylogs-styles.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Bold.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Bold.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Bold.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-BoldItalic.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Italic.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Italic.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Italic.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Medium.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Medium.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Medium.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-MediumItalic.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Regular.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Regular.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-Regular.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-SemiBold.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-SemiBold.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-SemiBold.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/images/placement-chart.png` & `whylogs-1.4.0rc0/whylogs/viz/html/images/placement-chart.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/images/whylabs-favicon.png` & `whylogs-1.4.0rc0/whylogs/viz/html/images/whylabs-favicon.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/js/d3.min.js` & `whylogs-1.4.0rc0/whylogs/viz/html/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/js/handlebars.js` & `whylogs-1.4.0rc0/whylogs/viz/html/js/handlebars.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/js/jquery-3.6.0.min.js` & `whylogs-1.4.0rc0/whylogs/viz/html/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/js/whylogs-script.js` & `whylogs-1.4.0rc0/whylogs/viz/html/js/whylogs-script.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/templates/index-hbs-library-all-in.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-library-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/templates/index-hbs.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/html/templates/index.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/notebook_profile_viz.py` & `whylogs-1.4.0rc0/whylogs/viz/notebook_profile_viz.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/utils/descriptive_stats.py` & `whylogs-1.4.0rc0/whylogs/viz/utils/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/utils/drift_calculations.py` & `whylogs-1.4.0rc0/whylogs/viz/utils/drift_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/utils/frequent_items_calculations.py` & `whylogs-1.4.0rc0/whylogs/viz/utils/frequent_items_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/utils/histogram_calculations.py` & `whylogs-1.4.0rc0/whylogs/viz/utils/histogram_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/utils/html_template_utils.py` & `whylogs-1.4.0rc0/whylogs/viz/utils/html_template_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/utils/profile_viz_calculations.py` & `whylogs-1.4.0rc0/whylogs/viz/utils/profile_viz_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/whylogs/viz/utils/quantile_stats.py` & `whylogs-1.4.0rc0/whylogs/viz/utils/quantile_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.4.0/PKG-INFO` & `whylogs-1.4.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,438 +1,438 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7768 796c  : 2.1.Name: whyl
 00000020: 6f67 730a 5665 7273 696f 6e3a 2031 2e34  ogs.Version: 1.4
-00000030: 2e30 0a53 756d 6d61 7279 3a20 5072 6f66  .0.Summary: Prof
-00000040: 696c 6520 616e 6420 6d6f 6e69 746f 7220  ile and monitor 
-00000050: 796f 7572 204d 4c20 6461 7461 2070 6970  your ML data pip
-00000060: 656c 696e 6520 656e 642d 746f 2d65 6e64  eline end-to-end
-00000070: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
-00000080: 733a 2f2f 646f 6373 2e77 6879 6c61 6273  s://docs.whylabs
-00000090: 2e61 690a 4c69 6365 6e73 653a 2041 7061  .ai.License: Apa
-000000a0: 6368 652d 322e 300a 4175 7468 6f72 3a20  che-2.0.Author: 
-000000b0: 5768 794c 6162 732e 6169 0a41 7574 686f  WhyLabs.ai.Autho
-000000c0: 722d 656d 6169 6c3a 2073 7570 706f 7274  r-email: support
-000000d0: 4077 6879 6c61 6273 2e61 690a 5265 7175  @whylabs.ai.Requ
-000000e0: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
-000000f0: 2e37 2e31 2c3c 340a 436c 6173 7369 6669  .7.1,<4.Classifi
-00000100: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
-00000110: 5349 2041 7070 726f 7665 6420 3a3a 2041  SI Approved :: A
-00000120: 7061 6368 6520 536f 6674 7761 7265 204c  pache Software L
-00000130: 6963 656e 7365 0a43 6c61 7373 6966 6965  icense.Classifie
-00000140: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000150: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000160: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
-00000170: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000180: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000190: 6e20 3a3a 2033 2e38 0a43 6c61 7373 6966  n :: 3.8.Classif
-000001a0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-000001b0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000001c0: 686f 6e20 3a3a 2033 2e39 0a43 6c61 7373  hon :: 3.9.Class
-000001d0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-000001e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001f0: 7974 686f 6e20 3a3a 2033 2e31 300a 436c  ython :: 3.10.Cl
-00000200: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000210: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000220: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
-00000230: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000240: 2061 6c6c 0a50 726f 7669 6465 732d 4578   all.Provides-Ex
-00000250: 7472 613a 2064 6174 6173 6574 730a 5072  tra: datasets.Pr
-00000260: 6f76 6964 6573 2d45 7874 7261 3a20 646f  ovides-Extra: do
-00000270: 6373 0a50 726f 7669 6465 732d 4578 7472  cs.Provides-Extr
-00000280: 613a 2065 6d62 6564 6469 6e67 730a 5072  a: embeddings.Pr
-00000290: 6f76 6964 6573 2d45 7874 7261 3a20 6675  ovides-Extra: fu
-000002a0: 6775 650a 5072 6f76 6964 6573 2d45 7874  gue.Provides-Ext
-000002b0: 7261 3a20 6763 730a 5072 6f76 6964 6573  ra: gcs.Provides
-000002c0: 2d45 7874 7261 3a20 696d 6167 650a 5072  -Extra: image.Pr
-000002d0: 6f76 6964 6573 2d45 7874 7261 3a20 6d6c  ovides-Extra: ml
-000002e0: 666c 6f77 0a50 726f 7669 6465 732d 4578  flow.Provides-Ex
-000002f0: 7472 613a 2070 726f 630a 5072 6f76 6964  tra: proc.Provid
-00000300: 6573 2d45 7874 7261 3a20 7072 6f63 2d6d  es-Extra: proc-m
-00000310: 700a 5072 6f76 6964 6573 2d45 7874 7261  p.Provides-Extra
-00000320: 3a20 7333 0a50 726f 7669 6465 732d 4578  : s3.Provides-Ex
-00000330: 7472 613a 2073 7061 726b 0a50 726f 7669  tra: spark.Provi
-00000340: 6465 732d 4578 7472 613a 2076 697a 0a52  des-Extra: viz.R
-00000350: 6571 7569 7265 732d 4469 7374 3a20 5069  equires-Dist: Pi
-00000360: 6c6c 6f77 2028 3e3d 392e 322e 302c 3c31  llow (>=9.2.0,<1
-00000370: 302e 302e 3029 203b 2065 7874 7261 203d  0.0.0) ; extra =
-00000380: 3d20 2276 697a 2220 6f72 2065 7874 7261  = "viz" or extra
-00000390: 203d 3d20 2269 6d61 6765 2220 6f72 2065   == "image" or e
-000003a0: 7874 7261 203d 3d20 2261 6c6c 220a 5265  xtra == "all".Re
-000003b0: 7175 6972 6573 2d44 6973 743a 2062 6f74  quires-Dist: bot
-000003c0: 6f33 2028 3e3d 312e 3232 2e31 332c 3c32  o3 (>=1.22.13,<2
-000003d0: 2e30 2e30 2920 3b20 6578 7472 6120 3d3d  .0.0) ; extra ==
-000003e0: 2022 7333 2220 6f72 2065 7874 7261 203d   "s3" or extra =
-000003f0: 3d20 2261 6c6c 220a 5265 7175 6972 6573  = "all".Requires
-00000400: 2d44 6973 743a 2066 6173 7465 722d 6669  -Dist: faster-fi
-00000410: 666f 2028 3e3d 312e 342e 352c 3c32 2e30  fo (>=1.4.5,<2.0
-00000420: 2e30 2920 3b20 6578 7472 6120 3d3d 2022  .0) ; extra == "
-00000430: 7072 6f63 2220 6f72 2065 7874 7261 203d  proc" or extra =
-00000440: 3d20 2261 6c6c 220a 5265 7175 6972 6573  = "all".Requires
-00000450: 2d44 6973 743a 2066 7567 7565 2028 3e3d  -Dist: fugue (>=
-00000460: 302e 382e 312c 3c30 2e39 2e30 2920 3b20  0.8.1,<0.9.0) ; 
-00000470: 6578 7472 6120 3d3d 2022 6675 6775 6522  extra == "fugue"
-00000480: 206f 7220 6578 7472 6120 3d3d 2022 616c   or extra == "al
-00000490: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
-000004a0: 3a20 6675 726f 2028 3e3d 3230 3232 2e33  : furo (>=2022.3
-000004b0: 2e34 2c3c 3230 3233 2e30 2e30 2920 3b20  .4,<2023.0.0) ; 
-000004c0: 6578 7472 6120 3d3d 2022 646f 6373 220a  extra == "docs".
-000004d0: 5265 7175 6972 6573 2d44 6973 743a 2067  Requires-Dist: g
-000004e0: 6f6f 676c 652d 636c 6f75 642d 7374 6f72  oogle-cloud-stor
-000004f0: 6167 6520 283e 3d32 2e35 2e30 2c3c 332e  age (>=2.5.0,<3.
-00000500: 302e 3029 203b 2065 7874 7261 203d 3d20  0.0) ; extra == 
-00000510: 2267 6373 2220 6f72 2065 7874 7261 203d  "gcs" or extra =
-00000520: 3d20 2261 6c6c 220a 5265 7175 6972 6573  = "all".Requires
-00000530: 2d44 6973 743a 2069 6d70 6f72 746c 6962  -Dist: importlib
-00000540: 2d6d 6574 6164 6174 6120 283c 342e 3329  -metadata (<4.3)
-00000550: 203b 2070 7974 686f 6e5f 7665 7273 696f   ; python_versio
-00000560: 6e20 3c20 2233 2e38 220a 5265 7175 6972  n < "3.8".Requir
-00000570: 6573 2d44 6973 743a 2069 7079 7468 6f6e  es-Dist: ipython
-00000580: 203b 2065 7874 7261 203d 3d20 2276 697a   ; extra == "viz
-00000590: 2220 6f72 2065 7874 7261 203d 3d20 2261  " or extra == "a
-000005a0: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
-000005b0: 743a 2069 7079 7468 6f6e 5f67 656e 7574  t: ipython_genut
-000005c0: 696c 7320 283e 3d30 2e32 2e30 2c3c 302e  ils (>=0.2.0,<0.
-000005d0: 332e 3029 203b 2065 7874 7261 203d 3d20  3.0) ; extra == 
-000005e0: 2264 6f63 7322 0a52 6571 7569 7265 732d  "docs".Requires-
-000005f0: 4469 7374 3a20 6d6c 666c 6f77 2d73 6b69  Dist: mlflow-ski
-00000600: 6e6e 7920 283c 322e 302e 3129 203b 2028  nny (<2.0.1) ; (
-00000610: 7079 7468 6f6e 5f76 6572 7369 6f6e 203c  python_version <
-00000620: 2022 332e 3822 2920 616e 6420 2865 7874   "3.8") and (ext
-00000630: 7261 203d 3d20 226d 6c66 6c6f 7722 206f  ra == "mlflow" o
-00000640: 7220 6578 7472 6120 3d3d 2022 616c 6c22  r extra == "all"
-00000650: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000660: 206d 6c66 6c6f 772d 736b 696e 6e79 2028   mlflow-skinny (
-00000670: 3e3d 322e 352e 302c 3c33 2e30 2e30 2920  >=2.5.0,<3.0.0) 
-00000680: 3b20 2870 7974 686f 6e5f 7665 7273 696f  ; (python_versio
-00000690: 6e20 3e3d 2022 332e 3822 2920 616e 6420  n >= "3.8") and 
-000006a0: 2865 7874 7261 203d 3d20 226d 6c66 6c6f  (extra == "mlflo
-000006b0: 7722 206f 7220 6578 7472 6120 3d3d 2022  w" or extra == "
-000006c0: 616c 6c22 290a 5265 7175 6972 6573 2d44  all").Requires-D
-000006d0: 6973 743a 206d 7973 742d 7061 7273 6572  ist: myst-parser
-000006e0: 5b73 7068 696e 785d 2028 3e3d 302e 3137  [sphinx] (>=0.17
-000006f0: 2e32 2c3c 302e 3138 2e30 2920 3b20 6578  .2,<0.18.0) ; ex
-00000700: 7472 6120 3d3d 2022 646f 6373 220a 5265  tra == "docs".Re
-00000710: 7175 6972 6573 2d44 6973 743a 206e 6263  quires-Dist: nbc
-00000720: 6f6e 7665 7274 2028 3e3d 372e 302e 302c  onvert (>=7.0.0,
-00000730: 3c38 2e30 2e30 2920 3b20 6578 7472 6120  <8.0.0) ; extra 
-00000740: 3d3d 2022 646f 6373 220a 5265 7175 6972  == "docs".Requir
-00000750: 6573 2d44 6973 743a 206e 6273 7068 696e  es-Dist: nbsphin
-00000760: 7820 283e 3d30 2e38 2e39 2c3c 302e 392e  x (>=0.8.9,<0.9.
-00000770: 3029 203b 2065 7874 7261 203d 3d20 2264  0) ; extra == "d
-00000780: 6f63 7322 0a52 6571 7569 7265 732d 4469  ocs".Requires-Di
-00000790: 7374 3a20 6e75 6d70 7920 283e 3d31 2e32  st: numpy (>=1.2
-000007a0: 332e 3229 203b 2028 7079 7468 6f6e 5f76  3.2) ; (python_v
-000007b0: 6572 7369 6f6e 203e 3d20 2233 2e31 3122  ersion >= "3.11"
-000007c0: 2920 616e 6420 2865 7874 7261 203d 3d20  ) and (extra == 
-000007d0: 2276 697a 2220 6f72 2065 7874 7261 203d  "viz" or extra =
-000007e0: 3d20 2269 6d61 6765 2220 6f72 2065 7874  = "image" or ext
-000007f0: 7261 203d 3d20 2265 6d62 6564 6469 6e67  ra == "embedding
-00000800: 7322 206f 7220 6578 7472 6120 3d3d 2022  s" or extra == "
-00000810: 616c 6c22 290a 5265 7175 6972 6573 2d44  all").Requires-D
-00000820: 6973 743a 206e 756d 7079 203b 2028 7079  ist: numpy ; (py
-00000830: 7468 6f6e 5f76 6572 7369 6f6e 203c 2022  thon_version < "
-00000840: 332e 3131 2229 2061 6e64 2028 6578 7472  3.11") and (extr
-00000850: 6120 3d3d 2022 7669 7a22 206f 7220 6578  a == "viz" or ex
-00000860: 7472 6120 3d3d 2022 696d 6167 6522 206f  tra == "image" o
-00000870: 7220 6578 7472 6120 3d3d 2022 656d 6265  r extra == "embe
-00000880: 6464 696e 6773 2220 6f72 2065 7874 7261  ddings" or extra
-00000890: 203d 3d20 2261 6c6c 2229 0a52 6571 7569   == "all").Requi
-000008a0: 7265 732d 4469 7374 3a20 6f72 6a73 6f6e  res-Dist: orjson
-000008b0: 2028 3e3d 332e 382e 3130 2c3c 342e 302e   (>=3.8.10,<4.0.
-000008c0: 3029 203b 2065 7874 7261 203d 3d20 2270  0) ; extra == "p
-000008d0: 726f 6322 206f 7220 6578 7472 6120 3d3d  roc" or extra ==
-000008e0: 2022 7072 6f63 2d6d 7022 206f 7220 6578   "proc-mp" or ex
-000008f0: 7472 6120 3d3d 2022 616c 6c22 0a52 6571  tra == "all".Req
-00000900: 7569 7265 732d 4469 7374 3a20 7061 6e64  uires-Dist: pand
-00000910: 6173 203b 2065 7874 7261 203d 3d20 2264  as ; extra == "d
-00000920: 6174 6173 6574 7322 206f 7220 6578 7472  atasets" or extr
-00000930: 6120 3d3d 2022 7072 6f63 2220 6f72 2065  a == "proc" or e
-00000940: 7874 7261 203d 3d20 2270 726f 632d 6d70  xtra == "proc-mp
-00000950: 2220 6f72 2065 7874 7261 203d 3d20 2261  " or extra == "a
-00000960: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
-00000970: 743a 2070 6c61 7466 6f72 6d64 6972 7320  t: platformdirs 
-00000980: 283e 3d33 2e35 2e30 2c3c 342e 302e 3029  (>=3.5.0,<4.0.0)
-00000990: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000009a0: 7072 6f74 6f62 7566 2028 3e3d 332e 3139  protobuf (>=3.19
-000009b0: 2e34 290a 5265 7175 6972 6573 2d44 6973  .4).Requires-Dis
-000009c0: 743a 2070 7961 7272 6f77 2028 3e3d 382e  t: pyarrow (>=8.
-000009d0: 302e 302c 3c31 3329 203b 2065 7874 7261  0.0,<13) ; extra
-000009e0: 203d 3d20 2273 7061 726b 2220 6f72 2065   == "spark" or e
-000009f0: 7874 7261 203d 3d20 2261 6c6c 220a 5265  xtra == "all".Re
-00000a00: 7175 6972 6573 2d44 6973 743a 2070 7962  quires-Dist: pyb
-00000a10: 6172 7333 2028 3e3d 302e 392c 3c30 2e31  ars3 (>=0.9,<0.1
-00000a20: 3029 203b 2065 7874 7261 203d 3d20 2276  0) ; extra == "v
-00000a30: 697a 2220 6f72 2065 7874 7261 203d 3d20  iz" or extra == 
-00000a40: 2261 6c6c 220a 5265 7175 6972 6573 2d44  "all".Requires-D
-00000a50: 6973 743a 2070 7973 7061 726b 2028 3e3d  ist: pyspark (>=
-00000a60: 332e 302e 302c 3c34 2e30 2e30 2920 3b20  3.0.0,<4.0.0) ; 
-00000a70: 6578 7472 6120 3d3d 2022 7370 6172 6b22  extra == "spark"
-00000a80: 206f 7220 6578 7472 6120 3d3d 2022 616c   or extra == "al
-00000a90: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
-00000aa0: 3a20 7265 7175 6573 7473 2028 3e3d 322e  : requests (>=2.
-00000ab0: 3237 2c3c 332e 3029 0a52 6571 7569 7265  27,<3.0).Require
-00000ac0: 732d 4469 7374 3a20 7363 696b 6974 2d6c  s-Dist: scikit-l
-00000ad0: 6561 726e 2028 3e3d 312e 302e 322c 3c32  earn (>=1.0.2,<2
-00000ae0: 2e30 2e30 2920 3b20 2870 7974 686f 6e5f  .0.0) ; (python_
-00000af0: 7665 7273 696f 6e20 3c20 2233 2e31 3122  version < "3.11"
-00000b00: 2920 616e 6420 2865 7874 7261 203d 3d20  ) and (extra == 
-00000b10: 2265 6d62 6564 6469 6e67 7322 206f 7220  "embeddings" or 
-00000b20: 6578 7472 6120 3d3d 2022 616c 6c22 290a  extra == "all").
-00000b30: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
-00000b40: 6369 6b69 742d 6c65 6172 6e20 283e 3d31  cikit-learn (>=1
-00000b50: 2e31 2e32 2c3c 3229 203b 2028 7079 7468  .1.2,<2) ; (pyth
-00000b60: 6f6e 5f76 6572 7369 6f6e 203e 3d20 2233  on_version >= "3
-00000b70: 2e31 3122 2920 616e 6420 2865 7874 7261  .11") and (extra
-00000b80: 203d 3d20 2265 6d62 6564 6469 6e67 7322   == "embeddings"
-00000b90: 206f 7220 6578 7472 6120 3d3d 2022 616c   or extra == "al
-00000ba0: 6c22 290a 5265 7175 6972 6573 2d44 6973  l").Requires-Dis
-00000bb0: 743a 2073 6369 7079 2028 3e3d 312e 3529  t: scipy (>=1.5)
-00000bc0: 203b 2028 7079 7468 6f6e 5f76 6572 7369   ; (python_versi
-00000bd0: 6f6e 203c 2022 332e 3131 2229 2061 6e64  on < "3.11") and
-00000be0: 2028 6578 7472 6120 3d3d 2022 7669 7a22   (extra == "viz"
-00000bf0: 206f 7220 6578 7472 6120 3d3d 2022 616c   or extra == "al
-00000c00: 6c22 290a 5265 7175 6972 6573 2d44 6973  l").Requires-Dis
-00000c10: 743a 2073 6369 7079 2028 3e3d 312e 392e  t: scipy (>=1.9.
-00000c20: 3229 203b 2028 7079 7468 6f6e 5f76 6572  2) ; (python_ver
-00000c30: 7369 6f6e 203e 3d20 2233 2e31 3122 2920  sion >= "3.11") 
-00000c40: 616e 6420 2865 7874 7261 203d 3d20 2276  and (extra == "v
-00000c50: 697a 2220 6f72 2065 7874 7261 203d 3d20  iz" or extra == 
-00000c60: 2261 6c6c 2229 0a52 6571 7569 7265 732d  "all").Requires-
-00000c70: 4469 7374 3a20 7370 6869 6e78 203b 2065  Dist: sphinx ; e
-00000c80: 7874 7261 203d 3d20 2264 6f63 7322 0a52  xtra == "docs".R
-00000c90: 6571 7569 7265 732d 4469 7374 3a20 7370  equires-Dist: sp
-00000ca0: 6869 6e78 2d61 7574 6f61 7069 203b 2065  hinx-autoapi ; e
-00000cb0: 7874 7261 203d 3d20 2264 6f63 7322 0a52  xtra == "docs".R
-00000cc0: 6571 7569 7265 732d 4469 7374 3a20 7370  equires-Dist: sp
-00000cd0: 6869 6e78 2d61 7574 6f62 7569 6c64 2028  hinx-autobuild (
-00000ce0: 3e3d 3230 3231 2e33 2e31 342c 3c32 3032  >=2021.3.14,<202
-00000cf0: 322e 302e 3029 203b 2065 7874 7261 203d  2.0.0) ; extra =
-00000d00: 3d20 2264 6f63 7322 0a52 6571 7569 7265  = "docs".Require
-00000d10: 732d 4469 7374 3a20 7370 6869 6e78 2d63  s-Dist: sphinx-c
-00000d20: 6f70 7962 7574 746f 6e20 283e 3d30 2e35  opybutton (>=0.5
-00000d30: 2e30 2c3c 302e 362e 3029 203b 2065 7874  .0,<0.6.0) ; ext
-00000d40: 7261 203d 3d20 2264 6f63 7322 0a52 6571  ra == "docs".Req
-00000d50: 7569 7265 732d 4469 7374 3a20 7370 6869  uires-Dist: sphi
-00000d60: 6e78 2d69 6e6c 696e 652d 7461 6273 203b  nx-inline-tabs ;
-00000d70: 2028 7079 7468 6f6e 5f76 6572 7369 6f6e   (python_version
-00000d80: 203e 3d20 2233 2e38 2220 616e 6420 7079   >= "3.8" and py
-00000d90: 7468 6f6e 5f76 6572 7369 6f6e 203c 2022  thon_version < "
-00000da0: 3422 2920 616e 6420 2865 7874 7261 203d  4") and (extra =
-00000db0: 3d20 2264 6f63 7322 290a 5265 7175 6972  = "docs").Requir
-00000dc0: 6573 2d44 6973 743a 2073 7068 696e 7865  es-Dist: sphinxe
-00000dd0: 7874 2d6f 7065 6e67 7261 7068 2028 3e3d  xt-opengraph (>=
-00000de0: 302e 362e 332c 3c30 2e37 2e30 2920 3b20  0.6.3,<0.7.0) ; 
-00000df0: 6578 7472 6120 3d3d 2022 646f 6373 220a  extra == "docs".
-00000e00: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
-00000e10: 7970 6573 2d72 6571 7565 7374 7320 283e  ypes-requests (>
-00000e20: 3d32 2e33 302e 302e 302c 3c33 2e30 2e30  =2.30.0.0,<3.0.0
-00000e30: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
-00000e40: 743a 2074 7970 696e 672d 6578 7465 6e73  t: typing-extens
-00000e50: 696f 6e73 2028 3e3d 332e 3130 2920 3b20  ions (>=3.10) ; 
-00000e60: 7079 7468 6f6e 5f76 6572 7369 6f6e 203c  python_version <
-00000e70: 2022 3422 0a52 6571 7569 7265 732d 4469   "4".Requires-Di
-00000e80: 7374 3a20 7768 796c 6162 732d 636c 6965  st: whylabs-clie
-00000e90: 6e74 2028 3e3d 302e 362e 322c 3c30 2e37  nt (>=0.6.2,<0.7
-00000ea0: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
-00000eb0: 743a 2077 6879 6c6f 6773 2d73 6b65 7463  t: whylogs-sketc
-00000ec0: 6869 6e67 2028 3e3d 332e 342e 312e 6465  hing (>=3.4.1.de
-00000ed0: 7633 290a 4465 7363 7269 7074 696f 6e2d  v3).Description-
-00000ee0: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
-00000ef0: 7874 2f6d 6172 6b64 6f77 6e0a 0a3c 696d  xt/markdown..<im
-00000f00: 6720 7372 633d 2268 7474 7073 3a2f 2f73  g src="https://s
-00000f10: 7461 7469 632e 7363 6172 662e 7368 2f61  tatic.scarf.sh/a
-00000f20: 2e70 6e67 3f78 2d70 7869 643d 6263 3363  .png?x-pxid=bc3c
-00000f30: 3537 6230 2d39 6136 352d 3439 6665 2d62  57b0-9a65-49fe-b
-00000f40: 3865 612d 6637 3131 6334 6433 3562 3832  8ea-f711c4d35b82
-00000f50: 2220 2f3e 3c70 2061 6c69 676e 3d22 6365  " /><p align="ce
-00000f60: 6e74 6572 223e 0a3c 696d 6720 7372 633d  nter">.<img src=
-00000f70: 2268 7474 7073 3a2f 2f69 2e69 6d67 7572  "https://i.imgur
-00000f80: 2e63 6f6d 2f6e 7633 3367 6f56 2e70 6e67  .com/nv33goV.png
-00000f90: 2220 7769 6474 683d 2233 3525 222f 3e0a  " width="35%"/>.
-00000fa0: 3c2f 6272 3e0a 0a3c 6831 2061 6c69 676e  </br>..<h1 align
-00000fb0: 3d22 6365 6e74 6572 223e 5468 6520 6f70  ="center">The op
-00000fc0: 656e 2073 7461 6e64 6172 6420 666f 7220  en standard for 
-00000fd0: 6461 7461 206c 6f67 6769 6e67 0a0a 203c  data logging.. <
-00000fe0: 2f68 313e 0a20 203c 6833 2061 6c69 676e  /h1>.  <h3 align
-00000ff0: 3d22 6365 6e74 6572 223e 0a20 2020 3c61  ="center">.   <a
-00001000: 2068 7265 663d 2268 7474 7073 3a2f 2f77   href="https://w
-00001010: 6879 6c6f 6773 2e72 6561 6474 6865 646f  hylogs.readthedo
-00001020: 6373 2e69 6f2f 223e 3c62 3e44 6f63 756d  cs.io/"><b>Docum
-00001030: 656e 7461 7469 6f6e 3c2f 623e 3c2f 613e  entation</b></a>
-00001040: 2026 6275 6c6c 3b0a 2020 203c 6120 6872   &bull;.   <a hr
-00001050: 6566 3d22 6874 7470 733a 2f2f 6269 742e  ef="https://bit.
-00001060: 6c79 2f77 6879 6c6f 6773 736c 6163 6b22  ly/whylogsslack"
-00001070: 3e3c 623e 536c 6163 6b20 436f 6d6d 756e  ><b>Slack Commun
-00001080: 6974 793c 2f62 3e3c 2f61 3e20 2662 756c  ity</b></a> &bul
-00001090: 6c3b 0a20 2020 3c61 2068 7265 663d 2268  l;.   <a href="h
-000010a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000010b0: 6d2f 7768 796c 6162 732f 7768 796c 6f67  m/whylabs/whylog
-000010c0: 7323 7079 7468 6f6e 2d71 7569 636b 7374  s#python-quickst
-000010d0: 6172 7422 3e3c 623e 5079 7468 6f6e 2051  art"><b>Python Q
-000010e0: 7569 636b 7374 6172 743c 2f62 3e3c 2f61  uickstart</b></a
-000010f0: 3e20 2662 756c 6c3b 0a20 2020 3c61 2068  > &bull;.   <a h
-00001100: 7265 663d 2268 7474 7073 3a2f 2f77 6879  ref="https://why
-00001110: 6c6f 6773 2e72 6561 6474 6865 646f 6373  logs.readthedocs
-00001120: 2e69 6f2f 656e 2f6c 6174 6573 742f 6578  .io/en/latest/ex
-00001130: 616d 706c 6573 2f69 6e74 6567 7261 7469  amples/integrati
-00001140: 6f6e 732f 7772 6974 6572 732f 5772 6974  ons/writers/Writ
-00001150: 696e 675f 746f 5f57 6879 4c61 6273 2e68  ing_to_WhyLabs.h
-00001160: 746d 6c22 3e3c 623e 5768 794c 6162 7320  tml"><b>WhyLabs 
-00001170: 5175 6963 6b73 7461 7274 3c2f 623e 3c2f  Quickstart</b></
-00001180: 613e 0a20 3c2f 6833 3e0a 0a3c 7020 616c  a>. </h3>..<p al
-00001190: 6967 6e3d 2263 656e 7465 7222 3e0a 3c61  ign="center">.<a
-000011a0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-000011b0: 6974 6875 622e 636f 6d2f 7768 796c 6162  ithub.com/whylab
-000011c0: 732f 7768 796c 6f67 732d 7079 7468 6f6e  s/whylogs-python
-000011d0: 2f62 6c6f 622f 6d61 696e 6c69 6e65 2f4c  /blob/mainline/L
-000011e0: 4943 454e 5345 2220 7461 7267 6574 3d22  ICENSE" target="
-000011f0: 5f62 6c61 6e6b 223e 0a20 2020 203c 696d  _blank">.    <im
-00001200: 6720 7372 633d 2268 7474 703a 2f2f 696d  g src="http://im
-00001210: 672e 7368 6965 6c64 732e 696f 2f3a 6c69  g.shields.io/:li
-00001220: 6365 6e73 652d 4170 6163 6865 2532 3032  cense-Apache%202
-00001230: 2d62 6c75 652e 7376 6722 2061 6c74 3d22  -blue.svg" alt="
-00001240: 4c69 6365 6e73 6522 3e0a 3c2f 613e 0a3c  License">.</a>.<
-00001250: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001260: 6261 6467 652e 6675 7279 2e69 6f2f 7079  badge.fury.io/py
-00001270: 2f77 6879 6c6f 6773 2220 7461 7267 6574  /whylogs" target
-00001280: 3d22 5f62 6c61 6e6b 223e 0a20 2020 203c  ="_blank">.    <
-00001290: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-000012a0: 2f62 6164 6765 2e66 7572 792e 696f 2f70  /badge.fury.io/p
-000012b0: 792f 7768 796c 6f67 732e 7376 6722 2061  y/whylogs.svg" a
-000012c0: 6c74 3d22 5079 5069 2056 6572 7369 6f6e  lt="PyPi Version
-000012d0: 223e 0a3c 2f61 3e0a 3c61 2068 7265 663d  ">.</a>.<a href=
-000012e0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-000012f0: 636f 6d2f 7079 7468 6f6e 2f62 6c61 636b  com/python/black
-00001300: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00001310: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
-00001320: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00001330: 656c 6473 2e69 6f2f 6261 6467 652f 636f  elds.io/badge/co
-00001340: 6465 2532 3073 7479 6c65 2d62 6c61 636b  de%20style-black
-00001350: 2d30 3030 3030 302e 7376 6722 2061 6c74  -000000.svg" alt
-00001360: 3d22 436f 6465 2073 7479 6c65 3a20 626c  ="Code style: bl
-00001370: 6163 6b22 3e0a 3c2f 613e 0a3c 6120 6872  ack">.</a>.<a hr
-00001380: 6566 3d22 6874 7470 733a 2f2f 7065 7079  ef="https://pepy
-00001390: 2e74 6563 682f 7072 6f6a 6563 742f 7768  .tech/project/wh
-000013a0: 796c 6f67 7322 2074 6172 6765 743d 225f  ylogs" target="_
-000013b0: 626c 616e 6b22 3e0a 2020 2020 3c69 6d67  blank">.    <img
-000013c0: 2073 7263 3d22 6874 7470 733a 2f2f 7065   src="https://pe
-000013d0: 7079 2e74 6563 682f 6261 6467 652f 7768  py.tech/badge/wh
-000013e0: 796c 6f67 7322 2061 6c74 3d22 5079 5069  ylogs" alt="PyPi
-000013f0: 2044 6f77 6e6c 6f61 6473 223e 0a3c 2f61   Downloads">.</a
-00001400: 3e0a 3c61 2068 7265 663d 2262 6974 2e6c  >.<a href="bit.l
-00001410: 792f 7768 796c 6f67 7322 2074 6172 6765  y/whylogs" targe
-00001420: 743d 225f 626c 616e 6b22 3e0a 2020 2020  t="_blank">.    
-00001430: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00001440: 2f2f 6769 7468 7562 2e63 6f6d 2f77 6879  //github.com/why
-00001450: 6c61 6273 2f77 6879 6c6f 6773 2d70 7974  labs/whylogs-pyt
-00001460: 686f 6e2f 776f 726b 666c 6f77 732f 7768  hon/workflows/wh
-00001470: 796c 6f67 7325 3230 4349 2f62 6164 6765  ylogs%20CI/badge
-00001480: 2e73 7667 2220 616c 743d 2243 4922 3e0a  .svg" alt="CI">.
-00001490: 3c2f 613e 0a3c 6120 6872 6566 3d22 6874  </a>.<a href="ht
-000014a0: 7470 733a 2f2f 636f 6465 636c 696d 6174  tps://codeclimat
-000014b0: 652e 636f 6d2f 6769 7468 7562 2f77 6879  e.com/github/why
-000014c0: 6c61 6273 2f77 6879 6c6f 6773 2d70 7974  labs/whylogs-pyt
-000014d0: 686f 6e2f 6d61 696e 7461 696e 6162 696c  hon/maintainabil
-000014e0: 6974 7922 2074 6172 6765 743d 225f 626c  ity" target="_bl
-000014f0: 616e 6b22 3e0a 2020 2020 3c69 6d67 2073  ank">.    <img s
-00001500: 7263 3d22 6874 7470 733a 2f2f 6170 692e  rc="https://api.
-00001510: 636f 6465 636c 696d 6174 652e 636f 6d2f  codeclimate.com/
-00001520: 7631 2f62 6164 6765 732f 3434 3266 3663  v1/badges/442f6c
-00001530: 6133 6463 6131 6535 3833 6134 3838 2f6d  a3dca1e583a488/m
-00001540: 6169 6e74 6169 6e61 6269 6c69 7479 2220  aintainability" 
-00001550: 616c 743d 224d 6169 6e74 6169 6e61 6269  alt="Maintainabi
-00001560: 6c69 7479 223e 0a3c 2f61 3e0a 3c2f 703e  lity">.</a>.</p>
-00001570: 0a0a 2323 2057 6861 7420 6973 2077 6879  ..## What is why
-00001580: 6c6f 6773 0a0a 7768 796c 6f67 7320 6973  logs..whylogs is
-00001590: 2061 6e20 6f70 656e 2073 6f75 7263 6520   an open source 
-000015a0: 6c69 6272 6172 7920 666f 7220 6c6f 6767  library for logg
-000015b0: 696e 6720 616e 7920 6b69 6e64 206f 6620  ing any kind of 
-000015c0: 6461 7461 2e20 5769 7468 2077 6879 6c6f  data. With whylo
-000015d0: 6773 2c20 7573 6572 7320 6172 6520 6162  gs, users are ab
-000015e0: 6c65 2074 6f20 6765 6e65 7261 7465 2073  le to generate s
-000015f0: 756d 6d61 7269 6573 206f 6620 7468 6569  ummaries of thei
-00001600: 7220 6461 7461 7365 7473 2028 6361 6c6c  r datasets (call
-00001610: 6564 205f 7768 796c 6f67 7320 7072 6f66  ed _whylogs prof
-00001620: 696c 6573 5f29 2077 6869 6368 2074 6865  iles_) which the
-00001630: 7920 6361 6e20 7573 6520 746f 3a0a 0a31  y can use to:..1
-00001640: 2e20 5472 6163 6b20 6368 616e 6765 7320  . Track changes 
-00001650: 696e 2074 6865 6972 2064 6174 6173 6574  in their dataset
-00001660: 0a32 2e20 4372 6561 7465 205f 6461 7461  .2. Create _data
-00001670: 2063 6f6e 7374 7261 696e 7473 5f20 746f   constraints_ to
-00001680: 206b 6e6f 7720 7768 6574 6865 7220 7468   know whether th
-00001690: 6569 7220 6461 7461 206c 6f6f 6b73 2074  eir data looks t
-000016a0: 6865 2077 6179 2069 7420 7368 6f75 6c64  he way it should
-000016b0: 0a33 2e20 5175 6963 6b6c 7920 7669 7375  .3. Quickly visu
-000016c0: 616c 697a 6520 6b65 7920 7375 6d6d 6172  alize key summar
-000016d0: 7920 7374 6174 6973 7469 6373 2061 626f  y statistics abo
-000016e0: 7574 2074 6865 6972 2064 6174 6173 6574  ut their dataset
-000016f0: 730a 0a54 6865 7365 2074 6872 6565 2066  s..These three f
-00001700: 756e 6374 696f 6e61 6c69 7469 6573 2065  unctionalities e
-00001710: 6e61 626c 6520 6120 7661 7269 6574 7920  nable a variety 
-00001720: 6f66 2075 7365 2063 6173 6573 2066 6f72  of use cases for
-00001730: 2064 6174 6120 7363 6965 6e74 6973 7473   data scientists
-00001740: 2c20 6d61 6368 696e 6520 6c65 6172 6e69  , machine learni
-00001750: 6e67 2065 6e67 696e 6565 7273 2c20 616e  ng engineers, an
-00001760: 6420 6461 7461 2065 6e67 696e 6565 7273  d data engineers
-00001770: 3a0a 0a2d 2044 6574 6563 7420 6461 7461  :..- Detect data
-00001780: 2064 7269 6674 2069 6e20 6d6f 6465 6c20   drift in model 
-00001790: 696e 7075 7420 6665 6174 7572 6573 0a2d  input features.-
-000017a0: 2044 6574 6563 7420 7472 6169 6e69 6e67   Detect training
-000017b0: 2d73 6572 7669 6e67 2073 6b65 772c 2063  -serving skew, c
-000017c0: 6f6e 6365 7074 2064 7269 6674 2c20 616e  oncept drift, an
-000017d0: 6420 6d6f 6465 6c20 7065 7266 6f72 6d61  d model performa
-000017e0: 6e63 6520 6465 6772 6164 6174 696f 6e0a  nce degradation.
-000017f0: 2d20 5661 6c69 6461 7465 2064 6174 6120  - Validate data 
-00001800: 7175 616c 6974 7920 696e 206d 6f64 656c  quality in model
-00001810: 2069 6e70 7574 7320 6f72 2069 6e20 6120   inputs or in a 
-00001820: 6461 7461 2070 6970 656c 696e 650a 2d20  data pipeline.- 
-00001830: 5065 7266 6f72 6d20 6578 706c 6f72 6174  Perform explorat
-00001840: 6f72 7920 6461 7461 2061 6e61 6c79 7369  ory data analysi
-00001850: 7320 6f66 206d 6173 7369 7665 2064 6174  s of massive dat
-00001860: 6173 6574 730a 2d20 5472 6163 6b20 6461  asets.- Track da
-00001870: 7461 2064 6973 7472 6962 7574 696f 6e73  ta distributions
-00001880: 2026 2064 6174 6120 7175 616c 6974 7920   & data quality 
-00001890: 666f 7220 4d4c 2065 7870 6572 696d 656e  for ML experimen
-000018a0: 7473 0a2d 2045 6e61 626c 6520 6461 7461  ts.- Enable data
-000018b0: 2061 7564 6974 696e 6720 616e 6420 676f   auditing and go
-000018c0: 7665 726e 616e 6365 2061 6372 6f73 7320  vernance across 
-000018d0: 7468 6520 6f72 6761 6e69 7a61 7469 6f6e  the organization
-000018e0: 0a2d 2053 7461 6e64 6172 6469 7a65 2064  .- Standardize d
-000018f0: 6174 6120 646f 6375 6d65 6e74 6174 696f  ata documentatio
-00001900: 6e20 7072 6163 7469 6365 7320 6163 726f  n practices acro
-00001910: 7373 2074 6865 206f 7267 616e 697a 6174  ss the organizat
-00001920: 696f 6e0a 2d20 416e 6420 6d6f 7265 0a0a  ion.- And more..
-00001930: 2323 2051 7569 636b 7374 6172 740a 0a49  ## Quickstart..I
-00001940: 6e73 7461 6c6c 2077 6879 6c6f 6773 2075  nstall whylogs u
-00001950: 7369 6e67 2074 6865 2070 6970 2070 6163  sing the pip pac
-00001960: 6b61 6765 206d 616e 6167 6572 2069 6e20  kage manager in 
-00001970: 6120 7465 726d 696e 616c 2062 7920 7275  a terminal by ru
-00001980: 6e6e 696e 673a 0a0a 6060 600a 7069 7020  nning:..```.pip 
-00001990: 696e 7374 616c 6c20 7768 796c 6f67 730a  install whylogs.
-000019a0: 6060 600a 0a54 6865 6e20 796f 7520 6361  ```..Then you ca
-000019b0: 6e20 6c6f 6720 6461 7461 2069 6e20 7079  n log data in py
-000019c0: 7468 6f6e 2061 7320 7369 6d70 6c79 2061  thon as simply a
-000019d0: 7320 7468 6973 3a0a 0a60 6060 7079 7468  s this:..```pyth
-000019e0: 6f6e 0a69 6d70 6f72 7420 7768 796c 6f67  on.import whylog
-000019f0: 7320 6173 2077 6879 0a69 6d70 6f72 7420  s as why.import 
-00001a00: 7061 6e64 6173 2061 7320 7064 0a0a 6466  pandas as pd..df
-00001a10: 203d 2070 642e 7265 6164 5f63 7376 2822   = pd.read_csv("
-00001a20: 7061 7468 2f74 6f2f 6669 6c65 2e63 7376  path/to/file.csv
-00001a30: 2229 0a72 6573 756c 7473 203d 2077 6879  ").results = why
-00001a40: 2e6c 6f67 2864 6629 0a60 6060 0a0a 416e  .log(df).```..An
-00001a50: 6420 766f 696c c3a0 2c20 796f 7520 6e6f  d voil.., you no
-00001a60: 7720 6861 7665 2061 2077 6879 6c6f 6773  w have a whylogs
-00001a70: 2070 726f 6669 6c65 2e20 546f 206c 6561   profile. To lea
-00001a80: 726e 206d 6f72 6520 6162 6f75 7420 7768  rn more about wh
-00001a90: 6174 2061 2077 6879 6c6f 6773 2070 726f  at a whylogs pro
-00001aa0: 6669 6c65 2069 7320 616e 6420 7768 6174  file is and what
-00001ab0: 2079 6f75 2063 616e 2064 6f20 7769 7468   you can do with
-00001ac0: 2069 742c 2063 6865 636b 206f 7574 206f   it, check out o
-00001ad0: 7572 205b 646f 6373 5d28 6874 7470 733a  ur [docs](https:
-00001ae0: 2f2f 7768 796c 6f67 732e 7265 6164 7468  //whylogs.readth
-00001af0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00001b00: 7374 2f29 2061 6e64 206f 7572 205b 6578  st/) and our [ex
-00001b10: 616d 706c 6573 5d28 6874 7470 733a 2f2f  amples](https://
-00001b20: 6769 7468 7562 2e63 6f6d 2f77 6879 6c61  github.com/whyla
-00001b30: 6273 2f77 6879 6c6f 6773 2f74 7265 652f  bs/whylogs/tree/
-00001b40: 6d61 696e 6c69 6e65 2f70 7974 686f 6e2f  mainline/python/
-00001b50: 6578 616d 706c 6573 292e 0a0a            examples)...
+00000030: 2e30 7263 300a 5375 6d6d 6172 793a 2050  .0rc0.Summary: P
+00000040: 726f 6669 6c65 2061 6e64 206d 6f6e 6974  rofile and monit
+00000050: 6f72 2079 6f75 7220 4d4c 2064 6174 6120  or your ML data 
+00000060: 7069 7065 6c69 6e65 2065 6e64 2d74 6f2d  pipeline end-to-
+00000070: 656e 640a 486f 6d65 2d70 6167 653a 2068  end.Home-page: h
+00000080: 7474 7073 3a2f 2f64 6f63 732e 7768 796c  ttps://docs.whyl
+00000090: 6162 732e 6169 0a4c 6963 656e 7365 3a20  abs.ai.License: 
+000000a0: 4170 6163 6865 2d32 2e30 0a41 7574 686f  Apache-2.0.Autho
+000000b0: 723a 2057 6879 4c61 6273 2e61 690a 4175  r: WhyLabs.ai.Au
+000000c0: 7468 6f72 2d65 6d61 696c 3a20 7375 7070  thor-email: supp
+000000d0: 6f72 7440 7768 796c 6162 732e 6169 0a52  ort@whylabs.ai.R
+000000e0: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
+000000f0: 3e3d 332e 372e 312c 3c34 0a43 6c61 7373  >=3.7.1,<4.Class
+00000100: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
+00000110: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+00000120: 3a20 4170 6163 6865 2053 6f66 7477 6172  : Apache Softwar
+00000130: 6520 4c69 6365 6e73 650a 436c 6173 7369  e License.Classi
+00000140: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000150: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000160: 7468 6f6e 203a 3a20 330a 436c 6173 7369  thon :: 3.Classi
+00000170: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000180: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000190: 7468 6f6e 203a 3a20 332e 380a 436c 6173  thon :: 3.8.Clas
+000001a0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000001b0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000001c0: 5079 7468 6f6e 203a 3a20 332e 390a 436c  Python :: 3.9.Cl
+000001d0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000001e0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000001f0: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+00000200: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000210: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000220: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000230: 2e31 310a 5072 6f76 6964 6573 2d45 7874  .11.Provides-Ext
+00000240: 7261 3a20 616c 6c0a 5072 6f76 6964 6573  ra: all.Provides
+00000250: 2d45 7874 7261 3a20 6461 7461 7365 7473  -Extra: datasets
+00000260: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+00000270: 2064 6f63 730a 5072 6f76 6964 6573 2d45   docs.Provides-E
+00000280: 7874 7261 3a20 656d 6265 6464 696e 6773  xtra: embeddings
+00000290: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+000002a0: 2066 7567 7565 0a50 726f 7669 6465 732d   fugue.Provides-
+000002b0: 4578 7472 613a 2067 6373 0a50 726f 7669  Extra: gcs.Provi
+000002c0: 6465 732d 4578 7472 613a 2069 6d61 6765  des-Extra: image
+000002d0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+000002e0: 206d 6c66 6c6f 770a 5072 6f76 6964 6573   mlflow.Provides
+000002f0: 2d45 7874 7261 3a20 7072 6f63 0a50 726f  -Extra: proc.Pro
+00000300: 7669 6465 732d 4578 7472 613a 2070 726f  vides-Extra: pro
+00000310: 632d 6d70 0a50 726f 7669 6465 732d 4578  c-mp.Provides-Ex
+00000320: 7472 613a 2073 330a 5072 6f76 6964 6573  tra: s3.Provides
+00000330: 2d45 7874 7261 3a20 7370 6172 6b0a 5072  -Extra: spark.Pr
+00000340: 6f76 6964 6573 2d45 7874 7261 3a20 7669  ovides-Extra: vi
+00000350: 7a0a 5265 7175 6972 6573 2d44 6973 743a  z.Requires-Dist:
+00000360: 2050 696c 6c6f 7720 283e 3d39 2e32 2e30   Pillow (>=9.2.0
+00000370: 2c3c 3130 2e30 2e30 2920 3b20 6578 7472  ,<10.0.0) ; extr
+00000380: 6120 3d3d 2022 7669 7a22 206f 7220 6578  a == "viz" or ex
+00000390: 7472 6120 3d3d 2022 696d 6167 6522 206f  tra == "image" o
+000003a0: 7220 6578 7472 6120 3d3d 2022 616c 6c22  r extra == "all"
+000003b0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000003c0: 626f 746f 3320 283e 3d31 2e32 322e 3133  boto3 (>=1.22.13
+000003d0: 2c3c 322e 302e 3029 203b 2065 7874 7261  ,<2.0.0) ; extra
+000003e0: 203d 3d20 2273 3322 206f 7220 6578 7472   == "s3" or extr
+000003f0: 6120 3d3d 2022 616c 6c22 0a52 6571 7569  a == "all".Requi
+00000400: 7265 732d 4469 7374 3a20 6661 7374 6572  res-Dist: faster
+00000410: 2d66 6966 6f20 283e 3d31 2e34 2e35 2c3c  -fifo (>=1.4.5,<
+00000420: 322e 302e 3029 203b 2065 7874 7261 203d  2.0.0) ; extra =
+00000430: 3d20 2270 726f 6322 206f 7220 6578 7472  = "proc" or extr
+00000440: 6120 3d3d 2022 616c 6c22 0a52 6571 7569  a == "all".Requi
+00000450: 7265 732d 4469 7374 3a20 6675 6775 6520  res-Dist: fugue 
+00000460: 283e 3d30 2e38 2e31 2c3c 302e 392e 3029  (>=0.8.1,<0.9.0)
+00000470: 203b 2065 7874 7261 203d 3d20 2266 7567   ; extra == "fug
+00000480: 7565 2220 6f72 2065 7874 7261 203d 3d20  ue" or extra == 
+00000490: 2261 6c6c 220a 5265 7175 6972 6573 2d44  "all".Requires-D
+000004a0: 6973 743a 2066 7572 6f20 283e 3d32 3032  ist: furo (>=202
+000004b0: 322e 332e 342c 3c32 3032 332e 302e 3029  2.3.4,<2023.0.0)
+000004c0: 203b 2065 7874 7261 203d 3d20 2264 6f63   ; extra == "doc
+000004d0: 7322 0a52 6571 7569 7265 732d 4469 7374  s".Requires-Dist
+000004e0: 3a20 676f 6f67 6c65 2d63 6c6f 7564 2d73  : google-cloud-s
+000004f0: 746f 7261 6765 2028 3e3d 322e 352e 302c  torage (>=2.5.0,
+00000500: 3c33 2e30 2e30 2920 3b20 6578 7472 6120  <3.0.0) ; extra 
+00000510: 3d3d 2022 6763 7322 206f 7220 6578 7472  == "gcs" or extr
+00000520: 6120 3d3d 2022 616c 6c22 0a52 6571 7569  a == "all".Requi
+00000530: 7265 732d 4469 7374 3a20 696d 706f 7274  res-Dist: import
+00000540: 6c69 622d 6d65 7461 6461 7461 2028 3c34  lib-metadata (<4
+00000550: 2e33 2920 3b20 7079 7468 6f6e 5f76 6572  .3) ; python_ver
+00000560: 7369 6f6e 203c 2022 332e 3822 0a52 6571  sion < "3.8".Req
+00000570: 7569 7265 732d 4469 7374 3a20 6970 7974  uires-Dist: ipyt
+00000580: 686f 6e20 3b20 6578 7472 6120 3d3d 2022  hon ; extra == "
+00000590: 7669 7a22 206f 7220 6578 7472 6120 3d3d  viz" or extra ==
+000005a0: 2022 616c 6c22 0a52 6571 7569 7265 732d   "all".Requires-
+000005b0: 4469 7374 3a20 6970 7974 686f 6e5f 6765  Dist: ipython_ge
+000005c0: 6e75 7469 6c73 2028 3e3d 302e 322e 302c  nutils (>=0.2.0,
+000005d0: 3c30 2e33 2e30 2920 3b20 6578 7472 6120  <0.3.0) ; extra 
+000005e0: 3d3d 2022 646f 6373 220a 5265 7175 6972  == "docs".Requir
+000005f0: 6573 2d44 6973 743a 206d 6c66 6c6f 772d  es-Dist: mlflow-
+00000600: 736b 696e 6e79 2028 3c32 2e30 2e31 2920  skinny (<2.0.1) 
+00000610: 3b20 2870 7974 686f 6e5f 7665 7273 696f  ; (python_versio
+00000620: 6e20 3c20 2233 2e38 2229 2061 6e64 2028  n < "3.8") and (
+00000630: 6578 7472 6120 3d3d 2022 6d6c 666c 6f77  extra == "mlflow
+00000640: 2220 6f72 2065 7874 7261 203d 3d20 2261  " or extra == "a
+00000650: 6c6c 2229 0a52 6571 7569 7265 732d 4469  ll").Requires-Di
+00000660: 7374 3a20 6d6c 666c 6f77 2d73 6b69 6e6e  st: mlflow-skinn
+00000670: 7920 283e 3d32 2e35 2e30 2c3c 332e 302e  y (>=2.5.0,<3.0.
+00000680: 3029 203b 2028 7079 7468 6f6e 5f76 6572  0) ; (python_ver
+00000690: 7369 6f6e 203e 3d20 2233 2e38 2229 2061  sion >= "3.8") a
+000006a0: 6e64 2028 6578 7472 6120 3d3d 2022 6d6c  nd (extra == "ml
+000006b0: 666c 6f77 2220 6f72 2065 7874 7261 203d  flow" or extra =
+000006c0: 3d20 2261 6c6c 2229 0a52 6571 7569 7265  = "all").Require
+000006d0: 732d 4469 7374 3a20 6d79 7374 2d70 6172  s-Dist: myst-par
+000006e0: 7365 725b 7370 6869 6e78 5d20 283e 3d30  ser[sphinx] (>=0
+000006f0: 2e31 372e 322c 3c30 2e31 382e 3029 203b  .17.2,<0.18.0) ;
+00000700: 2065 7874 7261 203d 3d20 2264 6f63 7322   extra == "docs"
+00000710: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000720: 6e62 636f 6e76 6572 7420 283e 3d37 2e30  nbconvert (>=7.0
+00000730: 2e30 2c3c 382e 302e 3029 203b 2065 7874  .0,<8.0.0) ; ext
+00000740: 7261 203d 3d20 2264 6f63 7322 0a52 6571  ra == "docs".Req
+00000750: 7569 7265 732d 4469 7374 3a20 6e62 7370  uires-Dist: nbsp
+00000760: 6869 6e78 2028 3e3d 302e 382e 392c 3c30  hinx (>=0.8.9,<0
+00000770: 2e39 2e30 2920 3b20 6578 7472 6120 3d3d  .9.0) ; extra ==
+00000780: 2022 646f 6373 220a 5265 7175 6972 6573   "docs".Requires
+00000790: 2d44 6973 743a 206e 756d 7079 2028 3e3d  -Dist: numpy (>=
+000007a0: 312e 3233 2e32 2920 3b20 2870 7974 686f  1.23.2) ; (pytho
+000007b0: 6e5f 7665 7273 696f 6e20 3e3d 2022 332e  n_version >= "3.
+000007c0: 3131 2229 2061 6e64 2028 6578 7472 6120  11") and (extra 
+000007d0: 3d3d 2022 7669 7a22 206f 7220 6578 7472  == "viz" or extr
+000007e0: 6120 3d3d 2022 696d 6167 6522 206f 7220  a == "image" or 
+000007f0: 6578 7472 6120 3d3d 2022 656d 6265 6464  extra == "embedd
+00000800: 696e 6773 2220 6f72 2065 7874 7261 203d  ings" or extra =
+00000810: 3d20 2261 6c6c 2229 0a52 6571 7569 7265  = "all").Require
+00000820: 732d 4469 7374 3a20 6e75 6d70 7920 3b20  s-Dist: numpy ; 
+00000830: 2870 7974 686f 6e5f 7665 7273 696f 6e20  (python_version 
+00000840: 3c20 2233 2e31 3122 2920 616e 6420 2865  < "3.11") and (e
+00000850: 7874 7261 203d 3d20 2276 697a 2220 6f72  xtra == "viz" or
+00000860: 2065 7874 7261 203d 3d20 2269 6d61 6765   extra == "image
+00000870: 2220 6f72 2065 7874 7261 203d 3d20 2265  " or extra == "e
+00000880: 6d62 6564 6469 6e67 7322 206f 7220 6578  mbeddings" or ex
+00000890: 7472 6120 3d3d 2022 616c 6c22 290a 5265  tra == "all").Re
+000008a0: 7175 6972 6573 2d44 6973 743a 206f 726a  quires-Dist: orj
+000008b0: 736f 6e20 283e 3d33 2e38 2e31 302c 3c34  son (>=3.8.10,<4
+000008c0: 2e30 2e30 2920 3b20 6578 7472 6120 3d3d  .0.0) ; extra ==
+000008d0: 2022 7072 6f63 2220 6f72 2065 7874 7261   "proc" or extra
+000008e0: 203d 3d20 2270 726f 632d 6d70 2220 6f72   == "proc-mp" or
+000008f0: 2065 7874 7261 203d 3d20 2261 6c6c 220a   extra == "all".
+00000900: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
+00000910: 616e 6461 7320 3b20 6578 7472 6120 3d3d  andas ; extra ==
+00000920: 2022 6461 7461 7365 7473 2220 6f72 2065   "datasets" or e
+00000930: 7874 7261 203d 3d20 2270 726f 6322 206f  xtra == "proc" o
+00000940: 7220 6578 7472 6120 3d3d 2022 7072 6f63  r extra == "proc
+00000950: 2d6d 7022 206f 7220 6578 7472 6120 3d3d  -mp" or extra ==
+00000960: 2022 616c 6c22 0a52 6571 7569 7265 732d   "all".Requires-
+00000970: 4469 7374 3a20 706c 6174 666f 726d 6469  Dist: platformdi
+00000980: 7273 2028 3e3d 332e 352e 302c 3c34 2e30  rs (>=3.5.0,<4.0
+00000990: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
+000009a0: 743a 2070 726f 746f 6275 6620 283e 3d33  t: protobuf (>=3
+000009b0: 2e31 392e 3429 0a52 6571 7569 7265 732d  .19.4).Requires-
+000009c0: 4469 7374 3a20 7079 6172 726f 7720 283e  Dist: pyarrow (>
+000009d0: 3d38 2e30 2e30 2c3c 3133 2920 3b20 6578  =8.0.0,<13) ; ex
+000009e0: 7472 6120 3d3d 2022 7370 6172 6b22 206f  tra == "spark" o
+000009f0: 7220 6578 7472 6120 3d3d 2022 616c 6c22  r extra == "all"
+00000a00: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000a10: 7079 6261 7273 3320 283e 3d30 2e39 2c3c  pybars3 (>=0.9,<
+00000a20: 302e 3130 2920 3b20 6578 7472 6120 3d3d  0.10) ; extra ==
+00000a30: 2022 7669 7a22 206f 7220 6578 7472 6120   "viz" or extra 
+00000a40: 3d3d 2022 616c 6c22 0a52 6571 7569 7265  == "all".Require
+00000a50: 732d 4469 7374 3a20 7079 7370 6172 6b20  s-Dist: pyspark 
+00000a60: 283e 3d33 2e30 2e30 2c3c 342e 302e 3029  (>=3.0.0,<4.0.0)
+00000a70: 203b 2065 7874 7261 203d 3d20 2273 7061   ; extra == "spa
+00000a80: 726b 2220 6f72 2065 7874 7261 203d 3d20  rk" or extra == 
+00000a90: 2261 6c6c 220a 5265 7175 6972 6573 2d44  "all".Requires-D
+00000aa0: 6973 743a 2072 6571 7565 7374 7320 283e  ist: requests (>
+00000ab0: 3d32 2e32 372c 3c33 2e30 290a 5265 7175  =2.27,<3.0).Requ
+00000ac0: 6972 6573 2d44 6973 743a 2073 6369 6b69  ires-Dist: sciki
+00000ad0: 742d 6c65 6172 6e20 283e 3d31 2e30 2e32  t-learn (>=1.0.2
+00000ae0: 2c3c 322e 302e 3029 203b 2028 7079 7468  ,<2.0.0) ; (pyth
+00000af0: 6f6e 5f76 6572 7369 6f6e 203c 2022 332e  on_version < "3.
+00000b00: 3131 2229 2061 6e64 2028 6578 7472 6120  11") and (extra 
+00000b10: 3d3d 2022 656d 6265 6464 696e 6773 2220  == "embeddings" 
+00000b20: 6f72 2065 7874 7261 203d 3d20 2261 6c6c  or extra == "all
+00000b30: 2229 0a52 6571 7569 7265 732d 4469 7374  ").Requires-Dist
+00000b40: 3a20 7363 696b 6974 2d6c 6561 726e 2028  : scikit-learn (
+00000b50: 3e3d 312e 312e 322c 3c32 2920 3b20 2870  >=1.1.2,<2) ; (p
+00000b60: 7974 686f 6e5f 7665 7273 696f 6e20 3e3d  ython_version >=
+00000b70: 2022 332e 3131 2229 2061 6e64 2028 6578   "3.11") and (ex
+00000b80: 7472 6120 3d3d 2022 656d 6265 6464 696e  tra == "embeddin
+00000b90: 6773 2220 6f72 2065 7874 7261 203d 3d20  gs" or extra == 
+00000ba0: 2261 6c6c 2229 0a52 6571 7569 7265 732d  "all").Requires-
+00000bb0: 4469 7374 3a20 7363 6970 7920 283e 3d31  Dist: scipy (>=1
+00000bc0: 2e35 2920 3b20 2870 7974 686f 6e5f 7665  .5) ; (python_ve
+00000bd0: 7273 696f 6e20 3c20 2233 2e31 3122 2920  rsion < "3.11") 
+00000be0: 616e 6420 2865 7874 7261 203d 3d20 2276  and (extra == "v
+00000bf0: 697a 2220 6f72 2065 7874 7261 203d 3d20  iz" or extra == 
+00000c00: 2261 6c6c 2229 0a52 6571 7569 7265 732d  "all").Requires-
+00000c10: 4469 7374 3a20 7363 6970 7920 283e 3d31  Dist: scipy (>=1
+00000c20: 2e39 2e32 2920 3b20 2870 7974 686f 6e5f  .9.2) ; (python_
+00000c30: 7665 7273 696f 6e20 3e3d 2022 332e 3131  version >= "3.11
+00000c40: 2229 2061 6e64 2028 6578 7472 6120 3d3d  ") and (extra ==
+00000c50: 2022 7669 7a22 206f 7220 6578 7472 6120   "viz" or extra 
+00000c60: 3d3d 2022 616c 6c22 290a 5265 7175 6972  == "all").Requir
+00000c70: 6573 2d44 6973 743a 2073 7068 696e 7820  es-Dist: sphinx 
+00000c80: 3b20 6578 7472 6120 3d3d 2022 646f 6373  ; extra == "docs
+00000c90: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000ca0: 2073 7068 696e 782d 6175 746f 6170 6920   sphinx-autoapi 
+00000cb0: 3b20 6578 7472 6120 3d3d 2022 646f 6373  ; extra == "docs
+00000cc0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000cd0: 2073 7068 696e 782d 6175 746f 6275 696c   sphinx-autobuil
+00000ce0: 6420 283e 3d32 3032 312e 332e 3134 2c3c  d (>=2021.3.14,<
+00000cf0: 3230 3232 2e30 2e30 2920 3b20 6578 7472  2022.0.0) ; extr
+00000d00: 6120 3d3d 2022 646f 6373 220a 5265 7175  a == "docs".Requ
+00000d10: 6972 6573 2d44 6973 743a 2073 7068 696e  ires-Dist: sphin
+00000d20: 782d 636f 7079 6275 7474 6f6e 2028 3e3d  x-copybutton (>=
+00000d30: 302e 352e 302c 3c30 2e36 2e30 2920 3b20  0.5.0,<0.6.0) ; 
+00000d40: 6578 7472 6120 3d3d 2022 646f 6373 220a  extra == "docs".
+00000d50: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
+00000d60: 7068 696e 782d 696e 6c69 6e65 2d74 6162  phinx-inline-tab
+00000d70: 7320 3b20 2870 7974 686f 6e5f 7665 7273  s ; (python_vers
+00000d80: 696f 6e20 3e3d 2022 332e 3822 2061 6e64  ion >= "3.8" and
+00000d90: 2070 7974 686f 6e5f 7665 7273 696f 6e20   python_version 
+00000da0: 3c20 2234 2229 2061 6e64 2028 6578 7472  < "4") and (extr
+00000db0: 6120 3d3d 2022 646f 6373 2229 0a52 6571  a == "docs").Req
+00000dc0: 7569 7265 732d 4469 7374 3a20 7370 6869  uires-Dist: sphi
+00000dd0: 6e78 6578 742d 6f70 656e 6772 6170 6820  nxext-opengraph 
+00000de0: 283e 3d30 2e36 2e33 2c3c 302e 372e 3029  (>=0.6.3,<0.7.0)
+00000df0: 203b 2065 7874 7261 203d 3d20 2264 6f63   ; extra == "doc
+00000e00: 7322 0a52 6571 7569 7265 732d 4469 7374  s".Requires-Dist
+00000e10: 3a20 7479 7065 732d 7265 7175 6573 7473  : types-requests
+00000e20: 2028 3e3d 322e 3330 2e30 2e30 2c3c 332e   (>=2.30.0.0,<3.
+00000e30: 302e 302e 3029 0a52 6571 7569 7265 732d  0.0.0).Requires-
+00000e40: 4469 7374 3a20 7479 7069 6e67 2d65 7874  Dist: typing-ext
+00000e50: 656e 7369 6f6e 7320 283e 3d33 2e31 3029  ensions (>=3.10)
+00000e60: 203b 2070 7974 686f 6e5f 7665 7273 696f   ; python_versio
+00000e70: 6e20 3c20 2234 220a 5265 7175 6972 6573  n < "4".Requires
+00000e80: 2d44 6973 743a 2077 6879 6c61 6273 2d63  -Dist: whylabs-c
+00000e90: 6c69 656e 7420 283e 3d30 2e36 2e32 2c3c  lient (>=0.6.2,<
+00000ea0: 302e 372e 3029 0a52 6571 7569 7265 732d  0.7.0).Requires-
+00000eb0: 4469 7374 3a20 7768 796c 6f67 732d 736b  Dist: whylogs-sk
+00000ec0: 6574 6368 696e 6720 283e 3d33 2e34 2e31  etching (>=3.4.1
+00000ed0: 2e64 6576 3329 0a44 6573 6372 6970 7469  .dev3).Descripti
+00000ee0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+00000ef0: 2074 6578 742f 6d61 726b 646f 776e 0a0a   text/markdown..
+00000f00: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000f10: 2f2f 7374 6174 6963 2e73 6361 7266 2e73  //static.scarf.s
+00000f20: 682f 612e 706e 673f 782d 7078 6964 3d62  h/a.png?x-pxid=b
+00000f30: 6333 6335 3762 302d 3961 3635 2d34 3966  c3c57b0-9a65-49f
+00000f40: 652d 6238 6561 2d66 3731 3163 3464 3335  e-b8ea-f711c4d35
+00000f50: 6238 3222 202f 3e3c 7020 616c 6967 6e3d  b82" /><p align=
+00000f60: 2263 656e 7465 7222 3e0a 3c69 6d67 2073  "center">.<img s
+00000f70: 7263 3d22 6874 7470 733a 2f2f 692e 696d  rc="https://i.im
+00000f80: 6775 722e 636f 6d2f 6e76 3333 676f 562e  gur.com/nv33goV.
+00000f90: 706e 6722 2077 6964 7468 3d22 3335 2522  png" width="35%"
+00000fa0: 2f3e 0a3c 2f62 723e 0a0a 3c68 3120 616c  />.</br>..<h1 al
+00000fb0: 6967 6e3d 2263 656e 7465 7222 3e54 6865  ign="center">The
+00000fc0: 206f 7065 6e20 7374 616e 6461 7264 2066   open standard f
+00000fd0: 6f72 2064 6174 6120 6c6f 6767 696e 670a  or data logging.
+00000fe0: 0a20 3c2f 6831 3e0a 2020 3c68 3320 616c  . </h1>.  <h3 al
+00000ff0: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00001000: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00001010: 2f2f 7768 796c 6f67 732e 7265 6164 7468  //whylogs.readth
+00001020: 6564 6f63 732e 696f 2f22 3e3c 623e 446f  edocs.io/"><b>Do
+00001030: 6375 6d65 6e74 6174 696f 6e3c 2f62 3e3c  cumentation</b><
+00001040: 2f61 3e20 2662 756c 6c3b 0a20 2020 3c61  /a> &bull;.   <a
+00001050: 2068 7265 663d 2268 7474 7073 3a2f 2f62   href="https://b
+00001060: 6974 2e6c 792f 7768 796c 6f67 7373 6c61  it.ly/whylogssla
+00001070: 636b 223e 3c62 3e53 6c61 636b 2043 6f6d  ck"><b>Slack Com
+00001080: 6d75 6e69 7479 3c2f 623e 3c2f 613e 2026  munity</b></a> &
+00001090: 6275 6c6c 3b0a 2020 203c 6120 6872 6566  bull;.   <a href
+000010a0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+000010b0: 2e63 6f6d 2f77 6879 6c61 6273 2f77 6879  .com/whylabs/why
+000010c0: 6c6f 6773 2370 7974 686f 6e2d 7175 6963  logs#python-quic
+000010d0: 6b73 7461 7274 223e 3c62 3e50 7974 686f  kstart"><b>Pytho
+000010e0: 6e20 5175 6963 6b73 7461 7274 3c2f 623e  n Quickstart</b>
+000010f0: 3c2f 613e 2026 6275 6c6c 3b0a 2020 203c  </a> &bull;.   <
+00001100: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001110: 7768 796c 6f67 732e 7265 6164 7468 6564  whylogs.readthed
+00001120: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00001130: 2f65 7861 6d70 6c65 732f 696e 7465 6772  /examples/integr
+00001140: 6174 696f 6e73 2f77 7269 7465 7273 2f57  ations/writers/W
+00001150: 7269 7469 6e67 5f74 6f5f 5768 794c 6162  riting_to_WhyLab
+00001160: 732e 6874 6d6c 223e 3c62 3e57 6879 4c61  s.html"><b>WhyLa
+00001170: 6273 2051 7569 636b 7374 6172 743c 2f62  bs Quickstart</b
+00001180: 3e3c 2f61 3e0a 203c 2f68 333e 0a0a 3c70  ></a>. </h3>..<p
+00001190: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+000011a0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+000011b0: 2f2f 6769 7468 7562 2e63 6f6d 2f77 6879  //github.com/why
+000011c0: 6c61 6273 2f77 6879 6c6f 6773 2d70 7974  labs/whylogs-pyt
+000011d0: 686f 6e2f 626c 6f62 2f6d 6169 6e6c 696e  hon/blob/mainlin
+000011e0: 652f 4c49 4345 4e53 4522 2074 6172 6765  e/LICENSE" targe
+000011f0: 743d 225f 626c 616e 6b22 3e0a 2020 2020  t="_blank">.    
+00001200: 3c69 6d67 2073 7263 3d22 6874 7470 3a2f  <img src="http:/
+00001210: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00001220: 3a6c 6963 656e 7365 2d41 7061 6368 6525  :license-Apache%
+00001230: 3230 322d 626c 7565 2e73 7667 2220 616c  202-blue.svg" al
+00001240: 743d 224c 6963 656e 7365 223e 0a3c 2f61  t="License">.</a
+00001250: 3e0a 3c61 2068 7265 663d 2268 7474 7073  >.<a href="https
+00001260: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
+00001270: 2f70 792f 7768 796c 6f67 7322 2074 6172  /py/whylogs" tar
+00001280: 6765 743d 225f 626c 616e 6b22 3e0a 2020  get="_blank">.  
+00001290: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+000012a0: 733a 2f2f 6261 6467 652e 6675 7279 2e69  s://badge.fury.i
+000012b0: 6f2f 7079 2f77 6879 6c6f 6773 2e73 7667  o/py/whylogs.svg
+000012c0: 2220 616c 743d 2250 7950 6920 5665 7273  " alt="PyPi Vers
+000012d0: 696f 6e22 3e0a 3c2f 613e 0a3c 6120 6872  ion">.</a>.<a hr
+000012e0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000012f0: 7562 2e63 6f6d 2f70 7974 686f 6e2f 626c  ub.com/python/bl
+00001300: 6163 6b22 2074 6172 6765 743d 225f 626c  ack" target="_bl
+00001310: 616e 6b22 3e0a 2020 2020 3c69 6d67 2073  ank">.    <img s
+00001320: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00001330: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00001340: 2f63 6f64 6525 3230 7374 796c 652d 626c  /code%20style-bl
+00001350: 6163 6b2d 3030 3030 3030 2e73 7667 2220  ack-000000.svg" 
+00001360: 616c 743d 2243 6f64 6520 7374 796c 653a  alt="Code style:
+00001370: 2062 6c61 636b 223e 0a3c 2f61 3e0a 3c61   black">.</a>.<a
+00001380: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
+00001390: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
+000013a0: 2f77 6879 6c6f 6773 2220 7461 7267 6574  /whylogs" target
+000013b0: 3d22 5f62 6c61 6e6b 223e 0a20 2020 203c  ="_blank">.    <
+000013c0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+000013d0: 2f70 6570 792e 7465 6368 2f62 6164 6765  /pepy.tech/badge
+000013e0: 2f77 6879 6c6f 6773 2220 616c 743d 2250  /whylogs" alt="P
+000013f0: 7950 6920 446f 776e 6c6f 6164 7322 3e0a  yPi Downloads">.
+00001400: 3c2f 613e 0a3c 6120 6872 6566 3d22 6269  </a>.<a href="bi
+00001410: 742e 6c79 2f77 6879 6c6f 6773 2220 7461  t.ly/whylogs" ta
+00001420: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a20  rget="_blank">. 
+00001430: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00001440: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001450: 7768 796c 6162 732f 7768 796c 6f67 732d  whylabs/whylogs-
+00001460: 7079 7468 6f6e 2f77 6f72 6b66 6c6f 7773  python/workflows
+00001470: 2f77 6879 6c6f 6773 2532 3043 492f 6261  /whylogs%20CI/ba
+00001480: 6467 652e 7376 6722 2061 6c74 3d22 4349  dge.svg" alt="CI
+00001490: 223e 0a3c 2f61 3e0a 3c61 2068 7265 663d  ">.</a>.<a href=
+000014a0: 2268 7474 7073 3a2f 2f63 6f64 6563 6c69  "https://codecli
+000014b0: 6d61 7465 2e63 6f6d 2f67 6974 6875 622f  mate.com/github/
+000014c0: 7768 796c 6162 732f 7768 796c 6f67 732d  whylabs/whylogs-
+000014d0: 7079 7468 6f6e 2f6d 6169 6e74 6169 6e61  python/maintaina
+000014e0: 6269 6c69 7479 2220 7461 7267 6574 3d22  bility" target="
+000014f0: 5f62 6c61 6e6b 223e 0a20 2020 203c 696d  _blank">.    <im
+00001500: 6720 7372 633d 2268 7474 7073 3a2f 2f61  g src="https://a
+00001510: 7069 2e63 6f64 6563 6c69 6d61 7465 2e63  pi.codeclimate.c
+00001520: 6f6d 2f76 312f 6261 6467 6573 2f34 3432  om/v1/badges/442
+00001530: 6636 6361 3364 6361 3165 3538 3361 3438  f6ca3dca1e583a48
+00001540: 382f 6d61 696e 7461 696e 6162 696c 6974  8/maintainabilit
+00001550: 7922 2061 6c74 3d22 4d61 696e 7461 696e  y" alt="Maintain
+00001560: 6162 696c 6974 7922 3e0a 3c2f 613e 0a3c  ability">.</a>.<
+00001570: 2f70 3e0a 0a23 2320 5768 6174 2069 7320  /p>..## What is 
+00001580: 7768 796c 6f67 730a 0a77 6879 6c6f 6773  whylogs..whylogs
+00001590: 2069 7320 616e 206f 7065 6e20 736f 7572   is an open sour
+000015a0: 6365 206c 6962 7261 7279 2066 6f72 206c  ce library for l
+000015b0: 6f67 6769 6e67 2061 6e79 206b 696e 6420  ogging any kind 
+000015c0: 6f66 2064 6174 612e 2057 6974 6820 7768  of data. With wh
+000015d0: 796c 6f67 732c 2075 7365 7273 2061 7265  ylogs, users are
+000015e0: 2061 626c 6520 746f 2067 656e 6572 6174   able to generat
+000015f0: 6520 7375 6d6d 6172 6965 7320 6f66 2074  e summaries of t
+00001600: 6865 6972 2064 6174 6173 6574 7320 2863  heir datasets (c
+00001610: 616c 6c65 6420 5f77 6879 6c6f 6773 2070  alled _whylogs p
+00001620: 726f 6669 6c65 735f 2920 7768 6963 6820  rofiles_) which 
+00001630: 7468 6579 2063 616e 2075 7365 2074 6f3a  they can use to:
+00001640: 0a0a 312e 2054 7261 636b 2063 6861 6e67  ..1. Track chang
+00001650: 6573 2069 6e20 7468 6569 7220 6461 7461  es in their data
+00001660: 7365 740a 322e 2043 7265 6174 6520 5f64  set.2. Create _d
+00001670: 6174 6120 636f 6e73 7472 6169 6e74 735f  ata constraints_
+00001680: 2074 6f20 6b6e 6f77 2077 6865 7468 6572   to know whether
+00001690: 2074 6865 6972 2064 6174 6120 6c6f 6f6b   their data look
+000016a0: 7320 7468 6520 7761 7920 6974 2073 686f  s the way it sho
+000016b0: 756c 640a 332e 2051 7569 636b 6c79 2076  uld.3. Quickly v
+000016c0: 6973 7561 6c69 7a65 206b 6579 2073 756d  isualize key sum
+000016d0: 6d61 7279 2073 7461 7469 7374 6963 7320  mary statistics 
+000016e0: 6162 6f75 7420 7468 6569 7220 6461 7461  about their data
+000016f0: 7365 7473 0a0a 5468 6573 6520 7468 7265  sets..These thre
+00001700: 6520 6675 6e63 7469 6f6e 616c 6974 6965  e functionalitie
+00001710: 7320 656e 6162 6c65 2061 2076 6172 6965  s enable a varie
+00001720: 7479 206f 6620 7573 6520 6361 7365 7320  ty of use cases 
+00001730: 666f 7220 6461 7461 2073 6369 656e 7469  for data scienti
+00001740: 7374 732c 206d 6163 6869 6e65 206c 6561  sts, machine lea
+00001750: 726e 696e 6720 656e 6769 6e65 6572 732c  rning engineers,
+00001760: 2061 6e64 2064 6174 6120 656e 6769 6e65   and data engine
+00001770: 6572 733a 0a0a 2d20 4465 7465 6374 2064  ers:..- Detect d
+00001780: 6174 6120 6472 6966 7420 696e 206d 6f64  ata drift in mod
+00001790: 656c 2069 6e70 7574 2066 6561 7475 7265  el input feature
+000017a0: 730a 2d20 4465 7465 6374 2074 7261 696e  s.- Detect train
+000017b0: 696e 672d 7365 7276 696e 6720 736b 6577  ing-serving skew
+000017c0: 2c20 636f 6e63 6570 7420 6472 6966 742c  , concept drift,
+000017d0: 2061 6e64 206d 6f64 656c 2070 6572 666f   and model perfo
+000017e0: 726d 616e 6365 2064 6567 7261 6461 7469  rmance degradati
+000017f0: 6f6e 0a2d 2056 616c 6964 6174 6520 6461  on.- Validate da
+00001800: 7461 2071 7561 6c69 7479 2069 6e20 6d6f  ta quality in mo
+00001810: 6465 6c20 696e 7075 7473 206f 7220 696e  del inputs or in
+00001820: 2061 2064 6174 6120 7069 7065 6c69 6e65   a data pipeline
+00001830: 0a2d 2050 6572 666f 726d 2065 7870 6c6f  .- Perform explo
+00001840: 7261 746f 7279 2064 6174 6120 616e 616c  ratory data anal
+00001850: 7973 6973 206f 6620 6d61 7373 6976 6520  ysis of massive 
+00001860: 6461 7461 7365 7473 0a2d 2054 7261 636b  datasets.- Track
+00001870: 2064 6174 6120 6469 7374 7269 6275 7469   data distributi
+00001880: 6f6e 7320 2620 6461 7461 2071 7561 6c69  ons & data quali
+00001890: 7479 2066 6f72 204d 4c20 6578 7065 7269  ty for ML experi
+000018a0: 6d65 6e74 730a 2d20 456e 6162 6c65 2064  ments.- Enable d
+000018b0: 6174 6120 6175 6469 7469 6e67 2061 6e64  ata auditing and
+000018c0: 2067 6f76 6572 6e61 6e63 6520 6163 726f   governance acro
+000018d0: 7373 2074 6865 206f 7267 616e 697a 6174  ss the organizat
+000018e0: 696f 6e0a 2d20 5374 616e 6461 7264 697a  ion.- Standardiz
+000018f0: 6520 6461 7461 2064 6f63 756d 656e 7461  e data documenta
+00001900: 7469 6f6e 2070 7261 6374 6963 6573 2061  tion practices a
+00001910: 6372 6f73 7320 7468 6520 6f72 6761 6e69  cross the organi
+00001920: 7a61 7469 6f6e 0a2d 2041 6e64 206d 6f72  zation.- And mor
+00001930: 650a 0a23 2320 5175 6963 6b73 7461 7274  e..## Quickstart
+00001940: 0a0a 496e 7374 616c 6c20 7768 796c 6f67  ..Install whylog
+00001950: 7320 7573 696e 6720 7468 6520 7069 7020  s using the pip 
+00001960: 7061 636b 6167 6520 6d61 6e61 6765 7220  package manager 
+00001970: 696e 2061 2074 6572 6d69 6e61 6c20 6279  in a terminal by
+00001980: 2072 756e 6e69 6e67 3a0a 0a60 6060 0a70   running:..```.p
+00001990: 6970 2069 6e73 7461 6c6c 2077 6879 6c6f  ip install whylo
+000019a0: 6773 0a60 6060 0a0a 5468 656e 2079 6f75  gs.```..Then you
+000019b0: 2063 616e 206c 6f67 2064 6174 6120 696e   can log data in
+000019c0: 2070 7974 686f 6e20 6173 2073 696d 706c   python as simpl
+000019d0: 7920 6173 2074 6869 733a 0a0a 6060 6070  y as this:..```p
+000019e0: 7974 686f 6e0a 696d 706f 7274 2077 6879  ython.import why
+000019f0: 6c6f 6773 2061 7320 7768 790a 696d 706f  logs as why.impo
+00001a00: 7274 2070 616e 6461 7320 6173 2070 640a  rt pandas as pd.
+00001a10: 0a64 6620 3d20 7064 2e72 6561 645f 6373  .df = pd.read_cs
+00001a20: 7628 2270 6174 682f 746f 2f66 696c 652e  v("path/to/file.
+00001a30: 6373 7622 290a 7265 7375 6c74 7320 3d20  csv").results = 
+00001a40: 7768 792e 6c6f 6728 6466 290a 6060 600a  why.log(df).```.
+00001a50: 0a41 6e64 2076 6f69 6cc3 a02c 2079 6f75  .And voil.., you
+00001a60: 206e 6f77 2068 6176 6520 6120 7768 796c   now have a whyl
+00001a70: 6f67 7320 7072 6f66 696c 652e 2054 6f20  ogs profile. To 
+00001a80: 6c65 6172 6e20 6d6f 7265 2061 626f 7574  learn more about
+00001a90: 2077 6861 7420 6120 7768 796c 6f67 7320   what a whylogs 
+00001aa0: 7072 6f66 696c 6520 6973 2061 6e64 2077  profile is and w
+00001ab0: 6861 7420 796f 7520 6361 6e20 646f 2077  hat you can do w
+00001ac0: 6974 6820 6974 2c20 6368 6563 6b20 6f75  ith it, check ou
+00001ad0: 7420 6f75 7220 5b64 6f63 735d 2868 7474  t our [docs](htt
+00001ae0: 7073 3a2f 2f77 6879 6c6f 6773 2e72 6561  ps://whylogs.rea
+00001af0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00001b00: 6174 6573 742f 2920 616e 6420 6f75 7220  atest/) and our 
+00001b10: 5b65 7861 6d70 6c65 735d 2868 7474 7073  [examples](https
+00001b20: 3a2f 2f67 6974 6875 622e 636f 6d2f 7768  ://github.com/wh
+00001b30: 796c 6162 732f 7768 796c 6f67 732f 7472  ylabs/whylogs/tr
+00001b40: 6565 2f6d 6169 6e6c 696e 652f 7079 7468  ee/mainline/pyth
+00001b50: 6f6e 2f65 7861 6d70 6c65 7329 2e0a 0a    on/examples)...
```

