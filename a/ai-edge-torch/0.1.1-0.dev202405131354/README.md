# Comparing `tmp/ai_edge_torch-0.1.1-py3-none-any.whl.zip` & `tmp/ai_edge_torch-0.dev202405131354-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,93 +1,93 @@
-Zip file size: 138720 bytes, number of entries: 91
--rw-r--r--  2.0 unx     1008 b- defN 24-May-13 17:28 ai_edge_torch/__init__.py
--rw-r--r--  2.0 unx     4243 b- defN 24-May-13 17:28 ai_edge_torch/model.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:28 ai_edge_torch/convert/__init__.py
--rw-r--r--  2.0 unx     4043 b- defN 24-May-13 17:28 ai_edge_torch/convert/conversion.py
--rw-r--r--  2.0 unx    11021 b- defN 24-May-13 17:28 ai_edge_torch/convert/conversion_utils.py
--rw-r--r--  2.0 unx     6927 b- defN 24-May-13 17:28 ai_edge_torch/convert/converter.py
--rw-r--r--  2.0 unx     2825 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/__init__.py
--rw-r--r--  2.0 unx     1652 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/_pass_base.py
--rw-r--r--  2.0 unx     6150 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/build_aten_composite_pass.py
--rw-r--r--  2.0 unx     2607 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/build_upsample_bilinear2d_composite_pass.py
--rw-r--r--  2.0 unx     1673 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/canonicalize_pass.py
--rw-r--r--  2.0 unx     2448 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/inject_mlir_debuginfo_pass.py
--rw-r--r--  2.0 unx      795 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/__init__.py
--rw-r--r--  2.0 unx     6870 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_check.py
--rw-r--r--  2.0 unx     1560 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_mark.py
--rw-r--r--  2.0 unx    12438 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_rewrite.py
--rw-r--r--  2.0 unx      982 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/op_func_registry.py
--rw-r--r--  2.0 unx    10030 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/pass_body.py
--rw-r--r--  2.0 unx     2076 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/utils.py
--rw-r--r--  2.0 unx      715 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/__init__.py
--rw-r--r--  2.0 unx     2279 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/greedy.py
--rw-r--r--  2.0 unx     6432 b- defN 24-May-13 17:28 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/min_cut.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:28 ai_edge_torch/convert/test/__init__.py
--rw-r--r--  2.0 unx     8092 b- defN 24-May-13 17:28 ai_edge_torch/convert/test/test_convert.py
--rw-r--r--  2.0 unx     6403 b- defN 24-May-13 17:28 ai_edge_torch/convert/test/test_convert_composites.py
--rw-r--r--  2.0 unx     4537 b- defN 24-May-13 17:28 ai_edge_torch/convert/test/test_convert_multisig.py
--rw-r--r--  2.0 unx      707 b- defN 24-May-13 17:28 ai_edge_torch/debug/__init__.py
--rw-r--r--  2.0 unx    12789 b- defN 24-May-13 17:28 ai_edge_torch/debug/culprit.py
--rw-r--r--  2.0 unx     1430 b- defN 24-May-13 17:28 ai_edge_torch/debug/utils.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:28 ai_edge_torch/debug/test/__init__.py
--rw-r--r--  2.0 unx     3731 b- defN 24-May-13 17:28 ai_edge_torch/debug/test/test_culprit.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:28 ai_edge_torch/experimental/__init__.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:28 ai_edge_torch/generative/__init__.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/__init__.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/gemma/__init__.py
--rw-r--r--  2.0 unx     2538 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/gemma/convert_to_tflite.py
--rw-r--r--  2.0 unx     5913 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/gemma/gemma.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/phi2/__init__.py
--rw-r--r--  2.0 unx     2512 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/phi2/convert_to_tflite.py
--rw-r--r--  2.0 unx     5540 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/phi2/phi2.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/t5/__init__.py
--rw-r--r--  2.0 unx     4536 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/t5/convert_to_tflite.py
--rw-r--r--  2.0 unx    21065 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/t5/t5.py
--rw-r--r--  2.0 unx     8998 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/t5/t5_attention.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/test_models/__init__.py
--rw-r--r--  2.0 unx     3791 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/test_models/toy_model.py
--rw-r--r--  2.0 unx     4831 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/test_models/toy_model_with_kv_cache.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/tiny_llama/__init__.py
--rw-r--r--  2.0 unx     2566 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/tiny_llama/convert_to_tflite.py
--rw-r--r--  2.0 unx     5629 b- defN 24-May-13 17:28 ai_edge_torch/generative/examples/tiny_llama/tiny_llama.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:28 ai_edge_torch/generative/layers/__init__.py
--rw-r--r--  2.0 unx     9127 b- defN 24-May-13 17:28 ai_edge_torch/generative/layers/attention.py
--rw-r--r--  2.0 unx     6350 b- defN 24-May-13 17:28 ai_edge_torch/generative/layers/attention_utils.py
--rw-r--r--  2.0 unx     3201 b- defN 24-May-13 17:28 ai_edge_torch/generative/layers/builder.py
--rw-r--r--  2.0 unx     2820 b- defN 24-May-13 17:28 ai_edge_torch/generative/layers/feed_forward.py
--rw-r--r--  2.0 unx     3090 b- defN 24-May-13 17:28 ai_edge_torch/generative/layers/kv_cache.py
--rw-r--r--  2.0 unx     4064 b- defN 24-May-13 17:28 ai_edge_torch/generative/layers/model_config.py
--rw-r--r--  2.0 unx     1867 b- defN 24-May-13 17:28 ai_edge_torch/generative/layers/normalization.py
--rw-r--r--  2.0 unx     1383 b- defN 24-May-13 17:28 ai_edge_torch/generative/layers/rotary_position_embedding.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:28 ai_edge_torch/generative/quantize/__init__.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-13 17:28 ai_edge_torch/generative/quantize/example.py
--rw-r--r--  2.0 unx     1862 b- defN 24-May-13 17:28 ai_edge_torch/generative/quantize/quant_attrs.py
--rw-r--r--  2.0 unx     3327 b- defN 24-May-13 17:28 ai_edge_torch/generative/quantize/quant_recipe.py
--rw-r--r--  2.0 unx     1913 b- defN 24-May-13 17:28 ai_edge_torch/generative/quantize/quant_recipe_utils.py
--rw-r--r--  2.0 unx     1798 b- defN 24-May-13 17:28 ai_edge_torch/generative/quantize/quant_recipes.py
--rw-r--r--  2.0 unx     1345 b- defN 24-May-13 17:28 ai_edge_torch/generative/quantize/supported_schemes.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:28 ai_edge_torch/generative/test/__init__.py
--rw-r--r--  2.0 unx     6500 b- defN 24-May-13 17:28 ai_edge_torch/generative/test/test_model_conversion.py
--rw-r--r--  2.0 unx     3728 b- defN 24-May-13 17:28 ai_edge_torch/generative/test/test_quantize.py
--rw-r--r--  2.0 unx      720 b- defN 24-May-13 17:28 ai_edge_torch/generative/utilities/__init__.py
--rw-r--r--  2.0 unx    10029 b- defN 24-May-13 17:28 ai_edge_torch/generative/utilities/loader.py
--rw-r--r--  2.0 unx    16156 b- defN 24-May-13 17:28 ai_edge_torch/generative/utilities/t5_loader.py
--rw-r--r--  2.0 unx      752 b- defN 24-May-13 17:28 ai_edge_torch/hlfb/__init__.py
--rw-r--r--  2.0 unx     4799 b- defN 24-May-13 17:28 ai_edge_torch/hlfb/mark_pattern/__init__.py
--rw-r--r--  2.0 unx     1539 b- defN 24-May-13 17:28 ai_edge_torch/hlfb/mark_pattern/passes.py
--rw-r--r--  2.0 unx     9206 b- defN 24-May-13 17:28 ai_edge_torch/hlfb/mark_pattern/pattern.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:28 ai_edge_torch/hlfb/test/__init__.py
--rw-r--r--  2.0 unx     4262 b- defN 24-May-13 17:28 ai_edge_torch/hlfb/test/test_mark_pattern.py
--rw-r--r--  2.0 unx     8190 b- defN 24-May-13 17:28 ai_edge_torch/hlfb/test/test_stablehlo_composite_builder.py
--rw-r--r--  2.0 unx      714 b- defN 24-May-13 17:28 ai_edge_torch/quantize/__init__.py
--rw-r--r--  2.0 unx    15602 b- defN 24-May-13 17:28 ai_edge_torch/quantize/pt2e_quantizer.py
--rw-r--r--  2.0 unx    36046 b- defN 24-May-13 17:28 ai_edge_torch/quantize/pt2e_quantizer_utils.py
--rw-r--r--  2.0 unx     3435 b- defN 24-May-13 17:28 ai_edge_torch/quantize/quant_config.py
--rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:28 ai_edge_torch/testing/__init__.py
--rw-r--r--  2.0 unx      765 b- defN 24-May-13 17:28 ai_edge_torch/testing/model_coverage/__init__.py
--rw-r--r--  2.0 unx     4286 b- defN 24-May-13 17:28 ai_edge_torch/testing/model_coverage/model_coverage.py
--rw-r--r--  2.0 unx    11358 b- defN 24-May-13 23:27 ai_edge_torch-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1636 b- defN 24-May-13 23:27 ai_edge_torch-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-13 23:27 ai_edge_torch-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-May-13 23:27 ai_edge_torch-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     9635 b- defN 24-May-13 23:27 ai_edge_torch-0.1.1.dist-info/RECORD
-91 files, 397601 bytes uncompressed, 122738 bytes compressed:  69.1%
+Zip file size: 138896 bytes, number of entries: 91
+-rw-r--r--  2.0 unx     1008 b- defN 24-May-13 17:24 ai_edge_torch/__init__.py
+-rw-r--r--  2.0 unx     4243 b- defN 24-May-13 17:24 ai_edge_torch/model.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/convert/__init__.py
+-rw-r--r--  2.0 unx     4043 b- defN 24-May-13 17:24 ai_edge_torch/convert/conversion.py
+-rw-r--r--  2.0 unx    11021 b- defN 24-May-13 17:24 ai_edge_torch/convert/conversion_utils.py
+-rw-r--r--  2.0 unx     6927 b- defN 24-May-13 17:24 ai_edge_torch/convert/converter.py
+-rw-r--r--  2.0 unx     2825 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/__init__.py
+-rw-r--r--  2.0 unx     1652 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/_pass_base.py
+-rw-r--r--  2.0 unx     6150 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/build_aten_composite_pass.py
+-rw-r--r--  2.0 unx     2607 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/build_upsample_bilinear2d_composite_pass.py
+-rw-r--r--  2.0 unx     1673 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/canonicalize_pass.py
+-rw-r--r--  2.0 unx     2448 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/inject_mlir_debuginfo_pass.py
+-rw-r--r--  2.0 unx      795 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/__init__.py
+-rw-r--r--  2.0 unx     6870 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_check.py
+-rw-r--r--  2.0 unx     1560 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_mark.py
+-rw-r--r--  2.0 unx    12438 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_rewrite.py
+-rw-r--r--  2.0 unx      982 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/op_func_registry.py
+-rw-r--r--  2.0 unx    10030 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/pass_body.py
+-rw-r--r--  2.0 unx     2076 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/utils.py
+-rw-r--r--  2.0 unx      715 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/__init__.py
+-rw-r--r--  2.0 unx     2279 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/greedy.py
+-rw-r--r--  2.0 unx     6432 b- defN 24-May-13 17:24 ai_edge_torch/convert/fx_passes/optimize_layout_transposes_pass/layout_partitioners/min_cut.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/convert/test/__init__.py
+-rw-r--r--  2.0 unx     8092 b- defN 24-May-13 17:24 ai_edge_torch/convert/test/test_convert.py
+-rw-r--r--  2.0 unx     6403 b- defN 24-May-13 17:24 ai_edge_torch/convert/test/test_convert_composites.py
+-rw-r--r--  2.0 unx     4537 b- defN 24-May-13 17:24 ai_edge_torch/convert/test/test_convert_multisig.py
+-rw-r--r--  2.0 unx      707 b- defN 24-May-13 17:24 ai_edge_torch/debug/__init__.py
+-rw-r--r--  2.0 unx    12789 b- defN 24-May-13 17:24 ai_edge_torch/debug/culprit.py
+-rw-r--r--  2.0 unx     1430 b- defN 24-May-13 17:24 ai_edge_torch/debug/utils.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/debug/test/__init__.py
+-rw-r--r--  2.0 unx     3731 b- defN 24-May-13 17:24 ai_edge_torch/debug/test/test_culprit.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/experimental/__init__.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/__init__.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/__init__.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/gemma/__init__.py
+-rw-r--r--  2.0 unx     2538 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/gemma/convert_to_tflite.py
+-rw-r--r--  2.0 unx     5913 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/gemma/gemma.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/phi2/__init__.py
+-rw-r--r--  2.0 unx     2512 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/phi2/convert_to_tflite.py
+-rw-r--r--  2.0 unx     5540 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/phi2/phi2.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/t5/__init__.py
+-rw-r--r--  2.0 unx     4536 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/t5/convert_to_tflite.py
+-rw-r--r--  2.0 unx    21065 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/t5/t5.py
+-rw-r--r--  2.0 unx     8998 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/t5/t5_attention.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/test_models/__init__.py
+-rw-r--r--  2.0 unx     3791 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/test_models/toy_model.py
+-rw-r--r--  2.0 unx     4831 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/test_models/toy_model_with_kv_cache.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/tiny_llama/__init__.py
+-rw-r--r--  2.0 unx     2566 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/tiny_llama/convert_to_tflite.py
+-rw-r--r--  2.0 unx     5629 b- defN 24-May-13 17:24 ai_edge_torch/generative/examples/tiny_llama/tiny_llama.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/__init__.py
+-rw-r--r--  2.0 unx     9127 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/attention.py
+-rw-r--r--  2.0 unx     6350 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/attention_utils.py
+-rw-r--r--  2.0 unx     3201 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/builder.py
+-rw-r--r--  2.0 unx     2820 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/feed_forward.py
+-rw-r--r--  2.0 unx     3090 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/kv_cache.py
+-rw-r--r--  2.0 unx     4064 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/model_config.py
+-rw-r--r--  2.0 unx     1867 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/normalization.py
+-rw-r--r--  2.0 unx     1383 b- defN 24-May-13 17:24 ai_edge_torch/generative/layers/rotary_position_embedding.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/quantize/__init__.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-13 17:24 ai_edge_torch/generative/quantize/example.py
+-rw-r--r--  2.0 unx     1862 b- defN 24-May-13 17:24 ai_edge_torch/generative/quantize/quant_attrs.py
+-rw-r--r--  2.0 unx     3327 b- defN 24-May-13 17:24 ai_edge_torch/generative/quantize/quant_recipe.py
+-rw-r--r--  2.0 unx     1913 b- defN 24-May-13 17:24 ai_edge_torch/generative/quantize/quant_recipe_utils.py
+-rw-r--r--  2.0 unx     1798 b- defN 24-May-13 17:24 ai_edge_torch/generative/quantize/quant_recipes.py
+-rw-r--r--  2.0 unx     1345 b- defN 24-May-13 17:24 ai_edge_torch/generative/quantize/supported_schemes.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/generative/test/__init__.py
+-rw-r--r--  2.0 unx     6500 b- defN 24-May-13 17:24 ai_edge_torch/generative/test/test_model_conversion.py
+-rw-r--r--  2.0 unx     3728 b- defN 24-May-13 17:24 ai_edge_torch/generative/test/test_quantize.py
+-rw-r--r--  2.0 unx      720 b- defN 24-May-13 17:24 ai_edge_torch/generative/utilities/__init__.py
+-rw-r--r--  2.0 unx    10029 b- defN 24-May-13 17:24 ai_edge_torch/generative/utilities/loader.py
+-rw-r--r--  2.0 unx    16156 b- defN 24-May-13 17:24 ai_edge_torch/generative/utilities/t5_loader.py
+-rw-r--r--  2.0 unx      752 b- defN 24-May-13 17:24 ai_edge_torch/hlfb/__init__.py
+-rw-r--r--  2.0 unx     4799 b- defN 24-May-13 17:24 ai_edge_torch/hlfb/mark_pattern/__init__.py
+-rw-r--r--  2.0 unx     1539 b- defN 24-May-13 17:24 ai_edge_torch/hlfb/mark_pattern/passes.py
+-rw-r--r--  2.0 unx     9206 b- defN 24-May-13 17:24 ai_edge_torch/hlfb/mark_pattern/pattern.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/hlfb/test/__init__.py
+-rw-r--r--  2.0 unx     4262 b- defN 24-May-13 17:24 ai_edge_torch/hlfb/test/test_mark_pattern.py
+-rw-r--r--  2.0 unx     8190 b- defN 24-May-13 17:24 ai_edge_torch/hlfb/test/test_stablehlo_composite_builder.py
+-rw-r--r--  2.0 unx      714 b- defN 24-May-13 17:24 ai_edge_torch/quantize/__init__.py
+-rw-r--r--  2.0 unx    15602 b- defN 24-May-13 17:24 ai_edge_torch/quantize/pt2e_quantizer.py
+-rw-r--r--  2.0 unx    36046 b- defN 24-May-13 17:24 ai_edge_torch/quantize/pt2e_quantizer_utils.py
+-rw-r--r--  2.0 unx     3435 b- defN 24-May-13 17:24 ai_edge_torch/quantize/quant_config.py
+-rw-r--r--  2.0 unx      671 b- defN 24-May-13 17:24 ai_edge_torch/testing/__init__.py
+-rw-r--r--  2.0 unx      765 b- defN 24-May-13 17:24 ai_edge_torch/testing/model_coverage/__init__.py
+-rw-r--r--  2.0 unx     4286 b- defN 24-May-13 17:24 ai_edge_torch/testing/model_coverage/model_coverage.py
+-rw-r--r--  2.0 unx    11358 b- defN 24-May-13 20:55 ai_edge_torch-0.dev202405131354.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1712 b- defN 24-May-13 20:55 ai_edge_torch-0.dev202405131354.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-13 20:55 ai_edge_torch-0.dev202405131354.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-May-13 20:55 ai_edge_torch-0.dev202405131354.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     9695 b- defN 24-May-13 20:55 ai_edge_torch-0.dev202405131354.dist-info/RECORD
+91 files, 397737 bytes uncompressed, 122794 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -252,23 +252,23 @@
 
 Filename: ai_edge_torch/testing/model_coverage/__init__.py
 Comment: 
 
 Filename: ai_edge_torch/testing/model_coverage/model_coverage.py
 Comment: 
 
