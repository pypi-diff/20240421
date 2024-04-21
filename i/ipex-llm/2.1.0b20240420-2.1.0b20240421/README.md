# Comparing `tmp/ipex_llm-2.1.0b20240420-py3-none-win_amd64.whl.zip` & `tmp/ipex_llm-2.1.0b20240421-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5348051 bytes, number of entries: 218
+Zip file size: 5348037 bytes, number of entries: 218
 -rw-------  2.0 unx     1898 b- defN 24-Mar-25 11:36 ipex_llm/__init__.py
 -rw-------  2.0 unx     6816 b- defN 24-Mar-25 11:36 ipex_llm/convert_model.py
 -rw-------  2.0 unx     3091 b- defN 24-Apr-17 15:07 ipex_llm/llm_patching.py
 -rw-------  2.0 unx     1177 b- defN 24-Mar-25 11:36 ipex_llm/models.py
 -rw-------  2.0 unx    12404 b- defN 24-Apr-18 12:34 ipex_llm/optimize.py
 -rw-------  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-chat.ps1
 -rwx------  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-cli.ps1
@@ -38,47 +38,47 @@
 -rw-------  2.0 unx     1189 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/__init__.py
 -rw-------  2.0 unx    13589 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/bigdlllm.py
 -rw-------  2.0 unx     7225 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/transformersembeddings.py
 -rw-------  2.0 unx     1636 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/__init__.py
 -rw-------  2.0 unx    24438 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/bigdlllm.py
 -rw-------  2.0 unx    10576 b- defN 24-Apr-03 15:07 ipex_llm/langchain/llms/transformersllm.py
 -rw-------  2.0 unx     7379 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformerspipelinellm.py
--rw-------  2.0 unx        0 b- defN 24-Apr-20 15:08 ipex_llm/libs/__init__.py
--rw-------  2.0 unx    36352 b- defN 24-Apr-20 15:08 ipex_llm/libs/bloom-api.dll
--rw-------  2.0 unx   460288 b- defN 24-Apr-20 15:08 ipex_llm/libs/bloom.dll
--rw-------  2.0 unx   852992 b- defN 24-Apr-20 15:08 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
--rw-------  2.0 unx   856064 b- defN 24-Apr-20 15:08 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
--rw-------  2.0 unx   843776 b- defN 24-Apr-20 15:08 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
--rw-------  2.0 unx    24576 b- defN 24-Apr-20 15:08 ipex_llm/libs/gptneox-api.dll
--rw-------  2.0 unx   520192 b- defN 24-Apr-20 15:08 ipex_llm/libs/gptneox.dll
--rw-------  2.0 unx   485888 b- defN 24-Apr-20 15:08 ipex_llm/libs/libbloom_avx.dll
--rw-------  2.0 unx   460800 b- defN 24-Apr-20 15:08 ipex_llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   545792 b- defN 24-Apr-20 15:08 ipex_llm/libs/libgptneox_avx.dll
--rw-------  2.0 unx   520704 b- defN 24-Apr-20 15:08 ipex_llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   540160 b- defN 24-Apr-20 15:08 ipex_llm/libs/libllama_avx.dll
--rw-------  2.0 unx   515072 b- defN 24-Apr-20 15:08 ipex_llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   577024 b- defN 24-Apr-20 15:08 ipex_llm/libs/libstarcoder_avx.dll
--rw-------  2.0 unx   551936 b- defN 24-Apr-20 15:08 ipex_llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 24-Apr-20 15:08 ipex_llm/libs/llama-api.dll
--rw-------  2.0 unx   514560 b- defN 24-Apr-20 15:08 ipex_llm/libs/llama.dll
--rw-------  2.0 unx   103424 b- defN 24-Apr-20 15:08 ipex_llm/libs/main-bloom.exe
--rw-------  2.0 unx   726016 b- defN 24-Apr-20 15:08 ipex_llm/libs/main-chatglm_vnni.exe
--rw-------  2.0 unx    98816 b- defN 24-Apr-20 15:08 ipex_llm/libs/main-gptneox.exe
--rw-------  2.0 unx    99840 b- defN 24-Apr-20 15:08 ipex_llm/libs/main-llama.exe
--rw-------  2.0 unx   157696 b- defN 24-Apr-20 15:08 ipex_llm/libs/main-starcoder.exe
--rw-------  2.0 unx   125952 b- defN 24-Apr-20 15:08 ipex_llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   127488 b- defN 24-Apr-20 15:08 ipex_llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx   103936 b- defN 24-Apr-20 15:08 ipex_llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx   104448 b- defN 24-Apr-20 15:08 ipex_llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   109056 b- defN 24-Apr-20 15:08 ipex_llm/libs/quantize-llama.exe
--rw-------  2.0 unx   110080 b- defN 24-Apr-20 15:08 ipex_llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   126976 b- defN 24-Apr-20 15:08 ipex_llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   128000 b- defN 24-Apr-20 15:08 ipex_llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 24-Apr-20 15:08 ipex_llm/libs/starcoder-api.dll
--rw-------  2.0 unx   551424 b- defN 24-Apr-20 15:08 ipex_llm/libs/starcoder.dll
+-rw-------  2.0 unx        0 b- defN 24-Apr-21 15:08 ipex_llm/libs/__init__.py
+-rw-------  2.0 unx    36352 b- defN 24-Apr-21 15:08 ipex_llm/libs/bloom-api.dll
+-rw-------  2.0 unx   460288 b- defN 24-Apr-21 15:08 ipex_llm/libs/bloom.dll
+-rw-------  2.0 unx   852992 b- defN 24-Apr-21 15:08 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
+-rw-------  2.0 unx   856064 b- defN 24-Apr-21 15:08 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
+-rw-------  2.0 unx   843776 b- defN 24-Apr-21 15:08 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
+-rw-------  2.0 unx    24576 b- defN 24-Apr-21 15:08 ipex_llm/libs/gptneox-api.dll
+-rw-------  2.0 unx   520192 b- defN 24-Apr-21 15:08 ipex_llm/libs/gptneox.dll
+-rw-------  2.0 unx   485888 b- defN 24-Apr-21 15:08 ipex_llm/libs/libbloom_avx.dll
+-rw-------  2.0 unx   460800 b- defN 24-Apr-21 15:08 ipex_llm/libs/libbloom_vnni.dll
+-rw-------  2.0 unx   545792 b- defN 24-Apr-21 15:08 ipex_llm/libs/libgptneox_avx.dll
+-rw-------  2.0 unx   520704 b- defN 24-Apr-21 15:08 ipex_llm/libs/libgptneox_vnni.dll
+-rw-------  2.0 unx   540160 b- defN 24-Apr-21 15:08 ipex_llm/libs/libllama_avx.dll
+-rw-------  2.0 unx   515072 b- defN 24-Apr-21 15:08 ipex_llm/libs/libllama_vnni.dll
+-rw-------  2.0 unx   577024 b- defN 24-Apr-21 15:08 ipex_llm/libs/libstarcoder_avx.dll
+-rw-------  2.0 unx   551936 b- defN 24-Apr-21 15:08 ipex_llm/libs/libstarcoder_vnni.dll
+-rw-------  2.0 unx    25088 b- defN 24-Apr-21 15:08 ipex_llm/libs/llama-api.dll
+-rw-------  2.0 unx   514560 b- defN 24-Apr-21 15:08 ipex_llm/libs/llama.dll
+-rw-------  2.0 unx   103424 b- defN 24-Apr-21 15:08 ipex_llm/libs/main-bloom.exe
+-rw-------  2.0 unx   726016 b- defN 24-Apr-21 15:08 ipex_llm/libs/main-chatglm_vnni.exe
+-rw-------  2.0 unx    98816 b- defN 24-Apr-21 15:08 ipex_llm/libs/main-gptneox.exe
+-rw-------  2.0 unx    99840 b- defN 24-Apr-21 15:08 ipex_llm/libs/main-llama.exe
+-rw-------  2.0 unx   157696 b- defN 24-Apr-21 15:08 ipex_llm/libs/main-starcoder.exe
+-rw-------  2.0 unx   125952 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-bloom.exe
+-rw-------  2.0 unx   127488 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-bloom_vnni.exe
+-rw-------  2.0 unx   103936 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-gptneox.exe
+-rw-------  2.0 unx   104448 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-gptneox_vnni.exe
+-rw-------  2.0 unx   109056 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-llama.exe
+-rw-------  2.0 unx   110080 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-llama_vnni.exe
+-rw-------  2.0 unx   126976 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-starcoder.exe
+-rw-------  2.0 unx   128000 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-starcoder_vnni.exe
+-rw-------  2.0 unx    21504 b- defN 24-Apr-21 15:08 ipex_llm/libs/starcoder-api.dll
+-rw-------  2.0 unx   551424 b- defN 24-Apr-21 15:08 ipex_llm/libs/starcoder.dll
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/__init__.py
 -rw-------  2.0 unx     1139 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/__init__.py
 -rw-------  2.0 unx    26314 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/bigdlllm.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/__init__.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/__init__.py
 -rw-------  2.0 unx    10084 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/bigdl_llm_model.py
 -rw-------  2.0 unx    11371 b- defN 24-Mar-27 11:49 ipex_llm/serving/fastchat/ipex_llm_worker.py
