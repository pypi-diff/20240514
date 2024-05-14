# Comparing `tmp/mistralrs_mkl-0.1.5.tar.gz` & `tmp/mistralrs_mkl-0.1.7.tar.gz`

## Comparing `mistralrs_mkl-0.1.5.tar` & `mistralrs_mkl-0.1.7.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0     1001      127      794 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-lora/Cargo.toml
--rw-r--r--   0     1001      127        0 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-lora/README.md
--rw-r--r--   0     1001      127     2429 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-lora/src/layer.rs
--rw-r--r--   0     1001      127     8618 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-lora/src/lib.rs
--rw-r--r--   0     1001      127    11219 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-lora/src/loralinear.rs
--rw-r--r--   0     1001      127    11929 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-lora/src/qloralinear.rs
--rw-r--r--   0     1001      127     2034 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/Cargo.toml
--rw-r--r--   0     1001      127        0 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/README.md
--rw-r--r--   0     1001      127      133 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/aici/README.md
--rw-r--r--   0     1001      127     6551 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/aici/bintokens.rs
--rw-r--r--   0     1001      127      320 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/aici/bytes.rs
--rw-r--r--   0     1001      127    15100 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/aici/cfg.rs
--rw-r--r--   0     1001      127     9819 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/aici/lex.rs
--rw-r--r--   0     1001      127      179 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/aici/mod.rs
--rw-r--r--   0     1001      127     2447 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/aici/recognizer.rs
--rw-r--r--   0     1001      127     1696 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/aici/rx.rs
--rw-r--r--   0     1001      127     3094 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/aici/svob.rs
--rw-r--r--   0     1001      127    17311 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/aici/toktree.rs
--rw-r--r--   0     1001      127     4674 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/device_map.rs
--rw-r--r--   0     1001      127    20762 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/engine/mod.rs
--rw-r--r--   0     1001      127    12620 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/layers.rs
--rw-r--r--   0     1001      127     7589 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/lib.rs
--rw-r--r--   0     1001      127     8538 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/model_loader.rs
--rw-r--r--   0     1001      127    10309 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/model_selected.rs
--rw-r--r--   0     1001      127    15657 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/models/gemma.rs
--rw-r--r--   0     1001      127    14521 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/models/llama.rs
--rw-r--r--   0     1001      127    16089 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/models/mistral.rs
--rw-r--r--   0     1001      127    20876 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/models/mixtral.rs
--rw-r--r--   0     1001      127     2877 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/models/mod.rs
--rw-r--r--   0     1001      127    15016 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/models/phi2.rs
--rw-r--r--   0     1001      127    15712 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/models/phi3.rs
--rw-r--r--   0     1001      127    18564 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/models/quantized_llama.rs
--rw-r--r--   0     1001      127     9221 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/models/quantized_phi2.rs
--rw-r--r--   0     1001      127    11195 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/models/quantized_phi3.rs
--rw-r--r--   0     1001      127    14488 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/models/qwen2.rs
--rw-r--r--   0     1001      127     5266 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/cache_manager.rs
--rw-r--r--   0     1001      127     5911 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/chat_template.rs
--rw-r--r--   0     1001      127    15865 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/ggml.rs
--rw-r--r--   0     1001      127    22111 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/gguf.rs
--rw-r--r--   0     1001      127    23366 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/loaders.rs
--rw-r--r--   0     1001      127    11539 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/macros.rs
--rw-r--r--   0     1001      127    45316 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/mod.rs
--rw-r--r--   0     1001      127    13640 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/normal.rs
--rw-r--r--   0     1001      127     3781 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/sampling.rs
--rw-r--r--   0     1001      127     9717 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/sampling_pipeline.rs
--rw-r--r--   0     1001      127    17616 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/speculative.rs
--rw-r--r--   0     1001      127     6693 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/prefix_cacher.rs
--rw-r--r--   0     1001      127     2116 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/request.rs
--rw-r--r--   0     1001      127     3848 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/response.rs
--rw-r--r--   0     1001      127    14833 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/sampler.rs
--rw-r--r--   0     1001      127     9205 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/scheduler.rs
--rw-r--r--   0     1001      127    18360 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/sequence.rs
--rw-r--r--   0     1001      127    14577 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/toml_selector.rs
--rw-r--r--   0     1001      127     7848 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/utils/mod.rs
--rw-r--r--   0     1001      127     1716 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/utils/tokens.rs
--rw-r--r--   0     1001      127     6749 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/utils/varbuilder_utils.rs
--rw-r--r--   0     1001      127    11049 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/classifier.rs
--rw-r--r--   0     1001      127     1544 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/config.rs
--rw-r--r--   0     1001      127    26953 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/gemma.rs
--rw-r--r--   0     1001      127    26176 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/llama.rs
--rw-r--r--   0     1001      127    27604 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/mistral.rs
--rw-r--r--   0     1001      127    33531 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/mixtral.rs
--rw-r--r--   0     1001      127     4388 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/mod.rs
--rw-r--r--   0     1001      127    25539 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/phi2.rs
--rw-r--r--   0     1001      127    25038 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/phi3.rs
--rw-r--r--   0     1001      127    36716 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/quantized_llama.rs
--rw-r--r--   0     1001      127    19395 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/quantized_phi3.rs
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.5/mistralrs-pyo3/Cargo.toml
--rw-r--r--   0     1001      127      686 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-pyo3/.gitignore
--rw-r--r--   0     1001      127     3358 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-pyo3/API.md
--rw-r--r--   0     1001      127      927 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-pyo3/Cargo_template.toml
--rw-r--r--   0     1001      127     3755 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-pyo3/README.md
--rw-r--r--   0     1001      127       71 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-pyo3/build.rs
--rw-r--r--   0     1001      127     8688 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-pyo3/mistralrs.pyi
--rw-r--r--   0     1001      127      530 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-pyo3/pyproject_template.toml
--rw-r--r--   0     1001      127    29216 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-pyo3/src/lib.rs
--rw-r--r--   0     1001      127     1672 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-pyo3/src/stream.rs
--rw-r--r--   0     1001      127     3020 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-pyo3/src/which.rs
--rwxr-xr-x   0     1001      127     2203 2024-05-13 09:33:43.000000 mistralrs_mkl-0.1.5/mistralrs-pyo3/upload.py
--rw-r--r--   0     1001      127   100112 2024-05-13 09:34:10.000000 mistralrs_mkl-0.1.5/Cargo.lock
--rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.5/Cargo.toml
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4449 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.5/PKG-INFO
+-rw-r--r--   0     1001      127      794 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-lora/Cargo.toml
+-rw-r--r--   0     1001      127        0 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-lora/README.md
+-rw-r--r--   0     1001      127     2429 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-lora/src/layer.rs
+-rw-r--r--   0     1001      127     8618 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-lora/src/lib.rs
+-rw-r--r--   0     1001      127    11219 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-lora/src/loralinear.rs
+-rw-r--r--   0     1001      127    11929 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-lora/src/qloralinear.rs
+-rw-r--r--   0     1001      127     2063 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/Cargo.toml
+-rw-r--r--   0     1001      127        0 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/README.md
+-rw-r--r--   0     1001      127      133 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/README.md
+-rw-r--r--   0     1001      127     6551 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/bintokens.rs
+-rw-r--r--   0     1001      127      320 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/bytes.rs
+-rw-r--r--   0     1001      127    15100 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/cfg.rs
+-rw-r--r--   0     1001      127     9819 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/lex.rs
+-rw-r--r--   0     1001      127      179 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/mod.rs
+-rw-r--r--   0     1001      127     2447 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/recognizer.rs
+-rw-r--r--   0     1001      127     1696 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/rx.rs
+-rw-r--r--   0     1001      127     3094 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/svob.rs
+-rw-r--r--   0     1001      127    17311 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/toktree.rs
+-rw-r--r--   0     1001      127     4674 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/device_map.rs
+-rw-r--r--   0     1001      127    21173 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/engine/mod.rs
+-rw-r--r--   0     1001      127    12620 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/layers.rs
+-rw-r--r--   0     1001      127     7871 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/lib.rs
+-rw-r--r--   0     1001      127     8538 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/model_loader.rs
+-rw-r--r--   0     1001      127    10309 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/model_selected.rs
+-rw-r--r--   0     1001      127    15657 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/gemma.rs
+-rw-r--r--   0     1001      127    14521 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/llama.rs
+-rw-r--r--   0     1001      127    16089 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/mistral.rs
+-rw-r--r--   0     1001      127    20876 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/mixtral.rs
+-rw-r--r--   0     1001      127     2877 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/mod.rs
+-rw-r--r--   0     1001      127    15016 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/phi2.rs
+-rw-r--r--   0     1001      127    15712 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/phi3.rs
+-rw-r--r--   0     1001      127    18564 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/quantized_llama.rs
+-rw-r--r--   0     1001      127     9221 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/quantized_phi2.rs
+-rw-r--r--   0     1001      127    11195 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/quantized_phi3.rs
+-rw-r--r--   0     1001      127    14488 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/qwen2.rs
+-rw-r--r--   0     1001      127     5266 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/cache_manager.rs
+-rw-r--r--   0     1001      127     5911 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/chat_template.rs
+-rw-r--r--   0     1001      127    15865 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/ggml.rs
+-rw-r--r--   0     1001      127    22111 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/gguf.rs
+-rw-r--r--   0     1001      127    23366 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/loaders.rs
+-rw-r--r--   0     1001      127    11539 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/macros.rs
+-rw-r--r--   0     1001      127    45316 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/mod.rs
+-rw-r--r--   0     1001      127    13640 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/normal.rs
+-rw-r--r--   0     1001      127     3781 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/sampling.rs
+-rw-r--r--   0     1001      127     9717 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/sampling_pipeline.rs
+-rw-r--r--   0     1001      127    17616 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/speculative.rs
+-rw-r--r--   0     1001      127     6693 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/prefix_cacher.rs
+-rw-r--r--   0     1001      127     2116 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/request.rs
+-rw-r--r--   0     1001      127     3848 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/response.rs
+-rw-r--r--   0     1001      127    14833 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/sampler.rs
+-rw-r--r--   0     1001      127     9630 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/scheduler.rs
+-rw-r--r--   0     1001      127    18535 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/sequence.rs
+-rw-r--r--   0     1001      127    14577 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/toml_selector.rs
+-rw-r--r--   0     1001      127     7848 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/utils/mod.rs
+-rw-r--r--   0     1001      127     1716 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/utils/tokens.rs
+-rw-r--r--   0     1001      127     6749 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/utils/varbuilder_utils.rs
+-rw-r--r--   0     1001      127    11049 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/classifier.rs
+-rw-r--r--   0     1001      127     1544 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/config.rs
+-rw-r--r--   0     1001      127    26953 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/gemma.rs
+-rw-r--r--   0     1001      127    26176 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/llama.rs
+-rw-r--r--   0     1001      127    27604 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/mistral.rs
+-rw-r--r--   0     1001      127    33531 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/mixtral.rs
+-rw-r--r--   0     1001      127     4388 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/mod.rs
+-rw-r--r--   0     1001      127    25539 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/phi2.rs
+-rw-r--r--   0     1001      127    25038 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/phi3.rs
+-rw-r--r--   0     1001      127    36716 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/quantized_llama.rs
+-rw-r--r--   0     1001      127    19395 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/quantized_phi3.rs
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/.gitignore
+-rw-r--r--   0     1001      127     3358 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/API.md
+-rw-r--r--   0     1001      127      927 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/Cargo_template.toml
+-rw-r--r--   0     1001      127     3755 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/README.md
+-rw-r--r--   0     1001      127       71 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/build.rs
+-rw-r--r--   0     1001      127     8688 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/mistralrs.pyi
+-rw-r--r--   0     1001      127      530 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/pyproject_template.toml
+-rw-r--r--   0     1001      127    29216 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/src/lib.rs
+-rw-r--r--   0     1001      127     1672 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/src/stream.rs
+-rw-r--r--   0     1001      127     3020 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/src/which.rs
+-rwxr-xr-x   0     1001      127     2203 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/upload.py
+-rw-r--r--   0     1001      127   100818 2024-05-14 12:14:03.000000 mistralrs_mkl-0.1.7/Cargo.lock
+-rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.7/Cargo.toml
+-rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4449 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.7/PKG-INFO
```

### Comparing `mistralrs_mkl-0.1.5/mistralrs-lora/Cargo.toml` & `mistralrs_mkl-0.1.7/mistralrs-lora/Cargo.toml`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-lora/src/layer.rs` & `mistralrs_mkl-0.1.7/mistralrs-lora/src/layer.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-lora/src/lib.rs` & `mistralrs_mkl-0.1.7/mistralrs-lora/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-lora/src/loralinear.rs` & `mistralrs_mkl-0.1.7/mistralrs-lora/src/loralinear.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-lora/src/qloralinear.rs` & `mistralrs_mkl-0.1.7/mistralrs-lora/src/qloralinear.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/Cargo.toml` & `mistralrs_mkl-0.1.7/mistralrs-core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 dirs = "5.0.1"
 hf-hub = "0.3.2"
 thiserror = "1.0.57"
 tokenizers = "0.15.2"
 tqdm = "0.7.0"
 range-checked = { git = "https://github.com/EricLBuehler/range-checked.git", version = "0.1.0" }
 chrono = "0.4.34"
-mistralrs-lora = { version = "0.1.5", path = "../mistralrs-lora" }
+mistralrs-lora = { version = "0.1.7", path = "../mistralrs-lora" }
 minijinja = "1.0.12"
 either.workspace = true
 indexmap.workspace = true
 half = "2.4.0"
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 tracing.workspace = true
@@ -50,16 +50,18 @@
 tokio-rayon = "2.1.0"
 rand_isaac = "0.3.0"
 futures.workspace = true
 indicatif = { version = "0.17.8", features = ["rayon"] }
 async-trait = "0.1.80"
 once_cell = "1.19.0"
 toml = "0.8.12"
+ctrlc = "3.4.4"
 
 [features]
 cuda = ["candle-core/cuda", "candle-nn/cuda", "candle-transformers/cuda"]
 cudnn = ["candle-core/cudnn"]
 metal = ["candle-core/metal", "candle-nn/metal", "candle-transformers/metal"]
 flash-attn = ["cuda", "candle-transformers/flash-attn", "dep:candle-flash-attn"]
 accelerate = ["candle-core/accelerate", "candle-nn/accelerate", "candle-transformers/accelerate"]
 mkl = ["candle-core/mkl", "candle-nn/mkl", "candle-transformers/mkl"]
+profile = []
```

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/aici/bintokens.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/aici/bintokens.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/aici/cfg.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/aici/cfg.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/aici/lex.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/aici/lex.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/aici/recognizer.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/aici/recognizer.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/aici/rx.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/aici/rx.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/aici/svob.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/aici/svob.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/aici/toktree.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/aici/toktree.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/device_map.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/device_map.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/engine/mod.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/engine/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 use std::{
     collections::{HashMap, VecDeque},
-    sync::Arc,
+    sync::{
+        atomic::{AtomicBool, Ordering},
+        Arc,
+    },
     time::{Instant, SystemTime, UNIX_EPOCH},
 };
 use tokio::sync::{mpsc::Receiver, Mutex};
 
 use crate::{
     aici::{cfg::CfgParser, recognizer::StackRecognizer, rx::RecRx},
     pipeline::{AdapterInstruction, CacheInstruction},
@@ -26,14 +29,15 @@
     sampler::Sampler,
     scheduler::{Scheduler, SchedulerMethod},
     sequence::{Sequence, SequenceGroup, SequenceRecognizer, SequenceState},
     Constraint, StopTokens,
 };
 
 const SEED: u64 = 0;
