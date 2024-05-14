# Comparing `tmp/ipex_llm-2.1.0b20240512-py3-none-win_amd64.whl.zip` & `tmp/ipex_llm-2.1.0b20240513-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5319449 bytes, number of entries: 189
+Zip file size: 5319572 bytes, number of entries: 189
 -rw-------  2.0 unx     1898 b- defN 24-Mar-25 11:36 ipex_llm/__init__.py
 -rw-------  2.0 unx     6816 b- defN 24-Mar-25 11:36 ipex_llm/convert_model.py
 -rw-------  2.0 unx     3232 b- defN 24-May-07 15:07 ipex_llm/llm_patching.py
 -rw-------  2.0 unx     1177 b- defN 24-Mar-25 11:36 ipex_llm/models.py
 -rw-------  2.0 unx    12404 b- defN 24-Apr-18 12:34 ipex_llm/optimize.py
 -rw-------  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-chat.ps1
 -rwx------  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-cli.ps1
@@ -38,64 +38,64 @@
 -rw-------  2.0 unx     1189 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/__init__.py
 -rw-------  2.0 unx    13589 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/bigdlllm.py
 -rw-------  2.0 unx     7225 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/transformersembeddings.py
 -rw-------  2.0 unx     1636 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/__init__.py
 -rw-------  2.0 unx    24438 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/bigdlllm.py
 -rw-------  2.0 unx    10576 b- defN 24-Apr-03 15:07 ipex_llm/langchain/llms/transformersllm.py
 -rw-------  2.0 unx     7379 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformerspipelinellm.py
--rw-------  2.0 unx        0 b- defN 24-May-12 15:07 ipex_llm/libs/__init__.py
--rw-------  2.0 unx    36352 b- defN 24-May-12 15:07 ipex_llm/libs/bloom-api.dll
--rw-------  2.0 unx   470528 b- defN 24-May-12 15:07 ipex_llm/libs/bloom.dll
--rw-------  2.0 unx   853504 b- defN 24-May-12 15:07 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
--rw-------  2.0 unx   856576 b- defN 24-May-12 15:07 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
--rw-------  2.0 unx   844288 b- defN 24-May-12 15:07 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
--rw-------  2.0 unx    24576 b- defN 24-May-12 15:07 ipex_llm/libs/gptneox-api.dll
--rw-------  2.0 unx   530432 b- defN 24-May-12 15:07 ipex_llm/libs/gptneox.dll
--rw-------  2.0 unx   496128 b- defN 24-May-12 15:07 ipex_llm/libs/libbloom_avx.dll
--rw-------  2.0 unx   471040 b- defN 24-May-12 15:07 ipex_llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   556032 b- defN 24-May-12 15:07 ipex_llm/libs/libgptneox_avx.dll
--rw-------  2.0 unx   530944 b- defN 24-May-12 15:07 ipex_llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   549888 b- defN 24-May-12 15:07 ipex_llm/libs/libllama_avx.dll
--rw-------  2.0 unx   525312 b- defN 24-May-12 15:07 ipex_llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   586752 b- defN 24-May-12 15:07 ipex_llm/libs/libstarcoder_avx.dll
--rw-------  2.0 unx   561664 b- defN 24-May-12 15:07 ipex_llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 24-May-12 15:07 ipex_llm/libs/llama-api.dll
--rw-------  2.0 unx   524288 b- defN 24-May-12 15:07 ipex_llm/libs/llama.dll
--rw-------  2.0 unx   103424 b- defN 24-May-12 15:07 ipex_llm/libs/main-bloom.exe
--rw-------  2.0 unx   726016 b- defN 24-May-12 15:07 ipex_llm/libs/main-chatglm_vnni.exe
--rw-------  2.0 unx    98816 b- defN 24-May-12 15:07 ipex_llm/libs/main-gptneox.exe
--rw-------  2.0 unx    99840 b- defN 24-May-12 15:07 ipex_llm/libs/main-llama.exe
--rw-------  2.0 unx   157696 b- defN 24-May-12 15:07 ipex_llm/libs/main-starcoder.exe
--rw-------  2.0 unx   126464 b- defN 24-May-12 15:07 ipex_llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   127488 b- defN 24-May-12 15:07 ipex_llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx   103936 b- defN 24-May-12 15:07 ipex_llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx   104448 b- defN 24-May-12 15:07 ipex_llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   109056 b- defN 24-May-12 15:07 ipex_llm/libs/quantize-llama.exe
--rw-------  2.0 unx   110080 b- defN 24-May-12 15:07 ipex_llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   126976 b- defN 24-May-12 15:07 ipex_llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   128512 b- defN 24-May-12 15:07 ipex_llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 24-May-12 15:07 ipex_llm/libs/starcoder-api.dll
--rw-------  2.0 unx   561152 b- defN 24-May-12 15:07 ipex_llm/libs/starcoder.dll
+-rw-------  2.0 unx        0 b- defN 24-May-13 15:08 ipex_llm/libs/__init__.py
+-rw-------  2.0 unx    36352 b- defN 24-May-13 15:08 ipex_llm/libs/bloom-api.dll
+-rw-------  2.0 unx   470528 b- defN 24-May-13 15:08 ipex_llm/libs/bloom.dll
+-rw-------  2.0 unx   853504 b- defN 24-May-13 15:08 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
+-rw-------  2.0 unx   856576 b- defN 24-May-13 15:08 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
+-rw-------  2.0 unx   844288 b- defN 24-May-13 15:08 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
+-rw-------  2.0 unx    24576 b- defN 24-May-13 15:08 ipex_llm/libs/gptneox-api.dll
+-rw-------  2.0 unx   530432 b- defN 24-May-13 15:08 ipex_llm/libs/gptneox.dll
+-rw-------  2.0 unx   496128 b- defN 24-May-13 15:08 ipex_llm/libs/libbloom_avx.dll
+-rw-------  2.0 unx   471040 b- defN 24-May-13 15:08 ipex_llm/libs/libbloom_vnni.dll
+-rw-------  2.0 unx   556032 b- defN 24-May-13 15:08 ipex_llm/libs/libgptneox_avx.dll
+-rw-------  2.0 unx   530944 b- defN 24-May-13 15:08 ipex_llm/libs/libgptneox_vnni.dll
+-rw-------  2.0 unx   549888 b- defN 24-May-13 15:08 ipex_llm/libs/libllama_avx.dll
+-rw-------  2.0 unx   525312 b- defN 24-May-13 15:08 ipex_llm/libs/libllama_vnni.dll
+-rw-------  2.0 unx   586752 b- defN 24-May-13 15:08 ipex_llm/libs/libstarcoder_avx.dll
+-rw-------  2.0 unx   561664 b- defN 24-May-13 15:08 ipex_llm/libs/libstarcoder_vnni.dll
+-rw-------  2.0 unx    25088 b- defN 24-May-13 15:08 ipex_llm/libs/llama-api.dll
+-rw-------  2.0 unx   524288 b- defN 24-May-13 15:08 ipex_llm/libs/llama.dll
+-rw-------  2.0 unx   103424 b- defN 24-May-13 15:08 ipex_llm/libs/main-bloom.exe
+-rw-------  2.0 unx   726016 b- defN 24-May-13 15:08 ipex_llm/libs/main-chatglm_vnni.exe
+-rw-------  2.0 unx    98816 b- defN 24-May-13 15:08 ipex_llm/libs/main-gptneox.exe
+-rw-------  2.0 unx    99840 b- defN 24-May-13 15:08 ipex_llm/libs/main-llama.exe
+-rw-------  2.0 unx   157696 b- defN 24-May-13 15:08 ipex_llm/libs/main-starcoder.exe
+-rw-------  2.0 unx   126464 b- defN 24-May-13 15:08 ipex_llm/libs/quantize-bloom.exe
+-rw-------  2.0 unx   127488 b- defN 24-May-13 15:08 ipex_llm/libs/quantize-bloom_vnni.exe
+-rw-------  2.0 unx   103936 b- defN 24-May-13 15:08 ipex_llm/libs/quantize-gptneox.exe
+-rw-------  2.0 unx   104448 b- defN 24-May-13 15:08 ipex_llm/libs/quantize-gptneox_vnni.exe
+-rw-------  2.0 unx   109056 b- defN 24-May-13 15:08 ipex_llm/libs/quantize-llama.exe
+-rw-------  2.0 unx   110080 b- defN 24-May-13 15:08 ipex_llm/libs/quantize-llama_vnni.exe
+-rw-------  2.0 unx   126976 b- defN 24-May-13 15:08 ipex_llm/libs/quantize-starcoder.exe
+-rw-------  2.0 unx   128512 b- defN 24-May-13 15:08 ipex_llm/libs/quantize-starcoder_vnni.exe
+-rw-------  2.0 unx    21504 b- defN 24-May-13 15:08 ipex_llm/libs/starcoder-api.dll
+-rw-------  2.0 unx   561152 b- defN 24-May-13 15:08 ipex_llm/libs/starcoder.dll
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/__init__.py
 -rw-------  2.0 unx     1139 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/__init__.py
 -rw-------  2.0 unx    26314 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/bigdlllm.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/__init__.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/__init__.py
 -rw-------  2.0 unx    10084 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/bigdl_llm_model.py
--rw-------  2.0 unx    18709 b- defN 24-May-07 15:07 ipex_llm/serving/fastchat/ipex_llm_worker.py
+-rw-------  2.0 unx    19162 b- defN 24-May-13 15:08 ipex_llm/serving/fastchat/ipex_llm_worker.py
 -rw-------  2.0 unx    16649 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/model_worker.py
 -rw-------  2.0 unx    10801 b- defN 24-Apr-29 15:08 ipex_llm/serving/fastchat/vllm_worker.py
 -rw-------  2.0 unx     1005 b- defN 24-Mar-25 11:36 ipex_llm/transformers/__init__.py
 -rw-------  2.0 unx     1213 b- defN 24-Mar-25 11:36 ipex_llm/transformers/bmm.py
