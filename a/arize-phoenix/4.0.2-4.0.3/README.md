# Comparing `tmp/arize_phoenix-4.0.2.tar.gz` & `tmp/arize_phoenix-4.0.3.tar.gz`

## Comparing `arize_phoenix-4.0.2.tar` & `arize_phoenix-4.0.3.tar`

### file list

```diff
@@ -1,200 +1,200 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/examples/manually-instrumented-chatbot/chat-service/chat/__init__.py
--rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/examples/manually-instrumented-chatbot/chat-service/chat/app.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/examples/manually-instrumented-chatbot/chat-service/chat/types.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/examples/manually-instrumented-chatbot/frontend/Dockerfile
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/examples/manually-instrumented-chatbot/frontend/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/examples/manually-instrumented-chatbot/frontend/__init__.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/examples/manually-instrumented-chatbot/frontend/pyproject.toml
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/examples/manually-instrumented-chatbot/frontend/requirements.txt
--rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/examples/manually-instrumented-chatbot/frontend/schema.json
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/__init__.py
--rw-r--r--   0        0        0     6879 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/config.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/datetime_utils.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/exceptions.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/py.typed
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/services.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/settings.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/core/__init__.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/core/embedding_dimension.py
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/core/model.py
--rw-r--r--   0        0        0    50222 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/core/model_schema.py
--rw-r--r--   0        0        0     8287 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/core/model_schema_adapter.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/README.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/__init__.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/alembic.ini
--rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/bulk_inserter.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/engines.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/helpers.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/migrate.py
--rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/insertion/__init__.py
--rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/insertion/evaluation.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/insertion/helpers.py
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/insertion/span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/migrations/__init__.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/migrations/env.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/migrations/script.py.mako
--rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/db/migrations/versions/cf03bd6bae1d_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/inferences/__init__.py
--rw-r--r--   0        0        0     8261 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/inferences/errors.py
--rw-r--r--   0        0        0    20711 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/inferences/fixtures.py
--rw-r--r--   0        0        0    30694 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/inferences/inferences.py
--rw-r--r--   0        0        0     6643 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/inferences/schema.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/inferences/validation.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/metrics/README.md
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/metrics/__init__.py
--rw-r--r--   0        0        0    12739 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/metrics/binning.py
--rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/metrics/metrics.py
--rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/metrics/mixins.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/metrics/retrieval_metrics.py
--rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/metrics/timeseries.py
--rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/metrics/wrappers.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/pointcloud/__init__.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/pointcloud/clustering.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/pointcloud/pointcloud.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/pointcloud/projectors.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/pointcloud/umap_parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/__init__.py
--rw-r--r--   0        0        0    16247 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/app.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/grpc_server.py
--rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/main.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/prometheus.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/telemetry.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/thread_server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/__init__.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/context.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/helpers.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/interceptor.py
--rw-r--r--   0        0        0    11605 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/schema.py
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/__init__.py
--rw-r--r--   0        0        0     5684 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/document_evaluation_summaries.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/document_evaluations.py
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/document_retrieval_metrics.py
--rw-r--r--   0        0        0     5724 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/evaluation_summaries.py
--rw-r--r--   0        0        0     7423 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/latency_ms_quantile.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/min_start_or_max_end_times.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/record_counts.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/span_descendants.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/span_evaluations.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/token_counts.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/trace_evaluations.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/cache/__init__.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/cache/two_tier_cache.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/input_types/ClusterInput.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/input_types/Coordinates.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/input_types/DataQualityMetricInput.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/input_types/DimensionFilter.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/input_types/DimensionInput.py
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/input_types/Granularity.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/input_types/PerformanceMetricInput.py
--rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/input_types/SpanSort.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/input_types/TimeRange.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/input_types/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/routers/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/routers/utils.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/routers/v1/__init__.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/routers/v1/evaluations.py
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/routers/v1/spans.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/routers/v1/traces.py
--rw-r--r--   0        0        0     5618 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/Cluster.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/DataQualityMetric.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/Dataset.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/DatasetRole.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/DatasetValues.py
--rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/Dimension.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/DimensionDataType.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/DimensionShape.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/DimensionType.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/DimensionWithValue.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/DocumentEvaluationSummary.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/DocumentRetrievalMetrics.py
--rw-r--r--   0        0        0    18678 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/EmbeddingDimension.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/EmbeddingMetadata.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/Evaluation.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/EvaluationSummary.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/Event.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/EventMetadata.py
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/ExportEventsMutation.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/ExportedFile.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/Functionality.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/MimeType.py
--rw-r--r--   0        0        0     7880 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/Model.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/NumericRange.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/PerformanceMetric.py
--rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/Project.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/PromptResponse.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/Retrieval.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/ScalarDriftMetricEnum.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/Segments.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/SortDir.py
--rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/Span.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/TimeSeries.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/Trace.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/UMAPPoints.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/ValidationResult.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/VectorDriftMetricEnum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/__init__.py
--rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/node.py
--rw-r--r--   0        0        0    10052 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/api/types/pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/openapi/__init__.py
--rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/openapi/docs.py
--rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon-114x114.png
--rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon-120x120.png
--rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon-144x144.png
--rw-r--r--   0        0        0    11082 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon-152x152.png
--rw-r--r--   0        0        0    12052 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon-180x180.png
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon-72x72.png
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon-76x76.png
--rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon.png
--rw-r--r--   0        0        0    34494 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/static/favicon.ico
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/static/index.css
--rw-r--r--   0        0        0  3350371 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/static/index.js
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/static/modernizr.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/templates/__init__.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/server/templates/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/session/__init__.py
--rw-r--r--   0        0        0    10097 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/session/client.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/session/data_extractor.py
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/session/evaluation.py
--rw-r--r--   0        0        0    26103 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/session/session.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/__init__.py
--rw-r--r--   0        0        0    12364 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/attributes.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/errors.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/evaluation_conventions.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/exporter.py
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/fixtures.py
--rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/otel.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/projects.py
--rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/schemas.py
--rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/span_evaluations.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/span_json_decoder.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/span_json_encoder.py
--rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/trace_dataset.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/utils.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/dsl/README.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/dsl/__init__.py
--rw-r--r--   0        0        0    31900 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/dsl/filter.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/dsl/helpers.py
--rw-r--r--   0        0        0    30316 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/dsl/query.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/langchain/__init__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/langchain/instrumentor.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/llama_index/__init__.py
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/llama_index/callback.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/openai/__init__.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/openai/instrumentor.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/v1/__init__.py
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/v1/evaluation_pb2.py
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/trace/v1/evaluation_pb2.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/utilities/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/utilities/deprecation.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/utilities/error_handling.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/utilities/logging.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/utilities/project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/src/phoenix/utilities/span_store.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/.gitignore
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/IP_NOTICE
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/LICENSE
--rw-r--r--   0        0        0    26114 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/README.md
--rw-r--r--   0        0        0     8971 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/pyproject.toml
--rw-r--r--   0        0        0    30464 2020-02-02 00:00:00.000000 arize_phoenix-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/examples/manually-instrumented-chatbot/chat-service/chat/__init__.py
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/examples/manually-instrumented-chatbot/chat-service/chat/app.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/examples/manually-instrumented-chatbot/chat-service/chat/types.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/examples/manually-instrumented-chatbot/frontend/Dockerfile
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/examples/manually-instrumented-chatbot/frontend/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/examples/manually-instrumented-chatbot/frontend/__init__.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/examples/manually-instrumented-chatbot/frontend/pyproject.toml
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/examples/manually-instrumented-chatbot/frontend/requirements.txt
+-rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/examples/manually-instrumented-chatbot/frontend/schema.json
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/__init__.py
+-rw-r--r--   0        0        0     6879 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/config.py
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/datetime_utils.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/exceptions.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/py.typed
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/services.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/settings.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/core/__init__.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/core/embedding_dimension.py
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/core/model.py
+-rw-r--r--   0        0        0    50222 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/core/model_schema.py
+-rw-r--r--   0        0        0     8287 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/core/model_schema_adapter.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/README.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/__init__.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/alembic.ini
+-rw-r--r--   0        0        0     9493 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/bulk_inserter.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/engines.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/helpers.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/migrate.py
+-rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/insertion/__init__.py
+-rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/insertion/evaluation.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/insertion/helpers.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/insertion/span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/migrations/__init__.py
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/migrations/env.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/migrations/script.py.mako
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/db/migrations/versions/cf03bd6bae1d_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/inferences/__init__.py
+-rw-r--r--   0        0        0     8261 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/inferences/errors.py
+-rw-r--r--   0        0        0    20711 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/inferences/fixtures.py
+-rw-r--r--   0        0        0    30694 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/inferences/inferences.py
+-rw-r--r--   0        0        0     6643 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/inferences/schema.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/inferences/validation.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/metrics/README.md
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/metrics/__init__.py
+-rw-r--r--   0        0        0    12739 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/metrics/binning.py
+-rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/metrics/metrics.py
+-rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/metrics/mixins.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/metrics/retrieval_metrics.py
+-rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/metrics/timeseries.py
+-rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/metrics/wrappers.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/pointcloud/__init__.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/pointcloud/clustering.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/pointcloud/pointcloud.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/pointcloud/projectors.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/pointcloud/umap_parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/__init__.py
+-rw-r--r--   0        0        0    16247 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/app.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/grpc_server.py
+-rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/main.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/prometheus.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/telemetry.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/thread_server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/__init__.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/context.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/helpers.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/interceptor.py
+-rw-r--r--   0        0        0    11605 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/schema.py
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/__init__.py
+-rw-r--r--   0        0        0     5684 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/document_evaluation_summaries.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/document_evaluations.py
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/document_retrieval_metrics.py
+-rw-r--r--   0        0        0     5724 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/evaluation_summaries.py
+-rw-r--r--   0        0        0     7423 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/latency_ms_quantile.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/min_start_or_max_end_times.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/record_counts.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/span_descendants.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/span_evaluations.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/token_counts.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/trace_evaluations.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/cache/__init__.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/cache/two_tier_cache.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/input_types/ClusterInput.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/input_types/Coordinates.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/input_types/DataQualityMetricInput.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/input_types/DimensionFilter.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/input_types/DimensionInput.py
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/input_types/Granularity.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/input_types/PerformanceMetricInput.py
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/input_types/SpanSort.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/input_types/TimeRange.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/input_types/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/routers/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/routers/utils.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/routers/v1/__init__.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/routers/v1/evaluations.py
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/routers/v1/spans.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/routers/v1/traces.py
+-rw-r--r--   0        0        0     5618 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/Cluster.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/DataQualityMetric.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/Dataset.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/DatasetRole.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/DatasetValues.py
+-rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/Dimension.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/DimensionDataType.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/DimensionShape.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/DimensionType.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/DimensionWithValue.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/DocumentEvaluationSummary.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/DocumentRetrievalMetrics.py
+-rw-r--r--   0        0        0    18678 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/EmbeddingDimension.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/EmbeddingMetadata.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/Evaluation.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/EvaluationSummary.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/Event.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/EventMetadata.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/ExportEventsMutation.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/ExportedFile.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/Functionality.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/MimeType.py
+-rw-r--r--   0        0        0     7880 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/Model.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/NumericRange.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/PerformanceMetric.py
+-rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/Project.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/PromptResponse.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/Retrieval.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/ScalarDriftMetricEnum.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/Segments.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/SortDir.py
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/Span.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/TimeSeries.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/Trace.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/UMAPPoints.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/ValidationResult.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/VectorDriftMetricEnum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/__init__.py
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/node.py
+-rw-r--r--   0        0        0    10052 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/api/types/pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/openapi/__init__.py
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/openapi/docs.py
+-rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon-114x114.png
+-rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon-120x120.png
+-rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon-144x144.png
+-rw-r--r--   0        0        0    11082 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon-152x152.png
+-rw-r--r--   0        0        0    12052 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon-180x180.png
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon-72x72.png
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon-76x76.png
+-rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon.png
+-rw-r--r--   0        0        0    34494 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/static/favicon.ico
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/static/index.css
+-rw-r--r--   0        0        0  3350371 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/static/index.js
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/static/modernizr.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/templates/__init__.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/server/templates/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/session/__init__.py
+-rw-r--r--   0        0        0    10097 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/session/client.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/session/data_extractor.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/session/evaluation.py
+-rw-r--r--   0        0        0    26103 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/session/session.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/__init__.py
+-rw-r--r--   0        0        0    12364 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/attributes.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/errors.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/evaluation_conventions.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/exporter.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/fixtures.py
+-rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/otel.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/projects.py
+-rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/schemas.py
+-rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/span_evaluations.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/span_json_decoder.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/span_json_encoder.py
+-rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/trace_dataset.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/utils.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/dsl/README.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/dsl/__init__.py
+-rw-r--r--   0        0        0    31900 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/dsl/filter.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/dsl/helpers.py
+-rw-r--r--   0        0        0    30316 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/dsl/query.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/langchain/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/langchain/instrumentor.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/llama_index/__init__.py
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/llama_index/callback.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/openai/__init__.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/openai/instrumentor.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/v1/__init__.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/v1/evaluation_pb2.py
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/trace/v1/evaluation_pb2.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/utilities/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/utilities/deprecation.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/utilities/error_handling.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/utilities/logging.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/utilities/project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/src/phoenix/utilities/span_store.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/.gitignore
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/IP_NOTICE
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/LICENSE
+-rw-r--r--   0        0        0    26114 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/README.md
+-rw-r--r--   0        0        0     8971 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0    30464 2020-02-02 00:00:00.000000 arize_phoenix-4.0.3/PKG-INFO
```