@@ -206,15 +206,15 @@
 -rw-------  2.0 unx     8707 b- defN 24-Mar-25 11:36 ipex_llm/vllm/transformers_utils/tokenizer.py
 -rw-------  2.0 unx    13950 b- defN 24-Mar-25 11:36 ipex_llm/vllm/worker/worker.py
 -rw-------  2.0 unx      585 b- defN 24-Apr-18 12:34 ipex_llm/vllm2/__init__.py
 -rw-------  2.0 unx     7208 b- defN 24-Apr-18 12:34 ipex_llm/vllm2/model_convert.py
 -rw-------  2.0 unx      747 b- defN 24-Apr-18 12:34 ipex_llm/vllm2/engine/__init__.py
 -rw-------  2.0 unx     5715 b- defN 24-Apr-18 12:34 ipex_llm/vllm2/engine/engine.py
 -rw-------  2.0 unx    10475 b- defN 24-Apr-18 12:34 ipex_llm/vllm2/entrypoints/openai/api_server.py
--rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240420.data/scripts/llm-chat.ps1
--rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240420.data/scripts/llm-cli.ps1
--rw-------  2.0 unx     4400 b- defN 24-Apr-20 15:08 ipex_llm-2.1.0b20240420.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 24-Apr-20 15:08 ipex_llm-2.1.0b20240420.dist-info/WHEEL
--rw-------  2.0 unx       61 b- defN 24-Apr-20 15:08 ipex_llm-2.1.0b20240420.dist-info/entry_points.txt
--rw-------  2.0 unx        9 b- defN 24-Apr-20 15:08 ipex_llm-2.1.0b20240420.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    20723 b- defN 24-Apr-20 15:08 ipex_llm-2.1.0b20240420.dist-info/RECORD
-218 files, 13087091 bytes uncompressed, 5314925 bytes compressed:  59.4%
+-rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240421.data/scripts/llm-chat.ps1
+-rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240421.data/scripts/llm-cli.ps1
+-rw-------  2.0 unx     4400 b- defN 24-Apr-21 15:08 ipex_llm-2.1.0b20240421.dist-info/METADATA
+-rw-------  2.0 unx       98 b- defN 24-Apr-21 15:08 ipex_llm-2.1.0b20240421.dist-info/WHEEL
+-rw-------  2.0 unx       61 b- defN 24-Apr-21 15:08 ipex_llm-2.1.0b20240421.dist-info/entry_points.txt
+-rw-------  2.0 unx        9 b- defN 24-Apr-21 15:08 ipex_llm-2.1.0b20240421.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    20723 b- defN 24-Apr-21 15:08 ipex_llm-2.1.0b20240421.dist-info/RECORD
+218 files, 13087091 bytes uncompressed, 5314911 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -627,29 +627,29 @@
 
 Filename: ipex_llm/vllm2/engine/engine.py
 Comment: 
 
 Filename: ipex_llm/vllm2/entrypoints/openai/api_server.py
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240420.data/scripts/llm-chat.ps1
+Filename: ipex_llm-2.1.0b20240421.data/scripts/llm-chat.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240420.data/scripts/llm-cli.ps1
+Filename: ipex_llm-2.1.0b20240421.data/scripts/llm-cli.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240420.dist-info/METADATA
+Filename: ipex_llm-2.1.0b20240421.dist-info/METADATA
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240420.dist-info/WHEEL
+Filename: ipex_llm-2.1.0b20240421.dist-info/WHEEL
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240420.dist-info/entry_points.txt
+Filename: ipex_llm-2.1.0b20240421.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240420.dist-info/top_level.txt
+Filename: ipex_llm-2.1.0b20240421.dist-info/top_level.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240420.dist-info/RECORD
+Filename: ipex_llm-2.1.0b20240421.dist-info/RECORD
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
 
-Time/Date		Sat Apr 20 15:06:55 2024
+Time/Date		Sun Apr 21 15:06:15 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000003200
 SizeOfInitializedData	0000000000005e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000036cc
@@ -6375,18 +6375,16 @@
    180005621:	push   %rdx
    180005622:	add    %al,0x1(%rax)
    180005628:	pop    %rax
    180005629:	push   %rdx
    18000562a:	add    %al,0x1(%rax)
    180005630:	add    %al,(%rax)
    180005632:	add    %al,(%rax)
-   180005634:	pminub (%rbx),%mm4
-   180005637:	data16 add %al,(%rax)
-   18000563a:	add    %al,(%rax)
-   18000563c:	or     $0xe0000000,%eax
+   180005634:	sub    0x66(%eip),%esp        # 0x1800056a1
+   18000563b:	add    %cl,-0x20000000(%rip)        # 0x160005641
    180005641:	add    (%rax),%al
    180005643:	add    %cl,(%rcx,%rbx,2)
    180005646:	add    %al,(%rax)
    180005648:	or     $0x3f,%al
 	...
    18000567e:	add    %al,(%rax)
    180005680:	add    %eax,(%rax)
```

## ipex_llm/libs/bloom.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180052e48
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Apr 20 15:06:55 2024
+Time/Date		Sun Apr 21 15:06:15 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000053400
 SizeOfInitializedData	00000000000bee00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000052e48
@@ -109410,19 +109410,17 @@
    18005c7ba:	add    $0x180,%eax
    18005c7bf:	add    %dh,0x56(%rax)
    18005c7c2:	add    $0x180,%eax
    18005c7c7:	add    %bh,0x56(%rax)
    18005c7ca:	add    $0x180,%eax
    18005c7cf:	add    %al,(%rax)
    18005c7d1:	add    %al,(%rax)
-   18005c7d3:	add    %cl,(%rdi)
-   18005c7d5:	fisubl (%rbx)
-   18005c7d7:	data16 add %al,(%rax)
-   18005c7da:	add    %al,(%rax)
-   18005c7dc:	or     $0x50000000,%eax
+   18005c7d3:	add    %ah,0x2b(%rdi)
+   18005c7d6:	and    $0x66,%eax
+   18005c7db:	add    %cl,0x50000000(%rip)        # 0x1d005c7e1
    18005c7e1:	add    (%rax),%eax
    18005c7e3:	add    %ah,-0x5ffffa2f(%rax)
    18005c7e9:	mov    $0x5,%ecx
 	...
    18005c7fe:	add    %al,(%rax)
    18005c800:	adc    %dl,%ch
    18005c802:	add    $0x180,%eax
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
 
-Time/Date		Sat Apr 20 15:06:55 2024
+Time/Date		Sun Apr 21 15:06:15 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002600
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002cbc
@@ -5058,18 +5058,16 @@
    1800049c0:	cmp    %al,0x0(%rdx)
    1800049c3:	addb   $0x0,(%rcx)
    1800049c6:	add    %al,(%rax)
    1800049c8:	rex
    1800049c9:	rex.X add %al,0x1(%rax)
    1800049d0:	add    %al,(%rax)
    1800049d2:	add    %al,(%rax)
-   1800049d4:	pminub (%rbx),%mm4
-   1800049d7:	data16 add %al,(%rax)
-   1800049da:	add    %al,(%rax)
-   1800049dc:	or     $0xe0000000,%eax
+   1800049d4:	sub    0x66(%eip),%esp        # 0x180004a41
+   1800049db:	add    %cl,-0x20000000(%rip)        # 0x1600049e1
    1800049e1:	add    (%rax),%al
    1800049e3:	add    %ah,0x0(%rsp,%rcx,2)
    1800049e7:	add    %ah,0x0(%rsi,%rsi,1)
 	...
    1800049ff:	add    %al,(%rcx)
 	...
    180004a09:	add    %al,(%rax)
```