--rw-------  2.0 unx    74718 b- defN 24-May-09 15:08 ipex_llm/transformers/convert.py
+-rw-------  2.0 unx    74449 b- defN 24-May-13 15:08 ipex_llm/transformers/convert.py
 -rw-------  2.0 unx    14334 b- defN 24-Apr-26 15:08 ipex_llm/transformers/convert_ipex.py
 -rw-------  2.0 unx     4613 b- defN 24-Mar-25 11:36 ipex_llm/transformers/embedding.py
 -rw-------  2.0 unx     4247 b- defN 24-Apr-29 15:08 ipex_llm/transformers/kv.py
 -rw-------  2.0 unx     3289 b- defN 24-Apr-18 12:34 ipex_llm/transformers/lisa.py
--rw-------  2.0 unx     5787 b- defN 24-May-06 15:07 ipex_llm/transformers/loader.py
+-rw-------  2.0 unx     6812 b- defN 24-May-13 15:08 ipex_llm/transformers/loader.py
 -rw-------  2.0 unx    14860 b- defN 24-Apr-28 15:07 ipex_llm/transformers/lookup.py
 -rw-------  2.0 unx    39805 b- defN 24-Apr-26 15:08 ipex_llm/transformers/low_bit_linear.py
 -rw-------  2.0 unx    36141 b- defN 24-May-08 15:07 ipex_llm/transformers/model.py
 -rw-------  2.0 unx     6921 b- defN 24-Mar-25 11:36 ipex_llm/transformers/modelling_bigdl.py
 -rw-------  2.0 unx    15520 b- defN 24-May-07 15:07 ipex_llm/transformers/qlora.py
 -rw-------  2.0 unx    16567 b- defN 24-Mar-25 11:36 ipex_llm/transformers/relora.py
 -rw-------  2.0 unx    56660 b- defN 24-May-08 15:07 ipex_llm/transformers/speculative.py
@@ -177,15 +177,15 @@
 -rw-------  2.0 unx     1763 b- defN 24-Mar-25 11:36 ipex_llm/utils/common/log4Error.py
 -rw-------  2.0 unx      585 b- defN 24-Apr-22 15:07 ipex_llm/vllm/__init__.py
 -rw-------  2.0 unx    18514 b- defN 24-Apr-26 15:08 ipex_llm/vllm/ipex_llm_gpu_executor.py
 -rw-------  2.0 unx     7208 b- defN 24-Apr-22 15:07 ipex_llm/vllm/model_convert.py
 -rw-------  2.0 unx      747 b- defN 24-Apr-22 15:07 ipex_llm/vllm/engine/__init__.py
 -rw-------  2.0 unx     5941 b- defN 24-Apr-26 15:08 ipex_llm/vllm/engine/engine.py
 -rw-------  2.0 unx    10564 b- defN 24-Apr-22 15:07 ipex_llm/vllm/entrypoints/openai/api_server.py
--rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240512.data/scripts/llm-chat.ps1
--rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240512.data/scripts/llm-cli.ps1
--rw-------  2.0 unx     4013 b- defN 24-May-12 15:07 ipex_llm-2.1.0b20240512.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 24-May-12 15:07 ipex_llm-2.1.0b20240512.dist-info/WHEEL
--rw-------  2.0 unx       61 b- defN 24-May-12 15:07 ipex_llm-2.1.0b20240512.dist-info/entry_points.txt
--rw-------  2.0 unx        9 b- defN 24-May-12 15:07 ipex_llm-2.1.0b20240512.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    17921 b- defN 24-May-12 15:07 ipex_llm-2.1.0b20240512.dist-info/RECORD
-189 files, 13003776 bytes uncompressed, 5290817 bytes compressed:  59.3%
+-rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240513.data/scripts/llm-chat.ps1
+-rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240513.data/scripts/llm-cli.ps1
+-rw-------  2.0 unx     4013 b- defN 24-May-13 15:08 ipex_llm-2.1.0b20240513.dist-info/METADATA
+-rw-------  2.0 unx       98 b- defN 24-May-13 15:08 ipex_llm-2.1.0b20240513.dist-info/WHEEL
+-rw-------  2.0 unx       61 b- defN 24-May-13 15:08 ipex_llm-2.1.0b20240513.dist-info/entry_points.txt
+-rw-------  2.0 unx        9 b- defN 24-May-13 15:08 ipex_llm-2.1.0b20240513.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    17921 b- defN 24-May-13 15:09 ipex_llm-2.1.0b20240513.dist-info/RECORD
+189 files, 13004985 bytes uncompressed, 5290940 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -540,29 +540,29 @@
 
 Filename: ipex_llm/vllm/engine/engine.py
 Comment: 
 
 Filename: ipex_llm/vllm/entrypoints/openai/api_server.py
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240512.data/scripts/llm-chat.ps1
+Filename: ipex_llm-2.1.0b20240513.data/scripts/llm-chat.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240512.data/scripts/llm-cli.ps1
+Filename: ipex_llm-2.1.0b20240513.data/scripts/llm-cli.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240512.dist-info/METADATA
+Filename: ipex_llm-2.1.0b20240513.dist-info/METADATA
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240512.dist-info/WHEEL
+Filename: ipex_llm-2.1.0b20240513.dist-info/WHEEL
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240512.dist-info/entry_points.txt
+Filename: ipex_llm-2.1.0b20240513.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240512.dist-info/top_level.txt
+Filename: ipex_llm-2.1.0b20240513.dist-info/top_level.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240512.dist-info/RECORD
+Filename: ipex_llm-2.1.0b20240513.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipex_llm/libs/bloom-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800036cc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:02:35 2024
+Time/Date		Mon May 13 15:03:28 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000003200
 SizeOfInitializedData	0000000000005e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000036cc
@@ -6375,16 +6375,15 @@
    180005621:	push   %rdx
    180005622:	add    %al,0x1(%rax)
    180005628:	pop    %rax
    180005629:	push   %rdx
    18000562a:	add    %al,0x1(%rax)
    180005630:	add    %al,(%rax)
    180005632:	add    %al,(%rax)
-   180005634:	or     %edx,%ebx
-   180005636:	rex
+   180005634:	shrb   $0x42,(%rbx)
    180005637:	data16 add %al,(%rax)
    18000563a:	add    %al,(%rax)
    18000563c:	or     $0xe0000000,%eax
    180005641:	add    (%rax),%al
    180005643:	add    %cl,(%rcx,%rbx,2)
    180005646:	add    %al,(%rax)
    180005648:	or     $0x3f,%al
```

## ipex_llm/libs/bloom.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800551e8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:02:35 2024
+Time/Date		Mon May 13 15:03:28 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000055800
 SizeOfInitializedData	00000000000bf200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000551e8
@@ -111728,16 +111728,16 @@
    18005e7fa:	add    $0x180,%eax
    18005e7ff:	add    %dh,0x76(%rax)
    18005e802:	add    $0x180,%eax
    18005e807:	add    %bh,0x76(%rax)
    18005e80a:	add    $0x180,%eax
    18005e80f:	add    %al,(%rax)
    18005e811:	add    %al,(%rax)
-   18005e813:	add    %cl,(%rbx)
-   18005e815:	fiaddl 0x66(%rax)
+   18005e813:	add    %al,%al
+   18005e815:	sub    0x66(%rdx),%eax
    18005e818:	add    %al,(%rax)
    18005e81a:	add    %al,(%rax)
    18005e81c:	or     $0x50000000,%eax
    18005e821:	add    (%rax),%eax
    18005e823:	add    %ah,(%rax)
    18005e825:	repnz add $0x5de2000,%eax
 	...
```

## ipex_llm/libs/gptneox-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002cbc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:02:35 2024
+Time/Date		Mon May 13 15:03:28 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002600
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002cbc
@@ -5058,16 +5058,15 @@
    1800049c0:	cmp    %al,0x0(%rdx)
    1800049c3:	addb   $0x0,(%rcx)
    1800049c6:	add    %al,(%rax)
    1800049c8:	rex
    1800049c9:	rex.X add %al,0x1(%rax)
    1800049d0:	add    %al,(%rax)
    1800049d2:	add    %al,(%rax)
-   1800049d4:	or     %edx,%ebx
-   1800049d6:	rex
+   1800049d4:	shrb   $0x42,(%rbx)
    1800049d7:	data16 add %al,(%rax)
    1800049da:	add    %al,(%rax)
    1800049dc:	or     $0xe0000000,%eax
    1800049e1:	add    (%rax),%al
    1800049e3:	add    %ah,0x0(%rsp,%rcx,2)
    1800049e7:	add    %ah,0x0(%rsi,%rsi,1)
 	...
```

## ipex_llm/libs/gptneox.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005c948
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:02:35 2024
+Time/Date		Mon May 13 15:03:29 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005d200
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005c948
@@ -123136,16 +123136,15 @@
    1800660bd:	add    %al,(%rax)
    1800660bf:	add    %bh,0x18005f6(%rax)
    1800660c5:	add    %al,(%rax)
    1800660c7:	add    %al,%al
    1800660c9:	testb  $0x0,0x180(%rip)        # 0x180066250
    1800660d0:	add    %al,(%rax)
    1800660d2:	add    %al,(%rax)
-   1800660d4:	or     %edx,%ebx
-   1800660d6:	rex
+   1800660d4:	shrl   $0x42,(%rbx)
    1800660d7:	data16 add %al,(%rax)
    1800660da:	add    %al,(%rax)
    1800660dc:	or     $0x50000000,%eax
    1800660e1:	add    (%rax),%eax
    1800660e3:	add    %al,0x53040006(,%rbp,2)
    1800660ea:	(bad)
 	...
```