+pub(crate) static TERMINATE_ALL_NEXT_STEP: AtomicBool = AtomicBool::new(false);
 
 pub struct Engine {
     rx: Receiver<Request>,
     pipeline: Arc<Mutex<dyn Pipeline>>,
     scheduler: Scheduler<VecDeque<Sequence>>,
     id: usize,
     truncate_sequence: bool,
@@ -50,17 +54,24 @@
         pipeline: Arc<Mutex<dyn Pipeline>>,
         method: SchedulerMethod,
         truncate_sequence: bool,
         no_kv_cache: bool,
         no_prefix_cache: bool,
         prefix_cache_n: usize,
         disable_eos_stop: bool,
+        interactive: bool,
     ) -> Self {
         let device = get_mut_arcmutex!(pipeline).device().clone();
         let is_xlora = get_mut_arcmutex!(pipeline).get_metadata().is_xlora;
+        if interactive {
+            ctrlc::set_handler(move || {
+                TERMINATE_ALL_NEXT_STEP.store(true, Ordering::SeqCst);
+            })
+            .expect("Failed to set CTRL-C handler for interactive mode");
+        }
         Self {
             rx,
             pipeline,
             scheduler: Scheduler::new(method),
             id: 0,
             truncate_sequence,
             no_kv_cache,
@@ -198,15 +209,15 @@
                     seq.prompt_tok_per_sec = prompt_tok_per_sec * 1000.;
                     seq.prompt_timestamp = Some(now);
                 }
                 last_completion_ids = vec![];
             }
 
             if self.is_debug {
-                let ms_from_last_run = run_start.elapsed().as_millis();
+                let ms_from_last_run = run_start.elapsed().as_secs_f64();
                 let total_len = scheduled.prompt.len() + scheduled.completion.len();
                 if total_len > 0 {
                     let prompt_lengths = scheduled
                         .prompt
                         .iter()
                         .map(|seq| seq.len().to_string())
                         .collect::<Vec<_>>()
@@ -219,15 +230,15 @@
                         .collect::<Vec<_>>()
                         .join(", ");
 
                     tracing::info!(
                         "Prompt[{}] Completion[{}] - {}ms",
                         prompt_lengths,
                         completion_lengths,
-                        ms_from_last_run
+                        ms_from_last_run * 1000.,
                     );
                 }
             }
             if scheduled.prompt.len() == 0
                 && scheduled.completion.len() == 0
                 && self.scheduler.waiting_len() == 0
             {
```

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/layers.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/layers.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/lib.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -73,27 +73,29 @@
     method: SchedulerMethod,
     log: Option<String>,
     truncate_sequence: Option<bool>,
     no_kv_cache: Option<bool>,
     no_prefix_cache: Option<bool>,
     prefix_cache_n: Option<usize>,
     disable_eos_stop: Option<bool>,
+    interactive: Option<bool>,
 }
 
 impl MistralRsBuilder {
     pub fn new(pipeline: Arc<tokio::sync::Mutex<dyn Pipeline>>, method: SchedulerMethod) -> Self {
         Self {
             pipeline,
             method,
             log: None,
             truncate_sequence: None,
             no_kv_cache: None,
             no_prefix_cache: None,
             prefix_cache_n: None,
             disable_eos_stop: None,
+            interactive: None,
         }
     }
 
     pub fn with_log(mut self, log: String) -> Self {
         self.log = Some(log);
         self
     }
@@ -117,14 +119,18 @@
         self.prefix_cache_n = Some(prefix_cache_n);
         self
     }
     pub fn with_disable_eos_stop(mut self, disable_eos_stop: bool) -> Self {
         self.disable_eos_stop = Some(disable_eos_stop);
         self
     }
+    pub fn with_interactive(mut self) -> Self {
+        self.interactive = Some(true);
+        self
+    }
 
     pub fn build(self) -> Arc<MistralRs> {
         MistralRs::new(self)
     }
 }
 
 impl MistralRs {
@@ -134,21 +140,23 @@
             method,
             log,
             truncate_sequence,
             no_kv_cache,
             no_prefix_cache,
             prefix_cache_n,
             disable_eos_stop,
+            interactive,
         } = config;
 
         let truncate_sequence = truncate_sequence.unwrap_or(false);
         let no_kv_cache = no_kv_cache.unwrap_or(false);
         let no_prefix_cache = no_prefix_cache.unwrap_or(false);
         let prefix_cache_n = prefix_cache_n.unwrap_or(16);
         let disable_eos_stop = disable_eos_stop.unwrap_or(false);
+        let interactive = interactive.unwrap_or(false);
 
         let (tx, rx) = channel(10_000);
 
         let this = Arc::new(Self {
             sender: tx,
             log,
             id: pipeline.try_lock().unwrap().name(),
@@ -166,14 +174,15 @@
                     pipeline,
                     method,
                     truncate_sequence,
                     no_kv_cache,
                     no_prefix_cache,
                     prefix_cache_n,
                     disable_eos_stop,
+                    interactive,
                 );
                 engine.run().await;
             });
         });
 
         this
     }
```

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/model_loader.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/model_loader.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/model_selected.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/model_selected.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/models/gemma.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/models/gemma.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/models/llama.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/models/llama.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/models/mistral.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/models/mistral.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/models/mixtral.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/models/mixtral.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/models/mod.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/models/phi2.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/models/phi2.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/models/phi3.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/models/phi3.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/models/quantized_llama.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/models/quantized_llama.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/models/quantized_phi2.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/models/quantized_phi2.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/models/quantized_phi3.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/models/quantized_phi3.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/models/qwen2.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/models/qwen2.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/cache_manager.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/cache_manager.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/chat_template.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/chat_template.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/ggml.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/ggml.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/gguf.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/gguf.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/loaders.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/loaders.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/macros.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/macros.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/mod.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/normal.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/normal.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/sampling.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/sampling.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/sampling_pipeline.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/sampling_pipeline.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/pipeline/speculative.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/speculative.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/prefix_cacher.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/prefix_cacher.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/request.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/request.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/response.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/response.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/sampler.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/sampler.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/scheduler.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/scheduler.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,16 @@
-use std::collections::{HashMap, VecDeque};
-
-use crate::sequence::{Sequence, SequenceState};
+use std::{
+    collections::{HashMap, VecDeque},
+    sync::atomic::Ordering,
+};
+
+use crate::{
+    engine::TERMINATE_ALL_NEXT_STEP,
+    sequence::{Sequence, SequenceState, StopReason},
+};
 use range_checked::UsizeBounded;
 
 pub trait FcfsBacker: Default {
     fn new() -> Self;
     fn add(&mut self, item: Sequence);
     fn into_iter(self) -> impl Iterator<Item = Sequence>;
     fn len(&self) -> usize;
@@ -210,14 +216,20 @@
                 return SchedulerOutput {
                     prompt: self.running.iter_mut().collect::<Vec<_>>().into(),
                     completion: vec![].into(),
                 };
             }
             (0, _) => {
                 self.running = self.bucket_and_waitlist_seqs(running);
+                if TERMINATE_ALL_NEXT_STEP.load(Ordering::SeqCst) {
+                    self.running
+                        .iter_mut()
+                        .for_each(|seq| seq.set_state(SequenceState::Done(StopReason::Canceled)));
+                    TERMINATE_ALL_NEXT_STEP.store(false, Ordering::SeqCst);
+                }
                 return SchedulerOutput {
                     prompt: vec![].into(),
                     completion: self.running.iter_mut().collect::<Vec<_>>().into(),
                 };
             }
             _ => {}
         }