## ipex_llm/libs/gptneox.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005a5a8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Apr 20 15:06:56 2024
+Time/Date		Sun Apr 21 15:06:16 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005ae00
 SizeOfInitializedData	00000000000c6000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005a5a8
@@ -120845,16 +120845,15 @@
    18006307d:	add    %al,(%rax)
    18006307f:	add    %bh,0x18005c6(%rax)
    180063085:	add    %al,(%rax)
    180063087:	add    %al,%al
    180063089:	movb   $0x0,0x180(%rip)        # 0x180063210
    180063090:	add    %al,(%rax)
    180063092:	add    %al,(%rax)
-   180063094:	adc    %bl,%dl
-   180063096:	and    0x0(%rsi),%esp
+   180063094:	push   $0x66252b
    180063099:	add    %al,(%rax)
    18006309b:	add    %cl,0x50000000(%rip)        # 0x1d00630a1
    1800630a1:	add    (%rax),%eax
    1800630a3:	add    %al,0x2f040006(,%rdi,1)
    1800630aa:	(bad)
 	...
    1800630ff:	add    %bh,0x40(%rax)
```

## ipex_llm/libs/libbloom_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180058c38
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Apr 20 15:08:00 2024
+Time/Date		Sun Apr 21 15:07:21 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000059200
 SizeOfInitializedData	00000000000bf400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000058c38
@@ -114727,16 +114727,15 @@
    1800626ed:	add    %al,(%rax)
    1800626ef:	add    %dh,-0x4a(%rax)
    1800626f2:	add    $0x180,%eax
    1800626f7:	add    %bh,-0x4a(%rax)
    1800626fa:	add    $0x180,%eax
    1800626ff:	add    %al,(%rax)
    180062701:	add    %al,(%rax)
-   180062703:	add    %dl,-0x26(%rax)
-   180062706:	and    0x0(%rsi),%esp
+   180062703:	add    %ch,0x66252b(%rcx)
    180062709:	add    %al,(%rax)
    18006270b:	add    %cl,0x50000000(%rip)        # 0x1d0062711
    180062711:	add    (%rax),%eax
    180062713:	add    %ah,(%rax)
    180062715:	xor    %eax,(%rsi)
    180062717:	add    %ah,(%rax)
    180062719:	(bad)
```

## ipex_llm/libs/libbloom_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180053058
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Apr 20 15:02:25 2024
+Time/Date		Sun Apr 21 15:02:49 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000053600
 SizeOfInitializedData	00000000000bee00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000053058
@@ -109461,19 +109461,17 @@
    18005c79a:	add    $0x180,%eax
    18005c79f:	add    %dh,0x56(%rax)
    18005c7a2:	add    $0x180,%eax
    18005c7a7:	add    %bh,0x56(%rax)
    18005c7aa:	add    $0x180,%eax
    18005c7af:	add    %al,(%rax)
    18005c7b1:	add    %al,(%rax)
-   18005c7b3:	add    %al,(%rcx)
-   18005c7b5:	fldenv (%rbx)
-   18005c7b7:	data16 add %al,(%rax)
-   18005c7ba:	add    %al,(%rax)
-   18005c7bc:	or     $0x50000000,%eax
+   18005c7b3:	add    %bl,0x66252a(%rcx)
+   18005c7b9:	add    %al,(%rax)
+   18005c7bb:	add    %cl,0x50000000(%rip)        # 0x1d005c7c1
    18005c7c1:	add    (%rax),%eax
    18005c7c3:	add    %ah,-0x5ffffa2f(%rax)
    18005c7c9:	mov    $0x5,%ebx
 	...
    18005c7fe:	add    %al,(%rax)
    18005c800:	adc    %dl,%ch
    18005c802:	add    $0x180,%eax
```

## ipex_llm/libs/libgptneox_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180060428
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Apr 20 15:08:01 2024
+Time/Date		Sun Apr 21 15:07:21 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000060c00
 SizeOfInitializedData	00000000000c6600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000060428
@@ -126192,19 +126192,17 @@
    180068fb5:	add    %al,(%rax)
    180068fb7:	add    %al,%al
    180068fb9:	es (bad)
    180068fbb:	addb   $0x0,(%rcx)
    180068fbe:	add    %al,(%rax)
    180068fc0:	add    %al,(%rax)
    180068fc2:	add    %al,(%rax)
-   180068fc4:	push   %rcx
-   180068fc5:	fisubl (%rbx)
-   180068fc7:	data16 add %al,(%rax)
-   180068fca:	add    %al,(%rax)
-   180068fcc:	or     $0x50000000,%eax
+   180068fc4:	test   $0x66252b,%eax
+   180068fc9:	add    %al,(%rax)
+   180068fcb:	add    %cl,0x50000000(%rip)        # 0x1d0068fd1
    180068fd1:	add    (%rax),%eax
    180068fd3:	add    %al,(%rsp,%rbx,4)
    180068fd6:	(bad)
    180068fd7:	add    %al,(%rsp,%rcx,4)
    180068fda:	(bad)
 	...
    180068fff:	add    %bh,-0x61(%rax)
```

## ipex_llm/libs/libgptneox_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005a7b8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Apr 20 15:02:26 2024
+Time/Date		Sun Apr 21 15:02:49 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005b000
 SizeOfInitializedData	00000000000c6000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005a7b8
@@ -121007,17 +121007,16 @@
    18006305d:	add    %al,(%rax)
    18006305f:	add    %bh,0x18005c6(%rax)
    180063065:	add    %al,(%rax)
    180063067:	add    %al,%al
    180063069:	movb   $0x0,0x180(%rip)        # 0x1800631f0
    180063070:	add    %al,(%rax)
    180063072:	add    %al,(%rax)
-   180063074:	add    %cl,%bl
-   180063076:	and    0x0(%rsi),%esp
-   180063079:	add    %al,(%rax)
+   180063074:	cltd
+   180063075:	sub    0x66(%rip),%ah        # 0x1800630e1
    18006307b:	add    %cl,0x50000000(%rip)        # 0x1d0063081
    180063081:	add    (%rax),%eax
    180063083:	add    %al,0x31040006(,%rdi,1)
    18006308a:	(bad)
 	...
    1800630ff:	add    %bh,0x40(%rax)
    180063102:	(bad)
```

## ipex_llm/libs/libllama_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005f138
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Apr 20 15:08:00 2024
+Time/Date		Sun Apr 21 15:07:21 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005f800
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005f138
@@ -124880,19 +124880,17 @@
    180068096:	add    %al,(%rax)
    180068098:	rclb   $1,(%rsi)
    18006809a:	(bad)
    18006809b:	addb   $0x0,(%rcx)
    18006809e:	add    %al,(%rax)
    1800680a0:	add    %al,(%rax)
    1800680a2:	add    %al,(%rax)
-   1800680a4:	push   %rax
-   1800680a5:	fisubl (%rbx)
-   1800680a7:	data16 add %al,(%rax)
-   1800680aa:	add    %al,(%rax)
-   1800680ac:	or     $0x50000000,%eax
+   1800680a4:	test   $0x66252b,%eax
+   1800680a9:	add    %al,(%rax)
+   1800680ab:	add    %cl,0x50000000(%rip)        # 0x1d00680b1
    1800680b1:	add    (%rax),%eax
    1800680b3:	add    %al,(%rax)
    1800680b5:	lea    (%rsi),%eax
    1800680b7:	add    %al,(%rax)
    1800680b9:	jns    0x1800680c1
 	...
    1800680ff:	add    %dh,-0x70(%rax)
```

## ipex_llm/libs/libllama_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800594c8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Apr 20 15:02:26 2024
+Time/Date		Sun Apr 21 15:02:49 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000059c00
 SizeOfInitializedData	00000000000c5e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000594c8
@@ -119683,17 +119683,16 @@
    180062140:	enter  $0x5b6,$0x80
    180062144:	add    %eax,(%rax)
    180062146:	add    %al,(%rax)
    180062148:	shlb   $1,0x18005(%rsi)
    18006214e:	add    %al,(%rax)
    180062150:	add    %al,(%rax)
    180062152:	add    %al,(%rax)