## ipex_llm/libs/libbloom_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005b148
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:03:37 2024
+Time/Date		Mon May 13 15:08:00 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005b600
 SizeOfInitializedData	00000000000bf800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005b148
@@ -117188,16 +117188,16 @@
    18006472a:	add    $0x180,%eax
    18006472f:	add    %dh,-0x2a(%rax)
    180064732:	add    $0x180,%eax
    180064737:	add    %bh,-0x2a(%rax)
    18006473a:	add    $0x180,%eax
    18006473f:	add    %al,(%rax)
    180064741:	add    %al,(%rax)
-   180064743:	add    %cl,-0x26(%rcx)
-   180064746:	rex
+   180064743:	add    %dl,%al
+   180064745:	sub    $0x42,%al
    180064747:	data16 add %al,(%rax)
    18006474a:	add    %al,(%rax)
    18006474c:	or     $0x50000000,%eax
    180064751:	add    (%rax),%eax
    180064753:	add    %ah,(%rax)
    180064755:	push   %rcx
    180064756:	(bad)
```

## ipex_llm/libs/libbloom_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800553f8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:04:32 2024
+Time/Date		Mon May 13 15:04:35 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000055a00
 SizeOfInitializedData	00000000000bf200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000553f8
@@ -111831,17 +111831,19 @@
    18005e7da:	add    $0x180,%eax
    18005e7df:	add    %dh,0x76(%rax)
    18005e7e2:	add    $0x180,%eax
    18005e7e7:	add    %bh,0x76(%rax)
    18005e7ea:	add    $0x180,%eax
    18005e7ef:	add    %al,(%rax)
    18005e7f1:	add    %al,(%rax)
-   18005e7f3:	add    %al,0x6640da(%rax)
-   18005e7f9:	add    %al,(%rax)
-   18005e7fb:	add    %cl,0x50000000(%rip)        # 0x1d005e801
+   18005e7f3:	add    %al,(%rbx)
+   18005e7f5:	sub    $0x42,%al
+   18005e7f7:	data16 add %al,(%rax)
+   18005e7fa:	add    %al,(%rax)
+   18005e7fc:	or     $0x50000000,%eax
    18005e801:	add    (%rax),%eax
    18005e803:	add    %ah,(%rax)
    18005e805:	repnz add $0x5e02000,%eax
 	...
    18005e87f:	add    %dl,0x18005f5(%rax)
    18005e885:	add    %al,(%rax)
    18005e887:	add    %bl,0x18005f5(%rax)
```

## ipex_llm/libs/libgptneox_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180062938
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:03:37 2024
+Time/Date		Mon May 13 15:08:00 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063200
 SizeOfInitializedData	00000000000c6800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000062938
@@ -128639,16 +128639,16 @@
    18006bff7:	add    %al,%al
    18006bff9:	push   %rsi
    18006bffa:	(bad)
    18006bffb:	addb   $0x0,(%rcx)
    18006bffe:	add    %al,(%rax)
    18006c000:	add    %al,(%rax)
    18006c002:	add    %al,(%rax)
-   18006c004:	rex.WB fiaddl 0x66(%r8)
-   18006c008:	add    %al,(%rax)
+   18006c004:	shrb   $1,(%rdx,%rax,2)
+   18006c007:	data16 add %al,(%rax)
    18006c00a:	add    %al,(%rax)
    18006c00c:	or     $0x50000000,%eax
    18006c011:	add    (%rax),%eax
    18006c013:	add    %al,-0x4d7bfffa(%rsp,%rcx,8)
    18006c01a:	(bad)
 	...
    18006c07f:	add    %bh,%al
```

## ipex_llm/libs/libgptneox_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005cb58
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:04:33 2024
+Time/Date		Mon May 13 15:04:36 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005d400
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005cb58
@@ -123256,15 +123256,17 @@
    18006609d:	add    %al,(%rax)
    18006609f:	add    %bh,0x18005f6(%rax)
    1800660a5:	add    %al,(%rax)
    1800660a7:	add    %al,%al
    1800660a9:	testb  $0x0,0x180(%rip)        # 0x180066230
    1800660b0:	add    %al,(%rax)
    1800660b2:	add    %al,(%rax)
-   1800660b4:	sbb    $0x6640,%edx
+   1800660b4:	add    $0x2c,%al
+   1800660b6:	rex.X
+   1800660b7:	data16 add %al,(%rax)
    1800660ba:	add    %al,(%rax)
    1800660bc:	or     $0x50000000,%eax
    1800660c1:	add    (%rax),%eax
    1800660c3:	add    %al,0x55040006(,%rbp,2)
    1800660ca:	(bad)
 	...
    1800660ff:	add    %bh,0x70(%rax)
```

## ipex_llm/libs/libllama_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180061648
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:03:37 2024
+Time/Date		Mon May 13 15:08:00 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000061e00
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000061648
@@ -127298,16 +127298,16 @@
    18006a0d6:	add    %al,(%rax)
    18006a0d8:	shlb   $1,(%rsi)
    18006a0da:	(bad)
    18006a0db:	addb   $0x0,(%rcx)
    18006a0de:	add    %al,(%rax)
    18006a0e0:	add    %al,(%rax)
    18006a0e2:	add    %al,(%rax)
-   18006a0e4:	rex.WB fiaddl 0x66(%r8)
-   18006a0e8:	add    %al,(%rax)
+   18006a0e4:	shrb   $1,(%rdx,%rax,2)
+   18006a0e7:	data16 add %al,(%rax)
    18006a0ea:	add    %al,(%rax)
    18006a0ec:	or     $0x50000000,%eax
    18006a0f1:	add    (%rax),%eax
    18006a0f3:	add    %al,(%rax)
    18006a0f5:	lods   %ds:(%rsi),%eax
    18006a0f6:	(bad)
    18006a0f7:	add    %al,(%rax)
```

## ipex_llm/libs/libllama_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005b868
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:04:33 2024
+Time/Date		Mon May 13 15:04:36 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c000
 SizeOfInitializedData	00000000000c6200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005b868
@@ -121930,17 +121930,19 @@
    180064181:	(bad)
    180064182:	add    $0x180,%eax
    180064187:	add    %dl,%al
    180064189:	(bad)
    18006418a:	add    $0x180,%eax
    18006418f:	add    %al,(%rax)
    180064191:	add    %al,(%rax)
-   180064193:	add    %al,0x6640da(%rcx)
-   180064199:	add    %al,(%rax)
-   18006419b:	add    %cl,0x50000000(%rip)        # 0x1d00641a1
+   180064193:	add    %al,(%rsp,%rbp,1)
+   180064196:	rex.X
+   180064197:	data16 add %al,(%rax)
+   18006419a:	add    %al,(%rax)
+   18006419c:	or     $0x50000000,%eax
    1800641a1:	add    (%rax),%eax
    1800641a3:	add    %al,(%rax)
    1800641a5:	rex.WRX (bad)
    1800641a7:	add    %al,(%rax)
    1800641a9:	rex.X (bad)
 	...
    1800641ff:	add    %dh,0x51(%rax)
```

## ipex_llm/libs/libstarcoder_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180068aa8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:03:37 2024
+Time/Date		Mon May 13 15:07:59 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000069000
 SizeOfInitializedData	00000000000c8200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000068aa8
@@ -137914,16 +137914,17 @@
    180071c27:	add    %al,%al
    180071c29:	cmpsb  %es:(%rdi),%ds:(%rsi)
    180071c2a:	(bad)
    180071c2b:	addb   $0x0,(%rcx)
    180071c2e:	add    %al,(%rax)
    180071c30:	add    %al,(%rax)
    180071c32:	add    %al,(%rax)
-   180071c34:	rex.WB fiaddl 0x66(%r8)
-   180071c38:	add    %al,(%rax)
+   180071c34:	iret
+   180071c35:	sub    $0x42,%al
+   180071c37:	data16 add %al,(%rax)
    180071c3a:	add    %al,(%rax)
    180071c3c:	or     $0x50000000,%eax
    180071c41:	add    (%rax),%eax
    180071c43:	add    %dl,%al
    180071c45:	sub    $0x21d00007,%eax
    180071c4a:	(bad)
 	...
```

## ipex_llm/libs/libstarcoder_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180062d58
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:04:32 2024
+Time/Date		Mon May 13 15:04:35 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063400
 SizeOfInitializedData	00000000000c7c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000062d58
@@ -132533,15 +132533,15 @@
    18006ccf7:	add    %al,%al
    18006ccf9:	push   %rsi
    18006ccfa:	(bad)
    18006ccfb:	addb   $0x0,(%rcx)
    18006ccfe:	add    %al,(%rax)
    18006cd00:	add    %al,(%rax)
    18006cd02:	add    %al,(%rax)
-   18006cd04:	sbb    $0x40,%dl
+   18006cd04:	add    (%rdx,%rax,2),%ebp
    18006cd07:	data16 add %al,(%rax)
    18006cd0a:	add    %al,(%rax)
    18006cd0c:	or     $0x50000000,%eax
    18006cd11:	add    (%rax),%eax
    18006cd13:	add    %dl,%al
    18006cd15:	fiadds (%rsi)
    18006cd17:	add    %dl,%al
```

## ipex_llm/libs/llama-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002dac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:02:35 2024
+Time/Date		Mon May 13 15:03:28 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002800
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002dac
@@ -5355,16 +5355,15 @@
    180004a20:	cmp    %al,0x0(%rdx)
    180004a23:	addb   $0x0,(%rcx)
    180004a26:	add    %al,(%rax)
    180004a28:	rex
    180004a29:	rex.X add %al,0x1(%rax)
    180004a30:	add    %al,(%rax)
    180004a32:	add    %al,(%rax)