```

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/sequence.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/sequence.rs`

 * *Files 1% similar despite different names*

```diff
@@ -355,14 +355,19 @@
     ) -> Option<StopReason> {
         let is_eos = match eos_tok {
             Some(eos_tok) => eos_tok.iter().any(|t| *t == tok),
             None => false,
         };
         if is_eos {
             Some(StopReason::Eos)
+        } else if matches!(
+            &*self.state.read().unwrap(),
+            SequenceState::Done(StopReason::Canceled)
+        ) {
+            Some(StopReason::Canceled)
         } else if self.stop_tokens.contains(&tok) {
             Some(StopReason::StopTok(tok))
         } else if self.max_len.is_some()
             && self.tokens.len().saturating_sub(self.prompt_len) == self.max_len.unwrap()
         {
             // add_token was already called
             Some(StopReason::Length(self.max_len.unwrap()))
```

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/toml_selector.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/toml_selector.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/utils/mod.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/utils/tokens.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/utils/tokens.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/utils/varbuilder_utils.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/utils/varbuilder_utils.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/classifier.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/classifier.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/config.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/config.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/gemma.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/gemma.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/llama.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/llama.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/mistral.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/mistral.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/mixtral.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/mixtral.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/mod.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/phi2.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/phi2.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/phi3.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/phi3.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/quantized_llama.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/quantized_llama.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-core/src/xlora_models/quantized_phi3.rs` & `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/quantized_phi3.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-pyo3/Cargo.toml` & `mistralrs_mkl-0.1.7/mistralrs-pyo3/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [lib]
 name = "mistralrs"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3.workspace = true