-   180062154:	add    %cl,%bl
-   180062156:	and    0x0(%rsi),%esp
-   180062159:	add    %al,(%rax)
+   180062154:	cltd
+   180062155:	sub    0x66(%rip),%ah        # 0x1800621c1
    18006215b:	add    %cl,0x50000000(%rip)        # 0x1d0062161
    180062161:	add    (%rax),%eax
    180062163:	add    %al,-0x7ffff9d3(%rax)
    180062169:	sbb    $0x6,%eax
 	...
    18006217e:	add    %al,(%rax)
    180062180:	lock xor %al,(%rsi)
```

## ipex_llm/libs/libstarcoder_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180066598
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Apr 20 15:08:00 2024
+Time/Date		Sun Apr 21 15:07:20 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000066c00
 SizeOfInitializedData	00000000000c8000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000066598
@@ -135439,19 +135439,17 @@
    18006fbe5:	add    %al,(%rax)
    18006fbe7:	add    %al,%al
    18006fbe9:	xchg   %al,(%rsi)
    18006fbeb:	addb   $0x0,(%rcx)
    18006fbee:	add    %al,(%rax)
    18006fbf0:	add    %al,(%rax)
    18006fbf2:	add    %al,(%rax)
-   18006fbf4:	push   %rax
-   18006fbf5:	fisubl (%rbx)
-   18006fbf7:	data16 add %al,(%rax)
-   18006fbfa:	add    %al,(%rax)
-   18006fbfc:	or     $0x50000000,%eax
+   18006fbf4:	test   $0x2b,%al
+   18006fbf6:	and    $0x66,%eax
+   18006fbfb:	add    %cl,0x50000000(%rip)        # 0x1d006fc01
    18006fc01:	add    (%rax),%eax
    18006fc03:	add    %dl,%al
    18006fc05:	or     $0xfdd00007,%eax
    18006fc0a:	(bad)
 	...
    18006fc7f:	add    %al,0x11(%rax)
    18006fc82:	(bad)
```

## ipex_llm/libs/libstarcoder_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800609b8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Apr 20 15:02:25 2024
+Time/Date		Sun Apr 21 15:02:49 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000061000
 SizeOfInitializedData	00000000000c7a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000609b8
@@ -130151,17 +130151,16 @@
    180069cb5:	add    %al,(%rax)
    180069cb7:	add    %al,%al
    180069cb9:	es (bad)
    180069cbb:	addb   $0x0,(%rcx)
    180069cbe:	add    %al,(%rax)
    180069cc0:	add    %al,(%rax)
    180069cc2:	add    %al,(%rax)
-   180069cc4:	add    %ebx,%ecx
-   180069cc6:	and    0x0(%rsi),%esp
-   180069cc9:	add    %al,(%rax)
+   180069cc4:	cltd
+   180069cc5:	sub    0x66(%rip),%ah        # 0x180069d31
    180069ccb:	add    %cl,0x50000000(%rip)        # 0x1d0069cd1
    180069cd1:	add    (%rax),%eax
    180069cd3:	add    %dl,-0x52(%rax)
    180069cd6:	(bad)
    180069cd7:	add    %dl,-0x5e(%rax)
    180069cda:	(bad)
 	...
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
 
-Time/Date		Sat Apr 20 15:06:55 2024
+Time/Date		Sun Apr 21 15:06:15 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002800
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002dac
@@ -5355,18 +5355,16 @@
    180004a20:	cmp    %al,0x0(%rdx)
    180004a23:	addb   $0x0,(%rcx)
    180004a26:	add    %al,(%rax)
    180004a28:	rex
    180004a29:	rex.X add %al,0x1(%rax)
    180004a30:	add    %al,(%rax)
    180004a32:	add    %al,(%rax)
-   180004a34:	pminub (%rbx),%mm4
-   180004a37:	data16 add %al,(%rax)
-   180004a3a:	add    %al,(%rax)
-   180004a3c:	or     $0xe0000000,%eax
+   180004a34:	sub    0x66(%eip),%esp        # 0x180004aa1
+   180004a3b:	add    %cl,-0x20000000(%rip)        # 0x160004a41
    180004a41:	add    (%rax),%al
    180004a43:	add    %ah,%ah
    180004a45:	rex.WR add %r8b,(%rax)
    180004a48:	in     $0x38,%al
 	...
    180004a7e:	add    %al,(%rax)
    180004a80:	add    %eax,(%rax)