-   180004a34:	or     %edx,%ebx
-   180004a36:	rex
+   180004a34:	shrb   $0x42,(%rbx)
    180004a37:	data16 add %al,(%rax)
    180004a3a:	add    %al,(%rax)
    180004a3c:	or     $0xe0000000,%eax
    180004a41:	add    (%rax),%al
    180004a43:	add    %ah,%ah
    180004a45:	rex.WR add %r8b,(%rax)
    180004a48:	in     $0x38,%al
```

## ipex_llm/libs/llama.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005b658
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:02:35 2024
+Time/Date		Mon May 13 15:03:29 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005be00
 SizeOfInitializedData	00000000000c6000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005b658
@@ -121795,16 +121795,16 @@
    1800641a1:	(bad)
    1800641a2:	add    $0x180,%eax
    1800641a7:	add    %dl,%al
    1800641a9:	(bad)
    1800641aa:	add    $0x180,%eax
    1800641af:	add    %al,(%rax)
    1800641b1:	add    %al,(%rax)
-   1800641b3:	add    %cl,(%rbx)
-   1800641b5:	fiaddl 0x66(%rax)
+   1800641b3:	add    %al,%cl
+   1800641b5:	sub    0x66(%rdx),%eax
    1800641b8:	add    %al,(%rax)
    1800641ba:	add    %al,(%rax)
    1800641bc:	or     $0x50000000,%eax
    1800641c1:	add    (%rax),%eax
    1800641c3:	add    %al,(%rax)
    1800641c5:	rex.WRX (bad)
    1800641c7:	add    %al,(%rax)
```

## ipex_llm/libs/main-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001045c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun May 12 15:02:35 2024
+Time/Date		Mon May 13 15:03:28 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010800
 SizeOfInitializedData	0000000000008e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001045c
@@ -25509,16 +25509,15 @@
    140014ab0:	enter  $0x125,$0x40
    140014ab4:	add    %eax,(%rax)
    140014ab6:	add    %al,(%rax)
    140014ab8:	shlb   $1,0x14001(%rip)        # 0x140028abf
    140014abe:	add    %al,(%rax)
    140014ac0:	add    %al,(%rax)
    140014ac2:	add    %al,(%rax)
-   140014ac4:	or     %edx,%ebx
-   140014ac6:	rex
+   140014ac4:	shrb   $0x42,(%rbx)
    140014ac7:	data16 add %al,(%rax)
    140014aca:	add    %al,(%rax)
    140014acc:	or     $0x20000000,%eax
    140014ad1:	add    (%rax),%eax
    140014ad3:	add    %cl,%ah
    140014ad5:	push   %rsp
    140014ad6:	add    %eax,(%rax)
```

## ipex_llm/libs/main-chatglm_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400836cc
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun May 12 15:04:59 2024
+Time/Date		Mon May 13 15:05:03 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000087c00
 SizeOfInitializedData	00000000000cbe00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000836cc
@@ -189047,17 +189047,19 @@
    140093ee5:	add    %al,(%rax)
    140093ee7:	add    %al,(%rax)
    140093ee9:	cltd
    140093eea:	or     %al,0x1(%rax)
    140093eed:	add    %al,(%rax)
    140093eef:	add    %al,(%rax)
    140093ef1:	add    %al,(%rax)
-   140093ef3:	add    %bl,0x6640da(%rbx)
-   140093ef9:	add    %al,(%rax)
-   140093efb:	add    %cl,-0x34000000(%rip)        # 0x10c093f01
+   140093ef3:	add    %bl,(%rdi)
+   140093ef5:	sub    $0x42,%al
+   140093ef7:	data16 add %al,(%rax)
+   140093efa:	add    %al,(%rax)
+   140093efc:	or     $0xcc000000,%eax
    140093f01:	add    (%rax),%eax
    140093f03:	add    %dl,-0x6ffff68d(%rax)
    140093f09:	movsxd (%rcx),%ecx
 	...
    140093f7f:	add    %al,0x1400977(%rax)
    140093f85:	add    %al,(%rax)
    140093f87:	add    %al,-0x61(%rbp)
```

## ipex_llm/libs/main-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000ef6c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun May 12 15:02:35 2024
+Time/Date		Mon May 13 15:03:28 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f200
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000ef6c
@@ -24136,16 +24136,15 @@
    140013edf:	add    %ch,%al
    140013ee1:	adc    $0x14001,%eax
    140013ee6:	add    %al,(%rax)
    140013ee8:	lock adc $0x14001,%eax
    140013eee:	add    %al,(%rax)
    140013ef0:	add    %al,(%rax)
    140013ef2:	add    %al,(%rax)
-   140013ef4:	or     %edx,%ebx
-   140013ef6:	rex
+   140013ef4:	shrb   $0x42,(%rbx)
    140013ef7:	data16 add %al,(%rax)
    140013efa:	add    %al,(%rax)
    140013efc:	or     $0x90000000,%eax
    140013f01:	add    (%rax),%eax
    140013f03:	add    %ch,0x1(%rcx,%rcx,2)
    140013f07:	add    %ch,0x1(%rdi,%rbp,1)
 	...
```

## ipex_llm/libs/main-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000f32c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun May 12 15:02:35 2024
+Time/Date		Mon May 13 15:03:28 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f600
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000f32c
@@ -24679,16 +24679,15 @@
    140013faf:	add    %ch,%al
    140013fb1:	adc    $0x14001,%eax
    140013fb6:	add    %al,(%rax)
    140013fb8:	lock adc $0x14001,%eax
    140013fbe:	add    %al,(%rax)
    140013fc0:	add    %al,(%rax)
    140013fc2:	add    %al,(%rax)
-   140013fc4:	or     %edx,%ebx
-   140013fc6:	rex
+   140013fc4:	shrb   $0x42,(%rbx)
    140013fc7:	data16 add %al,(%rax)
    140013fca:	add    %al,(%rax)
    140013fcc:	or     $0x90000000,%eax
    140013fd1:	add    (%rax),%eax
    140013fd3:	add    %ch,%ah
    140013fd5:	add    %rax,(%r8)
    140013fd8:	in     (%dx),%al
```

## ipex_llm/libs/main-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001a85c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun May 12 15:02:35 2024
+Time/Date		Mon May 13 15:03:28 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000001b000
 SizeOfInitializedData	000000000000bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001a85c
@@ -40341,16 +40341,16 @@
    14001f111:	movb   $0x40,(%rcx)
    14001f114:	add    %eax,(%rax)
    14001f116:	add    %al,(%rax)
    14001f118:	push   $0x14001c6
    14001f11d:	add    %al,(%rax)
    14001f11f:	add    %al,(%rax)
    14001f121:	add    %al,(%rax)
-   14001f123:	add    %cl,(%rbx)
-   14001f125:	fiaddl 0x66(%rax)
+   14001f123:	add    %al,%al
+   14001f125:	sub    0x66(%rdx),%eax
    14001f128:	add    %al,(%rax)
    14001f12a:	add    %al,(%rax)
    14001f12c:	or     $0x20000000,%eax
    14001f131:	add    (%rax),%eax
    14001f133:	add    %dl,(%rbx,%rax,1)
    14001f136:	add    (%rax),%al
    14001f138:	adc    $0xf7,%al
```

## ipex_llm/libs/quantize-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013918
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun May 12 15:02:35 2024
+Time/Date		Mon May 13 15:03:28 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013a00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013918
@@ -32229,16 +32229,16 @@
    1400191e5:	add    %al,(%rax)
    1400191e7:	add    %al,(%rax)
    1400191e9:	push   %rbp
    1400191ea:	add    %eax,0x1(%rax)
    1400191ed:	add    %al,(%rax)
    1400191ef:	add    %al,(%rax)
    1400191f1:	add    %al,(%rax)
-   1400191f3:	add    %cl,(%rbx)
-   1400191f5:	fiaddl 0x66(%rax)
+   1400191f3:	add    %al,%al
+   1400191f5:	sub    0x66(%rdx),%eax
    1400191f8:	add    %al,(%rax)
    1400191fa:	add    %al,(%rax)
    1400191fc:	or     $0x20000000,%eax
    140019201:	add    (%rax),%eax
    140019203:	add    %dh,%al
    140019205:	movabs 0x18ff00001,%eax
 	...
```

## ipex_llm/libs/quantize-bloom_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013b28
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun May 12 15:04:32 2024
+Time/Date		Mon May 13 15:04:35 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013b28
@@ -32355,17 +32355,19 @@
    1400191c5:	add    %al,(%rax)
    1400191c7:	add    %al,(%rax)
    1400191c9:	push   %rbp
    1400191ca:	add    %eax,0x1(%rax)
    1400191cd:	add    %al,(%rax)
    1400191cf:	add    %al,(%rax)
    1400191d1:	add    %al,(%rax)
-   1400191d3:	add    %al,0x6640da(%rax)
-   1400191d9:	add    %al,(%rax)
-   1400191db:	add    %cl,0x20000000(%rip)        # 0x1600191e1
+   1400191d3:	add    %al,(%rbx)
+   1400191d5:	sub    $0x42,%al
+   1400191d7:	data16 add %al,(%rax)
+   1400191da:	add    %al,(%rax)
+   1400191dc:	or     $0x20000000,%eax
    1400191e1:	add    (%rax),%eax
    1400191e3:	add    %dh,-0x5f(%rax)
    1400191e6:	add    %eax,(%rax)
    1400191e8:	jo     0x14001917b
    1400191ea:	add    %eax,(%rax)
 	...
    140019200:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010988
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun May 12 15:02:34 2024
+Time/Date		Mon May 13 15:03:27 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010988
@@ -27178,19 +27178,17 @@
    140015fe0:	push   $0x1400123
    140015fe5:	add    %al,(%rax)
    140015fe7:	add    %dh,0x23(%rax)
    140015fea:	add    %eax,0x1(%rax)
    140015fed:	add    %al,(%rax)
    140015fef:	add    %al,(%rax)
    140015ff1:	add    %al,(%rax)