-mistralrs-core = { version = "0.1.5", path = "../mistralrs-core", features=["mkl"] }
+mistralrs-core = { version = "0.1.7", path = "../mistralrs-core", features=["mkl"] }
 serde.workspace = true
 serde_json.workspace = true
 candle-core = { git = "https://github.com/EricLBuehler/candle.git", version = "0.5.0", features=["mkl"] }
 indexmap.workspace = true
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 either.workspace = true
```

### Comparing `mistralrs_mkl-0.1.5/mistralrs-pyo3/.gitignore` & `mistralrs_mkl-0.1.7/mistralrs-pyo3/.gitignore`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-pyo3/API.md` & `mistralrs_mkl-0.1.7/mistralrs-pyo3/API.md`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-pyo3/Cargo_template.toml` & `mistralrs_mkl-0.1.7/mistralrs-pyo3/Cargo_template.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [lib]
 name = "mistralrs"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3.workspace = true
-mistralrs-core = { version = "0.1.5", path = "../mistralrs-core", features=["$feature_name"] }
+mistralrs-core = { version = "0.1.7", path = "../mistralrs-core", features=["$feature_name"] }
 serde.workspace = true
 serde_json.workspace = true
 candle-core = { git = "https://github.com/EricLBuehler/candle.git", version = "0.5.0", features=["$feature_name"] }
 indexmap.workspace = true
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 either.workspace = true
```

### Comparing `mistralrs_mkl-0.1.5/mistralrs-pyo3/README.md` & `mistralrs_mkl-0.1.7/mistralrs-pyo3/README.md`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-pyo3/mistralrs.pyi` & `mistralrs_mkl-0.1.7/mistralrs-pyo3/mistralrs.pyi`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-pyo3/pyproject_template.toml` & `mistralrs_mkl-0.1.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["maturin==1.4"]
 build-backend = "maturin"
 
 [project]