-Filename: ai_edge_torch-0.1.1.dist-info/LICENSE
+Filename: ai_edge_torch-0.dev202405131354.dist-info/LICENSE
 Comment: 
 
-Filename: ai_edge_torch-0.1.1.dist-info/METADATA
+Filename: ai_edge_torch-0.dev202405131354.dist-info/METADATA
 Comment: 
 
-Filename: ai_edge_torch-0.1.1.dist-info/WHEEL
+Filename: ai_edge_torch-0.dev202405131354.dist-info/WHEEL
 Comment: 
 
-Filename: ai_edge_torch-0.1.1.dist-info/top_level.txt
+Filename: ai_edge_torch-0.dev202405131354.dist-info/top_level.txt
 Comment: 
 
-Filename: ai_edge_torch-0.1.1.dist-info/RECORD
+Filename: ai_edge_torch-0.dev202405131354.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ai_edge_torch-0.1.1.dist-info/LICENSE` & `ai_edge_torch-0.dev202405131354.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ai_edge_torch-0.1.1.dist-info/METADATA` & `ai_edge_torch-0.dev202405131354.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-edge-torch
-Version: 0.1.1
+Version: 0.dev202405131354
 Summary: Supporting PyTorch models with the Google AI Edge TFLite runtime.
 Home-page: https://github.com/google-ai-edge/ai-edge-torch
 Keywords: On-Device ML,AI,Google,TFLite,PyTorch,LLMs,GenAI
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -20,17 +20,20 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: scipy
 Requires-Dist: safetensors