-   140015ff3:	add    %cl,(%rdx)
-   140015ff5:	fiaddl 0x66(%rax)
-   140015ff8:	add    %al,(%rax)
-   140015ffa:	add    %al,(%rax)
-   140015ffc:	or     $0x90000000,%eax
+   140015ff3:	add    %bh,0x66422b(%rdi)
+   140015ff9:	add    %al,(%rax)
+   140015ffb:	add    %cl,-0x70000000(%rip)        # 0xd0016001
    140016001:	add    (%rax),%eax
    140016003:	add    %ch,%al
    140016005:	add    %eax,%gs:(%rax)
    140016008:	call   0x140016160
 	...
    14001607d:	add    %al,(%rax)
    14001607f:	add    %bl,0x1400169(%rax)
```

## ipex_llm/libs/quantize-gptneox_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010b98
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun May 12 15:04:31 2024
+Time/Date		Mon May 13 15:04:34 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010c00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010b98
@@ -27305,16 +27305,16 @@
    140015fc0:	push   $0x1400123
    140015fc5:	add    %al,(%rax)
    140015fc7:	add    %dh,0x23(%rax)
    140015fca:	add    %eax,0x1(%rax)
    140015fcd:	add    %al,(%rax)
    140015fcf:	add    %al,(%rax)
    140015fd1:	add    %al,(%rax)
-   140015fd3:	add    %bh,-0x26(%rdi)
-   140015fd6:	rex
+   140015fd3:	add    %al,(%rdx)
+   140015fd5:	sub    $0x42,%al
    140015fd7:	data16 add %al,(%rax)
    140015fda:	add    %al,(%rax)
    140015fdc:	or     $0x90000000,%eax
    140015fe1:	add    (%rax),%eax
    140015fe3:	add    %ch,0x65(%rax)
    140015fe6:	add    %eax,(%rax)
    140015fe8:	push   $0x155
```

## ipex_llm/libs/quantize-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400118e8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun May 12 15:02:34 2024
+Time/Date		Mon May 13 15:03:28 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011800
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000118e8
@@ -28462,16 +28462,16 @@
    1400170cd:	add    %al,(%rax)
    1400170cf:	add    %cl,0x1400133(%rax)
    1400170d5:	add    %al,(%rax)
    1400170d7:	add    %dl,0x1400133(%rax)
    1400170dd:	add    %al,(%rax)
    1400170df:	add    %al,(%rax)
    1400170e1:	add    %al,(%rax)
-   1400170e3:	add    %cl,(%rdx)
-   1400170e5:	fiaddl 0x66(%rax)
+   1400170e3:	add    %al,%al
+   1400170e5:	sub    0x66(%rdx),%eax
    1400170e8:	add    %al,(%rax)
    1400170ea:	add    %al,(%rax)
    1400170ec:	or     $0x90000000,%eax
    1400170f1:	add    (%rax),%eax
    1400170f3:	add    %ch,0x1(%rsi,%rsi,2)
    1400170f7:	add    %ch,0x1(%rdx,%riz,2)
    1400170fb:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-llama_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140011af8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun May 12 15:04:31 2024
+Time/Date		Mon May 13 15:04:34 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011c00
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000011af8
@@ -28607,16 +28607,16 @@
    1400170ad:	add    %al,(%rax)
    1400170af:	add    %cl,0x1400133(%rax)
    1400170b5:	add    %al,(%rax)
    1400170b7:	add    %dl,0x1400133(%rax)
    1400170bd:	add    %al,(%rax)
    1400170bf:	add    %al,(%rax)
    1400170c1:	add    %al,(%rax)
-   1400170c3:	add    %bh,-0x26(%rdi)
-   1400170c6:	rex
+   1400170c3:	add    %al,(%rdx)
+   1400170c5:	sub    $0x42,%al
    1400170c7:	data16 add %al,(%rax)
    1400170ca:	add    %al,(%rax)
    1400170cc:	or     $0x90000000,%eax
    1400170d1:	add    (%rax),%eax
    1400170d3:	add    %ch,0x1(%rsi,%rsi,2)
    1400170d7:	add    %ch,0x1(%rsi,%riz,2)
 	...
```

## ipex_llm/libs/quantize-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013c70
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun May 12 15:02:35 2024
+Time/Date		Mon May 13 15:03:28 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013c70
@@ -32576,16 +32576,16 @@
    140019305:	add    %al,(%rax)
    140019307:	add    %al,(%rax)
    140019309:	push   %rbp
    14001930a:	add    %eax,0x1(%rax)
    14001930d:	add    %al,(%rax)
    14001930f:	add    %al,(%rax)
    140019311:	add    %al,(%rax)
-   140019313:	add    %cl,(%rbx)
-   140019315:	fiaddl 0x66(%rax)
+   140019313:	add    %al,%al
+   140019315:	sub    0x66(%rdx),%eax
    140019318:	add    %al,(%rax)
    14001931a:	add    %al,(%rax)
    14001931c:	or     $0x20000000,%eax
    140019321:	add    (%rax),%eax
    140019323:	add    %bh,%ah
    140019325:	movabs %al,0x192fc0001
 	...
```

## ipex_llm/libs/quantize-starcoder_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013e80
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun May 12 15:04:32 2024
+Time/Date		Mon May 13 15:04:35 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013e00
 SizeOfInitializedData	00000000000ad200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013e80
@@ -32701,17 +32701,19 @@
    1400192e5:	add    %al,(%rax)
    1400192e7:	add    %al,(%rax)
    1400192e9:	push   %rbp
    1400192ea:	add    %eax,0x1(%rax)
    1400192ed:	add    %al,(%rax)
    1400192ef:	add    %al,(%rax)
    1400192f1:	add    %al,(%rax)
-   1400192f3:	add    %al,0x6640da(%rax)
-   1400192f9:	add    %al,(%rax)
-   1400192fb:	add    %cl,0x20000000(%rip)        # 0x160019301
+   1400192f3:	add    %al,(%rbx)
+   1400192f5:	sub    $0x42,%al
+   1400192f7:	data16 add %al,(%rax)
+   1400192fa:	add    %al,(%rax)
+   1400192fc:	or     $0x20000000,%eax
    140019301:	add    (%rax),%eax
    140019303:	add    %bh,%ah
    140019305:	movabs %al,0x194fc0001
 	...
    14001937e:	add    %al,(%rax)
    140019380:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/starcoder-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000277c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:02:35 2024
+Time/Date		Mon May 13 15:03:28 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002200
 SizeOfInitializedData	0000000000003400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000277c
@@ -4028,16 +4028,15 @@
    1800045f0:	cmp    %al,0x0(%rdx)
    1800045f3:	addb   $0x0,(%rcx)
    1800045f6:	add    %al,(%rax)
    1800045f8:	rex
    1800045f9:	rex.X add %al,0x1(%rax)
    180004600:	add    %al,(%rax)
    180004602:	add    %al,(%rax)
-   180004604:	or     %edx,%ebx
-   180004606:	rex
+   180004604:	shrb   $0x42,(%rbx)
    180004607:	data16 add %al,(%rax)
    18000460a:	add    %al,(%rax)
    18000460c:	or     $0xe0000000,%eax
    180004611:	add    (%rax),%al
    180004613:	add    %ah,%ah
    180004615:	rex.W add %al,(%rax)
    180004618:	in     $0x2e,%al
```

## ipex_llm/libs/starcoder.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180062b48
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun May 12 15:02:35 2024
+Time/Date		Mon May 13 15:03:28 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063200
 SizeOfInitializedData	00000000000c7c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000062b48
@@ -132428,16 +132428,15 @@
    18006cd17:	add    %al,%al
    18006cd19:	push   %rsi
    18006cd1a:	(bad)
    18006cd1b:	addb   $0x0,(%rcx)
    18006cd1e:	add    %al,(%rax)
    18006cd20:	add    %al,(%rax)
    18006cd22:	add    %al,(%rax)
-   18006cd24:	or     %edx,%ebx
-   18006cd26:	rex
+   18006cd24:	shrb   $0x42,(%rbx)
    18006cd27:	data16 add %al,(%rax)
    18006cd2a:	add    %al,(%rax)
    18006cd2c:	or     $0x50000000,%eax
    18006cd31:	add    (%rax),%eax
    18006cd33:	add    %dl,%al
    18006cd35:	fiadds (%rsi)
    18006cd37:	add    %dl,%al
```

## ipex_llm/serving/fastchat/ipex_llm_worker.py