```

## ipex_llm/libs/llama.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800592b8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Apr 20 15:06:56 2024
+Time/Date		Sun Apr 21 15:06:16 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000059a00
 SizeOfInitializedData	00000000000c5e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000592b8
@@ -119535,16 +119535,15 @@
    180062160:	enter  $0x5b6,$0x80
    180062164:	add    %eax,(%rax)
    180062166:	add    %al,(%rax)
    180062168:	shlb   $1,0x18005(%rsi)
    18006216e:	add    %al,(%rax)
    180062170:	add    %al,(%rax)
    180062172:	add    %al,(%rax)
-   180062174:	adc    %bl,%dl
-   180062176:	and    0x0(%rsi),%esp
+   180062174:	push   $0x66252b
    180062179:	add    %al,(%rax)
    18006217b:	add    %cl,0x50000000(%rip)        # 0x1d0062181
    180062181:	add    (%rax),%eax
    180062183:	add    %al,(%rax)
    180062185:	cs (bad)
    180062187:	add    %al,(%rax)
    180062189:	sbb    $0x6,%al
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
 
-Time/Date		Sat Apr 20 15:06:55 2024
+Time/Date		Sun Apr 21 15:06:15 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010800
 SizeOfInitializedData	0000000000008e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001045c
@@ -25509,18 +25509,16 @@
    140014ab0:	enter  $0x125,$0x40
    140014ab4:	add    %eax,(%rax)
    140014ab6:	add    %al,(%rax)
    140014ab8:	shlb   $1,0x14001(%rip)        # 0x140028abf
    140014abe:	add    %al,(%rax)
    140014ac0:	add    %al,(%rax)
    140014ac2:	add    %al,(%rax)
-   140014ac4:	pminub (%rbx),%mm4
-   140014ac7:	data16 add %al,(%rax)
-   140014aca:	add    %al,(%rax)
-   140014acc:	or     $0x20000000,%eax
+   140014ac4:	sub    0x66(%eip),%esp        # 0x140014b31
+   140014acb:	add    %cl,0x20000000(%rip)        # 0x160014ad1
    140014ad1:	add    (%rax),%eax
    140014ad3:	add    %cl,%ah
    140014ad5:	push   %rsp
    140014ad6:	add    %eax,(%rax)
    140014ad8:	int3
    140014ad9:	rex add %eax,(%rax)
 	...
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
 
-Time/Date		Sat Apr 20 15:02:54 2024
+Time/Date		Sun Apr 21 15:03:17 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000087c00
 SizeOfInitializedData	00000000000cbe00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000836cc
@@ -189024,19 +189024,17 @@
    140093ea5:	add    %al,(%rax)
    140093ea7:	add    %al,(%rax)
    140093ea9:	cltd
    140093eaa:	or     %al,0x1(%rax)
    140093ead:	add    %al,(%rax)
    140093eaf:	add    %al,(%rax)
    140093eb1:	add    %al,(%rax)
-   140093eb3:	add    %bl,(%rsi)
-   140093eb5:	fldenv (%rbx)
-   140093eb7:	data16 add %al,(%rax)
-   140093eba:	add    %al,(%rax)
-   140093ebc:	or     $0xcc000000,%eax
+   140093eb3:	add    %dh,0x66252a(%rbp)
+   140093eb9:	add    %al,(%rax)
+   140093ebb:	add    %cl,-0x34000000(%rip)        # 0x10c093ec1
    140093ec1:	add    (%rax),%eax
    140093ec3:	add    %dl,(%rax)
    140093ec5:	jae    0x140093ed0
    140093ec7:	add    %dl,(%rax)
    140093ec9:	movsxd (%rcx),%ecx
 	...
    140093eff:	add    %al,(%rax)
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
 
-Time/Date		Sat Apr 20 15:06:55 2024
+Time/Date		Sun Apr 21 15:06:15 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f200
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000ef6c
@@ -24136,18 +24136,16 @@
    140013edf:	add    %ch,%al
    140013ee1:	adc    $0x14001,%eax
    140013ee6:	add    %al,(%rax)
    140013ee8:	lock adc $0x14001,%eax
    140013eee:	add    %al,(%rax)
    140013ef0:	add    %al,(%rax)
    140013ef2:	add    %al,(%rax)
-   140013ef4:	pminub (%rbx),%mm4
-   140013ef7:	data16 add %al,(%rax)
-   140013efa:	add    %al,(%rax)
-   140013efc:	or     $0x90000000,%eax
+   140013ef4:	sub    0x66(%eip),%esp        # 0x140013f61
+   140013efb:	add    %cl,-0x70000000(%rip)        # 0xd0013f01
    140013f01:	add    (%rax),%eax
    140013f03:	add    %ch,0x1(%rcx,%rcx,2)
    140013f07:	add    %ch,0x1(%rdi,%rbp,1)
 	...
    140013f7f:	add    %ah,(%rax)
    140013f81:	add    %r8,0x1(%r8)
    140013f85:	add    %al,(%rax)
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
 
-Time/Date		Sat Apr 20 15:06:55 2024
+Time/Date		Sun Apr 21 15:06:15 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f600
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000f32c
@@ -24679,18 +24679,16 @@
    140013faf:	add    %ch,%al
    140013fb1:	adc    $0x14001,%eax
    140013fb6:	add    %al,(%rax)
    140013fb8:	lock adc $0x14001,%eax
    140013fbe:	add    %al,(%rax)
    140013fc0:	add    %al,(%rax)
    140013fc2:	add    %al,(%rax)
-   140013fc4:	pminub (%rbx),%mm4
-   140013fc7:	data16 add %al,(%rax)
-   140013fca:	add    %al,(%rax)
-   140013fcc:	or     $0x90000000,%eax
+   140013fc4:	sub    0x66(%eip),%esp        # 0x140014031
+   140013fcb:	add    %cl,-0x70000000(%rip)        # 0xd0013fd1
    140013fd1:	add    (%rax),%eax
    140013fd3:	add    %ch,%ah
    140013fd5:	add    %rax,(%r8)
    140013fd8:	in     (%dx),%al
    140013fd9:	xor    (%rcx),%eax
 	...
    140013fff:	add    %ah,0x140014d(%rax)
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
 
-Time/Date		Sat Apr 20 15:06:55 2024
+Time/Date		Sun Apr 21 15:06:15 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000001b000
 SizeOfInitializedData	000000000000bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001a85c
@@ -40341,19 +40341,17 @@
    14001f111:	movb   $0x40,(%rcx)
    14001f114:	add    %eax,(%rax)
    14001f116:	add    %al,(%rax)
    14001f118:	push   $0x14001c6
    14001f11d:	add    %al,(%rax)
    14001f11f:	add    %al,(%rax)
    14001f121:	add    %al,(%rax)
-   14001f123:	add    %cl,(%rdi)
-   14001f125:	fisubl (%rbx)
-   14001f127:	data16 add %al,(%rax)
-   14001f12a:	add    %al,(%rax)
-   14001f12c:	or     $0x20000000,%eax
+   14001f123:	add    %ah,0x2b(%rdi)
+   14001f126:	and    $0x66,%eax
+   14001f12b:	add    %cl,0x20000000(%rip)        # 0x16001f131
    14001f131:	add    (%rax),%eax
    14001f133:	add    %dl,(%rbx,%rax,1)
    14001f136:	add    (%rax),%al
    14001f138:	adc    $0xf7,%al
    14001f13a:	add    %eax,(%rax)
 	...
    14001f180:	add    %eax,(%rax)
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
 
-Time/Date		Sat Apr 20 15:06:55 2024
+Time/Date		Sun Apr 21 15:06:15 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013a00
 SizeOfInitializedData	00000000000acc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013918
@@ -32227,19 +32227,17 @@
    1400191a5:	add    %al,(%rax)
    1400191a7:	add    %al,(%rax)
    1400191a9:	push   %rbp
    1400191aa:	add    %eax,0x1(%rax)
    1400191ad:	add    %al,(%rax)
    1400191af:	add    %al,(%rax)
    1400191b1:	add    %al,(%rax)
-   1400191b3:	add    %cl,(%rdi)
-   1400191b5:	fisubl (%rbx)
-   1400191b7:	data16 add %al,(%rax)
-   1400191ba:	add    %al,(%rax)
-   1400191bc:	or     $0x20000000,%eax
+   1400191b3:	add    %ah,0x2b(%rdi)
+   1400191b6:	and    $0x66,%eax
+   1400191bb:	add    %cl,0x20000000(%rip)        # 0x1600191c1
    1400191c1:	add    (%rax),%eax
    1400191c3:	add    %dh,-0x5f(%rax)
    1400191c6:	add    %eax,(%rax)
    1400191c8:	jo     0x140019159
    1400191ca:	add    %eax,(%rax)
 	...
    140019200:	add    %eax,(%rax)
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
 
-Time/Date		Sat Apr 20 15:02:25 2024
+Time/Date		Sun Apr 21 15:02:49 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013b28
@@ -32344,19 +32344,17 @@
    140019185:	add    %al,(%rax)
    140019187:	add    %al,(%rax)
    140019189:	push   %rbp
    14001918a:	add    %eax,0x1(%rax)
    14001918d:	add    %al,(%rax)
    14001918f:	add    %al,(%rax)
    140019191:	add    %al,(%rax)
-   140019193:	add    %al,(%rcx)
-   140019195:	fldenv (%rbx)
-   140019197:	data16 add %al,(%rax)
-   14001919a:	add    %al,(%rax)
-   14001919c:	or     $0x20000000,%eax
+   140019193:	add    %bl,0x66252a(%rcx)
+   140019199:	add    %al,(%rax)
+   14001919b:	add    %cl,0x20000000(%rip)        # 0x1600191a1
    1400191a1:	add    (%rax),%eax
    1400191a3:	add    %dh,-0x5f(%rax)
    1400191a6:	add    %eax,(%rax)
    1400191a8:	jo     0x14001913b
    1400191aa:	add    %eax,(%rax)
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
 
-Time/Date		Sat Apr 20 15:06:54 2024
+Time/Date		Sun Apr 21 15:06:14 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010988
@@ -27188,19 +27188,17 @@
    140015f80:	push   $0x1400123
    140015f85:	add    %al,(%rax)
    140015f87:	add    %dh,0x23(%rax)
    140015f8a:	add    %eax,0x1(%rax)
    140015f8d:	add    %al,(%rax)
    140015f8f:	add    %al,(%rax)
    140015f91:	add    %al,(%rax)
-   140015f93:	add    %cl,(%rsi)
-   140015f95:	fisubl (%rbx)
-   140015f97:	data16 add %al,(%rax)
-   140015f9a:	add    %al,(%rax)
-   140015f9c:	or     $0x90000000,%eax
+   140015f93:	add    %ah,0x2b(%rsi)
+   140015f96:	and    $0x66,%eax
+   140015f9b:	add    %cl,-0x70000000(%rip)        # 0xd0015fa1
    140015fa1:	add    (%rax),%eax
    140015fa3:	add    %ch,0x65(%rax)
    140015fa6:	add    %eax,(%rax)
    140015fa8:	push   $0x153
 	...
    140015ffd:	add    %al,(%rax)
    140015fff:	add    %bl,(%rax)
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
 
-Time/Date		Sat Apr 20 15:02:25 2024
+Time/Date		Sun Apr 21 15:02:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010c00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010b98
@@ -27296,19 +27296,17 @@
    140015f60:	push   $0x1400123
    140015f65:	add    %al,(%rax)
    140015f67:	add    %dh,0x23(%rax)
    140015f6a:	add    %eax,0x1(%rax)
    140015f6d:	add    %al,(%rax)
    140015f6f:	add    %al,(%rax)
    140015f71:	add    %al,(%rax)
-   140015f73:	add    %al,(%rcx)
-   140015f75:	fldenv (%rbx)
-   140015f77:	data16 add %al,(%rax)
-   140015f7a:	add    %al,(%rax)
-   140015f7c:	or     $0x90000000,%eax
+   140015f73:	add    %bl,0x66252a(%rax)
+   140015f79:	add    %al,(%rax)
+   140015f7b:	add    %cl,-0x70000000(%rip)        # 0xd0015f81
    140015f81:	add    (%rax),%eax
    140015f83:	add    %ch,0x65(%rax)
    140015f86:	add    %eax,(%rax)
    140015f88:	push   $0x155
 	...
    140015ffd:	add    %al,(%rax)
    140015fff:	add    %bl,(%rax)
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
 
-Time/Date		Sat Apr 20 15:06:55 2024
+Time/Date		Sun Apr 21 15:06:14 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011800
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000118e8
@@ -28454,19 +28454,17 @@
    14001706d:	add    %al,(%rax)
    14001706f:	add    %cl,0x1400133(%rax)
    140017075:	add    %al,(%rax)
    140017077:	add    %dl,0x1400133(%rax)
    14001707d:	add    %al,(%rax)
    14001707f:	add    %al,(%rax)
    140017081:	add    %al,(%rax)
-   140017083:	add    %cl,(%rdi)
-   140017085:	fisubl (%rbx)
-   140017087:	data16 add %al,(%rax)
-   14001708a:	add    %al,(%rax)
-   14001708c:	or     $0x90000000,%eax
+   140017083:	add    %ah,0x2b(%rsi)
+   140017086:	and    $0x66,%eax
+   14001708b:	add    %cl,-0x70000000(%rip)        # 0xd0017091
    140017091:	add    (%rax),%eax
    140017093:	add    %ch,0x1(%rsi,%rsi,2)
    140017097:	add    %ch,0x1(%rdx,%riz,2)
 	...
    1400170ff:	add    %ah,(%rax)
    140017101:	jp     0x140017104
    140017103:	rex add %eax,(%rax)
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
 
-Time/Date		Sat Apr 20 15:02:25 2024
+Time/Date		Sun Apr 21 15:02:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011c00
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000011af8
@@ -28600,19 +28600,17 @@
    14001704d:	add    %al,(%rax)
    14001704f:	add    %cl,0x1400133(%rax)
    140017055:	add    %al,(%rax)
    140017057:	add    %dl,0x1400133(%rax)
    14001705d:	add    %al,(%rax)
    14001705f:	add    %al,(%rax)
    140017061:	add    %al,(%rax)
-   140017063:	add    %al,(%rcx)
-   140017065:	fldenv (%rbx)
-   140017067:	data16 add %al,(%rax)
-   14001706a:	add    %al,(%rax)
-   14001706c:	or     $0x90000000,%eax
+   140017063:	add    %bl,0x66252a(%rax)
+   140017069:	add    %al,(%rax)
+   14001706b:	add    %cl,-0x70000000(%rip)        # 0xd0017071
    140017071:	add    (%rax),%eax
    140017073:	add    %ch,%ah
    140017075:	jne    0x140017078
    140017077:	add    %ch,%ah
    140017079:	add    %eax,%gs:(%rax)
    14001707c:	add    %al,(%rax)
    14001707e:	add    %al,(%rax)
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
 
-Time/Date		Sat Apr 20 15:06:55 2024
+Time/Date		Sun Apr 21 15:06:15 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013c70
@@ -32545,19 +32545,17 @@
    1400192a5:	add    %al,(%rax)
    1400192a7:	add    %al,(%rax)
    1400192a9:	push   %rbp
    1400192aa:	add    %eax,0x1(%rax)
    1400192ad:	add    %al,(%rax)
    1400192af:	add    %al,(%rax)
    1400192b1:	add    %al,(%rax)
-   1400192b3:	add    %cl,(%rdi)
-   1400192b5:	fisubl (%rbx)
-   1400192b7:	data16 add %al,(%rax)
-   1400192ba:	add    %al,(%rax)
-   1400192bc:	or     $0x20000000,%eax
+   1400192b3:	add    %ah,0x2b(%rdi)
+   1400192b6:	and    $0x66,%eax
+   1400192bb:	add    %cl,0x20000000(%rip)        # 0x1600192c1
    1400192c1:	add    (%rax),%eax
    1400192c3:	add    %bh,0x1(%rdx,%riz,4)
    1400192c7:	add    %bh,0x1(%rdx,%rdx,4)
 	...
    1400192ff:	add    %al,(%rcx)
 	...
    140019309:	add    %al,(%rax)
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
 
-Time/Date		Sat Apr 20 15:02:25 2024
+Time/Date		Sun Apr 21 15:02:49 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013e00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013e80
@@ -32652,19 +32652,17 @@
    140019285:	add    %al,(%rax)
    140019287:	add    %al,(%rax)
    140019289:	push   %rbp
    14001928a:	add    %eax,0x1(%rax)
    14001928d:	add    %al,(%rax)
    14001928f:	add    %al,(%rax)
    140019291:	add    %al,(%rax)
-   140019293:	add    %al,(%rcx)
-   140019295:	fldenv (%rbx)
-   140019297:	data16 add %al,(%rax)
-   14001929a:	add    %al,(%rax)
-   14001929c:	or     $0x20000000,%eax
+   140019293:	add    %bl,0x66252a(%rcx)
+   140019299:	add    %al,(%rax)
+   14001929b:	add    %cl,0x20000000(%rip)        # 0x1600192a1
    1400192a1:	add    (%rax),%eax
    1400192a3:	add    %bh,0x1(%rdx,%riz,4)
    1400192a7:	add    %bh,0x1(%rsp,%rdx,4)
 	...
    1400192ff:	add    %al,(%rcx)
 	...
    140019309:	add    %al,(%rax)
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
 
-Time/Date		Sat Apr 20 15:06:55 2024
+Time/Date		Sun Apr 21 15:06:15 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002200
 SizeOfInitializedData	0000000000003400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000277c
@@ -4028,18 +4028,16 @@
    1800045f0:	cmp    %al,0x0(%rdx)
    1800045f3:	addb   $0x0,(%rcx)
    1800045f6:	add    %al,(%rax)
    1800045f8:	rex
    1800045f9:	rex.X add %al,0x1(%rax)
    180004600:	add    %al,(%rax)
    180004602:	add    %al,(%rax)
-   180004604:	pminub (%rbx),%mm4
-   180004607:	data16 add %al,(%rax)
-   18000460a:	add    %al,(%rax)
-   18000460c:	or     $0xe0000000,%eax
+   180004604:	sub    0x66(%eip),%esp        # 0x180004671
+   18000460b:	add    %cl,-0x20000000(%rip)        # 0x160004611
    180004611:	add    (%rax),%al
    180004613:	add    %ah,%ah
    180004615:	rex.W add %al,(%rax)
    180004618:	in     $0x2e,%al
 	...
    18000467e:	add    %al,(%rax)
    180004680:	add    %eax,(%rax)
```