+Requires-Dist: scipy
 Requires-Dist: tabulate
 Requires-Dist: torch ==2.4.*
 
-Library that supports converting PyTorch models into a .tflite format, which can
-then be run with TensorFlow Lite and MediaPipe.  This enables applications for
-Android, iOS and IOT that can run models completely on-device.
+This pacakge has two primary components:
+
+1. PyTorch Converter: A direct path from PyTorch to [TFLite runtime](https://www.tensorflow.org/lite/guide/inference).
+
+1. Generative API: Python library that allows developers to author high performance LLMs for
+     Mobile devices in PyTorch.
 
 More details are in the project's [GitHub repository](https://github.com/google-ai-edge/ai-edge-torch).
```

## Comparing `ai_edge_torch-0.1.1.dist-info/RECORD` & `ai_edge_torch-0.dev202405131354.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -80,12 +80,12 @@
 ai_edge_torch/quantize/__init__.py,sha256=aB5dXot04bqyUhpsDFvxt9CIi15QAC4euvqOndJ0XLU,714
 ai_edge_torch/quantize/pt2e_quantizer.py,sha256=ye1f5vAZ0Vr4RWAtfrgU1o3JLs03Sa4inHRq3YxJDGo,15602
 ai_edge_torch/quantize/pt2e_quantizer_utils.py,sha256=yjzKoptnfEeW_sN7sODUfj3nCtUMXVzq3vHKxblsd5Y,36046
 ai_edge_torch/quantize/quant_config.py,sha256=ExThdTXqnWmGC3-F6sdXbXr8nYzkEe_qCziCfhsoMPA,3435
 ai_edge_torch/testing/__init__.py,sha256=hHLluseD2R0Hh4W6XZRIXY_dRQeYudjsrKGf6LZz65g,671
 ai_edge_torch/testing/model_coverage/__init__.py,sha256=5P8J6Zk5YYtDvTBucFvB9NGSRI7Gw_24WnrbhXgycEE,765
 ai_edge_torch/testing/model_coverage/model_coverage.py,sha256=EIyKz-HY70DguWuSrJal8LpYXQ5ZSEUf3ZrVl7jikFM,4286
-ai_edge_torch-0.1.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-ai_edge_torch-0.1.1.dist-info/METADATA,sha256=wSem4XEdsN4xUD4RssVUHsjnOmxfspU6trSH1Tck0aw,1636
-ai_edge_torch-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ai_edge_torch-0.1.1.dist-info/top_level.txt,sha256=5KXRaF2hwkApYxf7Y8y_tVb9aulGTlbOoNdbx1aKRkE,14
-ai_edge_torch-0.1.1.dist-info/RECORD,,
+ai_edge_torch-0.dev202405131354.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+ai_edge_torch-0.dev202405131354.dist-info/METADATA,sha256=Cafs18a-YkHqnxbt5hCjuggE_riDZthkogZksoHq_b8,1712
+ai_edge_torch-0.dev202405131354.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ai_edge_torch-0.dev202405131354.dist-info/top_level.txt,sha256=5KXRaF2hwkApYxf7Y8y_tVb9aulGTlbOoNdbx1aKRkE,14
+ai_edge_torch-0.dev202405131354.dist-info/RECORD,,
```