```diff
@@ -65,40 +65,47 @@
         conv_template: str = None,
         load_in_low_bit: str = "sym_int4",
         device: str = "cpu",
         no_register: bool = False,
         trust_remote_code: bool = False,
         embed_in_truncate: bool = False,
         speculative: bool = False,
+        load_low_bit_model: bool = False,
         stream_interval: int = 4,
     ):
         super().__init__(
             controller_addr,
             worker_addr,
             worker_id,
             model_path,
             model_names,
             limit_worker_concurrency,
             conv_template,
         )
 
         self.load_in_low_bit = load_in_low_bit
+        self.load_low_bit_model = load_low_bit_model
         logger.info(
             f"Loading the model {self.model_names} on worker {worker_id},"
             f" worker type: BigDLLLM worker..."
         )
 
         logger.info(f"Using low bit format: {self.load_in_low_bit}, device: {device}")
         if speculative:
             logger.info(f"Using Self-Speculative decoding to generate")
 
         self.device = device
         self.speculative = speculative
         self.model, self.tokenizer = load_model(
-            model_path, device, self.load_in_low_bit, trust_remote_code, speculative
+            model_path,
+            device,
+            self.load_in_low_bit,
+            trust_remote_code,
+            speculative,
+            load_low_bit_model,
         )
         self.stream_interval = stream_interval
         self.context_len = get_context_length(self.model.config)
         self.embed_in_truncate = embed_in_truncate
         if not no_register:
             self.init_heart_beat()
 
@@ -491,14 +498,20 @@
     parser.add_argument(
         "--trust-remote-code",
         action="store_true",
         default=False,
         help="Trust remote code (e.g., from HuggingFace) when"
         "downloading the model and tokenizer.",
     )
+    parser.add_argument(
+        "--load-low-bit-model",
+        action="store_true",
+        default=False,
+        help="Load models that have been converted/saved using ipex-llm's save_low_bit interface",
+    )
     parser.add_argument("--embed-in-truncate", action="store_true")
 
     args = parser.parse_args()
     worker = BigDLLLMWorker(
         args.controller_address,
         args.worker_address,
         worker_id,
@@ -508,9 +521,11 @@
         args.conv_template,
         args.low_bit,
         args.device,
         args.no_register,
         args.trust_remote_code,
         args.embed_in_truncate,
         args.speculative,
+        args.load_low_bit_model,
+        args.stream_interval,
     )
     uvicorn.run(app, host=args.host, port=args.port, log_level="info")
```

## ipex_llm/transformers/convert.py

```diff
@@ -184,21 +184,14 @@
                 result = False
         else:
             result = False
 
     return result, (in_features, out_features, mp_group)
 
 
-def empty_cache_post(module, input, output):
-    try:
-        torch.xpu.empty_cache()
-    except:  # cpu
-        pass
-
-
 def convert_gptq(module, awq=False, llm_awq=False, act_order=False):
     from ipex_llm.transformers.low_bit_linear import get_block_size
     Q4_1 = get_block_size("asym_int4")
 
     scales = module.scales
 
     zeros = torch.bitwise_right_shift(
@@ -1520,16 +1513,14 @@
         from ipex_llm.transformers.models.phi3 import attention_forward
         convert_forward(model, module.Phi3Attention, attention_forward)
         from ipex_llm.transformers.models.phi3 import mlp_forward
         convert_forward(model, module.Phi3MLP, mlp_forward)
         from ipex_llm.transformers.models.phi3 import model_forward_wrapper
         model_forward = model_forward_wrapper(module.Phi3Model.forward)
         convert_forward(model, module.Phi3Model, model_forward)
-        # Empty cache after the first attention to run long context.
-        model.model.layers[0].self_attn.register_forward_hook(empty_cache_post)
     elif model.config.model_type == 'yuan':
         modeling_module_name = model.__class__.__module__
         module = importlib.import_module(modeling_module_name)
         from ipex_llm.transformers.models.yuan import yuan_attention_forward
         # from ipex_llm.transformers.models.yuan import yuan_mlp_forward
         convert_forward(model,
                         module.YuanAttention,
```

## ipex_llm/transformers/loader.py

```diff
@@ -42,58 +42,72 @@
 
 def load_model(
     model_path: str,
     device: str = "cpu",
     low_bit: str = 'sym_int4',
     trust_remote_code: bool = True,
     speculative: bool = False,
+    load_low_bit_model: bool = False,
 ):
     """Load a model using BigDL LLM backend."""
 
     # Do a sanity check for device:
     invalidInputError(device == 'cpu' or device == 'xpu',
                       "BigDL-LLM only supports device cpu or xpu")
 
-    tokenizer_cls = get_tokenizer_cls(model_path)
     model_cls = get_model_cls(model_path, low_bit)
-    model_kwargs = {"use_cache": True}
-    if trust_remote_code:
-        model_kwargs["trust_remote_code"] = True
-    if low_bit == "bf16":
-        model_kwargs.update({"load_in_low_bit": low_bit, "torch_dtype": torch.bfloat16})
-    elif low_bit == "fp16":
-        model_kwargs.update({"load_in_low_bit": low_bit, "torch_dtype": torch.float16})
-    else:
-        model_kwargs.update({"load_in_low_bit": low_bit, "torch_dtype": 'auto'})
+    # Load tokenizer
+    tokenizer_cls = get_tokenizer_cls(model_path)
 
+    model_kwargs = {"use_cache": True}
     if speculative:
+        invalidInputError(load_low_bit_model is not True,
+                          "Self-Speculative currently do not support load low-bit format models")
         invalidInputError(low_bit == "fp16" or low_bit == "bf16",
                           "Self-Speculative only supports low_bit fp16 or bf16")
         model_kwargs["speculative"] = True
 
-    # Load tokenizer
-    tokenizer = tokenizer_cls.from_pretrained(model_path, trust_remote_code=True)
-    model = model_cls.from_pretrained(model_path, **model_kwargs)
+    if trust_remote_code:
+        model_kwargs["trust_remote_code"] = True
+
+    if load_low_bit_model:
+        # After save_low_bit, the from_pretrained interface does not accept trust_remote_code=True
+        tokenizer = tokenizer_cls.from_pretrained(model_path)
+        model = model_cls.load_low_bit(model_path, **model_kwargs)
+    else:
+        if trust_remote_code:
+            tokenizer = tokenizer_cls.from_pretrained(model_path, trust_remote_code=True)
+        else:
+            tokenizer = tokenizer_cls.from_pretrained(model_path)
+        if low_bit == "bf16":
+            model_kwargs.update({"load_in_low_bit": low_bit, "torch_dtype": torch.bfloat16})
+        elif low_bit == "fp16":
+            model_kwargs.update({"load_in_low_bit": low_bit, "torch_dtype": torch.float16})
+        else:
+            model_kwargs.update({"load_in_low_bit": low_bit, "torch_dtype": 'auto'})
+
+        model = model_cls.from_pretrained(model_path, **model_kwargs)
     if not get_enable_ipex():
         model = model.eval()
 
     if device == "xpu":
         import intel_extension_for_pytorch as ipex
         model = model.to('xpu')
 
     return model, tokenizer
 
 
-def try_run_test_generation(local_model_hub, model_path, device, low_bit):
+def try_run_test_generation(local_model_hub, model_path, device, low_bit, load_low_bit_model):
     path = get_model_path(model_path, local_model_hub)
     try:
-        run_test_generation(path, device, low_bit)
+        run_test_generation(path, device, low_bit, load_low_bit_model)
     except:
         print(f"Loading model failed for model {model_path} \
-              with device:{device} and low_bit:{low_bit}")
+              with device:{device} and low_bit:{low_bit} \
+              and load_low_bit_model {load_low_bit_model}")
         return "False"
     return "True"
 
 
 def get_model_path(repo_id, local_model_hub):
     if local_model_hub:
         repo_model_name = repo_id.split("/")[1]
@@ -101,19 +115,19 @@
         invalidInputError(os.path.isdir(local_model_path),
                           local_model_path + " not exists!, Please check your models' folder.")
         return local_model_path
     else:
         return repo_id
 
 
-def run_test_generation(model_path, device, low_bit):
-    model, tokenizer = load_model(model_path, device, low_bit, True)
+def run_test_generation(model_path, device, low_bit, load_low_bit_model):
+    # Disable speculative by default
+    model, tokenizer = load_model(model_path, device, low_bit, True, False, load_low_bit_model)
     with torch.inference_mode():
         prompt = "What is AI?"
-        # TODO: if gpu, will need to move the tensor to xpu
         input_ids = tokenizer.encode(prompt, return_tensors="pt")
         if device == 'xpu':
             input_ids = input_ids.to('xpu')
         st = time.time()
         # if your selected model is capable of utilizing previous key/value attentions
         # to enhance decoding speed, but has `"use_cache": false` in its model config,
         # it is important to set `use_cache=True` explicitly in the `generate` function
@@ -129,24 +143,29 @@
         print(output_str)
 
 
 # Provide a main method for test loads
 # Note that this only test loading models instead of generation correctness
 if __name__ == '__main__':
     import os
-    # TODO: move config.yaml to a different folder
     current_dir = os.path.dirname(os.path.realpath(__file__))
     results = []
     from omegaconf import OmegaConf
     conf = OmegaConf.load(f'{current_dir}/load_config.yaml')
     today = date.today()
     import pandas as pd
     csv_name = f'{current_dir}/loader-results-{today}.csv'
     for model in conf.repo_id:
         for low_bit in conf.low_bit:
             for device in conf.device:
-                result = try_run_test_generation(conf['local_model_hub'], model, device, low_bit)
-                results.append([model, device, low_bit, result])
+                result = try_run_test_generation(conf['local_model_hub'],
+                                                 model,
+                                                 device,
+                                                 low_bit,
+                                                 conf["load_low_bit_model"]
+                                                 )
+                results.append([model, device, low_bit, conf["load_low_bit_model"], result])
 
-    df = pd.DataFrame(results, columns=['model', 'device', 'low_bit', 'result'])
+    df = pd.DataFrame(results,
+                      columns=['model', 'device', 'low_bit', 'use_low_bit_model', 'result'])
     df.to_csv(csv_name)
     results = []
```

## Comparing `ipex_llm-2.1.0b20240512.data/scripts/llm-chat.ps1` & `ipex_llm-2.1.0b20240513.data/scripts/llm-chat.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240512.data/scripts/llm-cli.ps1` & `ipex_llm-2.1.0b20240513.data/scripts/llm-cli.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240512.dist-info/METADATA` & `ipex_llm-2.1.0b20240513.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipex-llm
-Version: 2.1.0b20240512
+Version: 2.1.0b20240513
 Summary: Large Language Model Develop Toolkit
 Home-page: https://github.com/intel-analytics/BigDL
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: windows
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 Requires-Dist: transformers (==4.31.0) ; extra == 'all'
 Requires-Dist: sentencepiece ; extra == 'all'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'all'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'all'
 Requires-Dist: tabulate ; extra == 'all'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'all'
 Provides-Extra: cpp