## ipex_llm/libs/starcoder.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800607a8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Apr 20 15:06:55 2024
+Time/Date		Sun Apr 21 15:06:15 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000060e00
 SizeOfInitializedData	00000000000c7a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000607a8
@@ -129991,18 +129991,16 @@
    180069cd5:	add    %al,(%rax)
    180069cd7:	add    %al,%al
    180069cd9:	es (bad)
    180069cdb:	addb   $0x0,(%rcx)
    180069cde:	add    %al,(%rax)
    180069ce0:	add    %al,(%rax)
    180069ce2:	add    %al,(%rax)
-   180069ce4:	pminub (%rbx),%mm4
-   180069ce7:	data16 add %al,(%rax)
-   180069cea:	add    %al,(%rax)
-   180069cec:	or     $0x50000000,%eax
+   180069ce4:	sub    0x66(%eip),%esp        # 0x180069d51
+   180069ceb:	add    %cl,0x50000000(%rip)        # 0x1d0069cf1
    180069cf1:	add    (%rax),%eax
    180069cf3:	add    %dl,-0x52(%rax)
    180069cf6:	(bad)
    180069cf7:	add    %dl,-0x60(%rax)
    180069cfa:	(bad)
    180069cfb:	add    %al,(%rax)
    180069cfd:	add    %al,(%rax)