-name = "$name"
-version = "0.1.5"
+name = "mistralrs-mkl"
+version = "0.1.7"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Rust",
 ]
 dynamic = ["description"]
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
+manifest-path = "mistralrs-pyo3/Cargo.toml"
```

### Comparing `mistralrs_mkl-0.1.5/mistralrs-pyo3/src/lib.rs` & `mistralrs_mkl-0.1.7/mistralrs-pyo3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-pyo3/src/stream.rs` & `mistralrs_mkl-0.1.7/mistralrs-pyo3/src/stream.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-pyo3/src/which.rs` & `mistralrs_mkl-0.1.7/mistralrs-pyo3/src/which.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/mistralrs-pyo3/upload.py` & `mistralrs_mkl-0.1.7/mistralrs-pyo3/upload.py`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.5/Cargo.lock` & `mistralrs_mkl-0.1.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -300,17 +300,17 @@
 name = "bumpalo"
 version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
+checksum = "78834c15cb5d5efe3452d58b1e8ba890dd62d21907f867f383358198e56ebca5"
 dependencies = [
  "bytemuck_derive",
 ]
 
 [[package]]
 name = "bytemuck_derive"
 version = "1.6.0"
@@ -452,14 +452,20 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "cfg_aliases"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fd16c4719339c4530435d38e511904438d07cce7950afa3718a84ac36c10e89e"
+
+[[package]]
 name = "cfgrammar"
 version = "0.13.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "163348850b1cd34fa99ef1592b5d598ea7e6752f18aff2125b67537e887edb36"
 dependencies = [
  "indexmap",
  "lazy_static",
@@ -716,14 +722,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5efa2b3d7902f4b634a20cae3c9c4e6209dc4779feb6863329607560143efa70"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "ctrlc"
+version = "3.4.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "672465ae37dc1bc6380a6547a8883d5dd397b0f1faaad4f265726cc7042a5345"
+dependencies = [
+ "nix",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "cudarc"
 version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c415f24c56f0bd4e0568e3ceea0bae6e5a1a96bda8ac177d0b6d7fcc7fa8de7a"
 dependencies = [
  "half",
  "libloading",
@@ -1860,26 +1876,26 @@
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "mistralrs"
-version = "0.1.5"
+version = "0.1.7"
 dependencies = [
  "anyhow",
  "candle-core",
  "mistralrs-core",
  "serde_json",
  "tokio",
 ]
 
 [[package]]
 name = "mistralrs-bench"
-version = "0.1.5"
+version = "0.1.7"
 dependencies = [
  "anyhow",
  "candle-core",
  "clap",
  "cli-table",
  "either",
  "mistralrs-core",
@@ -1888,27 +1904,28 @@
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "mistralrs-core"
-version = "0.1.5"
+version = "0.1.7"
 dependencies = [
  "accelerate-src",
  "anyhow",
  "async-trait",
  "bytemuck",
  "candle-core",
  "candle-flash-attn",
  "candle-nn",
  "candle-transformers",
  "cfgrammar",
  "chrono",
  "clap",
+ "ctrlc",
  "dirs",
  "either",
  "futures",
  "galil-seiferas",
  "half",
  "hf-hub",
  "indexmap",
@@ -1936,28 +1953,28 @@
  "tqdm",
  "tracing",
  "vob",
 ]
 
 [[package]]
 name = "mistralrs-lora"
-version = "0.1.5"
+version = "0.1.7"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "candle-nn",
  "either",
  "intel-mkl-src",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "mistralrs-pyo3"
-version = "0.1.5"
+version = "0.1.7"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "either",
  "futures",
  "indexmap",
  "intel-mkl-src",
@@ -1968,15 +1985,15 @@
  "serde_json",
  "tokio",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "mistralrs-server"
-version = "0.1.5"
+version = "0.1.7"
 dependencies = [
  "accelerate-src",
  "anyhow",
  "axum",
  "candle-core",
  "clap",
  "dyn-fmt",
@@ -2040,14 +2057,26 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77a5d83df9f36fe23f0c3648c6bbb8b0298bb5f1939c8f2704431371f4b84d43"
 dependencies = [
  "smallvec",
 ]
 
 [[package]]
+name = "nix"
+version = "0.28.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ab2156c4fce2f8df6c499cc1c763e4394b7482525bf2a9701c9d79d215f519e4"
+dependencies = [
+ "bitflags 2.5.0",
+ "cfg-if",
+ "cfg_aliases",
+ "libc",
+]
+
+[[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
```

### Comparing `mistralrs_mkl-0.1.5/Cargo.toml` & `mistralrs_mkl-0.1.7/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["mistralrs-core", "mistralrs-lora", "mistralrs-pyo3"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.5"
+version = "0.1.7"
 edition = "2021"
 description = "Fast and easy LLM serving."
 homepage = "https://github.com/EricLBuehler/mistral.rs"
 repository = "https://github.com/EricLBuehler/mistral.rs"
 keywords = ["machine-learning"]
 categories = ["science"]
 license = "MIT"
```

### Comparing `mistralrs_mkl-0.1.5/PKG-INFO` & `mistralrs_mkl-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistralrs-mkl
-Version: 0.1.5
+Version: 0.1.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Rust
 Summary: Fast and easy LLM serving.
```