-Requires-Dist: bigdl-core-cpp (==2.5.0b20240512) ; extra == 'cpp'
+Requires-Dist: bigdl-core-cpp (==2.5.0b20240513) ; extra == 'cpp'
 Provides-Extra: llama-index
 Requires-Dist: py-cpuinfo ; extra == 'llama-index'
 Requires-Dist: protobuf ; extra == 'llama-index'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'llama-index'
 Requires-Dist: numpy (==1.26.4) ; extra == 'llama-index'
 Requires-Dist: sentencepiece ; extra == 'llama-index'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'llama-index'
@@ -51,31 +51,31 @@
 Requires-Dist: sentencepiece ; extra == 'xpu'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu'
 Requires-Dist: tabulate ; extra == 'xpu'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240512) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240512) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240513) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240513) ; extra == 'xpu'
 Provides-Extra: xpu-2-1
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-1'
 Requires-Dist: protobuf ; extra == 'xpu-2-1'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-1'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-1'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-1'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-1'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-1'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-1'
 Requires-Dist: tabulate ; extra == 'xpu-2-1'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240512) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240512) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240513) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240513) ; extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu'
 
 
 IPEX LLM
```

## Comparing `ipex_llm-2.1.0b20240512.dist-info/RECORD` & `ipex_llm-2.1.0b20240513.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -38,63 +38,63 @@
 ipex_llm/langchain/embeddings/bigdlllm.py,sha256=auNueZ-S5RQrngss_huXlYdWImX2vPYfuEVOZsx35rk,13589
 ipex_llm/langchain/embeddings/transformersembeddings.py,sha256=hBtqBfGmGg_xjb4Us7hLNfyvbLMo5mJk9a0iooOWtPM,7225
 ipex_llm/langchain/llms/__init__.py,sha256=vBCl9JF45vnk9CWBG1k8lp8J6F8OCR9UY2E-idkkm5Y,1636
 ipex_llm/langchain/llms/bigdlllm.py,sha256=FAZG6cAIJhRgbxm16gMq-cyBwLe-u165zE7yyxD7r9E,24438
 ipex_llm/langchain/llms/transformersllm.py,sha256=7eaIkJi1CbTCSgNxBCoZTe-o_5FYjD1GTYPWpn0Ccr4,10576
 ipex_llm/langchain/llms/transformerspipelinellm.py,sha256=vm522YPPwWxxAPVvQBtxRfBinC4hIbXdKW6VjHDaFXY,7379
 ipex_llm/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ipex_llm/libs/bloom-api.dll,sha256=RSut-8s3SQXZTptSXg394Q1pwn-eCeyLUQ1jLpWqBE0,36352
-ipex_llm/libs/bloom.dll,sha256=fwc8RviRxK41OUmBJd0MrVGpnH9aDzwnOItIotpxFP8,470528
-ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=8v1kgwoWrBC3RGPLWYQdNNbk1E0G16YdQVTsFbUbyQs,853504
-ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=8n1w9-XuY5dRFKUYdengwfshZDWbLG85E2qjKedNKgc,856576
-ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=XrsXC1Ib-2nahn1dlzzLmCZXud69dY464EZgZl0XOuI,844288
-ipex_llm/libs/gptneox-api.dll,sha256=tfVpNVZrMhCYgxt4JAB_AfaZnrwwthBgCIWdszs4iX0,24576
-ipex_llm/libs/gptneox.dll,sha256=vrXE754oRIVazPgclegxD9G4SFS2rRIFWaEZKMFc338,530432
-ipex_llm/libs/libbloom_avx.dll,sha256=Z6BJPPPDHUwKegCjU0xqUhQfJtyvs3it7ROUYWKXL0U,496128
-ipex_llm/libs/libbloom_vnni.dll,sha256=b9MT3pEWwVlWQ6Q8YsGg7HQh9SY239_d9P_L4xMoUAs,471040
-ipex_llm/libs/libgptneox_avx.dll,sha256=jglNc4Pu0rU_OqqW-0PxmEE6QV6h3Hd9HuEw5GSd9xw,556032
-ipex_llm/libs/libgptneox_vnni.dll,sha256=FwMPthTJsKDh_0HbQp2Y3dZrwfnoUHjDJvYLw3pe_gM,530944
-ipex_llm/libs/libllama_avx.dll,sha256=8fIY0P5ououmKsIEXfN_dV0_dQCqJDBrym5orgDuKcY,549888
-ipex_llm/libs/libllama_vnni.dll,sha256=0BDOc3C3IxEGqqlDsuIp899XnZ360gyJl4L1qX8SZnw,525312
-ipex_llm/libs/libstarcoder_avx.dll,sha256=RlYMotnQLHiXaxKdnBYuyA_7ae_Cl1h5rm4PbxMQuzo,586752
-ipex_llm/libs/libstarcoder_vnni.dll,sha256=cK-1dzLBzPvr9NZoT_ChXJYSTMx70kY4D4oN6fhwKMI,561664
-ipex_llm/libs/llama-api.dll,sha256=ci-EwSoc9lXK14gQjbmWI4p73TiCVAhfmnNXgE9lvk4,25088
-ipex_llm/libs/llama.dll,sha256=8JxS6yrv2SyIwD1fNkvi1KUzXFrXuYBCdfCVHmds_H0,524288
-ipex_llm/libs/main-bloom.exe,sha256=PnJr56BD_su_43qGbYUJNEXeANx59-N4WjEcgx22gYw,103424
-ipex_llm/libs/main-chatglm_vnni.exe,sha256=tk8Kk-bMV9WIVOBHv6K2eVkKtcGmoi-vy0QIkHG9qdg,726016
-ipex_llm/libs/main-gptneox.exe,sha256=ouawZb69pnBiYa2hr4t4TxGZpFtne1LgBKYKVBIaqIU,98816
-ipex_llm/libs/main-llama.exe,sha256=u_Ec6ioZEbdnTVbx3eTvPl4_vf-_Z4mlW_TrWSnZsdc,99840
-ipex_llm/libs/main-starcoder.exe,sha256=ixuV96B9L3QSQsMjiYCAfFcXTYnH-jgyKlSvU7vsc_8,157696
-ipex_llm/libs/quantize-bloom.exe,sha256=I4Wc4M6yGgn_i2E2g6FHDTJOzNmVnEmeGo7HyfveQFQ,126464
-ipex_llm/libs/quantize-bloom_vnni.exe,sha256=0X2xQm-z8JiuRrpSEcys2rXTd-pOI1XMcHVD94uC0Y0,127488
-ipex_llm/libs/quantize-gptneox.exe,sha256=nMvEk7onjUzmY8BSPZaHYgZv5TGZzAXET9w0Mh-MPmw,103936
-ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=xYUsJDMexpH0mMEP7NV1EitYn_Rh2tnsEemNsEKkv64,104448
-ipex_llm/libs/quantize-llama.exe,sha256=ywQVS196fBX25LQNx5bZYavR942p6o4OyrZ0kxubaOk,109056
-ipex_llm/libs/quantize-llama_vnni.exe,sha256=RjXGxp9wQGtgVLrbl1y5dg1tUJMU4jCDxMKVfwGzaFY,110080
-ipex_llm/libs/quantize-starcoder.exe,sha256=JZCTccbM8ACBTnFc6mb7gkVPwfRzZDcTQFhTnJaonuo,126976
-ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=FqiFtKBX2gNQtheZ_yKE5kYbqfDXZrk7LftdQnDRwU4,128512
-ipex_llm/libs/starcoder-api.dll,sha256=Bxlqr83aucXccNZnPBkYh9NogvF2kuP7DQjMpLGzJCM,21504
-ipex_llm/libs/starcoder.dll,sha256=eJt8Y10pnCez-M3EbCIA4mEAxeCkoD_VLwZZIcN4AFM,561152
+ipex_llm/libs/bloom-api.dll,sha256=oVyG2W3coNaho4PrlYDBQ0i3UyXxqeMDCXqfDreGMYM,36352
+ipex_llm/libs/bloom.dll,sha256=5Yg_duWAzB3kTrq3dbBGCwtz-RChAP1RpdseTQ5j730,470528
+ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=DiR6CHJlm_Sf5yfQf7QkVpx2fSLnImGPpMniT4Rm2A4,853504
+ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=nXbZZyDKW1WdMWvxDxgYuIbLMhgLP3DqQ8qb3vtW8V8,856576
+ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=c1X_J97unlOLomCBT6VLZ1sJ4CJvgK7gMC2az7OO4xk,844288
+ipex_llm/libs/gptneox-api.dll,sha256=t6amoyj30od91Rm7EJnra4b3Ssu8Rh67y0ieeTa0cbA,24576
+ipex_llm/libs/gptneox.dll,sha256=_Y0O5kvr_xLWyIBU5IVb4ukuuuui6HY1O0vdZsU0n-4,530432
+ipex_llm/libs/libbloom_avx.dll,sha256=PHyAk65zVy0jsZbtDBADJdKwpSeE4-r_ye9XVUDwJRI,496128
+ipex_llm/libs/libbloom_vnni.dll,sha256=PBeZ1SWlD0CpimLfH0vcISGIZqEUV1Va_Cw6WI36fQk,471040
+ipex_llm/libs/libgptneox_avx.dll,sha256=0YIQ1S8Had12rx_OfZZii0JEOGXf03aWPag3MspXn0U,556032
+ipex_llm/libs/libgptneox_vnni.dll,sha256=XWPjDsnqdnn0vx6czd40fMFKbrX-vptl-JjGU2f4u7c,530944
+ipex_llm/libs/libllama_avx.dll,sha256=NtBNNi8GvGVQFzhnV68MZSwHGnAinTQZ26P-coZOiDA,549888
+ipex_llm/libs/libllama_vnni.dll,sha256=VyEOH-B43yb_n_2pHP0kWWLFNfXgKZXiaXqwexiW5Os,525312
+ipex_llm/libs/libstarcoder_avx.dll,sha256=SFgVkvM1G3-B4SJC7_q1RXOEFdTzqdNFVwVDk3SQrCY,586752
+ipex_llm/libs/libstarcoder_vnni.dll,sha256=D2oU00G4_y0xrZKVYBKbFZyEQihhXD5mWEDm42caKdc,561664
+ipex_llm/libs/llama-api.dll,sha256=U_63N5l-RKXDDFeQU6ImNUPYv_WExzYOBH9UDlNIIIo,25088
+ipex_llm/libs/llama.dll,sha256=Q9OEeDhmds-3XpDGDdTEBF_hfW25IElo-hZJmKhEG1Y,524288
+ipex_llm/libs/main-bloom.exe,sha256=-oqsw7GUi7ZcMWL9uezyCh7KuDBPttmQF1zfF6agzuc,103424
+ipex_llm/libs/main-chatglm_vnni.exe,sha256=hVxGhHWAY8dx_TVwYIUH0RpqZ5wUFahXIF2-uXeS_Ec,726016
+ipex_llm/libs/main-gptneox.exe,sha256=zz58YLb-m_D4_V5zmSVjExUwF9HkNjsrUeO2rchsy40,98816
+ipex_llm/libs/main-llama.exe,sha256=or3kxORlOCfEoMsrKu1TCSREMwWVqMi8p8jehkXuiE0,99840
+ipex_llm/libs/main-starcoder.exe,sha256=8W2As06kZChTZ8zVz19qg52Ib6KThHsPRJErg1PDwbY,157696
+ipex_llm/libs/quantize-bloom.exe,sha256=OmTdtCGvS-xw7Yz_hNJFaIFycFx2W6y6Pbl61MKj6bc,126464
+ipex_llm/libs/quantize-bloom_vnni.exe,sha256=W2OS1sJhstttYUoCqKqiXntHjWXhDWz-ShaREYRIKaU,127488
+ipex_llm/libs/quantize-gptneox.exe,sha256=OBncPEY4aBnAaBAtzIZUtRmIMkF94cext9hsDR2d_zQ,103936
+ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=m1n7MFkMjHwgiZO-pqUEn7o1pHZxMxH9SdWT1b8R5B4,104448
+ipex_llm/libs/quantize-llama.exe,sha256=7cqHtZPmVM1Z1FadImk7pvPA69l7lRDTUj5fUxXTcz8,109056
+ipex_llm/libs/quantize-llama_vnni.exe,sha256=jnMqWPDoCNlN63pb3DAn58RQBvwypNY1Tmh1vhPQVM4,110080
+ipex_llm/libs/quantize-starcoder.exe,sha256=hdqSogA_SG0UnQa2AXbfZa1p6069q5BdKS6xmBs2YGU,126976
+ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=DZI7jo9R645hQfYGCV_5rEt-vgjGAJuhrlBJ1ZMh-fM,128512
+ipex_llm/libs/starcoder-api.dll,sha256=Rj8tuGtcnjhweXP1jfM6Jk900ROMyNUhnkqvfaSi3co,21504
+ipex_llm/libs/starcoder.dll,sha256=P1LugYovhquzCYBltK0M8WVEytGCZoO0gJcFWDRpaL4,561152
 ipex_llm/llamaindex/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/llamaindex/llms/__init__.py,sha256=KP1lEdGqDuxPoxL1ZSH25Pm2kKMPJBWUTLR0ckSLMIU,1139
 ipex_llm/llamaindex/llms/bigdlllm.py,sha256=FQBzq1KOjfc6uofTXAha3O7TqpJkNfOFepXQmOVlbnI,26314
 ipex_llm/serving/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/bigdl_llm_model.py,sha256=NXEN_3EPmcP3dDnvug4MokEXXE2zVUnENgBYxfubqic,10084
-ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=cxg-L4hPIUPr9tQ5TVwCdH2nt7IdcAmPmkKcK13vI7s,18709
+ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=buXy_2asQJWjqjKozc_YIR9QQ-iMjV2jFe_qJ4LzcVU,19162
 ipex_llm/serving/fastchat/model_worker.py,sha256=qJSLyWNkP6z70ysq4AV5SqHzXPJJiX2tz7AORB6jEvM,16649
 ipex_llm/serving/fastchat/vllm_worker.py,sha256=r_2yiI4v69w8teNzh8mZrKMsJ0l6NvWFl8TxEkvq0ug,10801
 ipex_llm/transformers/__init__.py,sha256=8zrY1AGBb2_AeKGDWHY4PCJyzelYA4KwahD54jPoiPg,1005
 ipex_llm/transformers/bmm.py,sha256=BlYrXqeJuw-m136Nf_ST9i6WtZrX6BiTG_psTe1M3Y0,1213
-ipex_llm/transformers/convert.py,sha256=2oqYHdtfHwl5jRmwa1xz0jaqav5P_2jAo4XGO81ujPU,74718
+ipex_llm/transformers/convert.py,sha256=sA77yNK0KcGfEvsbKJuJZXsGmGG9m_68nPfpWZLZa1A,74449
 ipex_llm/transformers/convert_ipex.py,sha256=iKXo0n8fVFTOA2fNYYrByMFK0dovL-kLd2sVDk88AlQ,14334
 ipex_llm/transformers/embedding.py,sha256=f3crD31fEq0pT-d4FV_fS_9uLhgW64BofAxhHSO1QbE,4613
 ipex_llm/transformers/kv.py,sha256=PDdcXWElpiPvzVJQdkkx6Vez0mhROW4K59sngYaX0yY,4247
 ipex_llm/transformers/lisa.py,sha256=F5WxbtXQ7RdKulj83h_2DnEIgKiKGZf7zvOmg6QBl2s,3289
-ipex_llm/transformers/loader.py,sha256=I2UnUGz985Y5dElsJStUB_rQ-K8SScrYisDEqFDvBfY,5787
+ipex_llm/transformers/loader.py,sha256=0wMJ9NM0QKRB3AgVRGLmOKcSHYlQ40Rj6UXba513NG0,6812
 ipex_llm/transformers/lookup.py,sha256=qwY7glWICvBoDVB1UeoSGcmwOgf8SCE7zBGkm3uCfHk,14860
 ipex_llm/transformers/low_bit_linear.py,sha256=6Rerga4ZfTlT0OYOvWaJcFZwIDkosnHpnxuzXkb8iYc,39805
 ipex_llm/transformers/model.py,sha256=9hU7ERlCcdhqi8JRj-xvlIkicKroGvyvuBqyWKM1sCQ,36141
 ipex_llm/transformers/modelling_bigdl.py,sha256=AqbRwpSAiHmKUo2FGOiwKtytlh-35NWb6eDy7YyNzoo,6921
 ipex_llm/transformers/qlora.py,sha256=Zo-XeDvTjw_Yzc7Pc3GtyV29SQuy_Zongl1B4iYQID8,15520
 ipex_llm/transformers/relora.py,sha256=-dYzUV0P-IhO2jFdnzN9-v_sFzJpRj3ZwN9eCJzOoCw,16567
 ipex_llm/transformers/speculative.py,sha256=AEda893ENQVFSAjGYLyDLglpCwD7aaCEbL_YMiR5PT4,56660
@@ -176,14 +176,14 @@
 ipex_llm/utils/common/log4Error.py,sha256=8UgIpEJYQasQO4gMOWO22nsOgr14w1emAJy4ts1VOb0,1763
 ipex_llm/vllm/__init__.py,sha256=zBSG6nzrVF5QnpR6_f7kPhBFeowTE9gaZ7D5m98E7_w,585
 ipex_llm/vllm/ipex_llm_gpu_executor.py,sha256=pY-8XxRRX1_9MTW0TUTidxHmjmXKGsvs1AIIVWU21yM,18514
 ipex_llm/vllm/model_convert.py,sha256=jbsUSUAeVHm24CokIiLdyv6ubd_HuCrN_pnF3cLhhWE,7208
 ipex_llm/vllm/engine/__init__.py,sha256=mzPVAyZdbvfzBQi-wxZh1sbme_NElPMmtrJ9C2zh8Us,747
 ipex_llm/vllm/engine/engine.py,sha256=mVuCyoTcCX7KnK819-8fL_rNAu05WF_gql6jEcZ9bn8,5941
 ipex_llm/vllm/entrypoints/openai/api_server.py,sha256=luEdC8lW0UZuFx_cWF13Yz7s1wUrvNhHnhAW_rHa1Ps,10564
-ipex_llm-2.1.0b20240512.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
-ipex_llm-2.1.0b20240512.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
-ipex_llm-2.1.0b20240512.dist-info/METADATA,sha256=9KNbr6hvHfdkoX5ydt0I80jwtI1JqhPggU_qNqYWWk8,4013
-ipex_llm-2.1.0b20240512.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-ipex_llm-2.1.0b20240512.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
-ipex_llm-2.1.0b20240512.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
-ipex_llm-2.1.0b20240512.dist-info/RECORD,,
+ipex_llm-2.1.0b20240513.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
+ipex_llm-2.1.0b20240513.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
+ipex_llm-2.1.0b20240513.dist-info/METADATA,sha256=Xb9tH2KhaGYSdRnD0GY5MRelHBnq7GzCC4GKMO5EeJE,4013
+ipex_llm-2.1.0b20240513.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+ipex_llm-2.1.0b20240513.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
+ipex_llm-2.1.0b20240513.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
+ipex_llm-2.1.0b20240513.dist-info/RECORD,,
```