```

## Comparing `ipex_llm-2.1.0b20240420.data/scripts/llm-chat.ps1` & `ipex_llm-2.1.0b20240421.data/scripts/llm-chat.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240420.data/scripts/llm-cli.ps1` & `ipex_llm-2.1.0b20240421.data/scripts/llm-cli.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240420.dist-info/METADATA` & `ipex_llm-2.1.0b20240421.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipex-llm
-Version: 2.1.0b20240420
+Version: 2.1.0b20240421
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
-Requires-Dist: bigdl-core-cpp (==2.5.0b20240420) ; extra == 'cpp'
+Requires-Dist: bigdl-core-cpp (==2.5.0b20240421) ; extra == 'cpp'
 Provides-Extra: serving
 Requires-Dist: py-cpuinfo ; extra == 'serving'
 Requires-Dist: fschat[model_worker,webui] (==0.2.36) ; extra == 'serving'
 Requires-Dist: protobuf ; extra == 'serving'
 Provides-Extra: xpu
 Requires-Dist: py-cpuinfo ; extra == 'xpu'
 Requires-Dist: protobuf ; extra == 'xpu'
@@ -39,47 +39,47 @@
 Requires-Dist: sentencepiece ; extra == 'xpu'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu'
 Requires-Dist: tabulate ; extra == 'xpu'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240420) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240420) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240421) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240421) ; extra == 'xpu'
 Provides-Extra: xpu-2-0
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-0'
 Requires-Dist: protobuf ; extra == 'xpu-2-0'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-0'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-0'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-0'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-0'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-0'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-0'
 Requires-Dist: tabulate ; extra == 'xpu-2-0'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-0'
 Requires-Dist: torch (==2.0.1a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Requires-Dist: torchvision (==0.15.2a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Requires-Dist: intel-extension-for-pytorch (==2.0.110+xpu) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe (==2.5.0b20240420) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240420) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe (==2.5.0b20240421) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240421) ; (platform_system == "Linux") and extra == 'xpu-2-0'
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
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240420) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240420) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240421) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240421) ; extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu'
 
 
 IPEX LLM
```

## Comparing `ipex_llm-2.1.0b20240420.dist-info/RECORD` & `ipex_llm-2.1.0b20240421.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -38,46 +38,46 @@
 ipex_llm/langchain/embeddings/bigdlllm.py,sha256=auNueZ-S5RQrngss_huXlYdWImX2vPYfuEVOZsx35rk,13589
 ipex_llm/langchain/embeddings/transformersembeddings.py,sha256=hBtqBfGmGg_xjb4Us7hLNfyvbLMo5mJk9a0iooOWtPM,7225
 ipex_llm/langchain/llms/__init__.py,sha256=vBCl9JF45vnk9CWBG1k8lp8J6F8OCR9UY2E-idkkm5Y,1636
 ipex_llm/langchain/llms/bigdlllm.py,sha256=FAZG6cAIJhRgbxm16gMq-cyBwLe-u165zE7yyxD7r9E,24438
 ipex_llm/langchain/llms/transformersllm.py,sha256=7eaIkJi1CbTCSgNxBCoZTe-o_5FYjD1GTYPWpn0Ccr4,10576
 ipex_llm/langchain/llms/transformerspipelinellm.py,sha256=vm522YPPwWxxAPVvQBtxRfBinC4hIbXdKW6VjHDaFXY,7379
 ipex_llm/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ipex_llm/libs/bloom-api.dll,sha256=6nJNPwbmK467kqgdjh5wB4ktBdKwMcFtX94oqdGSErE,36352