### Comparing `arize_phoenix-4.0.2/examples/manually-instrumented-chatbot/chat-service/chat/app.py` & `arize_phoenix-4.0.3/examples/manually-instrumented-chatbot/chat-service/chat/app.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/examples/manually-instrumented-chatbot/frontend/requirements.txt` & `arize_phoenix-4.0.3/examples/manually-instrumented-chatbot/frontend/requirements.txt`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/examples/manually-instrumented-chatbot/frontend/schema.json` & `arize_phoenix-4.0.3/examples/manually-instrumented-chatbot/frontend/schema.json`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/__init__.py` & `arize_phoenix-4.0.3/src/phoenix/__init__.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/config.py` & `arize_phoenix-4.0.3/src/phoenix/config.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/datetime_utils.py` & `arize_phoenix-4.0.3/src/phoenix/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/services.py` & `arize_phoenix-4.0.3/src/phoenix/services.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/core/model.py` & `arize_phoenix-4.0.3/src/phoenix/core/model.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/core/model_schema.py` & `arize_phoenix-4.0.3/src/phoenix/core/model_schema.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/core/model_schema_adapter.py` & `arize_phoenix-4.0.3/src/phoenix/core/model_schema_adapter.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/db/README.md` & `arize_phoenix-4.0.3/src/phoenix/db/README.md`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/db/alembic.ini` & `arize_phoenix-4.0.3/src/phoenix/db/alembic.ini`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/db/bulk_inserter.py` & `arize_phoenix-4.0.3/src/phoenix/db/bulk_inserter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import logging
 from dataclasses import dataclass, field
 from datetime import datetime, timezone
 from itertools import islice