-ipex_llm/libs/bloom.dll,sha256=SfXrjYfJreKxFZLo-wUgIpSRv8_Vq9p4z4TD_R-iXhc,460288
-ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=3nRqx6j_WzfbT8f9yOfrSwIZlviK_1d8JazCquqAMeM,852992
-ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=ggxJvvcIkDVuKP8DBksF-_g9gbxRYaULPeQdYrt95Lw,856064
-ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=linII9fQNODLq7xmo3i6GDT8cx4QQrsvvMtKkjEp-qM,843776
-ipex_llm/libs/gptneox-api.dll,sha256=qn2Q2wl_PZDNVqlaOe102uRtKpYKjUJ5agYMAkIJuvA,24576
-ipex_llm/libs/gptneox.dll,sha256=eG26aSx5PaRfp74KTKtR7x_613LWE7Trdtt9pMzjAYU,520192
-ipex_llm/libs/libbloom_avx.dll,sha256=q2nIZzzmTkyLefXtfVR2YnSt487GU6kaE3gcSvT7w10,485888
-ipex_llm/libs/libbloom_vnni.dll,sha256=Hga022rVxHlh9nx93xitMZ8-ZStCA_3eyhG746DRlBg,460800
-ipex_llm/libs/libgptneox_avx.dll,sha256=7EMKfNuk2B6O7viysohQOU93UNjrc-5-6UKRKnBBG4k,545792
-ipex_llm/libs/libgptneox_vnni.dll,sha256=QE--mvg8OehIA28_i2dNJzl9NoTgPpClGta4TTzRX4g,520704
-ipex_llm/libs/libllama_avx.dll,sha256=9CAN2jBUdN8FbWJEfBS1ogrGT4jvHZk_s_4TyMlF5pA,540160
-ipex_llm/libs/libllama_vnni.dll,sha256=wHeGuQtIignnYrcMUzoqhD6rbbJbuc6jOY-zhJ7BV2I,515072
-ipex_llm/libs/libstarcoder_avx.dll,sha256=RulQylPUFJN8HxK49nfqqGw0uhnuxpCFD9cmMtieCJc,577024
-ipex_llm/libs/libstarcoder_vnni.dll,sha256=ZRr5llw18mwZRK6IywVJOUeigj3p3aZIXWeP5Qiouvs,551936
-ipex_llm/libs/llama-api.dll,sha256=lWQBxdPGUYrL8amrYqX_VUe33Sd1WgFrlKHXlJxN2tE,25088
-ipex_llm/libs/llama.dll,sha256=YJw31ppGf3XtT2wPQw3fFhHFGQSynH_I10TJflvBLHQ,514560
-ipex_llm/libs/main-bloom.exe,sha256=U9UW2JCT0T0osT9kHDZ_tMf-5piaa2ZtIS5fEDWqTmI,103424
-ipex_llm/libs/main-chatglm_vnni.exe,sha256=kR-XnJn4o0s2_FIMnysN5BdYSz2HqUJqQCPA0bfBpC0,726016
-ipex_llm/libs/main-gptneox.exe,sha256=SGcLSSdfmqY5KEFP8_sVqVpe0CWj6gPYGBYBqukf4vQ,98816
-ipex_llm/libs/main-llama.exe,sha256=YHyHHNb0_f9oQioFv-Lu7xWeR2bZbNioRXJ6mVjt75U,99840
-ipex_llm/libs/main-starcoder.exe,sha256=t_ZwoJaYLdkPMhdCjFMrpR4Dk90fx3OQ_z0CrATNgXU,157696
-ipex_llm/libs/quantize-bloom.exe,sha256=V5NjTRq2TXOY_E2Vi8cj7mgvfIRf1FKgfXhq2JUeX24,125952
-ipex_llm/libs/quantize-bloom_vnni.exe,sha256=nFYD_U3_iDT4XQDMUszasDlrA93-gpcD9Vu9cOucgW8,127488
-ipex_llm/libs/quantize-gptneox.exe,sha256=QqDLSSDVEPB_9XDcojym_rD7Ql4idNKBM49UPlvnY6E,103936
-ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=GDqDSx-K4lg55C0g-fUz9hW3VDmQcBiM42qlVhRJ2Bw,104448
-ipex_llm/libs/quantize-llama.exe,sha256=V4MGldUMr_RbFaNrBps2bKtjcq0V4z2mlEO-r6izsyE,109056
-ipex_llm/libs/quantize-llama_vnni.exe,sha256=6hCCHgKwdBowUYv7cyelRNnw9BqB17h6GvOtkTL5-hU,110080
-ipex_llm/libs/quantize-starcoder.exe,sha256=JVHQfw1oJUXwSaydkt8OVMQSW5KEU8acF3FLvnITjXQ,126976
-ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=deJ6IzPYeg6hUGr1-6txiSBJOU8FmEc5eeNy0ylKfL4,128000
-ipex_llm/libs/starcoder-api.dll,sha256=xqu5dZwjuyGteOaELYsXGrcjg6GnFvUc7CU6LybTZpQ,21504
-ipex_llm/libs/starcoder.dll,sha256=NW9rFYxmT8vnh4lO-cl1ARCaTY5fmlt7zqFTHgehAKE,551424
+ipex_llm/libs/bloom-api.dll,sha256=ZkOop2NrTlLf6sKCFWGGExGoOhjAEkpKTO-AVl2QxVM,36352
+ipex_llm/libs/bloom.dll,sha256=E02GE8sqGkmXtdKFFz4azolzvrhzHNQLuF2uw9PHCMw,460288
+ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=7e9FMUPjf6EIgZUZPDZ30kaZqkeheUdclWhKBGUAB30,852992
+ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=0PDUtA5warS-tf0RI8MIvdz13NEyohhuv9sR3YnViUI,856064
+ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=-pDZnJkObvcSbgWmKohPZoeeXRJiKnPDsQXwdDMA69g,843776
+ipex_llm/libs/gptneox-api.dll,sha256=CURBvu1-YJUH-RNmM0RI89MTJAmDSL3x6sKtK4i_vGA,24576
+ipex_llm/libs/gptneox.dll,sha256=6iOydIoF_NHuYjHO4PhmcHSXtMiK_CMeA1TarL9qGSE,520192
+ipex_llm/libs/libbloom_avx.dll,sha256=X5k8VRgYhpHyGiX6KCffvEKG0zDjOAYqXxxLPO0UsYQ,485888
+ipex_llm/libs/libbloom_vnni.dll,sha256=8uVDkWmRLN4fzWnh4aLuFUKdm3dZqF-yJAfx3eVAmHc,460800
+ipex_llm/libs/libgptneox_avx.dll,sha256=q-gz9en4cP13eWKf3bVz4OKCqIE6GRvptCi2M_8VO2o,545792
+ipex_llm/libs/libgptneox_vnni.dll,sha256=CIhG1CQKHTj93V5k4VdBoADXcOAcK9GsedAHHNNAX2g,520704
+ipex_llm/libs/libllama_avx.dll,sha256=jqW3w-FVtyFvaMi4QoQTFXA6Rr-3kuFQj_2JsOtw6yk,540160
+ipex_llm/libs/libllama_vnni.dll,sha256=nVf5Yc5ZzeHOnnPNVPdCMRKQPFX7zC-6oGz9cK7qW94,515072
+ipex_llm/libs/libstarcoder_avx.dll,sha256=iAgsHRa2g22tTpYfGT0WNDwMt2IBvy20dt1pXIeBtAk,577024
+ipex_llm/libs/libstarcoder_vnni.dll,sha256=CzWwAKBOUt7cMXVQFG_aNonwglkHNxBDOhQF-xw1Di0,551936
+ipex_llm/libs/llama-api.dll,sha256=TtBBevciqsxTfb4nrK1Pk4J4osP7KETPg76ItYHm_gY,25088
+ipex_llm/libs/llama.dll,sha256=uJvNt5_90aVWwlC-QtePjq7gkJIWL2lOcfp7Km-TaKo,514560
+ipex_llm/libs/main-bloom.exe,sha256=vhyLpebr8qpgY8N2uT8c1Pc0_d-xI8uVlYIAEyIWAnk,103424
+ipex_llm/libs/main-chatglm_vnni.exe,sha256=9TmJ5ZzokFImV2wb4uHXOzlX3hzcE6BoDgJ9abKxb8g,726016
+ipex_llm/libs/main-gptneox.exe,sha256=efW8AzNTxAXfL7YtQLMFicyYDpu9QbP6b3gqpDbYtm0,98816
+ipex_llm/libs/main-llama.exe,sha256=UxLg0d9ZrER6_jJ5cLnX33d_qMcgzbPoae5tuLrI0qo,99840
+ipex_llm/libs/main-starcoder.exe,sha256=nE37zf2f6d5iddUyGyX9TlSK7hVZwz9SMgl_-rdz-do,157696
+ipex_llm/libs/quantize-bloom.exe,sha256=izbDkxvfP1sUDc0s5q0RtpKy7yCtQqG1sSe0Tfrxqd8,125952
+ipex_llm/libs/quantize-bloom_vnni.exe,sha256=V-vSD7J_QY0Wtyc5mjfBgjhMHSsdoFSYsatBjuTLb5s,127488
+ipex_llm/libs/quantize-gptneox.exe,sha256=mLXthXl0kGYjmi0AEyw6FiZXGbFAa5t3o9rsA3Sgk40,103936
+ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=ojeATK03mgoJYKbQy7MLjQ1GS5Ha6vlG0XDYQj8IyPA,104448
+ipex_llm/libs/quantize-llama.exe,sha256=5qpQSiAbr8kRc41kSIXZMMF6b47UQTkVHFBiyanboPo,109056
+ipex_llm/libs/quantize-llama_vnni.exe,sha256=z2nzd8ACgTVXIjPziGw8XrwwHt84umbyPWNDV29ylCQ,110080
+ipex_llm/libs/quantize-starcoder.exe,sha256=Z2fjFudTOkKAPneI9XJ1fuNgTZOv74J9IyRaUIo4bIQ,126976
+ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=l2RlRdm0BzlexIg3BIMhJmgTSnfRHKlq8L332KONpnE,128000
+ipex_llm/libs/starcoder-api.dll,sha256=3kIsK50EG74cwbxmcekQNnfaCKKwSh0Dknm9XMNvCpo,21504
+ipex_llm/libs/starcoder.dll,sha256=rh1HkdLL7-WybMScqEGt-Q0S4tvEqADTrfHeJBjf5yA,551424
 ipex_llm/llamaindex/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/llamaindex/llms/__init__.py,sha256=KP1lEdGqDuxPoxL1ZSH25Pm2kKMPJBWUTLR0ckSLMIU,1139
 ipex_llm/llamaindex/llms/bigdlllm.py,sha256=FQBzq1KOjfc6uofTXAha3O7TqpJkNfOFepXQmOVlbnI,26314
 ipex_llm/serving/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/bigdl_llm_model.py,sha256=NXEN_3EPmcP3dDnvug4MokEXXE2zVUnENgBYxfubqic,10084
 ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=LNMHFYgJqna-4TfIYH7zfKElUXIYMqE0J0ICHpvMGPk,11371
@@ -205,14 +205,14 @@
 ipex_llm/vllm/transformers_utils/tokenizer.py,sha256=PKmEi1ROhf9dKRa-7AuKYwvAY-htP-ZIAz4HhNqhokU,8707
 ipex_llm/vllm/worker/worker.py,sha256=eifKuzefL9HC1R62P0mCYBsZlclo_5hQf01vFgc6mFA,13950
 ipex_llm/vllm2/__init__.py,sha256=zBSG6nzrVF5QnpR6_f7kPhBFeowTE9gaZ7D5m98E7_w,585
 ipex_llm/vllm2/model_convert.py,sha256=jbsUSUAeVHm24CokIiLdyv6ubd_HuCrN_pnF3cLhhWE,7208
 ipex_llm/vllm2/engine/__init__.py,sha256=mzPVAyZdbvfzBQi-wxZh1sbme_NElPMmtrJ9C2zh8Us,747
 ipex_llm/vllm2/engine/engine.py,sha256=4jQucwE46X_Bn2dA7uzjWKSJWeSiDZ76-9XW7WHJHAA,5715
 ipex_llm/vllm2/entrypoints/openai/api_server.py,sha256=M7pwasNK1J6kTTrcFgbxgXmKnPWUA4D6cw89EeA7Vw0,10475
-ipex_llm-2.1.0b20240420.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
-ipex_llm-2.1.0b20240420.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
-ipex_llm-2.1.0b20240420.dist-info/METADATA,sha256=Bv2f7v8Euf_vTznNmhynG_WS-zwtE7ETVZwg2KSEvCk,4400
-ipex_llm-2.1.0b20240420.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-ipex_llm-2.1.0b20240420.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
-ipex_llm-2.1.0b20240420.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
-ipex_llm-2.1.0b20240420.dist-info/RECORD,,
+ipex_llm-2.1.0b20240421.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
+ipex_llm-2.1.0b20240421.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
+ipex_llm-2.1.0b20240421.dist-info/METADATA,sha256=hStuh9WEFKa8RJtkCJQQ_H4UllPv1qxrR9r798WjsgA,4400
+ipex_llm-2.1.0b20240421.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+ipex_llm-2.1.0b20240421.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
+ipex_llm-2.1.0b20240421.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
+ipex_llm-2.1.0b20240421.dist-info/RECORD,,
```