-from time import perf_counter, time
+from time import perf_counter
 from typing import (
     Any,
     AsyncContextManager,
     Awaitable,
     Callable,
     Iterable,
     List,
@@ -44,33 +44,28 @@
     def __init__(
         self,
         db: Callable[[], AsyncContextManager[AsyncSession]],
         *,
         cache_for_dataloaders: Optional[CacheForDataLoaders] = None,
         initial_batch_of_spans: Optional[Iterable[Tuple[Span, str]]] = None,
         initial_batch_of_evaluations: Optional[Iterable[pb.Evaluation]] = None,
-        run_interval_in_seconds: float = 2,
+        sleep: float = 0.1,
         max_num_per_transaction: int = 1000,
         enable_prometheus: bool = False,
     ) -> None:
         """
         :param db: A function to initiate a new database session.
         :param initial_batch_of_spans: Initial batch of spans to insert.
-        :param run_interval_in_seconds: The time interval between the starts of each
-        bulk insert. If there's nothing to insert, the inserter goes back to sleep.
+        :param sleep: The time to sleep between bulk insertions
         :param max_num_per_transaction: The maximum number of items to insert in a single
         transaction. Multiple transactions will be used if there are more items in the batch.
         """
         self._db = db
         self._running = False
-        self._run_interval_seconds = run_interval_in_seconds
-
-        # tracks time between insertions to improve responsiveness for small batches
-        self._last_insertion_time = time() - self._run_interval_seconds
-
+        self._sleep = sleep
         self._max_num_per_transaction = max_num_per_transaction
         self._spans: List[Tuple[Span, str]] = (
             [] if initial_batch_of_spans is None else list(initial_batch_of_spans)
         )
         self._evaluations: List[pb.Evaluation] = (
             [] if initial_batch_of_evaluations is None else list(initial_batch_of_evaluations)
         )
@@ -100,17 +95,16 @@
     async def _queue_evaluation(self, evaluation: pb.Evaluation) -> None:
         self._evaluations.append(evaluation)
 
     async def _bulk_insert(self) -> None:
         spans_buffer, evaluations_buffer = None, None
         # start first insert immediately if the inserter has not run recently
         while self._spans or self._evaluations or self._running:
-            next_run_at = self._last_insertion_time + self._run_interval_seconds
-            await asyncio.sleep(max(next_run_at - time(), 0))
             if not (self._spans or self._evaluations):
+                await asyncio.sleep(self._sleep)
                 continue
             # It's important to grab the buffers at the same time so there's
             # no race condition, since an eval insertion will fail if the span
             # it references doesn't exist. Grabbing the eval buffer later may
             # include an eval whose span is in the queue but missed being
             # included in the span buffer that was grabbed previously.
             if self._spans:
@@ -128,15 +122,15 @@
                 spans_buffer = None
             if evaluations_buffer:
                 result = await self._insert_evaluations(evaluations_buffer)
                 transaction_result.updated_project_rowids.update(result.updated_project_rowids)
                 evaluations_buffer = None
             for project_rowid in transaction_result.updated_project_rowids:
                 self._last_updated_at_by_project[project_rowid] = datetime.now(timezone.utc)
-            self._last_insertion_time = time()
+            await asyncio.sleep(self._sleep)
 
     async def _insert_spans(self, spans: List[Tuple[Span, str]]) -> TransactionResult:
         transaction_result = TransactionResult()
         for i in range(0, len(spans), self._max_num_per_transaction):
             try:
                 start = perf_counter()
                 async with self._db() as session:
```

### Comparing `arize_phoenix-4.0.2/src/phoenix/db/engines.py` & `arize_phoenix-4.0.3/src/phoenix/db/engines.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/db/helpers.py` & `arize_phoenix-4.0.3/src/phoenix/db/helpers.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/db/migrate.py` & `arize_phoenix-4.0.3/src/phoenix/db/migrate.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/db/models.py` & `arize_phoenix-4.0.3/src/phoenix/db/models.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/db/insertion/evaluation.py` & `arize_phoenix-4.0.3/src/phoenix/db/insertion/evaluation.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/db/insertion/helpers.py` & `arize_phoenix-4.0.3/src/phoenix/db/insertion/helpers.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/db/insertion/span.py` & `arize_phoenix-4.0.3/src/phoenix/db/insertion/span.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/db/migrations/env.py` & `arize_phoenix-4.0.3/src/phoenix/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/db/migrations/script.py.mako` & `arize_phoenix-4.0.3/src/phoenix/db/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/db/migrations/versions/cf03bd6bae1d_init.py` & `arize_phoenix-4.0.3/src/phoenix/db/migrations/versions/cf03bd6bae1d_init.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/inferences/errors.py` & `arize_phoenix-4.0.3/src/phoenix/inferences/errors.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/inferences/fixtures.py` & `arize_phoenix-4.0.3/src/phoenix/inferences/fixtures.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/inferences/inferences.py` & `arize_phoenix-4.0.3/src/phoenix/inferences/inferences.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/inferences/schema.py` & `arize_phoenix-4.0.3/src/phoenix/inferences/schema.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/inferences/validation.py` & `arize_phoenix-4.0.3/src/phoenix/inferences/validation.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/metrics/README.md` & `arize_phoenix-4.0.3/src/phoenix/metrics/README.md`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/metrics/__init__.py` & `arize_phoenix-4.0.3/src/phoenix/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/metrics/binning.py` & `arize_phoenix-4.0.3/src/phoenix/metrics/binning.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/metrics/metrics.py` & `arize_phoenix-4.0.3/src/phoenix/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/metrics/mixins.py` & `arize_phoenix-4.0.3/src/phoenix/metrics/mixins.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/metrics/retrieval_metrics.py` & `arize_phoenix-4.0.3/src/phoenix/metrics/retrieval_metrics.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/metrics/timeseries.py` & `arize_phoenix-4.0.3/src/phoenix/metrics/timeseries.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/metrics/wrappers.py` & `arize_phoenix-4.0.3/src/phoenix/metrics/wrappers.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/pointcloud/clustering.py` & `arize_phoenix-4.0.3/src/phoenix/pointcloud/clustering.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/pointcloud/pointcloud.py` & `arize_phoenix-4.0.3/src/phoenix/pointcloud/pointcloud.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/pointcloud/projectors.py` & `arize_phoenix-4.0.3/src/phoenix/pointcloud/projectors.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/pointcloud/umap_parameters.py` & `arize_phoenix-4.0.3/src/phoenix/pointcloud/umap_parameters.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/app.py` & `arize_phoenix-4.0.3/src/phoenix/server/app.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/grpc_server.py` & `arize_phoenix-4.0.3/src/phoenix/server/grpc_server.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/main.py` & `arize_phoenix-4.0.3/src/phoenix/server/main.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/prometheus.py` & `arize_phoenix-4.0.3/src/phoenix/server/prometheus.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/telemetry.py` & `arize_phoenix-4.0.3/src/phoenix/server/telemetry.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/thread_server.py` & `arize_phoenix-4.0.3/src/phoenix/server/thread_server.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/context.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/context.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/interceptor.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/interceptor.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/schema.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/schema.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/__init__.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/document_evaluation_summaries.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/document_evaluation_summaries.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/document_evaluations.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/document_evaluations.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/document_retrieval_metrics.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/document_retrieval_metrics.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/evaluation_summaries.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/evaluation_summaries.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/latency_ms_quantile.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/latency_ms_quantile.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/min_start_or_max_end_times.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/min_start_or_max_end_times.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/record_counts.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/record_counts.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/span_descendants.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/span_descendants.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/span_evaluations.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/span_evaluations.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/token_counts.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/token_counts.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/trace_evaluations.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/trace_evaluations.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/dataloaders/cache/two_tier_cache.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/dataloaders/cache/two_tier_cache.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/input_types/DataQualityMetricInput.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/input_types/DataQualityMetricInput.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/input_types/DimensionFilter.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/input_types/DimensionFilter.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/input_types/Granularity.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/input_types/Granularity.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/input_types/PerformanceMetricInput.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/input_types/PerformanceMetricInput.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/input_types/SpanSort.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/input_types/SpanSort.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/input_types/TimeRange.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/input_types/TimeRange.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/routers/utils.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/routers/utils.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/routers/v1/evaluations.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/routers/v1/evaluations.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/routers/v1/spans.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/routers/v1/spans.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/routers/v1/traces.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/routers/v1/traces.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/Cluster.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/Cluster.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/DataQualityMetric.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/DataQualityMetric.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/Dataset.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/Dataset.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/DatasetRole.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/DatasetRole.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/DatasetValues.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/DatasetValues.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/Dimension.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/Dimension.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/DimensionShape.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/DimensionShape.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/DimensionType.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/DimensionType.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/DocumentEvaluationSummary.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/DocumentEvaluationSummary.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/DocumentRetrievalMetrics.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/DocumentRetrievalMetrics.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/EmbeddingDimension.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/EmbeddingDimension.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/Evaluation.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/Evaluation.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/EvaluationSummary.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/EvaluationSummary.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/Event.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/Event.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/EventMetadata.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/EventMetadata.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/ExportEventsMutation.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/ExportEventsMutation.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/Model.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/Model.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/Project.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/Project.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/PromptResponse.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/PromptResponse.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/Segments.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/Segments.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/Span.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/Span.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/TimeSeries.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/Trace.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/Trace.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/UMAPPoints.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/UMAPPoints.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/node.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/node.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/api/types/pagination.py` & `arize_phoenix-4.0.3/src/phoenix/server/api/types/pagination.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/openapi/docs.py` & `arize_phoenix-4.0.3/src/phoenix/server/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon-114x114.png` & `arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon-120x120.png` & `arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon-144x144.png` & `arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon-152x152.png` & `arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon-180x180.png` & `arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon-72x72.png` & `arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon-76x76.png` & `arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/static/apple-touch-icon.png` & `arize_phoenix-4.0.3/src/phoenix/server/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/static/favicon.ico` & `arize_phoenix-4.0.3/src/phoenix/server/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/static/index.css` & `arize_phoenix-4.0.3/src/phoenix/server/static/index.css`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/static/index.js` & `arize_phoenix-4.0.3/src/phoenix/server/static/index.js`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/static/modernizr.js` & `arize_phoenix-4.0.3/src/phoenix/server/static/modernizr.js`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/server/templates/index.html` & `arize_phoenix-4.0.3/src/phoenix/server/templates/index.html`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/session/client.py` & `arize_phoenix-4.0.3/src/phoenix/session/client.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/session/data_extractor.py` & `arize_phoenix-4.0.3/src/phoenix/session/data_extractor.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/session/evaluation.py` & `arize_phoenix-4.0.3/src/phoenix/session/evaluation.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/session/session.py` & `arize_phoenix-4.0.3/src/phoenix/session/session.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/attributes.py` & `arize_phoenix-4.0.3/src/phoenix/trace/attributes.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/evaluation_conventions.py` & `arize_phoenix-4.0.3/src/phoenix/trace/evaluation_conventions.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/exporter.py` & `arize_phoenix-4.0.3/src/phoenix/trace/exporter.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/fixtures.py` & `arize_phoenix-4.0.3/src/phoenix/trace/fixtures.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/otel.py` & `arize_phoenix-4.0.3/src/phoenix/trace/otel.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/projects.py` & `arize_phoenix-4.0.3/src/phoenix/trace/projects.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/schemas.py` & `arize_phoenix-4.0.3/src/phoenix/trace/schemas.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/span_evaluations.py` & `arize_phoenix-4.0.3/src/phoenix/trace/span_evaluations.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/span_json_decoder.py` & `arize_phoenix-4.0.3/src/phoenix/trace/span_json_decoder.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/span_json_encoder.py` & `arize_phoenix-4.0.3/src/phoenix/trace/span_json_encoder.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/trace_dataset.py` & `arize_phoenix-4.0.3/src/phoenix/trace/trace_dataset.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/utils.py` & `arize_phoenix-4.0.3/src/phoenix/trace/utils.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/dsl/README.md` & `arize_phoenix-4.0.3/src/phoenix/trace/dsl/README.md`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/dsl/filter.py` & `arize_phoenix-4.0.3/src/phoenix/trace/dsl/filter.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/dsl/helpers.py` & `arize_phoenix-4.0.3/src/phoenix/trace/dsl/helpers.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/dsl/query.py` & `arize_phoenix-4.0.3/src/phoenix/trace/dsl/query.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/langchain/instrumentor.py` & `arize_phoenix-4.0.3/src/phoenix/trace/langchain/instrumentor.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/llama_index/callback.py` & `arize_phoenix-4.0.3/src/phoenix/trace/llama_index/callback.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/openai/instrumentor.py` & `arize_phoenix-4.0.3/src/phoenix/trace/openai/instrumentor.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/v1/evaluation_pb2.py` & `arize_phoenix-4.0.3/src/phoenix/trace/v1/evaluation_pb2.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/trace/v1/evaluation_pb2.pyi` & `arize_phoenix-4.0.3/src/phoenix/trace/v1/evaluation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/utilities/deprecation.py` & `arize_phoenix-4.0.3/src/phoenix/utilities/deprecation.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/src/phoenix/utilities/error_handling.py` & `arize_phoenix-4.0.3/src/phoenix/utilities/error_handling.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/LICENSE` & `arize_phoenix-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/README.md` & `arize_phoenix-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/pyproject.toml` & `arize_phoenix-4.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arize_phoenix-4.0.2/PKG-INFO` & `arize_phoenix-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arize-phoenix
-Version: 4.0.2
+Version: 4.0.3
 Summary: AI Observability and Evaluation
 Project-URL: Documentation, https://docs.arize.com/phoenix/
 Project-URL: Issues, https://github.com/Arize-ai/phoenix/issues
 Project-URL: Source, https://github.com/Arize-ai/phoenix
 Author-email: Arize AI <phoenix-devs@arize.com>
 License: Elastic-2.0
 License-File: IP_NOTICE
```

