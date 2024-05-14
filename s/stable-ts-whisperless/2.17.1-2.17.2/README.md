# Comparing `tmp/stable-ts-whisperless-2.17.1.tar.gz` & `tmp/stable-ts-whisperless-2.17.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-whisperless-2.17.1.tar", last modified: Sat May  4 01:23:21 2024, max compression
+gzip compressed data, was "stable-ts-whisperless-2.17.2.tar", last modified: Tue May 14 02:23:31 2024, max compression
```

## Comparing `stable-ts-whisperless-2.17.1.tar` & `stable-ts-whisperless-2.17.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 01:23:21.509606 stable-ts-whisperless-2.17.1/
--rw-rw-rw-   0        0        0     1082 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/LICENSE
--rw-rw-rw-   0        0        0    86923 2024-05-04 01:23:21.508604 stable-ts-whisperless-2.17.1/PKG-INFO
--rw-rw-rw-   0        0        0    86522 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 01:23:21.509606 stable-ts-whisperless-2.17.1/setup.cfg
--rw-rw-rw-   0        0        0     1040 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 01:23:21.506602 stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/
--rw-rw-rw-   0        0        0    86923 2024-05-04 01:23:20.000000 stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1287 2024-05-04 01:23:21.000000 stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 01:23:20.000000 stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-04 01:23:20.000000 stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-05-04 01:23:20.000000 stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-04 01:23:20.000000 stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 01:23:21.389603 stable-ts-whisperless-2.17.1/stable_whisper/
--rw-rw-rw-   0        0        0      353 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       50 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       24 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/_version.py
--rw-rw-rw-   0        0        0    70127 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/alignment.py
-drwxrwxrwx   0        0        0        0 2024-05-04 01:23:21.438605 stable-ts-whisperless-2.17.1/stable_whisper/audio/
--rw-rw-rw-   0        0        0    24130 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/audio/__init__.py
--rw-rw-rw-   0        0        0     7657 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/audio/demucs.py
--rw-rw-rw-   0        0        0     3276 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/audio/dfnet.py
--rw-rw-rw-   0        0        0     2952 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/audio/noisereduce.py
--rw-rw-rw-   0        0        0     1977 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/audio/output.py
--rw-rw-rw-   0        0        0     8761 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/audio/utils.py
--rw-rw-rw-   0        0        0     4522 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/decode.py
--rw-rw-rw-   0        0        0     2047 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/default.py
--rw-rw-rw-   0        0        0    16051 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/non_whisper.py
--rw-rw-rw-   0        0        0     2308 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0   103457 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/result.py
-drwxrwxrwx   0        0        0        0 2024-05-04 01:23:21.463603 stable-ts-whisperless-2.17.1/stable_whisper/stabilization/
--rw-rw-rw-   0        0        0    18720 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/stabilization/__init__.py
--rw-rw-rw-   0        0        0     4936 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/stabilization/nonvad.py
--rw-rw-rw-   0        0        0     2246 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/stabilization/silero_vad.py
--rw-rw-rw-   0        0        0     4491 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/stabilization/utils.py
--rw-rw-rw-   0        0        0    24042 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    11983 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2622 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/utils.py
--rw-rw-rw-   0        0        0     4020 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0     9426 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/whisper_compatibility.py
-drwxrwxrwx   0        0        0        0 2024-05-04 01:23:21.503602 stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/
--rw-rw-rw-   0        0        0      454 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/__init__.py
--rw-rw-rw-   0        0        0    39229 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/cli.py
--rw-rw-rw-   0        0        0    11231 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/faster_whisper.py
--rw-rw-rw-   0        0        0     9957 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/hf_whisper.py
--rw-rw-rw-   0        0        0    42315 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/original_whisper.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:23:31.671008 stable-ts-whisperless-2.17.2/
+-rw-rw-rw-   0        0        0     1082 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/LICENSE
+-rw-rw-rw-   0        0        0    87743 2024-05-14 02:23:31.670008 stable-ts-whisperless-2.17.2/PKG-INFO
+-rw-rw-rw-   0        0        0    87342 2024-05-14 00:42:59.000000 stable-ts-whisperless-2.17.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 02:23:31.671008 stable-ts-whisperless-2.17.2/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:23:31.669009 stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/
+-rw-rw-rw-   0        0        0    87743 2024-05-14 02:23:31.000000 stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1287 2024-05-14 02:23:31.000000 stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 02:23:31.000000 stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-14 02:23:31.000000 stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-05-14 02:23:31.000000 stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-14 02:23:31.000000 stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 02:23:31.644008 stable-ts-whisperless-2.17.2/stable_whisper/
+-rw-rw-rw-   0        0        0      353 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       50 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       24 2024-05-14 00:50:46.000000 stable-ts-whisperless-2.17.2/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0    70716 2024-05-14 01:52:58.000000 stable-ts-whisperless-2.17.2/stable_whisper/alignment.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:23:31.653008 stable-ts-whisperless-2.17.2/stable_whisper/audio/
+-rw-rw-rw-   0        0        0    24130 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/audio/__init__.py
+-rw-rw-rw-   0        0        0     7657 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/audio/demucs.py
+-rw-rw-rw-   0        0        0     3276 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/audio/dfnet.py
+-rw-rw-rw-   0        0        0     2952 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/audio/noisereduce.py
+-rw-rw-rw-   0        0        0     1977 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/audio/output.py
+-rw-rw-rw-   0        0        0     8761 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/audio/utils.py
+-rw-rw-rw-   0        0        0     4522 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0     2047 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/default.py
+-rw-rw-rw-   0        0        0    16093 2024-05-14 01:08:23.000000 stable-ts-whisperless-2.17.2/stable_whisper/non_whisper.py
+-rw-rw-rw-   0        0        0     2308 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0   103762 2024-05-14 02:04:09.000000 stable-ts-whisperless-2.17.2/stable_whisper/result.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:23:31.659010 stable-ts-whisperless-2.17.2/stable_whisper/stabilization/
+-rw-rw-rw-   0        0        0    18720 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/stabilization/__init__.py
+-rw-rw-rw-   0        0        0     4936 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/stabilization/nonvad.py
+-rw-rw-rw-   0        0        0     2246 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/stabilization/silero_vad.py
+-rw-rw-rw-   0        0        0     4491 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/stabilization/utils.py
+-rw-rw-rw-   0        0        0    24045 2024-05-13 21:51:05.000000 stable-ts-whisperless-2.17.2/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    11983 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2622 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/utils.py
+-rw-rw-rw-   0        0        0     4020 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0     9426 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/whisper_compatibility.py
+drwxrwxrwx   0        0        0        0 2024-05-14 02:23:31.667008 stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/
+-rw-rw-rw-   0        0        0      454 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/__init__.py
+-rw-rw-rw-   0        0        0    39229 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/cli.py
+-rw-rw-rw-   0        0        0    11231 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/faster_whisper.py
+-rw-rw-rw-   0        0        0     9957 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/hf_whisper.py
+-rw-rw-rw-   0        0        0    42315 2024-05-04 01:20:55.000000 stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/original_whisper.py
```

### Comparing `stable-ts-whisperless-2.17.1/LICENSE` & `stable-ts-whisperless-2.17.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/PKG-INFO` & `stable-ts-whisperless-2.17.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts-whisperless
-Version: 2.17.1
+Version: 2.17.2
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -33,14 +33,49 @@
   * [Tips](#tips)
   * [Visualizing Suppression](#visualizing-suppression)
   * [Encode Comparison](#encode-comparison)
   * [Use with any ASR](#any-asr)
 * [Quick 1.X → 2.X Guide](#quick-1x--2x-guide)
 
 ## Setup
+<details>
+<summary>Prerequisites: FFmpeg & PyTorch</summary>
+
+<details>
+<summary>FFmpeg</summary>
+
+Requires [FFmpeg](https://ffmpeg.org/) in PATH 
+```
+# on Ubuntu or Debian
+sudo apt update && sudo apt install ffmpeg
+
+# on Arch Linux
+sudo pacman -S ffmpeg
+
+# on MacOS using Homebrew (https://brew.sh/)
+brew install ffmpeg
+
+# on Windows using Chocolatey (https://chocolatey.org/)
+choco install ffmpeg
+
+# on Windows using Scoop (https://scoop.sh/)
+scoop install ffmpeg
+```
+</details>
+
+<details>
+<summary>PyTorch</summary>
+
+If PyTorch is not installed when installing Stable-ts, 
+the default version will be installed which may not have GPU support.
+To avoid this issue, install your preferred version with instructions at https://pytorch.org/get-started/locally/.
+</details>
+
+</details>
+
 ```
 pip install -U stable-ts
 ```
 
 To install the latest commit:
 ```
 pip install -U git+https://github.com/jianfch/stable-ts.git
```

### Comparing `stable-ts-whisperless-2.17.1/README.md` & `stable-ts-whisperless-2.17.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,49 @@
   * [Tips](#tips)
   * [Visualizing Suppression](#visualizing-suppression)
   * [Encode Comparison](#encode-comparison)
   * [Use with any ASR](#any-asr)
 * [Quick 1.X → 2.X Guide](#quick-1x--2x-guide)
 
 ## Setup
+<details>
+<summary>Prerequisites: FFmpeg & PyTorch</summary>
+
+<details>
+<summary>FFmpeg</summary>
+
+Requires [FFmpeg](https://ffmpeg.org/) in PATH 
+```
+# on Ubuntu or Debian
+sudo apt update && sudo apt install ffmpeg
+
+# on Arch Linux
+sudo pacman -S ffmpeg
+
+# on MacOS using Homebrew (https://brew.sh/)
+brew install ffmpeg
+
+# on Windows using Chocolatey (https://chocolatey.org/)
+choco install ffmpeg
+
+# on Windows using Scoop (https://scoop.sh/)
+scoop install ffmpeg
+```
+</details>
+
+<details>
+<summary>PyTorch</summary>
+
+If PyTorch is not installed when installing Stable-ts, 
+the default version will be installed which may not have GPU support.
+To avoid this issue, install your preferred version with instructions at https://pytorch.org/get-started/locally/.
+</details>
+
+</details>
+
 ```
 pip install -U stable-ts
 ```
 
 To install the latest commit:
 ```
 pip install -U git+https://github.com/jianfch/stable-ts.git
```

### Comparing `stable-ts-whisperless-2.17.1/setup.py` & `stable-ts-whisperless-2.17.2/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/PKG-INFO` & `stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts-whisperless
-Version: 2.17.1
+Version: 2.17.2
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -33,14 +33,49 @@
   * [Tips](#tips)
   * [Visualizing Suppression](#visualizing-suppression)
   * [Encode Comparison](#encode-comparison)
   * [Use with any ASR](#any-asr)
 * [Quick 1.X → 2.X Guide](#quick-1x--2x-guide)
 
 ## Setup
+<details>
+<summary>Prerequisites: FFmpeg & PyTorch</summary>
+
+<details>
+<summary>FFmpeg</summary>
+
+Requires [FFmpeg](https://ffmpeg.org/) in PATH 
+```
+# on Ubuntu or Debian
+sudo apt update && sudo apt install ffmpeg
+
+# on Arch Linux
+sudo pacman -S ffmpeg
+
+# on MacOS using Homebrew (https://brew.sh/)
+brew install ffmpeg
+
+# on Windows using Chocolatey (https://chocolatey.org/)
+choco install ffmpeg
+
+# on Windows using Scoop (https://scoop.sh/)
+scoop install ffmpeg
+```
+</details>
+
+<details>
+<summary>PyTorch</summary>
+
+If PyTorch is not installed when installing Stable-ts, 
+the default version will be installed which may not have GPU support.
+To avoid this issue, install your preferred version with instructions at https://pytorch.org/get-started/locally/.
+</details>
+
+</details>
+
 ```
 pip install -U stable-ts
 ```
 
 To install the latest commit:
 ```
 pip install -U git+https://github.com/jianfch/stable-ts.git
```

### Comparing `stable-ts-whisperless-2.17.1/stable_ts_whisperless.egg-info/SOURCES.txt` & `stable-ts-whisperless-2.17.2/stable_ts_whisperless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/alignment.py` & `stable-ts-whisperless-2.17.2/stable_whisper/alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -433,25 +433,25 @@
             second_word_src, word_sources = fix_temp_words(second_target, word_sources[1:])
             if second_word_src is not None:
                 word_sources = [second_word_src] + word_sources
             return first_word_src, word_sources
 
         return first_word_src, word_sources[1:]
 
-    def speech_percentage(_word: dict, _mask: torch.Tensor, _offset: float):
+    def speech_percentage(_word: dict, _mask: torch.Tensor, _offset: float) -> float:
         if _mask is None:
             return 1
         s, e = _word['start'], _word['end']
         s = int((s - _offset) * TOKENS_PER_SECOND)
         e = int((e - _offset) * TOKENS_PER_SECOND)
-        return 1 - _mask[s:e].float().mean().nan_to_num()
+        return 1 - _mask[s:e].float().mean().nan_to_num().item()
 
     def is_new_better(w0, m0, o0, w1, m1, o1):
-        speech0 = speech_percentage(w0, m0, o0).round(decimals=1)
-        speech1 = speech_percentage(w1, m1, o1).round(decimals=1)
+        speech0 = round(speech_percentage(w0, m0, o0), 1)
+        speech1 = round(speech_percentage(w1, m1, o1), 1)
         w0p, w1p = w0['probability'], w1['probability']
         return ((w1p**0.75 - w0p**0.75) < 0.35 and speech0 >= speech1) or w0p >= w1p
 
     with tqdm(total=initial_duration, unit='sec', disable=verbose is not False, desc='Align') as tqdm_pbar:
 
         def update_pbar(finish: bool = False):
             curr_total = audio.get_duration(2)
@@ -691,14 +691,15 @@
             min_word_dur=min_word_dur,
             word_level=suppress_word_ts,
             nonspeech_error=nonspeech_error,
             use_word_position=use_word_position,
             verbose=verbose is not None
         )
         result.update_nonspeech_sections(*nonspeech_timings)
+        result.set_current_as_orig()
     if not original_split:
         result.regroup(regroup)
 
     if fail_segs := len([None for s in result.segments if s.end-s.start <= 0]):
         warnings.warn(f'{fail_segs}/{len(result.segments)} segments failed to align.', stacklevel=2)
 
     return result
@@ -794,14 +795,18 @@
     >>> import stable_whisper
     >>> model = stable_whisper.load_model('base')
     >>> result = model.transcribe('audio.mp3')
     >>> model.refine('audio.mp3', result)
     >>> result.to_srt_vtt('audio.srt')
     Saved 'audio.srt'
     """
+    if result and not all(part.tokens for part in result.all_words_or_segments()):
+        raise NotImplementedError('The are missing tokens in the result. '
+                                  'Refinement currently only supports results produced by '
+                                  '``transcribe()`` on vanilla Whisper models.')
     audioloader_not_supported(audio)
     if not steps:
         steps = 'se'
     if precision is None:
         precision = 0.1
     if invalid_steps := steps.replace('s', '').replace('e', ''):
         raise ValueError(f'Invalid step(s): {", ".join(invalid_steps)}')
@@ -958,26 +963,25 @@
                 new_ts = round(time_offset + (changes[idx, -1] / FRAMES_PER_SECOND), 3)
                 if changes[idx, 0] and not changes[idx, 1]:
                     if is_end_ts:
                         if new_ts <= words[idx].end:
                             return
                     elif new_ts >= words[idx].start:
                         return
-                if not verbose:
-                    return
-                curr_word = words[idx]
-                word_info = (f'[Word="{curr_word.word}"] '
-                             f'[Segment ID: {curr_word.segment_id}] '
-                             f'[Word ID: {curr_word.id}]')
                 if is_end_ts:
-                    print(f'End: {words[idx].end} -> {new_ts}  {word_info}')
+                    old_ts = words[idx].end
                     words[idx].end = new_ts
                 else:
-                    print(f'Start: {words[idx].start} -> {new_ts}  {word_info}')
+                    old_ts = words[idx].start
                     words[idx].start = new_ts
+                if verbose and old_ts != new_ts:
+                    word_info = (f'[Word="{words[idx].word}"] '
+                                 f'[Segment ID: {words[idx].segment_id}] '
+                                 f'[Word ID: {words[idx].id}]')
+                    print(f'{"End" if is_end_ts else "Start"}: {old_ts} -> {new_ts}  {word_info}')
 
             mel_segment = orig_mel_segment.clone().repeat_interleave(2, 0)
             is_end_ts = _step == 'e'
 
             prob_indices = []
             is_finish = np.less([w.probability for w in words], prob_threshold)
             is_finish = np.logical_or(is_finish, [w.duration == 0 for w in words])
@@ -1071,21 +1075,26 @@
 
             update_pbar(words[-1].end)
 
     with tqdm(total=round(total_duration, 2), unit='sec', disable=verbose is not False, desc='Refine') as tqdm_pbar:
 
         def update_pbar(last_ts: float):
             nonlocal prev_ts
-            tqdm_pbar.update(round(((last_ts - prev_ts) / len(steps)), 2))
+            if last_ts == tqdm_pbar.total:
+                new_n = pbar_step * step_count
+            else:
+                new_n = ((last_ts - prev_ts) / len(steps)) + tqdm_pbar.n
+            tqdm_pbar.update(min(round(new_n, 2) - tqdm_pbar.n, tqdm_pbar.total))
             prev_ts = last_ts
 
+        pbar_step = tqdm_pbar.total / len(steps)
         for step_count, step in enumerate(steps, 1):
             prev_ts = 0
             _refine(step)
-            update_pbar(round(tqdm_pbar.total / len(step), 2))
+            update_pbar(tqdm_pbar.total)
         tqdm_pbar.update(tqdm_pbar.total - tqdm_pbar.n)
 
     result.reassign_ids()
 
     return result
```

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/audio/__init__.py` & `stable-ts-whisperless-2.17.2/stable_whisper/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/audio/demucs.py` & `stable-ts-whisperless-2.17.2/stable_whisper/audio/demucs.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/audio/dfnet.py` & `stable-ts-whisperless-2.17.2/stable_whisper/audio/dfnet.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/audio/noisereduce.py` & `stable-ts-whisperless-2.17.2/stable_whisper/audio/noisereduce.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/audio/output.py` & `stable-ts-whisperless-2.17.2/stable_whisper/audio/output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/audio/utils.py` & `stable-ts-whisperless-2.17.2/stable_whisper/audio/utils.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/decode.py` & `stable-ts-whisperless-2.17.2/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/default.py` & `stable-ts-whisperless-2.17.2/stable_whisper/default.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/non_whisper.py` & `stable-ts-whisperless-2.17.2/stable_whisper/non_whisper.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,14 +350,15 @@
                 q_levels=q_levels, k_size=k_size,
                 sample_rate=curr_audio_sr(True), min_word_dur=min_word_dur,
                 word_level=suppress_word_ts, verbose=True,
                 nonspeech_error=nonspeech_error,
                 use_word_position=use_word_position,
                 min_silence_dur=min_silence_dur
             )
+            result.set_current_as_orig()
 
         if result.has_words and regroup:
             result.regroup(regroup)
 
     finally:
         if temp_audio_file is not None:
             try:
```

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/quantization.py` & `stable-ts-whisperless-2.17.2/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/result.py` & `stable-ts-whisperless-2.17.2/stable_whisper/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -3250,3218 +3250,3237 @@
 0000cb10: 2064 6566 2061 6c6c 5f74 6f6b 656e 7328   def all_tokens(
 0000cb20: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
 0000cb30: 7265 7475 726e 206c 6973 7428 6368 6169  return list(chai
 0000cb40: 6e2e 6672 6f6d 5f69 7465 7261 626c 6528  n.from_iterable(
 0000cb50: 732e 746f 6b65 6e73 2066 6f72 2073 2069  s.tokens for s i
 0000cb60: 6e20 7365 6c66 2e61 6c6c 5f77 6f72 6473  n self.all_words
 0000cb70: 2829 2929 0d0a 0d0a 2020 2020 6465 6620  ()))....    def 
-0000cb80: 746f 5f64 6963 7428 7365 6c66 293a 0d0a  to_dict(self):..
-0000cb90: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-0000cba0: 6963 7428 7465 7874 3d73 656c 662e 7465  ict(text=self.te
-0000cbb0: 7874 2c0d 0a20 2020 2020 2020 2020 2020  xt,..           
-0000cbc0: 2020 2020 2020 2020 2073 6567 6d65 6e74           segment
-0000cbd0: 733d 7365 6c66 2e73 6567 6d65 6e74 735f  s=self.segments_
-0000cbe0: 746f 5f64 6963 7473 2829 2c0d 0a20 2020  to_dicts(),..   
-0000cbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc00: 206c 616e 6775 6167 653d 7365 6c66 2e6c   language=self.l
-0000cc10: 616e 6775 6167 652c 0d0a 2020 2020 2020  anguage,..      
-0000cc20: 2020 2020 2020 2020 2020 2020 2020 6f72                or
-0000cc30: 695f 6469 6374 3d73 656c 662e 6f72 695f  i_dict=self.ori_
-0000cc40: 6469 6374 2c0d 0a20 2020 2020 2020 2020  dict,..         
-0000cc50: 2020 2020 2020 2020 2020 2072 6567 726f             regro
-0000cc60: 7570 5f68 6973 746f 7279 3d73 656c 662e  up_history=self.
-0000cc70: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
-0000cc80: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000cc90: 2020 2020 2020 206e 6f6e 7370 6565 6368         nonspeech
-0000cca0: 5f73 6563 7469 6f6e 733d 7365 6c66 2e5f  _sections=self._
-0000ccb0: 6e6f 6e73 7065 6563 685f 7365 6374 696f  nonspeech_sectio
-0000ccc0: 6e73 290d 0a0d 0a20 2020 2064 6566 2073  ns)....    def s
-0000ccd0: 6567 6d65 6e74 735f 746f 5f64 6963 7473  egments_to_dicts
-0000cce0: 2873 656c 662c 2072 6576 6572 7365 5f74  (self, reverse_t
-0000ccf0: 6578 743a 2055 6e69 6f6e 5b62 6f6f 6c2c  ext: Union[bool,
-0000cd00: 2074 7570 6c65 5d20 3d20 4661 6c73 6529   tuple] = False)
-0000cd10: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-0000cd20: 6e20 5b73 2e74 6f5f 6469 6374 2872 6576  n [s.to_dict(rev
-0000cd30: 6572 7365 5f74 6578 743d 7265 7665 7273  erse_text=revers
-0000cd40: 655f 7465 7874 2920 666f 7220 7320 696e  e_text) for s in
-0000cd50: 2073 656c 662e 7365 676d 656e 7473 5d0d   self.segments].
-0000cd60: 0a0d 0a20 2020 2064 6566 205f 7370 6c69  ...    def _spli
-0000cd70: 745f 7365 676d 656e 7473 2873 656c 662c  t_segments(self,
-0000cd80: 2067 6574 5f69 6e64 6963 6573 2c20 6172   get_indices, ar
-0000cd90: 6773 3a20 6c69 7374 203d 204e 6f6e 652c  gs: list = None,
-0000cda0: 202a 2c20 6c6f 636b 3a20 626f 6f6c 203d   *, lock: bool =
-0000cdb0: 2046 616c 7365 2c20 6e65 776c 696e 653a   False, newline:
-0000cdc0: 2062 6f6f 6c20 3d20 4661 6c73 6529 3a0d   bool = False):.
-0000cdd0: 0a20 2020 2020 2020 2069 6620 6172 6773  .        if args
-0000cde0: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-0000cdf0: 2020 2020 2020 2061 7267 7320 3d20 5b5d         args = []
-0000ce00: 0d0a 2020 2020 2020 2020 6e6f 5f77 6f72  ..        no_wor
-0000ce10: 6473 203d 2046 616c 7365 0d0a 2020 2020  ds = False..    
-0000ce20: 2020 2020 666f 7220 6920 696e 2072 6576      for i in rev
-0000ce30: 6572 7365 6428 7261 6e67 6528 302c 206c  ersed(range(0, l
-0000ce40: 656e 2873 656c 662e 7365 676d 656e 7473  en(self.segments
-0000ce50: 2929 293a 0d0a 2020 2020 2020 2020 2020  ))):..          
-0000ce60: 2020 6e6f 5f77 6f72 6473 203d 206e 6f5f    no_words = no_
-0000ce70: 776f 7264 7320 6f72 206e 6f74 2073 656c  words or not sel
-0000ce80: 662e 7365 676d 656e 7473 5b69 5d2e 6861  f.segments[i].ha
-0000ce90: 735f 776f 7264 730d 0a20 2020 2020 2020  s_words..       
-0000cea0: 2020 2020 2069 6e64 6963 6573 203d 2073       indices = s
-0000ceb0: 6f72 7465 6428 7365 7428 6765 745f 696e  orted(set(get_in
-0000cec0: 6469 6365 7328 7365 6c66 2e73 6567 6d65  dices(self.segme
-0000ced0: 6e74 735b 695d 2c20 2a61 7267 7329 2929  nts[i], *args)))
-0000cee0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000cef0: 206e 6f74 2069 6e64 6963 6573 3a0d 0a20   not indices:.. 
-0000cf00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000cf10: 6f6e 7469 6e75 650d 0a20 2020 2020 2020  ontinue..       
-0000cf20: 2020 2020 2069 6620 6e65 776c 696e 653a       if newline:
-0000cf30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000cf40: 2020 6966 2069 6e64 6963 6573 5b2d 315d    if indices[-1]
-0000cf50: 203d 3d20 6c65 6e28 7365 6c66 2e73 6567   == len(self.seg
-0000cf60: 6d65 6e74 735b 695d 2e77 6f72 6473 2920  ments[i].words) 
-0000cf70: 2d20 313a 0d0a 2020 2020 2020 2020 2020  - 1:..          
-0000cf80: 2020 2020 2020 2020 2020 6465 6c20 696e            del in
-0000cf90: 6469 6365 735b 2d31 5d0d 0a20 2020 2020  dices[-1]..     
-0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000cfb0: 6620 6e6f 7420 696e 6469 6365 733a 0d0a  f not indices:..
+0000cb80: 746f 5f64 6963 7428 7365 6c66 2c20 6b65  to_dict(self, ke
+0000cb90: 6570 5f6f 7269 673a 2062 6f6f 6c20 3d20  ep_orig: bool = 
+0000cba0: 5472 7565 293a 0d0a 2020 2020 2020 2020  True):..        
+0000cbb0: 6f72 695f 6469 6374 203d 2073 656c 662e  ori_dict = self.
+0000cbc0: 6f72 695f 6469 6374 2069 6620 6b65 6570  ori_dict if keep
+0000cbd0: 5f6f 7269 6720 656c 7365 207b 7d0d 0a20  _orig else {}.. 
+0000cbe0: 2020 2020 2020 2072 6574 7572 6e20 6469         return di
+0000cbf0: 6374 2874 6578 743d 7365 6c66 2e74 6578  ct(text=self.tex
+0000cc00: 742c 0d0a 2020 2020 2020 2020 2020 2020  t,..            
+0000cc10: 2020 2020 2020 2020 7365 676d 656e 7473          segments
+0000cc20: 3d73 656c 662e 7365 676d 656e 7473 5f74  =self.segments_t
+0000cc30: 6f5f 6469 6374 7328 292c 0d0a 2020 2020  o_dicts(),..    
+0000cc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc50: 6c61 6e67 7561 6765 3d73 656c 662e 6c61  language=self.la
+0000cc60: 6e67 7561 6765 2c0d 0a20 2020 2020 2020  nguage,..       
+0000cc70: 2020 2020 2020 2020 2020 2020 206f 7269               ori
+0000cc80: 5f64 6963 743d 6f72 695f 6469 6374 2c0d  _dict=ori_dict,.
+0000cc90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cca0: 2020 2020 2072 6567 726f 7570 5f68 6973       regroup_his
+0000ccb0: 746f 7279 3d73 656c 662e 5f72 6567 726f  tory=self._regro
+0000ccc0: 7570 5f68 6973 746f 7279 2c0d 0a20 2020  up_history,..   
+0000ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cce0: 206e 6f6e 7370 6565 6368 5f73 6563 7469   nonspeech_secti
+0000ccf0: 6f6e 733d 7365 6c66 2e5f 6e6f 6e73 7065  ons=self._nonspe
+0000cd00: 6563 685f 7365 6374 696f 6e73 290d 0a0d  ech_sections)...
+0000cd10: 0a20 2020 2064 6566 2073 6567 6d65 6e74  .    def segment
+0000cd20: 735f 746f 5f64 6963 7473 2873 656c 662c  s_to_dicts(self,
+0000cd30: 2072 6576 6572 7365 5f74 6578 743a 2055   reverse_text: U
+0000cd40: 6e69 6f6e 5b62 6f6f 6c2c 2074 7570 6c65  nion[bool, tuple
+0000cd50: 5d20 3d20 4661 6c73 6529 3a0d 0a20 2020  ] = False):..   
+0000cd60: 2020 2020 2072 6574 7572 6e20 5b73 2e74       return [s.t
+0000cd70: 6f5f 6469 6374 2872 6576 6572 7365 5f74  o_dict(reverse_t
+0000cd80: 6578 743d 7265 7665 7273 655f 7465 7874  ext=reverse_text
+0000cd90: 2920 666f 7220 7320 696e 2073 656c 662e  ) for s in self.
+0000cda0: 7365 676d 656e 7473 5d0d 0a0d 0a20 2020  segments]....   
+0000cdb0: 2064 6566 205f 7370 6c69 745f 7365 676d   def _split_segm
+0000cdc0: 656e 7473 2873 656c 662c 2067 6574 5f69  ents(self, get_i
+0000cdd0: 6e64 6963 6573 2c20 6172 6773 3a20 6c69  ndices, args: li
+0000cde0: 7374 203d 204e 6f6e 652c 202a 2c20 6c6f  st = None, *, lo
+0000cdf0: 636b 3a20 626f 6f6c 203d 2046 616c 7365  ck: bool = False
+0000ce00: 2c20 6e65 776c 696e 653a 2062 6f6f 6c20  , newline: bool 
+0000ce10: 3d20 4661 6c73 6529 3a0d 0a20 2020 2020  = False):..     
+0000ce20: 2020 2069 6620 6172 6773 2069 7320 4e6f     if args is No
+0000ce30: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000ce40: 2061 7267 7320 3d20 5b5d 0d0a 2020 2020   args = []..    
+0000ce50: 2020 2020 6e6f 5f77 6f72 6473 203d 2046      no_words = F
+0000ce60: 616c 7365 0d0a 2020 2020 2020 2020 666f  alse..        fo
+0000ce70: 7220 6920 696e 2072 6576 6572 7365 6428  r i in reversed(
+0000ce80: 7261 6e67 6528 302c 206c 656e 2873 656c  range(0, len(sel
+0000ce90: 662e 7365 676d 656e 7473 2929 293a 0d0a  f.segments))):..
+0000cea0: 2020 2020 2020 2020 2020 2020 6e6f 5f77              no_w
+0000ceb0: 6f72 6473 203d 206e 6f5f 776f 7264 7320  ords = no_words 
+0000cec0: 6f72 206e 6f74 2073 656c 662e 7365 676d  or not self.segm
+0000ced0: 656e 7473 5b69 5d2e 6861 735f 776f 7264  ents[i].has_word
+0000cee0: 730d 0a20 2020 2020 2020 2020 2020 2069  s..            i
+0000cef0: 6e64 6963 6573 203d 2073 6f72 7465 6428  ndices = sorted(
+0000cf00: 7365 7428 6765 745f 696e 6469 6365 7328  set(get_indices(
+0000cf10: 7365 6c66 2e73 6567 6d65 6e74 735b 695d  self.segments[i]
+0000cf20: 2c20 2a61 7267 7329 2929 0d0a 2020 2020  , *args)))..    
+0000cf30: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+0000cf40: 6e64 6963 6573 3a0d 0a20 2020 2020 2020  ndices:..       
+0000cf50: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+0000cf60: 650d 0a20 2020 2020 2020 2020 2020 2069  e..            i
+0000cf70: 6620 6e65 776c 696e 653a 0d0a 2020 2020  f newline:..    
+0000cf80: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0000cf90: 6e64 6963 6573 5b2d 315d 203d 3d20 6c65  ndices[-1] == le
+0000cfa0: 6e28 7365 6c66 2e73 6567 6d65 6e74 735b  n(self.segments[
+0000cfb0: 695d 2e77 6f72 6473 2920 2d20 313a 0d0a  i].words) - 1:..
 0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfd0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-0000cfe0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000cff0: 2020 2020 666f 7220 776f 7264 5f69 6478      for word_idx
-0000d000: 2069 6e20 696e 6469 6365 733a 0d0a 2020   in indices:..  
+0000cfd0: 2020 2020 6465 6c20 696e 6469 6365 735b      del indices[
+0000cfe0: 2d31 5d0d 0a20 2020 2020 2020 2020 2020  -1]..           
+0000cff0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0000d000: 696e 6469 6365 733a 0d0a 2020 2020 2020  indices:..      
 0000d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d020: 2020 6966 2073 656c 662e 7365 676d 656e    if self.segmen
-0000d030: 7473 5b69 5d2e 776f 7264 735b 776f 7264  ts[i].words[word
-0000d040: 5f69 6478 5d2e 776f 7264 2e65 6e64 7377  _idx].word.endsw
-0000d050: 6974 6828 275c 6e27 293a 0d0a 2020 2020  ith('\n'):..    
-0000d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d070: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
-0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d090: 2020 7365 6c66 2e73 6567 6d65 6e74 735b    self.segments[
-0000d0a0: 695d 2e77 6f72 6473 5b77 6f72 645f 6964  i].words[word_id
-0000d0b0: 785d 2e77 6f72 6420 2b3d 2027 5c6e 270d  x].word += '\n'.
-0000d0c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d0d0: 2020 2020 2069 6620 6c6f 636b 3a0d 0a20       if lock:.. 
-0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0f0: 2020 2020 2020 2073 656c 662e 7365 676d         self.segm
-0000d100: 656e 7473 5b69 5d2e 776f 7264 735b 776f  ents[i].words[wo
-0000d110: 7264 5f69 6478 5d2e 6c6f 636b 5f72 6967  rd_idx].lock_rig
-0000d120: 6874 2829 0d0a 2020 2020 2020 2020 2020  ht()..          
-0000d130: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000d140: 2077 6f72 645f 6964 7820 2b20 3120 3c20   word_idx + 1 < 
-0000d150: 6c65 6e28 7365 6c66 2e73 6567 6d65 6e74  len(self.segment
-0000d160: 735b 695d 2e77 6f72 6473 293a 0d0a 2020  s[i].words):..  
+0000d020: 2020 636f 6e74 696e 7565 0d0a 0d0a 2020    continue....  
+0000d030: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000d040: 7220 776f 7264 5f69 6478 2069 6e20 696e  r word_idx in in
+0000d050: 6469 6365 733a 0d0a 2020 2020 2020 2020  dices:..        
+0000d060: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000d070: 656c 662e 7365 676d 656e 7473 5b69 5d2e  elf.segments[i].
+0000d080: 776f 7264 735b 776f 7264 5f69 6478 5d2e  words[word_idx].
+0000d090: 776f 7264 2e65 6e64 7377 6974 6828 275c  word.endswith('\
+0000d0a0: 6e27 293a 0d0a 2020 2020 2020 2020 2020  n'):..          
+0000d0b0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000d0c0: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
+0000d0d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d0e0: 2e73 6567 6d65 6e74 735b 695d 2e77 6f72  .segments[i].wor
+0000d0f0: 6473 5b77 6f72 645f 6964 785d 2e77 6f72  ds[word_idx].wor
+0000d100: 6420 2b3d 2027 5c6e 270d 0a20 2020 2020  d += '\n'..     
+0000d110: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000d120: 6620 6c6f 636b 3a0d 0a20 2020 2020 2020  f lock:..       
+0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d140: 2073 656c 662e 7365 676d 656e 7473 5b69   self.segments[i
+0000d150: 5d2e 776f 7264 735b 776f 7264 5f69 6478  ].words[word_idx
+0000d160: 5d2e 6c6f 636b 5f72 6967 6874 2829 0d0a  ].lock_right()..
 0000d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d180: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000d190: 6567 6d65 6e74 735b 695d 2e77 6f72 6473  egments[i].words
-0000d1a0: 5b77 6f72 645f 6964 782b 315d 2e6c 6f63  [word_idx+1].loc
-0000d1b0: 6b5f 6c65 6674 2829 0d0a 2020 2020 2020  k_left()..      
-0000d1c0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-0000d1d0: 2020 2020 2020 2020 2020 2020 206e 6577               new
-0000d1e0: 5f73 6567 6d65 6e74 7320 3d20 7365 6c66  _segments = self
-0000d1f0: 2e73 6567 6d65 6e74 735b 695d 2e73 706c  .segments[i].spl
-0000d200: 6974 2869 6e64 6963 6573 290d 0a20 2020  it(indices)..   
-0000d210: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000d220: 6c6f 636b 3a0d 0a20 2020 2020 2020 2020  lock:..         
-0000d230: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-0000d240: 2069 6e20 6e65 775f 7365 676d 656e 7473   in new_segments
-0000d250: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000d260: 2020 2020 2020 2020 2020 2069 6620 7320             if s 
-0000d270: 3d3d 206e 6577 5f73 6567 6d65 6e74 735b  == new_segments[
-0000d280: 305d 3a0d 0a20 2020 2020 2020 2020 2020  0]:..           
-0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2a0: 2073 2e6c 6f63 6b5f 7269 6768 7428 290d   s.lock_right().
-0000d2b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d2c0: 2020 2020 2020 2020 2065 6c69 6620 7320           elif s 
-0000d2d0: 3d3d 206e 6577 5f73 6567 6d65 6e74 735b  == new_segments[
-0000d2e0: 2d31 5d3a 0d0a 2020 2020 2020 2020 2020  -1]:..          
-0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d300: 2020 732e 6c6f 636b 5f6c 6566 7428 290d    s.lock_left().
-0000d310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d320: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+0000d180: 2020 2020 2020 2020 6966 2077 6f72 645f          if word_
+0000d190: 6964 7820 2b20 3120 3c20 6c65 6e28 7365  idx + 1 < len(se
+0000d1a0: 6c66 2e73 6567 6d65 6e74 735b 695d 2e77  lf.segments[i].w
+0000d1b0: 6f72 6473 293a 0d0a 2020 2020 2020 2020  ords):..        
+0000d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1d0: 2020 2020 7365 6c66 2e73 6567 6d65 6e74      self.segment
+0000d1e0: 735b 695d 2e77 6f72 6473 5b77 6f72 645f  s[i].words[word_
+0000d1f0: 6964 782b 315d 2e6c 6f63 6b5f 6c65 6674  idx+1].lock_left
+0000d200: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+0000d210: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0000d220: 2020 2020 2020 206e 6577 5f73 6567 6d65         new_segme
+0000d230: 6e74 7320 3d20 7365 6c66 2e73 6567 6d65  nts = self.segme
+0000d240: 6e74 735b 695d 2e73 706c 6974 2869 6e64  nts[i].split(ind
+0000d250: 6963 6573 290d 0a20 2020 2020 2020 2020  ices)..         
+0000d260: 2020 2020 2020 2069 6620 6c6f 636b 3a0d         if lock:.
+0000d270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d280: 2020 2020 2066 6f72 2073 2069 6e20 6e65       for s in ne
+0000d290: 775f 7365 676d 656e 7473 3a0d 0a20 2020  w_segments:..   
+0000d2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2b0: 2020 2020 2069 6620 7320 3d3d 206e 6577       if s == new
+0000d2c0: 5f73 6567 6d65 6e74 735b 305d 3a0d 0a20  _segments[0]:.. 
+0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2e0: 2020 2020 2020 2020 2020 2073 2e6c 6f63             s.loc
+0000d2f0: 6b5f 7269 6768 7428 290d 0a20 2020 2020  k_right()..     
+0000d300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d310: 2020 2065 6c69 6620 7320 3d3d 206e 6577     elif s == new
+0000d320: 5f73 6567 6d65 6e74 735b 2d31 5d3a 0d0a  _segments[-1]:..
 0000d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d340: 2020 2020 2020 2020 2020 2020 732e 6c6f              s.lo
-0000d350: 636b 5f62 6f74 6828 290d 0a20 2020 2020  ck_both()..     
-0000d360: 2020 2020 2020 2020 2020 2064 656c 2073             del s
-0000d370: 656c 662e 7365 676d 656e 7473 5b69 5d0d  elf.segments[i].
-0000d380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d390: 2066 6f72 2073 2069 6e20 7265 7665 7273   for s in revers
-0000d3a0: 6564 286e 6577 5f73 6567 6d65 6e74 7329  ed(new_segments)
-0000d3b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000d3c0: 2020 2020 2020 2073 656c 662e 7365 676d         self.segm
-0000d3d0: 656e 7473 2e69 6e73 6572 7428 692c 2073  ents.insert(i, s
-0000d3e0: 290d 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
-0000d3f0: 5f77 6f72 6473 3a0d 0a20 2020 2020 2020  _words:..       
-0000d400: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-0000d410: 726e 2827 466f 756e 6420 7365 676d 656e  rn('Found segmen
-0000d420: 7428 7329 2077 6974 686f 7574 2077 6f72  t(s) without wor
-0000d430: 6420 7469 6d69 6e67 732e 2054 6865 7365  d timings. These
-0000d440: 2073 6567 6d65 6e74 2873 2920 6361 6e6e   segment(s) cann
-0000d450: 6f74 2062 6520 7370 6c69 742e 2729 0d0a  ot be split.')..
-0000d460: 2020 2020 2020 2020 7365 6c66 2e72 656d          self.rem
-0000d470: 6f76 655f 6e6f 5f77 6f72 645f 7365 676d  ove_no_word_segm
-0000d480: 656e 7473 2829 0d0a 0d0a 2020 2020 6465  ents()....    de
-0000d490: 6620 5f6d 6572 6765 5f73 6567 6d65 6e74  f _merge_segment
-0000d4a0: 7328 7365 6c66 2c20 696e 6469 6365 733a  s(self, indices:
-0000d4b0: 204c 6973 745b 696e 745d 2c0d 0a20 2020   List[int],..   
-0000d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4d0: 2020 2020 202a 2c20 6d61 785f 776f 7264       *, max_word
-0000d4e0: 733a 2069 6e74 203d 204e 6f6e 652c 206d  s: int = None, m
-0000d4f0: 6178 5f63 6861 7273 3a20 696e 7420 3d20  ax_chars: int = 
-0000d500: 4e6f 6e65 2c20 6973 5f73 756d 5f6d 6178  None, is_sum_max
-0000d510: 3a20 626f 6f6c 203d 2046 616c 7365 2c20  : bool = False, 
-0000d520: 6c6f 636b 3a20 626f 6f6c 203d 2046 616c  lock: bool = Fal
-0000d530: 7365 293a 0d0a 2020 2020 2020 2020 6966  se):..        if
-0000d540: 206c 656e 2869 6e64 6963 6573 2920 3d3d   len(indices) ==
-0000d550: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-0000d560: 2072 6574 7572 6e0d 0a20 2020 2020 2020   return..       
-0000d570: 2066 6f72 2069 2069 6e20 7265 7665 7273   for i in revers
-0000d580: 6564 2869 6e64 6963 6573 293a 0d0a 2020  ed(indices):..  
-0000d590: 2020 2020 2020 2020 2020 7365 6720 3d20            seg = 
-0000d5a0: 7365 6c66 2e73 6567 6d65 6e74 735b 695d  self.segments[i]
-0000d5b0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000d5c0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-0000d5d0: 2020 2020 2020 2020 280d 0a20 2020 2020          (..     
-0000d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5f0: 2020 2020 2020 206d 6178 5f77 6f72 6473         max_words
-0000d600: 2061 6e64 0d0a 2020 2020 2020 2020 2020   and..          
+0000d350: 636b 5f6c 6566 7428 290d 0a20 2020 2020  ck_left()..     
+0000d360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d370: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0000d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d390: 2020 2020 2020 732e 6c6f 636b 5f62 6f74        s.lock_bot
+0000d3a0: 6828 290d 0a20 2020 2020 2020 2020 2020  h()..           
+0000d3b0: 2020 2020 2064 656c 2073 656c 662e 7365       del self.se
+0000d3c0: 676d 656e 7473 5b69 5d0d 0a20 2020 2020  gments[i]..     
+0000d3d0: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
+0000d3e0: 2069 6e20 7265 7665 7273 6564 286e 6577   in reversed(new
+0000d3f0: 5f73 6567 6d65 6e74 7329 3a0d 0a20 2020  _segments):..   
+0000d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d410: 2073 656c 662e 7365 676d 656e 7473 2e69   self.segments.i
+0000d420: 6e73 6572 7428 692c 2073 290d 0a20 2020  nsert(i, s)..   
+0000d430: 2020 2020 2069 6620 6e6f 5f77 6f72 6473       if no_words
+0000d440: 3a0d 0a20 2020 2020 2020 2020 2020 2077  :..            w
+0000d450: 6172 6e69 6e67 732e 7761 726e 2827 466f  arnings.warn('Fo
+0000d460: 756e 6420 7365 676d 656e 7428 7329 2077  und segment(s) w
+0000d470: 6974 686f 7574 2077 6f72 6420 7469 6d69  ithout word timi
+0000d480: 6e67 732e 2054 6865 7365 2073 6567 6d65  ngs. These segme
+0000d490: 6e74 2873 2920 6361 6e6e 6f74 2062 6520  nt(s) cannot be 
+0000d4a0: 7370 6c69 742e 2729 0d0a 2020 2020 2020  split.')..      
+0000d4b0: 2020 7365 6c66 2e72 656d 6f76 655f 6e6f    self.remove_no
+0000d4c0: 5f77 6f72 645f 7365 676d 656e 7473 2829  _word_segments()
+0000d4d0: 0d0a 0d0a 2020 2020 6465 6620 5f6d 6572  ....    def _mer
+0000d4e0: 6765 5f73 6567 6d65 6e74 7328 7365 6c66  ge_segments(self
+0000d4f0: 2c20 696e 6469 6365 733a 204c 6973 745b  , indices: List[
+0000d500: 696e 745d 2c0d 0a20 2020 2020 2020 2020  int],..         
+0000d510: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+0000d520: 2c20 6d61 785f 776f 7264 733a 2069 6e74  , max_words: int
+0000d530: 203d 204e 6f6e 652c 206d 6178 5f63 6861   = None, max_cha
+0000d540: 7273 3a20 696e 7420 3d20 4e6f 6e65 2c20  rs: int = None, 
+0000d550: 6973 5f73 756d 5f6d 6178 3a20 626f 6f6c  is_sum_max: bool
+0000d560: 203d 2046 616c 7365 2c20 6c6f 636b 3a20   = False, lock: 
+0000d570: 626f 6f6c 203d 2046 616c 7365 293a 0d0a  bool = False):..
+0000d580: 2020 2020 2020 2020 6966 206c 656e 2869          if len(i
+0000d590: 6e64 6963 6573 2920 3d3d 2030 3a0d 0a20  ndices) == 0:.. 
+0000d5a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000d5b0: 6e0d 0a20 2020 2020 2020 2066 6f72 2069  n..        for i
+0000d5c0: 2069 6e20 7265 7665 7273 6564 2869 6e64   in reversed(ind
+0000d5d0: 6963 6573 293a 0d0a 2020 2020 2020 2020  ices):..        
+0000d5e0: 2020 2020 7365 6720 3d20 7365 6c66 2e73      seg = self.s
+0000d5f0: 6567 6d65 6e74 735b 695d 0d0a 2020 2020  egments[i]..    
+0000d600: 2020 2020 2020 2020 6966 2028 0d0a 2020          if (..  
 0000d610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d620: 2020 7365 672e 6861 735f 776f 7264 7320    seg.has_words 
-0000d630: 616e 640d 0a20 2020 2020 2020 2020 2020  and..           
-0000d640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d650: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-0000d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d670: 2020 2020 2020 2020 2873 6567 2e77 6f72          (seg.wor
-0000d680: 645f 636f 756e 7428 2920 2b20 7365 6c66  d_count() + self
-0000d690: 2e73 6567 6d65 6e74 735b 6920 2b20 315d  .segments[i + 1]
-0000d6a0: 2e77 6f72 645f 636f 756e 7428 2920 3e20  .word_count() > 
-0000d6b0: 6d61 785f 776f 7264 7329 0d0a 2020 2020  max_words)..    
-0000d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6e0: 6966 2069 735f 7375 6d5f 6d61 7820 656c  if is_sum_max el
-0000d6f0: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
-0000d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d710: 2020 2020 2020 2020 2873 6567 2e77 6f72          (seg.wor
-0000d720: 645f 636f 756e 7428 2920 3e20 6d61 785f  d_count() > max_
-0000d730: 776f 7264 7320 616e 6420 7365 6c66 2e73  words and self.s
-0000d740: 6567 6d65 6e74 735b 6920 2b20 315d 2e77  egments[i + 1].w
-0000d750: 6f72 645f 636f 756e 7428 2920 3e20 6d61  ord_count() > ma
-0000d760: 785f 776f 7264 7329 0d0a 2020 2020 2020  x_words)..      
-0000d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d780: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0000d790: 2020 2020 2020 2020 2020 2020 2029 206f               ) o
-0000d7a0: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
-0000d7b0: 2020 2020 2020 2028 0d0a 2020 2020 2020         (..      
+0000d620: 2020 280d 0a20 2020 2020 2020 2020 2020    (..           
+0000d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d640: 206d 6178 5f77 6f72 6473 2061 6e64 0d0a   max_words and..
+0000d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d660: 2020 2020 2020 2020 2020 2020 7365 672e              seg.
+0000d670: 6861 735f 776f 7264 7320 616e 640d 0a20  has_words and.. 
+0000d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d690: 2020 2020 2020 2020 2020 2028 0d0a 2020             (..  
+0000d6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6c0: 2020 2873 6567 2e77 6f72 645f 636f 756e    (seg.word_coun
+0000d6d0: 7428 2920 2b20 7365 6c66 2e73 6567 6d65  t() + self.segme
+0000d6e0: 6e74 735b 6920 2b20 315d 2e77 6f72 645f  nts[i + 1].word_
+0000d6f0: 636f 756e 7428 2920 3e20 6d61 785f 776f  count() > max_wo
+0000d700: 7264 7329 0d0a 2020 2020 2020 2020 2020  rds)..          
+0000d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d720: 2020 2020 2020 2020 2020 6966 2069 735f            if is_
+0000d730: 7375 6d5f 6d61 7820 656c 7365 0d0a 2020  sum_max else..  
+0000d740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d760: 2020 2873 6567 2e77 6f72 645f 636f 756e    (seg.word_coun
+0000d770: 7428 2920 3e20 6d61 785f 776f 7264 7320  t() > max_words 
+0000d780: 616e 6420 7365 6c66 2e73 6567 6d65 6e74  and self.segment
+0000d790: 735b 6920 2b20 315d 2e77 6f72 645f 636f  s[i + 1].word_co
+0000d7a0: 756e 7428 2920 3e20 6d61 785f 776f 7264  unt() > max_word
+0000d7b0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
 0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7d0: 2020 2020 2020 6d61 785f 6368 6172 7320        max_chars 
-0000d7e0: 616e 640d 0a20 2020 2020 2020 2020 2020  and..           
+0000d7d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000d7e0: 2020 2020 2020 2029 206f 720d 0a20 2020         ) or..   
 0000d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d800: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
 0000d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d820: 2020 2020 2020 2020 2873 6567 2e63 6861          (seg.cha
-0000d830: 725f 636f 756e 7428 2920 2b20 7365 6c66  r_count() + self
-0000d840: 2e73 6567 6d65 6e74 735b 6920 2b20 315d  .segments[i + 1]
-0000d850: 2e63 6861 725f 636f 756e 7428 2920 3e20  .char_count() > 
-0000d860: 6d61 785f 6368 6172 7329 0d0a 2020 2020  max_chars)..    
-0000d870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d890: 6966 2069 735f 7375 6d5f 6d61 7820 656c  if is_sum_max el
-0000d8a0: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
-0000d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8c0: 2020 2020 2020 2020 2873 6567 2e63 6861          (seg.cha
-0000d8d0: 725f 636f 756e 7428 2920 3e20 6d61 785f  r_count() > max_
-0000d8e0: 6368 6172 7320 616e 6420 7365 6c66 2e73  chars and self.s
-0000d8f0: 6567 6d65 6e74 735b 6920 2b20 315d 2e63  egments[i + 1].c
-0000d900: 6861 725f 636f 756e 7428 2920 3e20 6d61  har_count() > ma
-0000d910: 785f 6368 6172 7329 0d0a 2020 2020 2020  x_chars)..      
-0000d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d930: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0000d940: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-0000d950: 2020 2020 2020 2020 2020 2020 293a 0d0a              ):..
-0000d960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d970: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
-0000d980: 2020 2020 2020 7365 6c66 2e61 6464 5f73        self.add_s
-0000d990: 6567 6d65 6e74 7328 692c 2069 202b 2031  egments(i, i + 1
-0000d9a0: 2c20 696e 706c 6163 653d 5472 7565 2c20  , inplace=True, 
-0000d9b0: 6c6f 636b 3d6c 6f63 6b29 0d0a 2020 2020  lock=lock)..    
-0000d9c0: 2020 2020 7365 6c66 2e72 656d 6f76 655f      self.remove_
-0000d9d0: 6e6f 5f77 6f72 645f 7365 676d 656e 7473  no_word_segments
-0000d9e0: 2829 0d0a 0d0a 2020 2020 6465 6620 6765  ()....    def ge
-0000d9f0: 745f 636f 6e74 656e 745f 6279 5f74 696d  t_content_by_tim
-0000da00: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
-0000da10: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-0000da20: 2020 2074 696d 653a 2055 6e69 6f6e 5b66     time: Union[f
-0000da30: 6c6f 6174 2c20 5475 706c 655b 666c 6f61  loat, Tuple[floa
-0000da40: 742c 2066 6c6f 6174 5d2c 2064 6963 745d  t, float], dict]
-0000da50: 2c0d 0a20 2020 2020 2020 2020 2020 2077  ,..            w
-0000da60: 6974 6869 6e3a 2062 6f6f 6c20 3d20 4661  ithin: bool = Fa
-0000da70: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
-0000da80: 2020 7365 676d 656e 745f 6c65 7665 6c3a    segment_level:
-0000da90: 2062 6f6f 6c20 3d20 4661 6c73 650d 0a20   bool = False.. 
-0000daa0: 2020 2029 202d 3e20 556e 696f 6e5b 4c69     ) -> Union[Li
-0000dab0: 7374 5b57 6f72 6454 696d 696e 675d 2c20  st[WordTiming], 
-0000dac0: 4c69 7374 5b53 6567 6d65 6e74 5d5d 3a0d  List[Segment]]:.
-0000dad0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0000dae0: 2020 2020 2020 5265 7475 726e 2063 6f6e        Return con
-0000daf0: 7465 6e74 2069 6e20 7468 6520 6060 7469  tent in the ``ti
-0000db00: 6d65 6060 2072 616e 6765 2e0d 0a0d 0a20  me`` range..... 
-0000db10: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-0000db20: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
-0000db30: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2074  -----..        t
-0000db40: 696d 6520 3a20 666c 6f61 7420 6f72 2074  ime : float or t
-0000db50: 7570 6c65 206f 6620 2866 6c6f 6174 2c20  uple of (float, 
-0000db60: 666c 6f61 7429 206f 7220 6469 6374 0d0a  float) or dict..
-0000db70: 2020 2020 2020 2020 2020 2020 5261 6e67              Rang
-0000db80: 6520 6f66 2074 696d 6520 746f 2066 696e  e of time to fin
-0000db90: 6420 636f 6e74 656e 742e 2046 6f72 2074  d content. For t
-0000dba0: 7570 6c65 206f 6620 7477 6f20 666c 6f61  uple of two floa
-0000dbb0: 7473 2c20 6669 7273 7420 7661 6c75 6520  ts, first value 
-0000dbc0: 6973 2074 6865 2073 7461 7274 2074 696d  is the start tim
-0000dbd0: 6520 616e 6420 7365 636f 6e64 2076 616c  e and second val
-0000dbe0: 7565 2069 730d 0a20 2020 2020 2020 2020  ue is..         
-0000dbf0: 2020 2074 6865 2065 6e64 2074 696d 652e     the end time.
-0000dc00: 2046 6f72 2061 2073 696e 676c 6520 666c   For a single fl
-0000dc10: 6f61 7420 7661 6c75 652c 2069 7420 6973  oat value, it is
-0000dc20: 2074 7265 6174 6564 2061 7320 626f 7468   treated as both
-0000dc30: 2074 6865 2073 7461 7274 2061 6e64 2065   the start and e
-0000dc40: 6e64 2074 696d 652e 0d0a 2020 2020 2020  nd time...      
-0000dc50: 2020 7769 7468 696e 203a 2062 6f6f 6c2c    within : bool,
-0000dc60: 2064 6566 6175 6c74 2046 616c 7365 0d0a   default False..
-0000dc70: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
-0000dc80: 6865 7220 746f 206f 6e6c 7920 6669 6e64  her to only find
-0000dc90: 2063 6f6e 7465 6e74 2066 756c 6c79 206f   content fully o
-0000dca0: 7665 726c 6170 7320 7769 7468 2060 6074  verlaps with ``t
-0000dcb0: 696d 6560 6020 7261 6e67 652e 0d0a 2020  ime`` range...  
-0000dcc0: 2020 2020 2020 7365 676d 656e 745f 6c65        segment_le
-0000dcd0: 7665 6c20 3a20 626f 6f6c 2c20 6465 6661  vel : bool, defa
-0000dce0: 756c 7420 4661 6c73 650d 0a20 2020 2020  ult False..     
-0000dcf0: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
-0000dd00: 6f20 6c6f 6f6b 206f 6e6c 7920 6f6e 2074  o look only on t
-0000dd10: 6865 2073 6567 6d65 6e74 206c 6576 656c  he segment level
-0000dd20: 2061 6e64 2072 6574 7572 6e20 696e 7374   and return inst
-0000dd30: 616e 6365 7320 6f66 203a 636c 6173 733a  ances of :class:
-0000dd40: 6073 7461 626c 655f 7768 6973 7065 722e  `stable_whisper.
-0000dd50: 7265 7375 6c74 2e53 6567 6d65 6e74 600d  result.Segment`.
-0000dd60: 0a20 2020 2020 2020 2020 2020 2069 6e73  .            ins
-0000dd70: 7465 6164 206f 6620 3a63 6c61 7373 3a60  tead of :class:`
-0000dd80: 7374 6162 6c65 5f77 6869 7370 6572 2e72  stable_whisper.r
-0000dd90: 6573 756c 742e 576f 7264 5469 6d69 6e67  esult.WordTiming
-0000dda0: 602e 0d0a 0d0a 2020 2020 2020 2020 5265  `.....        Re
-0000ddb0: 7475 726e 730d 0a20 2020 2020 2020 202d  turns..        -
-0000ddc0: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
-0000ddd0: 6c69 7374 206f 6620 7374 6162 6c65 5f77  list of stable_w
-0000dde0: 6869 7370 6572 2e72 6573 756c 742e 576f  hisper.result.Wo
-0000ddf0: 7264 5469 6d69 6e67 206f 7220 6c69 7374  rdTiming or list
-0000de00: 206f 6620 7374 6162 6c65 5f77 6869 7370   of stable_whisp
-0000de10: 6572 2e72 6573 756c 742e 5365 676d 656e  er.result.Segmen
-0000de20: 740d 0a20 2020 2020 2020 2020 2020 204c  t..            L
-0000de30: 6973 7420 6f66 2063 6f6e 7465 6e74 7320  ist of contents 
-0000de40: 696e 2074 6865 2060 6074 696d 6560 6020  in the ``time`` 
-0000de50: 7261 6e67 652e 2054 6865 2063 6f6e 7465  range. The conte
-0000de60: 6e74 7320 6172 6520 696e 7374 616e 6365  nts are instance
-0000de70: 7320 6f66 0d0a 2020 2020 2020 2020 2020  s of..          
-0000de80: 2020 3a63 6c61 7373 3a60 7374 6162 6c65    :class:`stable
-0000de90: 5f77 6869 7370 6572 2e72 6573 756c 742e  _whisper.result.
-0000dea0: 5365 676d 656e 7460 2069 6620 6060 7365  Segment` if ``se
-0000deb0: 676d 656e 745f 6c65 7665 6c20 3d20 5472  gment_level = Tr
-0000dec0: 7565 6060 2065 6c73 650d 0a20 2020 2020  ue`` else..     
-0000ded0: 2020 2020 2020 203a 636c 6173 733a 6073         :class:`s
-0000dee0: 7461 626c 655f 7768 6973 7065 722e 7265  table_whisper.re
-0000def0: 7375 6c74 2e57 6f72 6454 696d 696e 6760  sult.WordTiming`
-0000df00: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-0000df10: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-0000df20: 6567 6d65 6e74 5f6c 6576 656c 2061 6e64  egment_level and
-0000df30: 206e 6f74 2073 656c 662e 6861 735f 776f   not self.has_wo
-0000df40: 7264 733a 0d0a 2020 2020 2020 2020 2020  rds:..          
-0000df50: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000df60: 6f72 2827 4d69 7373 696e 6720 776f 7264  or('Missing word
-0000df70: 2074 696d 6573 7461 6d70 7320 696e 2072   timestamps in r
-0000df80: 6573 756c 742e 2055 7365 2060 6073 6567  esult. Use ``seg
-0000df90: 6d65 6e74 5f6c 6576 656c 3d54 7275 6560  ment_level=True`
-0000dfa0: 6020 696e 7374 6561 642e 2729 0d0a 2020  ` instead.')..  
-0000dfb0: 2020 2020 2020 636f 6e74 656e 7473 203d        contents =
-0000dfc0: 2073 656c 662e 7365 676d 656e 7473 2069   self.segments i
-0000dfd0: 6620 7365 676d 656e 745f 6c65 7665 6c20  f segment_level 
-0000dfe0: 656c 7365 2073 656c 662e 616c 6c5f 776f  else self.all_wo
-0000dff0: 7264 7328 290d 0a20 2020 2020 2020 2069  rds()..        i
-0000e000: 6620 6973 696e 7374 616e 6365 2874 696d  f isinstance(tim
-0000e010: 652c 2028 666c 6f61 742c 2069 6e74 2929  e, (float, int))
-0000e020: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
-0000e030: 696d 6520 3d20 5b74 696d 652c 2074 696d  ime = [time, tim
-0000e040: 655d 0d0a 2020 2020 2020 2020 656c 6966  e]..        elif
-0000e050: 2069 7369 6e73 7461 6e63 6528 7469 6d65   isinstance(time
-0000e060: 2c20 6469 6374 293a 0d0a 2020 2020 2020  , dict):..      
-0000e070: 2020 2020 2020 7469 6d65 203d 205b 7469        time = [ti
-0000e080: 6d65 5b27 7374 6172 7427 5d2c 2074 696d  me['start'], tim
-0000e090: 655b 2765 6e64 275d 5d0d 0a20 2020 2020  e['end']]..     
-0000e0a0: 2020 2073 7461 7274 2c20 656e 6420 3d20     start, end = 
-0000e0b0: 7469 6d65 0d0a 0d0a 2020 2020 2020 2020  time....        
-0000e0c0: 6966 2077 6974 6869 6e3a 0d0a 2020 2020  if within:..    
-0000e0d0: 2020 2020 2020 2020 6465 6620 6973 5f69          def is_i
-0000e0e0: 6e5f 7261 6e67 6528 6329 3a0d 0a20 2020  n_range(c):..   
-0000e0f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000e100: 7572 6e20 7374 6172 7420 3c3d 2063 2e73  urn start <= c.s
-0000e110: 7461 7274 2061 6e64 2065 6e64 203e 3d20  tart and end >= 
-0000e120: 632e 656e 640d 0a20 2020 2020 2020 2065  c.end..        e
-0000e130: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-0000e140: 2020 6465 6620 6973 5f69 6e5f 7261 6e67    def is_in_rang
-0000e150: 6528 6329 3a0d 0a20 2020 2020 2020 2020  e(c):..         
-0000e160: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
-0000e170: 6172 7420 3c3d 2063 2e65 6e64 2061 6e64  art <= c.end and
-0000e180: 2065 6e64 203e 3d20 632e 7374 6172 740d   end >= c.start.
-0000e190: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-0000e1a0: 6e20 5b63 2066 6f72 2063 2069 6e20 636f  n [c for c in co
-0000e1b0: 6e74 656e 7473 2069 6620 6973 5f69 6e5f  ntents if is_in_
-0000e1c0: 7261 6e67 6528 6329 5d0d 0a0d 0a20 2020  range(c)]....   
-0000e1d0: 2064 6566 2073 706c 6974 5f62 795f 6761   def split_by_ga
-0000e1e0: 7028 0d0a 2020 2020 2020 2020 2020 2020  p(..            
-0000e1f0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-0000e200: 2020 206d 6178 5f67 6170 3a20 666c 6f61     max_gap: floa
-0000e210: 7420 3d20 302e 312c 0d0a 2020 2020 2020  t = 0.1,..      
-0000e220: 2020 2020 2020 6c6f 636b 3a20 626f 6f6c        lock: bool
-0000e230: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
-0000e240: 2020 2020 2020 206e 6577 6c69 6e65 3a20         newline: 
-0000e250: 626f 6f6c 203d 2046 616c 7365 0d0a 2020  bool = False..  
-0000e260: 2020 2920 2d3e 2022 5768 6973 7065 7252    ) -> "WhisperR
-0000e270: 6573 756c 7422 3a0d 0a20 2020 2020 2020  esult":..       
-0000e280: 2022 2222 0d0a 2020 2020 2020 2020 5370   """..        Sp
-0000e290: 6c69 7420 2869 6e2d 706c 6163 6529 2061  lit (in-place) a
-0000e2a0: 6e79 2073 6567 6d65 6e74 2077 6865 7265  ny segment where
-0000e2b0: 2074 6865 2067 6170 2062 6574 7765 656e   the gap between
-0000e2c0: 2074 776f 206f 6620 6974 7320 776f 7264   two of its word
-0000e2d0: 7320 6973 2067 7265 6174 6572 2074 6861  s is greater tha
-0000e2e0: 6e20 6060 6d61 785f 6761 7060 602e 0d0a  n ``max_gap``...
-0000e2f0: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0000e300: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
-0000e310: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-0000e320: 2020 6d61 785f 6761 7020 3a20 666c 6f61    max_gap : floa
-0000e330: 742c 2064 6566 6175 6c74 2030 2e31 0d0a  t, default 0.1..
-0000e340: 2020 2020 2020 2020 2020 2020 4d61 7869              Maxi
-0000e350: 6d75 6d20 7365 636f 6e64 2873 2920 616c  mum second(s) al
-0000e360: 6c6f 7765 6420 6265 7477 6565 6e20 7477  lowed between tw
-0000e370: 6f20 776f 7264 7320 6966 2074 6865 2073  o words if the s
-0000e380: 616d 6520 7365 676d 656e 742e 0d0a 2020  ame segment...  
-0000e390: 2020 2020 2020 6c6f 636b 203a 2062 6f6f        lock : boo
-0000e3a0: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
-0000e3b0: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-0000e3c0: 6574 6865 7220 746f 2070 7265 7665 6e74  ether to prevent
-0000e3d0: 2066 7574 7572 6520 7370 6c69 7473 2f6d   future splits/m
-0000e3e0: 6572 6765 7320 6672 6f6d 2061 6c74 6572  erges from alter
-0000e3f0: 696e 6720 6368 616e 6765 7320 6d61 6465  ing changes made
-0000e400: 2062 7920 7468 6973 206d 6574 686f 642e   by this method.
-0000e410: 0d0a 2020 2020 2020 2020 6e65 776c 696e  ..        newlin
-0000e420: 653a 2062 6f6f 6c2c 2064 6566 6175 6c74  e: bool, default
-0000e430: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-0000e440: 2020 2020 5768 6574 6865 7220 746f 2069      Whether to i
-0000e450: 6e73 6572 7420 6c69 6e65 2062 7265 616b  nsert line break
-0000e460: 2061 7420 7468 6520 7370 6c69 7420 706f   at the split po
-0000e470: 696e 7473 2069 6e73 7465 6164 206f 6620  ints instead of 
-0000e480: 7370 6c69 7474 696e 6720 696e 746f 2073  splitting into s
-0000e490: 6570 6172 6174 6520 7365 676d 656e 7473  eparate segments
-0000e4a0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
-0000e4b0: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
-0000e4c0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
-0000e4d0: 7461 626c 655f 7768 6973 7065 722e 7265  table_whisper.re
-0000e4e0: 7375 6c74 2e57 6869 7370 6572 5265 7375  sult.WhisperResu
-0000e4f0: 6c74 0d0a 2020 2020 2020 2020 2020 2020  lt..            
-0000e500: 5468 6520 6375 7272 656e 7420 696e 7374  The current inst
-0000e510: 616e 6365 2061 6674 6572 2074 6865 2063  ance after the c
-0000e520: 6861 6e67 6573 2e0d 0a20 2020 2020 2020  hanges...       
-0000e530: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
-0000e540: 6c66 2e5f 7370 6c69 745f 7365 676d 656e  lf._split_segmen
-0000e550: 7473 286c 616d 6264 6120 783a 2078 2e67  ts(lambda x: x.g
-0000e560: 6574 5f67 6170 5f69 6e64 6963 6573 286d  et_gap_indices(m
-0000e570: 6178 5f67 6170 292c 206c 6f63 6b3d 6c6f  ax_gap), lock=lo
-0000e580: 636b 2c20 6e65 776c 696e 653d 6e65 776c  ck, newline=newl
-0000e590: 696e 6529 0d0a 2020 2020 2020 2020 6966  ine)..        if
-0000e5a0: 2073 656c 662e 5f72 6567 726f 7570 5f68   self._regroup_h
-0000e5b0: 6973 746f 7279 3a0d 0a20 2020 2020 2020  istory:..       
-0000e5c0: 2020 2020 2073 656c 662e 5f72 6567 726f       self._regro
-0000e5d0: 7570 5f68 6973 746f 7279 202b 3d20 275f  up_history += '_
-0000e5e0: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
+0000d820: 6d61 785f 6368 6172 7320 616e 640d 0a20  max_chars and.. 
+0000d830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d840: 2020 2020 2020 2020 2020 2028 0d0a 2020             (..  
+0000d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d870: 2020 2873 6567 2e63 6861 725f 636f 756e    (seg.char_coun
+0000d880: 7428 2920 2b20 7365 6c66 2e73 6567 6d65  t() + self.segme
+0000d890: 6e74 735b 6920 2b20 315d 2e63 6861 725f  nts[i + 1].char_
+0000d8a0: 636f 756e 7428 2920 3e20 6d61 785f 6368  count() > max_ch
+0000d8b0: 6172 7329 0d0a 2020 2020 2020 2020 2020  ars)..          
+0000d8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8d0: 2020 2020 2020 2020 2020 6966 2069 735f            if is_
+0000d8e0: 7375 6d5f 6d61 7820 656c 7365 0d0a 2020  sum_max else..  
+0000d8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d910: 2020 2873 6567 2e63 6861 725f 636f 756e    (seg.char_coun
+0000d920: 7428 2920 3e20 6d61 785f 6368 6172 7320  t() > max_chars 
+0000d930: 616e 6420 7365 6c66 2e73 6567 6d65 6e74  and self.segment
+0000d940: 735b 6920 2b20 315d 2e63 6861 725f 636f  s[i + 1].char_co
+0000d950: 756e 7428 2920 3e20 6d61 785f 6368 6172  unt() > max_char
+0000d960: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+0000d970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d980: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000d990: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0000d9a0: 2020 2020 2020 293a 0d0a 2020 2020 2020        ):..      
+0000d9b0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+0000d9c0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+0000d9d0: 7365 6c66 2e61 6464 5f73 6567 6d65 6e74  self.add_segment
+0000d9e0: 7328 692c 2069 202b 2031 2c20 696e 706c  s(i, i + 1, inpl
+0000d9f0: 6163 653d 5472 7565 2c20 6c6f 636b 3d6c  ace=True, lock=l
+0000da00: 6f63 6b29 0d0a 2020 2020 2020 2020 7365  ock)..        se
+0000da10: 6c66 2e72 656d 6f76 655f 6e6f 5f77 6f72  lf.remove_no_wor
+0000da20: 645f 7365 676d 656e 7473 2829 0d0a 0d0a  d_segments()....
+0000da30: 2020 2020 6465 6620 6765 745f 636f 6e74      def get_cont
+0000da40: 656e 745f 6279 5f74 696d 6528 0d0a 2020  ent_by_time(..  
+0000da50: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
+0000da60: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+0000da70: 653a 2055 6e69 6f6e 5b66 6c6f 6174 2c20  e: Union[float, 
+0000da80: 5475 706c 655b 666c 6f61 742c 2066 6c6f  Tuple[float, flo
+0000da90: 6174 5d2c 2064 6963 745d 2c0d 0a20 2020  at], dict],..   
+0000daa0: 2020 2020 2020 2020 2077 6974 6869 6e3a           within:
+0000dab0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
+0000dac0: 2020 2020 2020 2020 2020 2020 7365 676d              segm
+0000dad0: 656e 745f 6c65 7665 6c3a 2062 6f6f 6c20  ent_level: bool 
+0000dae0: 3d20 4661 6c73 650d 0a20 2020 2029 202d  = False..    ) -
+0000daf0: 3e20 556e 696f 6e5b 4c69 7374 5b57 6f72  > Union[List[Wor
+0000db00: 6454 696d 696e 675d 2c20 4c69 7374 5b53  dTiming], List[S
+0000db10: 6567 6d65 6e74 5d5d 3a0d 0a20 2020 2020  egment]]:..     
+0000db20: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+0000db30: 5265 7475 726e 2063 6f6e 7465 6e74 2069  Return content i
+0000db40: 6e20 7468 6520 6060 7469 6d65 6060 2072  n the ``time`` r
+0000db50: 616e 6765 2e0d 0a0d 0a20 2020 2020 2020  ange.....       
+0000db60: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
+0000db70: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d       ----------.
+0000db80: 0a20 2020 2020 2020 2074 696d 6520 3a20  .        time : 
+0000db90: 666c 6f61 7420 6f72 2074 7570 6c65 206f  float or tuple o
+0000dba0: 6620 2866 6c6f 6174 2c20 666c 6f61 7429  f (float, float)
+0000dbb0: 206f 7220 6469 6374 0d0a 2020 2020 2020   or dict..      
+0000dbc0: 2020 2020 2020 5261 6e67 6520 6f66 2074        Range of t
+0000dbd0: 696d 6520 746f 2066 696e 6420 636f 6e74  ime to find cont
+0000dbe0: 656e 742e 2046 6f72 2074 7570 6c65 206f  ent. For tuple o
+0000dbf0: 6620 7477 6f20 666c 6f61 7473 2c20 6669  f two floats, fi
+0000dc00: 7273 7420 7661 6c75 6520 6973 2074 6865  rst value is the
+0000dc10: 2073 7461 7274 2074 696d 6520 616e 6420   start time and 
+0000dc20: 7365 636f 6e64 2076 616c 7565 2069 730d  second value is.
+0000dc30: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+0000dc40: 2065 6e64 2074 696d 652e 2046 6f72 2061   end time. For a
+0000dc50: 2073 696e 676c 6520 666c 6f61 7420 7661   single float va
+0000dc60: 6c75 652c 2069 7420 6973 2074 7265 6174  lue, it is treat
+0000dc70: 6564 2061 7320 626f 7468 2074 6865 2073  ed as both the s
+0000dc80: 7461 7274 2061 6e64 2065 6e64 2074 696d  tart and end tim
+0000dc90: 652e 0d0a 2020 2020 2020 2020 7769 7468  e...        with
+0000dca0: 696e 203a 2062 6f6f 6c2c 2064 6566 6175  in : bool, defau
+0000dcb0: 6c74 2046 616c 7365 0d0a 2020 2020 2020  lt False..      
+0000dcc0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+0000dcd0: 206f 6e6c 7920 6669 6e64 2063 6f6e 7465   only find conte
+0000dce0: 6e74 2066 756c 6c79 206f 7665 726c 6170  nt fully overlap
+0000dcf0: 7320 7769 7468 2060 6074 696d 6560 6020  s with ``time`` 
+0000dd00: 7261 6e67 652e 0d0a 2020 2020 2020 2020  range...        
+0000dd10: 7365 676d 656e 745f 6c65 7665 6c20 3a20  segment_level : 
+0000dd20: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
+0000dd30: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+0000dd40: 2057 6865 7468 6572 2074 6f20 6c6f 6f6b   Whether to look
+0000dd50: 206f 6e6c 7920 6f6e 2074 6865 2073 6567   only on the seg
+0000dd60: 6d65 6e74 206c 6576 656c 2061 6e64 2072  ment level and r
+0000dd70: 6574 7572 6e20 696e 7374 616e 6365 7320  eturn instances 
+0000dd80: 6f66 203a 636c 6173 733a 6073 7461 626c  of :class:`stabl
+0000dd90: 655f 7768 6973 7065 722e 7265 7375 6c74  e_whisper.result
+0000dda0: 2e53 6567 6d65 6e74 600d 0a20 2020 2020  .Segment`..     
+0000ddb0: 2020 2020 2020 2069 6e73 7465 6164 206f         instead o
+0000ddc0: 6620 3a63 6c61 7373 3a60 7374 6162 6c65  f :class:`stable
+0000ddd0: 5f77 6869 7370 6572 2e72 6573 756c 742e  _whisper.result.
+0000dde0: 576f 7264 5469 6d69 6e67 602e 0d0a 0d0a  WordTiming`.....
+0000ddf0: 2020 2020 2020 2020 5265 7475 726e 730d          Returns.
+0000de00: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000de10: 0d0a 2020 2020 2020 2020 6c69 7374 206f  ..        list o
+0000de20: 6620 7374 6162 6c65 5f77 6869 7370 6572  f stable_whisper
+0000de30: 2e72 6573 756c 742e 576f 7264 5469 6d69  .result.WordTimi
+0000de40: 6e67 206f 7220 6c69 7374 206f 6620 7374  ng or list of st
+0000de50: 6162 6c65 5f77 6869 7370 6572 2e72 6573  able_whisper.res
+0000de60: 756c 742e 5365 676d 656e 740d 0a20 2020  ult.Segment..   
+0000de70: 2020 2020 2020 2020 204c 6973 7420 6f66           List of
+0000de80: 2063 6f6e 7465 6e74 7320 696e 2074 6865   contents in the
+0000de90: 2060 6074 696d 6560 6020 7261 6e67 652e   ``time`` range.
+0000dea0: 2054 6865 2063 6f6e 7465 6e74 7320 6172   The contents ar
+0000deb0: 6520 696e 7374 616e 6365 7320 6f66 0d0a  e instances of..
+0000dec0: 2020 2020 2020 2020 2020 2020 3a63 6c61              :cla
+0000ded0: 7373 3a60 7374 6162 6c65 5f77 6869 7370  ss:`stable_whisp
+0000dee0: 6572 2e72 6573 756c 742e 5365 676d 656e  er.result.Segmen
+0000def0: 7460 2069 6620 6060 7365 676d 656e 745f  t` if ``segment_
+0000df00: 6c65 7665 6c20 3d20 5472 7565 6060 2065  level = True`` e
+0000df10: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+0000df20: 203a 636c 6173 733a 6073 7461 626c 655f   :class:`stable_
+0000df30: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
+0000df40: 6f72 6454 696d 696e 6760 2e0d 0a20 2020  ordTiming`...   
+0000df50: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+0000df60: 2020 6966 206e 6f74 2073 6567 6d65 6e74    if not segment
+0000df70: 5f6c 6576 656c 2061 6e64 206e 6f74 2073  _level and not s
+0000df80: 656c 662e 6861 735f 776f 7264 733a 0d0a  elf.has_words:..
+0000df90: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000dfa0: 6520 5661 6c75 6545 7272 6f72 2827 4d69  e ValueError('Mi
+0000dfb0: 7373 696e 6720 776f 7264 2074 696d 6573  ssing word times
+0000dfc0: 7461 6d70 7320 696e 2072 6573 756c 742e  tamps in result.
+0000dfd0: 2055 7365 2060 6073 6567 6d65 6e74 5f6c   Use ``segment_l
+0000dfe0: 6576 656c 3d54 7275 6560 6020 696e 7374  evel=True`` inst
+0000dff0: 6561 642e 2729 0d0a 2020 2020 2020 2020  ead.')..        
+0000e000: 636f 6e74 656e 7473 203d 2073 656c 662e  contents = self.
+0000e010: 7365 676d 656e 7473 2069 6620 7365 676d  segments if segm
+0000e020: 656e 745f 6c65 7665 6c20 656c 7365 2073  ent_level else s
+0000e030: 656c 662e 616c 6c5f 776f 7264 7328 290d  elf.all_words().
+0000e040: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+0000e050: 7374 616e 6365 2874 696d 652c 2028 666c  stance(time, (fl
+0000e060: 6f61 742c 2069 6e74 2929 3a0d 0a20 2020  oat, int)):..   
+0000e070: 2020 2020 2020 2020 2074 696d 6520 3d20           time = 
+0000e080: 5b74 696d 652c 2074 696d 655d 0d0a 2020  [time, time]..  
+0000e090: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+0000e0a0: 7461 6e63 6528 7469 6d65 2c20 6469 6374  tance(time, dict
+0000e0b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000e0c0: 7469 6d65 203d 205b 7469 6d65 5b27 7374  time = [time['st
+0000e0d0: 6172 7427 5d2c 2074 696d 655b 2765 6e64  art'], time['end
+0000e0e0: 275d 5d0d 0a20 2020 2020 2020 2073 7461  ']]..        sta
+0000e0f0: 7274 2c20 656e 6420 3d20 7469 6d65 0d0a  rt, end = time..
+0000e100: 0d0a 2020 2020 2020 2020 6966 2077 6974  ..        if wit
+0000e110: 6869 6e3a 0d0a 2020 2020 2020 2020 2020  hin:..          
+0000e120: 2020 6465 6620 6973 5f69 6e5f 7261 6e67    def is_in_rang
+0000e130: 6528 6329 3a0d 0a20 2020 2020 2020 2020  e(c):..         
+0000e140: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+0000e150: 6172 7420 3c3d 2063 2e73 7461 7274 2061  art <= c.start a
+0000e160: 6e64 2065 6e64 203e 3d20 632e 656e 640d  nd end >= c.end.
+0000e170: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+0000e180: 2020 2020 2020 2020 2020 2020 6465 6620              def 
+0000e190: 6973 5f69 6e5f 7261 6e67 6528 6329 3a0d  is_in_range(c):.
+0000e1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e1b0: 2072 6574 7572 6e20 7374 6172 7420 3c3d   return start <=
+0000e1c0: 2063 2e65 6e64 2061 6e64 2065 6e64 203e   c.end and end >
+0000e1d0: 3d20 632e 7374 6172 740d 0a0d 0a20 2020  = c.start....   
+0000e1e0: 2020 2020 2072 6574 7572 6e20 5b63 2066       return [c f
+0000e1f0: 6f72 2063 2069 6e20 636f 6e74 656e 7473  or c in contents
+0000e200: 2069 6620 6973 5f69 6e5f 7261 6e67 6528   if is_in_range(
+0000e210: 6329 5d0d 0a0d 0a20 2020 2064 6566 2073  c)]....    def s
+0000e220: 706c 6974 5f62 795f 6761 7028 0d0a 2020  plit_by_gap(..  
+0000e230: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
+0000e240: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+0000e250: 5f67 6170 3a20 666c 6f61 7420 3d20 302e  _gap: float = 0.
+0000e260: 312c 0d0a 2020 2020 2020 2020 2020 2020  1,..            
+0000e270: 6c6f 636b 3a20 626f 6f6c 203d 2046 616c  lock: bool = Fal
+0000e280: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
+0000e290: 206e 6577 6c69 6e65 3a20 626f 6f6c 203d   newline: bool =
+0000e2a0: 2046 616c 7365 0d0a 2020 2020 2920 2d3e   False..    ) ->
+0000e2b0: 2022 5768 6973 7065 7252 6573 756c 7422   "WhisperResult"
+0000e2c0: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+0000e2d0: 2020 2020 2020 2020 5370 6c69 7420 2869          Split (i
+0000e2e0: 6e2d 706c 6163 6529 2061 6e79 2073 6567  n-place) any seg
+0000e2f0: 6d65 6e74 2077 6865 7265 2074 6865 2067  ment where the g
+0000e300: 6170 2062 6574 7765 656e 2074 776f 206f  ap between two o
+0000e310: 6620 6974 7320 776f 7264 7320 6973 2067  f its words is g
+0000e320: 7265 6174 6572 2074 6861 6e20 6060 6d61  reater than ``ma
+0000e330: 785f 6761 7060 602e 0d0a 0d0a 2020 2020  x_gap``.....    
+0000e340: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
+0000e350: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+0000e360: 2d2d 0d0a 2020 2020 2020 2020 6d61 785f  --..        max_
+0000e370: 6761 7020 3a20 666c 6f61 742c 2064 6566  gap : float, def
+0000e380: 6175 6c74 2030 2e31 0d0a 2020 2020 2020  ault 0.1..      
+0000e390: 2020 2020 2020 4d61 7869 6d75 6d20 7365        Maximum se
+0000e3a0: 636f 6e64 2873 2920 616c 6c6f 7765 6420  cond(s) allowed 
+0000e3b0: 6265 7477 6565 6e20 7477 6f20 776f 7264  between two word
+0000e3c0: 7320 6966 2074 6865 2073 616d 6520 7365  s if the same se
+0000e3d0: 676d 656e 742e 0d0a 2020 2020 2020 2020  gment...        
+0000e3e0: 6c6f 636b 203a 2062 6f6f 6c2c 2064 6566  lock : bool, def
+0000e3f0: 6175 6c74 2046 616c 7365 0d0a 2020 2020  ault False..    
+0000e400: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
+0000e410: 746f 2070 7265 7665 6e74 2066 7574 7572  to prevent futur
+0000e420: 6520 7370 6c69 7473 2f6d 6572 6765 7320  e splits/merges 
+0000e430: 6672 6f6d 2061 6c74 6572 696e 6720 6368  from altering ch
+0000e440: 616e 6765 7320 6d61 6465 2062 7920 7468  anges made by th
+0000e450: 6973 206d 6574 686f 642e 0d0a 2020 2020  is method...    
+0000e460: 2020 2020 6e65 776c 696e 653a 2062 6f6f      newline: boo
+0000e470: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
+0000e480: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
+0000e490: 6574 6865 7220 746f 2069 6e73 6572 7420  ether to insert 
+0000e4a0: 6c69 6e65 2062 7265 616b 2061 7420 7468  line break at th
+0000e4b0: 6520 7370 6c69 7420 706f 696e 7473 2069  e split points i
+0000e4c0: 6e73 7465 6164 206f 6620 7370 6c69 7474  nstead of splitt
+0000e4d0: 696e 6720 696e 746f 2073 6570 6172 6174  ing into separat
+0000e4e0: 6520 7365 676d 656e 7473 2e0d 0a0d 0a20  e segments..... 
+0000e4f0: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
+0000e500: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
+0000e510: 0a20 2020 2020 2020 2073 7461 626c 655f  .        stable_
+0000e520: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
+0000e530: 6869 7370 6572 5265 7375 6c74 0d0a 2020  hisperResult..  
+0000e540: 2020 2020 2020 2020 2020 5468 6520 6375            The cu
+0000e550: 7272 656e 7420 696e 7374 616e 6365 2061  rrent instance a
+0000e560: 6674 6572 2074 6865 2063 6861 6e67 6573  fter the changes
+0000e570: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+0000e580: 2020 2020 2020 2020 7365 6c66 2e5f 7370          self._sp
+0000e590: 6c69 745f 7365 676d 656e 7473 286c 616d  lit_segments(lam
+0000e5a0: 6264 6120 783a 2078 2e67 6574 5f67 6170  bda x: x.get_gap
+0000e5b0: 5f69 6e64 6963 6573 286d 6178 5f67 6170  _indices(max_gap
+0000e5c0: 292c 206c 6f63 6b3d 6c6f 636b 2c20 6e65  ), lock=lock, ne
+0000e5d0: 776c 696e 653d 6e65 776c 696e 6529 0d0a  wline=newline)..
+0000e5e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
 0000e5f0: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
-0000e600: 202b 3d20 6627 7367 3d7b 6d61 785f 6761   += f'sg={max_ga
-0000e610: 707d 2b7b 696e 7428 6c6f 636b 297d 2b7b  p}+{int(lock)}+{
-0000e620: 696e 7428 6e65 776c 696e 6529 7d27 0d0a  int(newline)}'..
-0000e630: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000e640: 656c 660d 0a0d 0a20 2020 2064 6566 206d  elf....    def m
-0000e650: 6572 6765 5f62 795f 6761 7028 0d0a 2020  erge_by_gap(..  
-0000e660: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
-0000e670: 0a20 2020 2020 2020 2020 2020 206d 696e  .            min
-0000e680: 5f67 6170 3a20 666c 6f61 7420 3d20 302e  _gap: float = 0.
-0000e690: 312c 0d0a 2020 2020 2020 2020 2020 2020  1,..            
-0000e6a0: 6d61 785f 776f 7264 733a 2069 6e74 203d  max_words: int =
-0000e6b0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-0000e6c0: 2020 2020 6d61 785f 6368 6172 733a 2069      max_chars: i
-0000e6d0: 6e74 203d 204e 6f6e 652c 0d0a 2020 2020  nt = None,..    
-0000e6e0: 2020 2020 2020 2020 6973 5f73 756d 5f6d          is_sum_m
-0000e6f0: 6178 3a20 626f 6f6c 203d 2046 616c 7365  ax: bool = False
-0000e700: 2c0d 0a20 2020 2020 2020 2020 2020 206c  ,..            l
-0000e710: 6f63 6b3a 2062 6f6f 6c20 3d20 4661 6c73  ock: bool = Fals
-0000e720: 650d 0a20 2020 2029 202d 3e20 2257 6869  e..    ) -> "Whi
-0000e730: 7370 6572 5265 7375 6c74 223a 0d0a 2020  sperResult":..  
-0000e740: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-0000e750: 2020 204d 6572 6765 2028 696e 2d70 6c61     Merge (in-pla
-0000e760: 6365 2920 616e 7920 7061 6972 206f 6620  ce) any pair of 
-0000e770: 6164 6a61 6365 6e74 2073 6567 6d65 6e74  adjacent segment
-0000e780: 7320 6966 2074 6865 2067 6170 2062 6574  s if the gap bet
-0000e790: 7765 656e 2074 6865 6d20 3c3d 2060 606d  ween them <= ``m
-0000e7a0: 696e 5f67 6170 6060 2e0d 0a0d 0a20 2020  in_gap``.....   
-0000e7b0: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
-0000e7c0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000e7d0: 2d2d 2d0d 0a20 2020 2020 2020 206d 696e  ---..        min
-0000e7e0: 5f67 6170 203a 2066 6c6f 6174 2c20 6465  _gap : float, de
-0000e7f0: 6661 756c 7420 302e 310d 0a20 2020 2020  fault 0.1..     
-0000e800: 2020 2020 2020 204d 696e 696d 756d 2073         Minimum s
-0000e810: 6563 6f6e 6428 7329 2061 6c6c 6f77 2062  econd(s) allow b
-0000e820: 6574 7765 656e 2074 776f 2073 6567 6d65  etween two segme
-0000e830: 6e74 2e0d 0a20 2020 2020 2020 206d 6178  nt...        max
-0000e840: 5f77 6f72 6473 203a 2069 6e74 2c20 6f70  _words : int, op
-0000e850: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-0000e860: 2020 2020 4d61 7869 6d75 6d20 6e75 6d62      Maximum numb
-0000e870: 6572 206f 6620 776f 7264 7320 616c 6c6f  er of words allo
-0000e880: 7765 6420 696e 2065 6163 6820 7365 676d  wed in each segm
-0000e890: 656e 742e 0d0a 2020 2020 2020 2020 6d61  ent...        ma
-0000e8a0: 785f 6368 6172 7320 3a20 696e 742c 206f  x_chars : int, o
-0000e8b0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-0000e8c0: 2020 2020 204d 6178 696d 756d 206e 756d       Maximum num
-0000e8d0: 6265 7220 6f66 2063 6861 7261 6374 6572  ber of character
-0000e8e0: 7320 616c 6c6f 7765 6420 696e 2065 6163  s allowed in eac
-0000e8f0: 6820 7365 676d 656e 742e 0d0a 2020 2020  h segment...    
-0000e900: 2020 2020 6973 5f73 756d 5f6d 6178 203a      is_sum_max :
-0000e910: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
-0000e920: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
-0000e930: 2020 5768 6574 6865 7220 6060 6d61 785f    Whether ``max_
-0000e940: 776f 7264 7360 6020 616e 6420 6060 6d61  words`` and ``ma
-0000e950: 785f 6368 6172 7360 6020 6973 2061 7070  x_chars`` is app
-0000e960: 6c69 6564 2074 6f20 7468 6520 6d65 7267  lied to the merg
-0000e970: 6564 2073 6567 6d65 6e74 2069 6e73 7465  ed segment inste
-0000e980: 6164 206f 6620 7468 6520 696e 6469 7669  ad of the indivi
-0000e990: 6475 616c 2073 6567 6d65 6e74 730d 0a20  dual segments.. 
-0000e9a0: 2020 2020 2020 2020 2020 2074 6f20 6265             to be
-0000e9b0: 206d 6572 6765 642e 0d0a 2020 2020 2020   merged...      
-0000e9c0: 2020 6c6f 636b 203a 2062 6f6f 6c2c 2064    lock : bool, d
-0000e9d0: 6566 6175 6c74 2046 616c 7365 0d0a 2020  efault False..  
-0000e9e0: 2020 2020 2020 2020 2020 5768 6574 6865            Whethe
-0000e9f0: 7220 746f 2070 7265 7665 6e74 2066 7574  r to prevent fut
-0000ea00: 7572 6520 7370 6c69 7473 2f6d 6572 6765  ure splits/merge
-0000ea10: 7320 6672 6f6d 2061 6c74 6572 696e 6720  s from altering 
-0000ea20: 6368 616e 6765 7320 6d61 6465 2062 7920  changes made by 
-0000ea30: 7468 6973 206d 6574 686f 642e 0d0a 0d0a  this method.....
-0000ea40: 2020 2020 2020 2020 5265 7475 726e 730d          Returns.
-0000ea50: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000ea60: 0d0a 2020 2020 2020 2020 7374 6162 6c65  ..        stable
-0000ea70: 5f77 6869 7370 6572 2e72 6573 756c 742e  _whisper.result.
-0000ea80: 5768 6973 7065 7252 6573 756c 740d 0a20  WhisperResult.. 
-0000ea90: 2020 2020 2020 2020 2020 2054 6865 2063             The c
-0000eaa0: 7572 7265 6e74 2069 6e73 7461 6e63 6520  urrent instance 
-0000eab0: 6166 7465 7220 7468 6520 6368 616e 6765  after the change
-0000eac0: 732e 0d0a 2020 2020 2020 2020 2222 220d  s...        """.
-0000ead0: 0a20 2020 2020 2020 2069 6e64 6963 6573  .        indices
-0000eae0: 203d 2073 656c 662e 6765 745f 6761 705f   = self.get_gap_
-0000eaf0: 696e 6469 6365 7328 6d69 6e5f 6761 7029  indices(min_gap)
-0000eb00: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-0000eb10: 6d65 7267 655f 7365 676d 656e 7473 2869  merge_segments(i
-0000eb20: 6e64 6963 6573 2c0d 0a20 2020 2020 2020  ndices,..       
-0000eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb40: 2020 2020 2020 6d61 785f 776f 7264 733d        max_words=
-0000eb50: 6d61 785f 776f 7264 732c 206d 6178 5f63  max_words, max_c
-0000eb60: 6861 7273 3d6d 6178 5f63 6861 7273 2c20  hars=max_chars, 
-0000eb70: 6973 5f73 756d 5f6d 6178 3d69 735f 7375  is_sum_max=is_su
-0000eb80: 6d5f 6d61 782c 206c 6f63 6b3d 6c6f 636b  m_max, lock=lock
-0000eb90: 290d 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-0000eba0: 6c66 2e5f 7265 6772 6f75 705f 6869 7374  lf._regroup_hist
-0000ebb0: 6f72 793a 0d0a 2020 2020 2020 2020 2020  ory:..          
-0000ebc0: 2020 7365 6c66 2e5f 7265 6772 6f75 705f    self._regroup_
-0000ebd0: 6869 7374 6f72 7920 2b3d 2027 5f27 0d0a  history += '_'..
-0000ebe0: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
-0000ebf0: 6772 6f75 705f 6869 7374 6f72 7920 2b3d  group_history +=
-0000ec00: 2066 276d 673d 7b6d 696e 5f67 6170 7d2b   f'mg={min_gap}+
-0000ec10: 7b6d 6178 5f77 6f72 6473 206f 7220 2222  {max_words or ""
-0000ec20: 7d2b 7b6d 6178 5f63 6861 7273 206f 7220  }+{max_chars or 
-0000ec30: 2222 7d2b 7b69 6e74 2869 735f 7375 6d5f  ""}+{int(is_sum_
-0000ec40: 6d61 7829 7d2b 7b69 6e74 286c 6f63 6b29  max)}+{int(lock)
-0000ec50: 7d27 0d0a 2020 2020 2020 2020 7265 7475  }'..        retu
-0000ec60: 726e 2073 656c 660d 0a0d 0a20 2020 2064  rn self....    d
-0000ec70: 6566 2073 706c 6974 5f62 795f 7075 6e63  ef split_by_punc
-0000ec80: 7475 6174 696f 6e28 0d0a 2020 2020 2020  tuation(..      
-0000ec90: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
-0000eca0: 2020 2020 2020 2020 2070 756e 6374 7561           punctua
-0000ecb0: 7469 6f6e 3a20 556e 696f 6e5b 4c69 7374  tion: Union[List
-0000ecc0: 5b73 7472 5d2c 204c 6973 745b 5475 706c  [str], List[Tupl
-0000ecd0: 655b 7374 722c 2073 7472 5d5d 2c20 7374  e[str, str]], st
-0000ece0: 725d 2c0d 0a20 2020 2020 2020 2020 2020  r],..           
-0000ecf0: 206c 6f63 6b3a 2062 6f6f 6c20 3d20 4661   lock: bool = Fa
-0000ed00: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
-0000ed10: 2020 6e65 776c 696e 653a 2062 6f6f 6c20    newline: bool 
-0000ed20: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
-0000ed30: 2020 2020 2020 6d69 6e5f 776f 7264 733a        min_words:
-0000ed40: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-0000ed50: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-0000ed60: 2020 2020 6d69 6e5f 6368 6172 733a 204f      min_chars: O
-0000ed70: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-0000ed80: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
-0000ed90: 2020 6d69 6e5f 6475 723a 204f 7074 696f    min_dur: Optio
-0000eda0: 6e61 6c5b 696e 745d 203d 204e 6f6e 650d  nal[int] = None.
-0000edb0: 0a20 2020 2029 202d 3e20 2257 6869 7370  .    ) -> "Whisp
-0000edc0: 6572 5265 7375 6c74 223a 0d0a 2020 2020  erResult":..    
-0000edd0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-0000ede0: 2053 706c 6974 2028 696e 2d70 6c61 6365   Split (in-place
-0000edf0: 2920 7365 676d 656e 7473 2061 7420 776f  ) segments at wo
-0000ee00: 7264 7320 7468 6174 2073 7461 7274 2f65  rds that start/e
-0000ee10: 6e64 2077 6974 6820 6060 7075 6e63 7475  nd with ``punctu
-0000ee20: 6174 696f 6e60 602e 0d0a 0d0a 2020 2020  ation``.....    
-0000ee30: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
-0000ee40: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-0000ee50: 2d2d 0d0a 2020 2020 2020 2020 7075 6e63  --..        punc
-0000ee60: 7475 6174 696f 6e20 3a20 6c69 7374 206f  tuation : list o
-0000ee70: 6620 7374 7220 6f66 206c 6973 7420 6f66  f str of list of
-0000ee80: 2074 7570 6c65 206f 6620 2873 7472 2c20   tuple of (str, 
-0000ee90: 7374 7229 206f 7220 7374 720d 0a20 2020  str) or str..   
-0000eea0: 2020 2020 2020 2020 2050 756e 6374 7561           Punctua
-0000eeb0: 7469 6f6e 2873 2920 746f 2073 706c 6974  tion(s) to split
-0000eec0: 2073 6567 6d65 6e74 7320 6279 2e0d 0a20   segments by... 
-0000eed0: 2020 2020 2020 206c 6f63 6b20 3a20 626f         lock : bo
-0000eee0: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
-0000eef0: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
-0000ef00: 6865 7468 6572 2074 6f20 7072 6576 656e  hether to preven
-0000ef10: 7420 6675 7475 7265 2073 706c 6974 732f  t future splits/
-0000ef20: 6d65 7267 6573 2066 726f 6d20 616c 7465  merges from alte
-0000ef30: 7269 6e67 2063 6861 6e67 6573 206d 6164  ring changes mad
-0000ef40: 6520 6279 2074 6869 7320 6d65 7468 6f64  e by this method
-0000ef50: 2e0d 0a20 2020 2020 2020 206e 6577 6c69  ...        newli
-0000ef60: 6e65 203a 2062 6f6f 6c2c 2064 6566 6175  ne : bool, defau
-0000ef70: 6c74 2046 616c 7365 0d0a 2020 2020 2020  lt False..      
-0000ef80: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
-0000ef90: 2069 6e73 6572 7420 6c69 6e65 2062 7265   insert line bre
-0000efa0: 616b 2061 7420 7468 6520 7370 6c69 7420  ak at the split 
-0000efb0: 706f 696e 7473 2069 6e73 7465 6164 206f  points instead o
-0000efc0: 6620 7370 6c69 7474 696e 6720 696e 746f  f splitting into
-0000efd0: 2073 6570 6172 6174 6520 7365 676d 656e   separate segmen
-0000efe0: 7473 2e0d 0a20 2020 2020 2020 206d 696e  ts...        min
-0000eff0: 5f77 6f72 6473 203a 2069 6e74 2c20 6f70  _words : int, op
-0000f000: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-0000f010: 2020 2020 5370 6c69 7420 7365 676d 656e      Split segmen
-0000f020: 7473 2077 6974 6820 776f 7264 7320 3e3d  ts with words >=
-0000f030: 2060 606d 696e 5f77 6f72 6473 6060 2e0d   ``min_words``..
-0000f040: 0a20 2020 2020 2020 206d 696e 5f63 6861  .        min_cha
-0000f050: 7273 203a 2069 6e74 2c20 6f70 7469 6f6e  rs : int, option
-0000f060: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
-0000f070: 5370 6c69 7420 7365 676d 656e 7473 2077  Split segments w
-0000f080: 6974 6820 6368 6172 6163 7465 7273 203e  ith characters >
-0000f090: 3d20 6060 6d69 6e5f 6368 6172 7360 602e  = ``min_chars``.
-0000f0a0: 0d0a 2020 2020 2020 2020 6d69 6e5f 6475  ..        min_du
-0000f0b0: 7220 3a20 696e 742c 206f 7074 696f 6e61  r : int, optiona
-0000f0c0: 6c0d 0a20 2020 2020 2020 2020 2020 2073  l..            s
-0000f0d0: 706c 6974 2073 6567 6d65 6e74 7320 7769  plit segments wi
-0000f0e0: 7468 2064 7572 6174 696f 6e20 2869 6e20  th duration (in 
-0000f0f0: 7365 636f 6e64 7329 203e 3d20 6060 6d69  seconds) >= ``mi
-0000f100: 6e5f 6475 7260 602e 0d0a 0d0a 2020 2020  n_dur``.....    
-0000f110: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
-0000f120: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
-0000f130: 2020 2020 2020 7374 6162 6c65 5f77 6869        stable_whi
-0000f140: 7370 6572 2e72 6573 756c 742e 5768 6973  sper.result.Whis
-0000f150: 7065 7252 6573 756c 740d 0a20 2020 2020  perResult..     
-0000f160: 2020 2020 2020 2054 6865 2063 7572 7265         The curre
-0000f170: 6e74 2069 6e73 7461 6e63 6520 6166 7465  nt instance afte
-0000f180: 7220 7468 6520 6368 616e 6765 732e 0d0a  r the changes...
-0000f190: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-0000f1a0: 2020 2020 2064 6566 205f 6f76 6572 5f6d       def _over_m
-0000f1b0: 6178 2878 3a20 5365 676d 656e 7429 3a0d  ax(x: Segment):.
-0000f1c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000f1d0: 7572 6e20 280d 0a20 2020 2020 2020 2020  urn (..         
-0000f1e0: 2020 2020 2020 2020 2020 2028 6d69 6e5f             (min_
-0000f1f0: 776f 7264 7320 616e 6420 6c65 6e28 782e  words and len(x.
-0000f200: 776f 7264 7329 203e 3d20 6d69 6e5f 776f  words) >= min_wo
-0000f210: 7264 7329 206f 720d 0a20 2020 2020 2020  rds) or..       
-0000f220: 2020 2020 2020 2020 2020 2020 2028 6d69               (mi
-0000f230: 6e5f 6368 6172 7320 616e 6420 782e 6368  n_chars and x.ch
-0000f240: 6172 5f63 6f75 6e74 2829 203e 3d20 6d69  ar_count() >= mi
-0000f250: 6e5f 6368 6172 7329 206f 720d 0a20 2020  n_chars) or..   
-0000f260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f270: 2028 6d69 6e5f 6475 7220 616e 6420 782e   (min_dur and x.
-0000f280: 6475 7261 7469 6f6e 203e 3d20 6d69 6e5f  duration >= min_
-0000f290: 6475 7229 0d0a 2020 2020 2020 2020 2020  dur)..          
-0000f2a0: 2020 290d 0a0d 0a20 2020 2020 2020 2069    )....        i
-0000f2b0: 6e64 6963 6573 203d 2073 6574 2873 2e69  ndices = set(s.i
-0000f2c0: 6420 666f 7220 7320 696e 2073 656c 662e  d for s in self.
-0000f2d0: 7365 676d 656e 7473 2069 6620 5f6f 7665  segments if _ove
-0000f2e0: 725f 6d61 7828 7329 2920 6966 2061 6e79  r_max(s)) if any
-0000f2f0: 2828 6d69 6e5f 776f 7264 732c 206d 696e  ((min_words, min
-0000f300: 5f63 6861 7273 2c20 6d69 6e5f 6475 7229  _chars, min_dur)
-0000f310: 2920 656c 7365 204e 6f6e 650d 0a0d 0a20  ) else None.... 
-0000f320: 2020 2020 2020 2064 6566 205f 6765 745f         def _get_
-0000f330: 696e 6469 6365 7328 783a 2053 6567 6d65  indices(x: Segme
-0000f340: 6e74 293a 0d0a 2020 2020 2020 2020 2020  nt):..          
-0000f350: 2020 7265 7475 726e 2078 2e67 6574 5f70    return x.get_p
-0000f360: 756e 6374 7561 7469 6f6e 5f69 6e64 6963  unctuation_indic
-0000f370: 6573 2870 756e 6374 7561 7469 6f6e 2920  es(punctuation) 
-0000f380: 6966 2069 6e64 6963 6573 2069 7320 4e6f  if indices is No
-0000f390: 6e65 206f 7220 782e 6964 2069 6e20 696e  ne or x.id in in
-0000f3a0: 6469 6365 7320 656c 7365 205b 5d0d 0a0d  dices else []...
-0000f3b0: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
-0000f3c0: 706c 6974 5f73 6567 6d65 6e74 7328 5f67  plit_segments(_g
-0000f3d0: 6574 5f69 6e64 6963 6573 2c20 6c6f 636b  et_indices, lock
-0000f3e0: 3d6c 6f63 6b2c 206e 6577 6c69 6e65 3d6e  =lock, newline=n
-0000f3f0: 6577 6c69 6e65 290d 0a20 2020 2020 2020  ewline)..       
-0000f400: 2069 6620 7365 6c66 2e5f 7265 6772 6f75   if self._regrou
-0000f410: 705f 6869 7374 6f72 793a 0d0a 2020 2020  p_history:..    
-0000f420: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
-0000f430: 6772 6f75 705f 6869 7374 6f72 7920 2b3d  group_history +=
-0000f440: 2027 5f27 0d0a 2020 2020 2020 2020 7075   '_'..        pu
-0000f450: 6e63 745f 7374 7220 3d20 272f 272e 6a6f  nct_str = '/'.jo
-0000f460: 696e 2870 2069 6620 6973 696e 7374 616e  in(p if isinstan
-0000f470: 6365 2870 2c20 7374 7229 2065 6c73 6520  ce(p, str) else 
-0000f480: 272a 272e 6a6f 696e 2870 2920 666f 7220  '*'.join(p) for 
-0000f490: 7020 696e 2070 756e 6374 7561 7469 6f6e  p in punctuation
-0000f4a0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0000f4b0: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
-0000f4c0: 202b 3d20 6627 7370 3d7b 7075 6e63 745f   += f'sp={punct_
-0000f4d0: 7374 727d 2b7b 696e 7428 6c6f 636b 297d  str}+{int(lock)}
-0000f4e0: 2b7b 696e 7428 6e65 776c 696e 6529 7d27  +{int(newline)}'
-0000f4f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-0000f500: 7265 6772 6f75 705f 6869 7374 6f72 7920  regroup_history 
-0000f510: 2b3d 2066 272b 7b6d 696e 5f77 6f72 6473  += f'+{min_words
-0000f520: 206f 7220 2222 7d2b 7b6d 696e 5f63 6861   or ""}+{min_cha
-0000f530: 7273 206f 7220 2222 7d2b 7b6d 696e 5f64  rs or ""}+{min_d
-0000f540: 7572 206f 7220 2222 7d27 2e72 7374 7269  ur or ""}'.rstri
-0000f550: 7028 272b 2729 0d0a 2020 2020 2020 2020  p('+')..        
-0000f560: 7265 7475 726e 2073 656c 660d 0a0d 0a20  return self.... 
-0000f570: 2020 2064 6566 206d 6572 6765 5f62 795f     def merge_by_
-0000f580: 7075 6e63 7475 6174 696f 6e28 0d0a 2020  punctuation(..  
-0000f590: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
-0000f5a0: 0a20 2020 2020 2020 2020 2020 2070 756e  .            pun
-0000f5b0: 6374 7561 7469 6f6e 3a20 556e 696f 6e5b  ctuation: Union[
-0000f5c0: 4c69 7374 5b73 7472 5d2c 204c 6973 745b  List[str], List[
-0000f5d0: 5475 706c 655b 7374 722c 2073 7472 5d5d  Tuple[str, str]]
-0000f5e0: 2c20 7374 725d 2c0d 0a20 2020 2020 2020  , str],..       
-0000f5f0: 2020 2020 206d 6178 5f77 6f72 6473 3a20       max_words: 
-0000f600: 696e 7420 3d20 4e6f 6e65 2c0d 0a20 2020  int = None,..   
-0000f610: 2020 2020 2020 2020 206d 6178 5f63 6861           max_cha
-0000f620: 7273 3a20 696e 7420 3d20 4e6f 6e65 2c0d  rs: int = None,.
-0000f630: 0a20 2020 2020 2020 2020 2020 2069 735f  .            is_
-0000f640: 7375 6d5f 6d61 783a 2062 6f6f 6c20 3d20  sum_max: bool = 
-0000f650: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-0000f660: 2020 2020 6c6f 636b 3a20 626f 6f6c 203d      lock: bool =
-0000f670: 2046 616c 7365 0d0a 2020 2020 2920 2d3e   False..    ) ->
-0000f680: 2022 5768 6973 7065 7252 6573 756c 7422   "WhisperResult"
-0000f690: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-0000f6a0: 2020 2020 2020 2020 4d65 7267 6520 2869          Merge (i
-0000f6b0: 6e2d 706c 6163 6529 2061 6e79 2074 776f  n-place) any two
-0000f6c0: 2073 6567 6d65 6e74 7320 7468 6174 2068   segments that h
-0000f6d0: 6173 2073 7065 6369 6669 6320 7075 6e63  as specific punc
-0000f6e0: 7475 6174 696f 6e73 2069 6e62 6574 7765  tuations inbetwe
-0000f6f0: 656e 2e0d 0a0d 0a20 2020 2020 2020 2050  en.....        P
-0000f700: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
-0000f710: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-0000f720: 2020 2020 2020 2070 756e 6374 7561 7469         punctuati
-0000f730: 6f6e 203a 206c 6973 7420 6f66 2073 7472  on : list of str
-0000f740: 206f 6620 6c69 7374 206f 6620 7475 706c   of list of tupl
-0000f750: 6520 6f66 2028 7374 722c 2073 7472 2920  e of (str, str) 
-0000f760: 6f72 2073 7472 0d0a 2020 2020 2020 2020  or str..        
-0000f770: 2020 2020 5075 6e63 7475 6174 696f 6e28      Punctuation(
-0000f780: 7329 2074 6f20 6d65 7267 6520 7365 676d  s) to merge segm
-0000f790: 656e 7473 2062 792e 0d0a 2020 2020 2020  ents by...      
-0000f7a0: 2020 6d61 785f 776f 7264 7320 3a20 696e    max_words : in
-0000f7b0: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
-0000f7c0: 2020 2020 2020 2020 204d 6178 696d 756d           Maximum
-0000f7d0: 206e 756d 6265 7220 6f66 2077 6f72 6473   number of words
-0000f7e0: 2061 6c6c 6f77 6564 2069 6e20 6561 6368   allowed in each
-0000f7f0: 2073 6567 6d65 6e74 2e0d 0a20 2020 2020   segment...     
-0000f800: 2020 206d 6178 5f63 6861 7273 203a 2069     max_chars : i
-0000f810: 6e74 2c20 6f70 7469 6f6e 616c 0d0a 2020  nt, optional..  
-0000f820: 2020 2020 2020 2020 2020 4d61 7869 6d75            Maximu
-0000f830: 6d20 6e75 6d62 6572 206f 6620 6368 6172  m number of char
-0000f840: 6163 7465 7273 2061 6c6c 6f77 6564 2069  acters allowed i
-0000f850: 6e20 6561 6368 2073 6567 6d65 6e74 2e0d  n each segment..
-0000f860: 0a20 2020 2020 2020 2069 735f 7375 6d5f  .        is_sum_
-0000f870: 6d61 7820 3a20 626f 6f6c 2c20 6465 6661  max : bool, defa
-0000f880: 756c 7420 4661 6c73 650d 0a20 2020 2020  ult False..     
-0000f890: 2020 2020 2020 2057 6865 7468 6572 2060         Whether `
-0000f8a0: 606d 6178 5f77 6f72 6473 6060 2061 6e64  `max_words`` and
-0000f8b0: 2060 606d 6178 5f63 6861 7273 6060 2069   ``max_chars`` i
-0000f8c0: 7320 6170 706c 6965 6420 746f 2074 6865  s applied to the
-0000f8d0: 206d 6572 6765 6420 7365 676d 656e 7420   merged segment 
-0000f8e0: 696e 7374 6561 6420 6f66 2074 6865 2069  instead of the i
-0000f8f0: 6e64 6976 6964 7561 6c20 7365 676d 656e  ndividual segmen
-0000f900: 7473 0d0a 2020 2020 2020 2020 2020 2020  ts..            
-0000f910: 746f 2062 6520 6d65 7267 6564 2e0d 0a20  to be merged... 
-0000f920: 2020 2020 2020 206c 6f63 6b20 3a20 626f         lock : bo
-0000f930: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
-0000f940: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
-0000f950: 6865 7468 6572 2074 6f20 7072 6576 656e  hether to preven
-0000f960: 7420 6675 7475 7265 2073 706c 6974 732f  t future splits/
-0000f970: 6d65 7267 6573 2066 726f 6d20 616c 7465  merges from alte
-0000f980: 7269 6e67 2063 6861 6e67 6573 206d 6164  ring changes mad
-0000f990: 6520 6279 2074 6869 7320 6d65 7468 6f64  e by this method
-0000f9a0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
-0000f9b0: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
-0000f9c0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
-0000f9d0: 7461 626c 655f 7768 6973 7065 722e 7265  table_whisper.re
-0000f9e0: 7375 6c74 2e57 6869 7370 6572 5265 7375  sult.WhisperResu
-0000f9f0: 6c74 0d0a 2020 2020 2020 2020 2020 2020  lt..            
-0000fa00: 5468 6520 6375 7272 656e 7420 696e 7374  The current inst
-0000fa10: 616e 6365 2061 6674 6572 2074 6865 2063  ance after the c
-0000fa20: 6861 6e67 6573 2e0d 0a20 2020 2020 2020  hanges...       
-0000fa30: 2022 2222 0d0a 2020 2020 2020 2020 696e   """..        in
-0000fa40: 6469 6365 7320 3d20 7365 6c66 2e67 6574  dices = self.get
-0000fa50: 5f70 756e 6374 7561 7469 6f6e 5f69 6e64  _punctuation_ind
-0000fa60: 6963 6573 2870 756e 6374 7561 7469 6f6e  ices(punctuation
-0000fa70: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0000fa80: 5f6d 6572 6765 5f73 6567 6d65 6e74 7328  _merge_segments(
-0000fa90: 696e 6469 6365 732c 0d0a 2020 2020 2020  indices,..      
-0000faa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fab0: 2020 2020 2020 206d 6178 5f77 6f72 6473         max_words
-0000fac0: 3d6d 6178 5f77 6f72 6473 2c20 6d61 785f  =max_words, max_
-0000fad0: 6368 6172 733d 6d61 785f 6368 6172 732c  chars=max_chars,
-0000fae0: 2069 735f 7375 6d5f 6d61 783d 6973 5f73   is_sum_max=is_s
-0000faf0: 756d 5f6d 6178 2c20 6c6f 636b 3d6c 6f63  um_max, lock=loc
-0000fb00: 6b29 0d0a 2020 2020 2020 2020 6966 2073  k)..        if s
-0000fb10: 656c 662e 5f72 6567 726f 7570 5f68 6973  elf._regroup_his
-0000fb20: 746f 7279 3a0d 0a20 2020 2020 2020 2020  tory:..         
-0000fb30: 2020 2073 656c 662e 5f72 6567 726f 7570     self._regroup
-0000fb40: 5f68 6973 746f 7279 202b 3d20 275f 270d  _history += '_'.
-0000fb50: 0a20 2020 2020 2020 2070 756e 6374 5f73  .        punct_s
-0000fb60: 7472 203d 2027 2f27 2e6a 6f69 6e28 7020  tr = '/'.join(p 
-0000fb70: 6966 2069 7369 6e73 7461 6e63 6528 702c  if isinstance(p,
-0000fb80: 2073 7472 2920 656c 7365 2027 2a27 2e6a   str) else '*'.j
-0000fb90: 6f69 6e28 7029 2066 6f72 2070 2069 6e20  oin(p) for p in 
-0000fba0: 7075 6e63 7475 6174 696f 6e29 0d0a 2020  punctuation)..  
-0000fbb0: 2020 2020 2020 7365 6c66 2e5f 7265 6772        self._regr
-0000fbc0: 6f75 705f 6869 7374 6f72 7920 2b3d 2066  oup_history += f
-0000fbd0: 276d 703d 7b70 756e 6374 5f73 7472 7d2b  'mp={punct_str}+
-0000fbe0: 7b6d 6178 5f77 6f72 6473 206f 7220 2222  {max_words or ""
-0000fbf0: 7d2b 7b6d 6178 5f63 6861 7273 206f 7220  }+{max_chars or 
-0000fc00: 2222 7d2b 7b69 6e74 2869 735f 7375 6d5f  ""}+{int(is_sum_
-0000fc10: 6d61 7829 7d2b 7b69 6e74 286c 6f63 6b29  max)}+{int(lock)
-0000fc20: 7d27 0d0a 2020 2020 2020 2020 7265 7475  }'..        retu
-0000fc30: 726e 2073 656c 660d 0a0d 0a20 2020 2064  rn self....    d
-0000fc40: 6566 206d 6572 6765 5f61 6c6c 5f73 6567  ef merge_all_seg
-0000fc50: 6d65 6e74 7328 7365 6c66 2920 2d3e 2022  ments(self) -> "
-0000fc60: 5768 6973 7065 7252 6573 756c 7422 3a0d  WhisperResult":.
-0000fc70: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0000fc80: 2020 2020 2020 4d65 7267 6520 616c 6c20        Merge all 
-0000fc90: 7365 676d 656e 7473 2069 6e74 6f20 6f6e  segments into on
-0000fca0: 6520 7365 676d 656e 742e 0d0a 0d0a 2020  e segment.....  
-0000fcb0: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
-0000fcc0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
-0000fcd0: 2020 2020 2020 2020 7374 6162 6c65 5f77          stable_w
-0000fce0: 6869 7370 6572 2e72 6573 756c 742e 5768  hisper.result.Wh
-0000fcf0: 6973 7065 7252 6573 756c 740d 0a20 2020  isperResult..   
-0000fd00: 2020 2020 2020 2020 2054 6865 2063 7572           The cur
-0000fd10: 7265 6e74 2069 6e73 7461 6e63 6520 6166  rent instance af
-0000fd20: 7465 7220 7468 6520 6368 616e 6765 732e  ter the changes.
-0000fd30: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-0000fd40: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-0000fd50: 6c66 2e73 6567 6d65 6e74 733a 0d0a 2020  lf.segments:..  
-0000fd60: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000fd70: 2073 656c 660d 0a20 2020 2020 2020 2069   self..        i
-0000fd80: 6620 7365 6c66 2e68 6173 5f77 6f72 6473  f self.has_words
-0000fd90: 3a0d 0a20 2020 2020 2020 2020 2020 206e  :..            n
-0000fda0: 6577 5f73 6567 203d 2073 656c 662e 7365  ew_seg = self.se
-0000fdb0: 676d 656e 7473 5b30 5d2e 636f 7079 2873  gments[0].copy(s
-0000fdc0: 656c 662e 616c 6c5f 776f 7264 7328 292c  elf.all_words(),
-0000fdd0: 206b 6565 705f 7265 7375 6c74 3d54 7275   keep_result=Tru
-0000fde0: 652c 2063 6f70 795f 776f 7264 733d 4661  e, copy_words=Fa
-0000fdf0: 6c73 6529 0d0a 2020 2020 2020 2020 656c  lse)..        el
-0000fe00: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0000fe10: 206e 6577 5f73 6567 203d 2073 656c 662e   new_seg = self.
-0000fe20: 7365 676d 656e 7473 5b30 5d0d 0a20 2020  segments[0]..   
-0000fe30: 2020 2020 2020 2020 206e 6577 5f73 6567           new_seg
-0000fe40: 2e5f 6465 6661 756c 745f 7465 7874 202b  ._default_text +
-0000fe50: 3d20 2727 2e6a 6f69 6e28 732e 7465 7874  = ''.join(s.text
-0000fe60: 2066 6f72 2073 2069 6e20 7365 6c66 2e73   for s in self.s
-0000fe70: 6567 6d65 6e74 735b 313a 5d29 0d0a 2020  egments[1:])..  
-0000fe80: 2020 2020 2020 2020 2020 6966 2061 6c6c            if all
-0000fe90: 2873 2e74 6f6b 656e 7320 6973 206e 6f74  (s.tokens is not
-0000fea0: 204e 6f6e 6520 666f 7220 7320 696e 2073   None for s in s
-0000feb0: 656c 662e 7365 676d 656e 7473 293a 0d0a  elf.segments):..
-0000fec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fed0: 6e65 775f 7365 672e 5f64 6566 6175 6c74  new_seg._default
-0000fee0: 5f74 6f6b 656e 7320 2b3d 206c 6973 7428  _tokens += list(
-0000fef0: 6368 6169 6e2e 6672 6f6d 5f69 7465 7261  chain.from_itera
-0000ff00: 626c 6528 732e 746f 6b65 6e73 2066 6f72  ble(s.tokens for
-0000ff10: 2073 2069 6e20 7365 6c66 2e73 6567 6d65   s in self.segme
-0000ff20: 6e74 735b 313a 5d29 290d 0a20 2020 2020  nts[1:]))..     
-0000ff30: 2020 2020 2020 206e 6577 5f73 6567 2e65         new_seg.e
-0000ff40: 6e64 203d 2073 656c 662e 7365 676d 656e  nd = self.segmen
-0000ff50: 7473 5b2d 315d 2e65 6e64 0d0a 2020 2020  ts[-1].end..    
-0000ff60: 2020 2020 7365 6c66 2e73 6567 6d65 6e74      self.segment
-0000ff70: 7320 3d20 5b6e 6577 5f73 6567 5d0d 0a20  s = [new_seg].. 
-0000ff80: 2020 2020 2020 2073 656c 662e 7265 6173         self.reas
-0000ff90: 7369 676e 5f69 6473 2829 0d0a 2020 2020  sign_ids()..    
-0000ffa0: 2020 2020 6966 2073 656c 662e 5f72 6567      if self._reg
-0000ffb0: 726f 7570 5f68 6973 746f 7279 3a0d 0a20  roup_history:.. 
-0000ffc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ffd0: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
-0000ffe0: 202b 3d20 275f 270d 0a20 2020 2020 2020   += '_'..       
+0000e600: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+0000e610: 656c 662e 5f72 6567 726f 7570 5f68 6973  elf._regroup_his
+0000e620: 746f 7279 202b 3d20 275f 270d 0a20 2020  tory += '_'..   
+0000e630: 2020 2020 2073 656c 662e 5f72 6567 726f       self._regro
+0000e640: 7570 5f68 6973 746f 7279 202b 3d20 6627  up_history += f'
+0000e650: 7367 3d7b 6d61 785f 6761 707d 2b7b 696e  sg={max_gap}+{in
+0000e660: 7428 6c6f 636b 297d 2b7b 696e 7428 6e65  t(lock)}+{int(ne
+0000e670: 776c 696e 6529 7d27 0d0a 2020 2020 2020  wline)}'..      
+0000e680: 2020 7265 7475 726e 2073 656c 660d 0a0d    return self...
+0000e690: 0a20 2020 2064 6566 206d 6572 6765 5f62  .    def merge_b
+0000e6a0: 795f 6761 7028 0d0a 2020 2020 2020 2020  y_gap(..        
+0000e6b0: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
+0000e6c0: 2020 2020 2020 206d 696e 5f67 6170 3a20         min_gap: 
+0000e6d0: 666c 6f61 7420 3d20 302e 312c 0d0a 2020  float = 0.1,..  
+0000e6e0: 2020 2020 2020 2020 2020 6d61 785f 776f            max_wo
+0000e6f0: 7264 733a 2069 6e74 203d 204e 6f6e 652c  rds: int = None,
+0000e700: 0d0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
+0000e710: 785f 6368 6172 733a 2069 6e74 203d 204e  x_chars: int = N
+0000e720: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+0000e730: 2020 6973 5f73 756d 5f6d 6178 3a20 626f    is_sum_max: bo
+0000e740: 6f6c 203d 2046 616c 7365 2c0d 0a20 2020  ol = False,..   
+0000e750: 2020 2020 2020 2020 206c 6f63 6b3a 2062           lock: b
+0000e760: 6f6f 6c20 3d20 4661 6c73 650d 0a20 2020  ool = False..   
+0000e770: 2029 202d 3e20 2257 6869 7370 6572 5265   ) -> "WhisperRe
+0000e780: 7375 6c74 223a 0d0a 2020 2020 2020 2020  sult":..        
+0000e790: 2222 220d 0a20 2020 2020 2020 204d 6572  """..        Mer
+0000e7a0: 6765 2028 696e 2d70 6c61 6365 2920 616e  ge (in-place) an
+0000e7b0: 7920 7061 6972 206f 6620 6164 6a61 6365  y pair of adjace
+0000e7c0: 6e74 2073 6567 6d65 6e74 7320 6966 2074  nt segments if t
+0000e7d0: 6865 2067 6170 2062 6574 7765 656e 2074  he gap between t
+0000e7e0: 6865 6d20 3c3d 2060 606d 696e 5f67 6170  hem <= ``min_gap
+0000e7f0: 6060 2e0d 0a0d 0a20 2020 2020 2020 2050  ``.....        P
+0000e800: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
+0000e810: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
+0000e820: 2020 2020 2020 206d 696e 5f67 6170 203a         min_gap :
+0000e830: 2066 6c6f 6174 2c20 6465 6661 756c 7420   float, default 
+0000e840: 302e 310d 0a20 2020 2020 2020 2020 2020  0.1..           
+0000e850: 204d 696e 696d 756d 2073 6563 6f6e 6428   Minimum second(
+0000e860: 7329 2061 6c6c 6f77 2062 6574 7765 656e  s) allow between
+0000e870: 2074 776f 2073 6567 6d65 6e74 2e0d 0a20   two segment... 
+0000e880: 2020 2020 2020 206d 6178 5f77 6f72 6473         max_words
+0000e890: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
+0000e8a0: 0d0a 2020 2020 2020 2020 2020 2020 4d61  ..            Ma
+0000e8b0: 7869 6d75 6d20 6e75 6d62 6572 206f 6620  ximum number of 
+0000e8c0: 776f 7264 7320 616c 6c6f 7765 6420 696e  words allowed in
+0000e8d0: 2065 6163 6820 7365 676d 656e 742e 0d0a   each segment...
+0000e8e0: 2020 2020 2020 2020 6d61 785f 6368 6172          max_char
+0000e8f0: 7320 3a20 696e 742c 206f 7074 696f 6e61  s : int, optiona
+0000e900: 6c0d 0a20 2020 2020 2020 2020 2020 204d  l..            M
+0000e910: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
+0000e920: 2063 6861 7261 6374 6572 7320 616c 6c6f   characters allo
+0000e930: 7765 6420 696e 2065 6163 6820 7365 676d  wed in each segm
+0000e940: 656e 742e 0d0a 2020 2020 2020 2020 6973  ent...        is
+0000e950: 5f73 756d 5f6d 6178 203a 2062 6f6f 6c2c  _sum_max : bool,
+0000e960: 2064 6566 6175 6c74 2046 616c 7365 0d0a   default False..
+0000e970: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
+0000e980: 6865 7220 6060 6d61 785f 776f 7264 7360  her ``max_words`
+0000e990: 6020 616e 6420 6060 6d61 785f 6368 6172  ` and ``max_char
+0000e9a0: 7360 6020 6973 2061 7070 6c69 6564 2074  s`` is applied t
+0000e9b0: 6f20 7468 6520 6d65 7267 6564 2073 6567  o the merged seg
+0000e9c0: 6d65 6e74 2069 6e73 7465 6164 206f 6620  ment instead of 
+0000e9d0: 7468 6520 696e 6469 7669 6475 616c 2073  the individual s
+0000e9e0: 6567 6d65 6e74 730d 0a20 2020 2020 2020  egments..       
+0000e9f0: 2020 2020 2074 6f20 6265 206d 6572 6765       to be merge
+0000ea00: 642e 0d0a 2020 2020 2020 2020 6c6f 636b  d...        lock
+0000ea10: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+0000ea20: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+0000ea30: 2020 2020 5768 6574 6865 7220 746f 2070      Whether to p
+0000ea40: 7265 7665 6e74 2066 7574 7572 6520 7370  revent future sp
+0000ea50: 6c69 7473 2f6d 6572 6765 7320 6672 6f6d  lits/merges from
+0000ea60: 2061 6c74 6572 696e 6720 6368 616e 6765   altering change
+0000ea70: 7320 6d61 6465 2062 7920 7468 6973 206d  s made by this m
+0000ea80: 6574 686f 642e 0d0a 0d0a 2020 2020 2020  ethod.....      
+0000ea90: 2020 5265 7475 726e 730d 0a20 2020 2020    Returns..     
+0000eaa0: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
+0000eab0: 2020 2020 7374 6162 6c65 5f77 6869 7370      stable_whisp
+0000eac0: 6572 2e72 6573 756c 742e 5768 6973 7065  er.result.Whispe
+0000ead0: 7252 6573 756c 740d 0a20 2020 2020 2020  rResult..       
+0000eae0: 2020 2020 2054 6865 2063 7572 7265 6e74       The current
+0000eaf0: 2069 6e73 7461 6e63 6520 6166 7465 7220   instance after 
+0000eb00: 7468 6520 6368 616e 6765 732e 0d0a 2020  the changes...  
+0000eb10: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0000eb20: 2020 2069 6e64 6963 6573 203d 2073 656c     indices = sel
+0000eb30: 662e 6765 745f 6761 705f 696e 6469 6365  f.get_gap_indice
+0000eb40: 7328 6d69 6e5f 6761 7029 0d0a 2020 2020  s(min_gap)..    
+0000eb50: 2020 2020 7365 6c66 2e5f 6d65 7267 655f      self._merge_
+0000eb60: 7365 676d 656e 7473 2869 6e64 6963 6573  segments(indices
+0000eb70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000eb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb90: 6d61 785f 776f 7264 733d 6d61 785f 776f  max_words=max_wo
+0000eba0: 7264 732c 206d 6178 5f63 6861 7273 3d6d  rds, max_chars=m
+0000ebb0: 6178 5f63 6861 7273 2c20 6973 5f73 756d  ax_chars, is_sum
+0000ebc0: 5f6d 6178 3d69 735f 7375 6d5f 6d61 782c  _max=is_sum_max,
+0000ebd0: 206c 6f63 6b3d 6c6f 636b 290d 0a20 2020   lock=lock)..   
+0000ebe0: 2020 2020 2069 6620 7365 6c66 2e5f 7265       if self._re
+0000ebf0: 6772 6f75 705f 6869 7374 6f72 793a 0d0a  group_history:..
+0000ec00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ec10: 2e5f 7265 6772 6f75 705f 6869 7374 6f72  ._regroup_histor
+0000ec20: 7920 2b3d 2027 5f27 0d0a 2020 2020 2020  y += '_'..      
+0000ec30: 2020 7365 6c66 2e5f 7265 6772 6f75 705f    self._regroup_
+0000ec40: 6869 7374 6f72 7920 2b3d 2066 276d 673d  history += f'mg=
+0000ec50: 7b6d 696e 5f67 6170 7d2b 7b6d 6178 5f77  {min_gap}+{max_w
+0000ec60: 6f72 6473 206f 7220 2222 7d2b 7b6d 6178  ords or ""}+{max
+0000ec70: 5f63 6861 7273 206f 7220 2222 7d2b 7b69  _chars or ""}+{i
+0000ec80: 6e74 2869 735f 7375 6d5f 6d61 7829 7d2b  nt(is_sum_max)}+
+0000ec90: 7b69 6e74 286c 6f63 6b29 7d27 0d0a 2020  {int(lock)}'..  
+0000eca0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000ecb0: 660d 0a0d 0a20 2020 2064 6566 2073 706c  f....    def spl
+0000ecc0: 6974 5f62 795f 7075 6e63 7475 6174 696f  it_by_punctuatio
+0000ecd0: 6e28 0d0a 2020 2020 2020 2020 2020 2020  n(..            
+0000ece0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+0000ecf0: 2020 2070 756e 6374 7561 7469 6f6e 3a20     punctuation: 
+0000ed00: 556e 696f 6e5b 4c69 7374 5b73 7472 5d2c  Union[List[str],
+0000ed10: 204c 6973 745b 5475 706c 655b 7374 722c   List[Tuple[str,
+0000ed20: 2073 7472 5d5d 2c20 7374 725d 2c0d 0a20   str]], str],.. 
+0000ed30: 2020 2020 2020 2020 2020 206c 6f63 6b3a             lock:
+0000ed40: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
+0000ed50: 2020 2020 2020 2020 2020 2020 6e65 776c              newl
+0000ed60: 696e 653a 2062 6f6f 6c20 3d20 4661 6c73  ine: bool = Fals
+0000ed70: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+0000ed80: 6d69 6e5f 776f 7264 733a 204f 7074 696f  min_words: Optio
+0000ed90: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
+0000eda0: 0d0a 2020 2020 2020 2020 2020 2020 6d69  ..            mi
+0000edb0: 6e5f 6368 6172 733a 204f 7074 696f 6e61  n_chars: Optiona
+0000edc0: 6c5b 696e 745d 203d 204e 6f6e 652c 0d0a  l[int] = None,..
+0000edd0: 2020 2020 2020 2020 2020 2020 6d69 6e5f              min_
+0000ede0: 6475 723a 204f 7074 696f 6e61 6c5b 696e  dur: Optional[in
+0000edf0: 745d 203d 204e 6f6e 650d 0a20 2020 2029  t] = None..    )
+0000ee00: 202d 3e20 2257 6869 7370 6572 5265 7375   -> "WhisperResu
+0000ee10: 6c74 223a 0d0a 2020 2020 2020 2020 2222  lt":..        ""
+0000ee20: 220d 0a20 2020 2020 2020 2053 706c 6974  "..        Split
+0000ee30: 2028 696e 2d70 6c61 6365 2920 7365 676d   (in-place) segm
+0000ee40: 656e 7473 2061 7420 776f 7264 7320 7468  ents at words th
+0000ee50: 6174 2073 7461 7274 2f65 6e64 2077 6974  at start/end wit
+0000ee60: 6820 6060 7075 6e63 7475 6174 696f 6e60  h ``punctuation`
+0000ee70: 602e 0d0a 0d0a 2020 2020 2020 2020 5061  `.....        Pa
+0000ee80: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
+0000ee90: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
+0000eea0: 2020 2020 2020 7075 6e63 7475 6174 696f        punctuatio
+0000eeb0: 6e20 3a20 6c69 7374 206f 6620 7374 7220  n : list of str 
+0000eec0: 6f66 206c 6973 7420 6f66 2074 7570 6c65  of list of tuple
+0000eed0: 206f 6620 2873 7472 2c20 7374 7229 206f   of (str, str) o
+0000eee0: 7220 7374 720d 0a20 2020 2020 2020 2020  r str..         
+0000eef0: 2020 2050 756e 6374 7561 7469 6f6e 2873     Punctuation(s
+0000ef00: 2920 746f 2073 706c 6974 2073 6567 6d65  ) to split segme
+0000ef10: 6e74 7320 6279 2e0d 0a20 2020 2020 2020  nts by...       
+0000ef20: 206c 6f63 6b20 3a20 626f 6f6c 2c20 6465   lock : bool, de
+0000ef30: 6661 756c 7420 4661 6c73 650d 0a20 2020  fault False..   
+0000ef40: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
+0000ef50: 2074 6f20 7072 6576 656e 7420 6675 7475   to prevent futu
+0000ef60: 7265 2073 706c 6974 732f 6d65 7267 6573  re splits/merges
+0000ef70: 2066 726f 6d20 616c 7465 7269 6e67 2063   from altering c
+0000ef80: 6861 6e67 6573 206d 6164 6520 6279 2074  hanges made by t
+0000ef90: 6869 7320 6d65 7468 6f64 2e0d 0a20 2020  his method...   
+0000efa0: 2020 2020 206e 6577 6c69 6e65 203a 2062       newline : b
+0000efb0: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
+0000efc0: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
+0000efd0: 5768 6574 6865 7220 746f 2069 6e73 6572  Whether to inser
+0000efe0: 7420 6c69 6e65 2062 7265 616b 2061 7420  t line break at 
+0000eff0: 7468 6520 7370 6c69 7420 706f 696e 7473  the split points
+0000f000: 2069 6e73 7465 6164 206f 6620 7370 6c69   instead of spli
+0000f010: 7474 696e 6720 696e 746f 2073 6570 6172  tting into separ
+0000f020: 6174 6520 7365 676d 656e 7473 2e0d 0a20  ate segments... 
+0000f030: 2020 2020 2020 206d 696e 5f77 6f72 6473         min_words
+0000f040: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
+0000f050: 0d0a 2020 2020 2020 2020 2020 2020 5370  ..            Sp
+0000f060: 6c69 7420 7365 676d 656e 7473 2077 6974  lit segments wit
+0000f070: 6820 776f 7264 7320 3e3d 2060 606d 696e  h words >= ``min
+0000f080: 5f77 6f72 6473 6060 2e0d 0a20 2020 2020  _words``...     
+0000f090: 2020 206d 696e 5f63 6861 7273 203a 2069     min_chars : i
+0000f0a0: 6e74 2c20 6f70 7469 6f6e 616c 0d0a 2020  nt, optional..  
+0000f0b0: 2020 2020 2020 2020 2020 5370 6c69 7420            Split 
+0000f0c0: 7365 676d 656e 7473 2077 6974 6820 6368  segments with ch
+0000f0d0: 6172 6163 7465 7273 203e 3d20 6060 6d69  aracters >= ``mi
+0000f0e0: 6e5f 6368 6172 7360 602e 0d0a 2020 2020  n_chars``...    
+0000f0f0: 2020 2020 6d69 6e5f 6475 7220 3a20 696e      min_dur : in
+0000f100: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
+0000f110: 2020 2020 2020 2020 2073 706c 6974 2073           split s
+0000f120: 6567 6d65 6e74 7320 7769 7468 2064 7572  egments with dur
+0000f130: 6174 696f 6e20 2869 6e20 7365 636f 6e64  ation (in second
+0000f140: 7329 203e 3d20 6060 6d69 6e5f 6475 7260  s) >= ``min_dur`
+0000f150: 602e 0d0a 0d0a 2020 2020 2020 2020 5265  `.....        Re
+0000f160: 7475 726e 730d 0a20 2020 2020 2020 202d  turns..        -
+0000f170: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+0000f180: 7374 6162 6c65 5f77 6869 7370 6572 2e72  stable_whisper.r
+0000f190: 6573 756c 742e 5768 6973 7065 7252 6573  esult.WhisperRes
+0000f1a0: 756c 740d 0a20 2020 2020 2020 2020 2020  ult..           
+0000f1b0: 2054 6865 2063 7572 7265 6e74 2069 6e73   The current ins
+0000f1c0: 7461 6e63 6520 6166 7465 7220 7468 6520  tance after the 
+0000f1d0: 6368 616e 6765 732e 0d0a 2020 2020 2020  changes...      
+0000f1e0: 2020 2222 220d 0a20 2020 2020 2020 2064    """..        d
+0000f1f0: 6566 205f 6f76 6572 5f6d 6178 2878 3a20  ef _over_max(x: 
+0000f200: 5365 676d 656e 7429 3a0d 0a20 2020 2020  Segment):..     
+0000f210: 2020 2020 2020 2072 6574 7572 6e20 280d         return (.
+0000f220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f230: 2020 2020 2028 6d69 6e5f 776f 7264 7320       (min_words 
+0000f240: 616e 6420 6c65 6e28 782e 776f 7264 7329  and len(x.words)
+0000f250: 203e 3d20 6d69 6e5f 776f 7264 7329 206f   >= min_words) o
+0000f260: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
+0000f270: 2020 2020 2020 2028 6d69 6e5f 6368 6172         (min_char
+0000f280: 7320 616e 6420 782e 6368 6172 5f63 6f75  s and x.char_cou
+0000f290: 6e74 2829 203e 3d20 6d69 6e5f 6368 6172  nt() >= min_char
+0000f2a0: 7329 206f 720d 0a20 2020 2020 2020 2020  s) or..         
+0000f2b0: 2020 2020 2020 2020 2020 2028 6d69 6e5f             (min_
+0000f2c0: 6475 7220 616e 6420 782e 6475 7261 7469  dur and x.durati
+0000f2d0: 6f6e 203e 3d20 6d69 6e5f 6475 7229 0d0a  on >= min_dur)..
+0000f2e0: 2020 2020 2020 2020 2020 2020 290d 0a0d              )...
+0000f2f0: 0a20 2020 2020 2020 2069 6e64 6963 6573  .        indices
+0000f300: 203d 2073 6574 2873 2e69 6420 666f 7220   = set(s.id for 
+0000f310: 7320 696e 2073 656c 662e 7365 676d 656e  s in self.segmen
+0000f320: 7473 2069 6620 5f6f 7665 725f 6d61 7828  ts if _over_max(
+0000f330: 7329 2920 6966 2061 6e79 2828 6d69 6e5f  s)) if any((min_
+0000f340: 776f 7264 732c 206d 696e 5f63 6861 7273  words, min_chars
+0000f350: 2c20 6d69 6e5f 6475 7229 2920 656c 7365  , min_dur)) else
+0000f360: 204e 6f6e 650d 0a0d 0a20 2020 2020 2020   None....       
+0000f370: 2064 6566 205f 6765 745f 696e 6469 6365   def _get_indice
+0000f380: 7328 783a 2053 6567 6d65 6e74 293a 0d0a  s(x: Segment):..
+0000f390: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000f3a0: 726e 2078 2e67 6574 5f70 756e 6374 7561  rn x.get_punctua
+0000f3b0: 7469 6f6e 5f69 6e64 6963 6573 2870 756e  tion_indices(pun
+0000f3c0: 6374 7561 7469 6f6e 2920 6966 2069 6e64  ctuation) if ind
+0000f3d0: 6963 6573 2069 7320 4e6f 6e65 206f 7220  ices is None or 
+0000f3e0: 782e 6964 2069 6e20 696e 6469 6365 7320  x.id in indices 
+0000f3f0: 656c 7365 205b 5d0d 0a0d 0a20 2020 2020  else []....     
+0000f400: 2020 2073 656c 662e 5f73 706c 6974 5f73     self._split_s
+0000f410: 6567 6d65 6e74 7328 5f67 6574 5f69 6e64  egments(_get_ind
+0000f420: 6963 6573 2c20 6c6f 636b 3d6c 6f63 6b2c  ices, lock=lock,
+0000f430: 206e 6577 6c69 6e65 3d6e 6577 6c69 6e65   newline=newline
+0000f440: 290d 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+0000f450: 6c66 2e5f 7265 6772 6f75 705f 6869 7374  lf._regroup_hist
+0000f460: 6f72 793a 0d0a 2020 2020 2020 2020 2020  ory:..          
+0000f470: 2020 7365 6c66 2e5f 7265 6772 6f75 705f    self._regroup_
+0000f480: 6869 7374 6f72 7920 2b3d 2027 5f27 0d0a  history += '_'..
+0000f490: 2020 2020 2020 2020 7075 6e63 745f 7374          punct_st
+0000f4a0: 7220 3d20 272f 272e 6a6f 696e 2870 2069  r = '/'.join(p i
+0000f4b0: 6620 6973 696e 7374 616e 6365 2870 2c20  f isinstance(p, 
+0000f4c0: 7374 7229 2065 6c73 6520 272a 272e 6a6f  str) else '*'.jo
+0000f4d0: 696e 2870 2920 666f 7220 7020 696e 2070  in(p) for p in p
+0000f4e0: 756e 6374 7561 7469 6f6e 290d 0a20 2020  unctuation)..   
+0000f4f0: 2020 2020 2073 656c 662e 5f72 6567 726f       self._regro
+0000f500: 7570 5f68 6973 746f 7279 202b 3d20 6627  up_history += f'
+0000f510: 7370 3d7b 7075 6e63 745f 7374 727d 2b7b  sp={punct_str}+{
+0000f520: 696e 7428 6c6f 636b 297d 2b7b 696e 7428  int(lock)}+{int(
+0000f530: 6e65 776c 696e 6529 7d27 0d0a 2020 2020  newline)}'..    
+0000f540: 2020 2020 7365 6c66 2e5f 7265 6772 6f75      self._regrou
+0000f550: 705f 6869 7374 6f72 7920 2b3d 2066 272b  p_history += f'+
+0000f560: 7b6d 696e 5f77 6f72 6473 206f 7220 2222  {min_words or ""
+0000f570: 7d2b 7b6d 696e 5f63 6861 7273 206f 7220  }+{min_chars or 
+0000f580: 2222 7d2b 7b6d 696e 5f64 7572 206f 7220  ""}+{min_dur or 
+0000f590: 2222 7d27 2e72 7374 7269 7028 272b 2729  ""}'.rstrip('+')
+0000f5a0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000f5b0: 2073 656c 660d 0a0d 0a20 2020 2064 6566   self....    def
+0000f5c0: 206d 6572 6765 5f62 795f 7075 6e63 7475   merge_by_punctu
+0000f5d0: 6174 696f 6e28 0d0a 2020 2020 2020 2020  ation(..        
+0000f5e0: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
+0000f5f0: 2020 2020 2020 2070 756e 6374 7561 7469         punctuati
+0000f600: 6f6e 3a20 556e 696f 6e5b 4c69 7374 5b73  on: Union[List[s
+0000f610: 7472 5d2c 204c 6973 745b 5475 706c 655b  tr], List[Tuple[
+0000f620: 7374 722c 2073 7472 5d5d 2c20 7374 725d  str, str]], str]
+0000f630: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
+0000f640: 6178 5f77 6f72 6473 3a20 696e 7420 3d20  ax_words: int = 
+0000f650: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
+0000f660: 2020 206d 6178 5f63 6861 7273 3a20 696e     max_chars: in
+0000f670: 7420 3d20 4e6f 6e65 2c0d 0a20 2020 2020  t = None,..     
+0000f680: 2020 2020 2020 2069 735f 7375 6d5f 6d61         is_sum_ma
+0000f690: 783a 2062 6f6f 6c20 3d20 4661 6c73 652c  x: bool = False,
+0000f6a0: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+0000f6b0: 636b 3a20 626f 6f6c 203d 2046 616c 7365  ck: bool = False
+0000f6c0: 0d0a 2020 2020 2920 2d3e 2022 5768 6973  ..    ) -> "Whis
+0000f6d0: 7065 7252 6573 756c 7422 3a0d 0a20 2020  perResult":..   
+0000f6e0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+0000f6f0: 2020 4d65 7267 6520 2869 6e2d 706c 6163    Merge (in-plac
+0000f700: 6529 2061 6e79 2074 776f 2073 6567 6d65  e) any two segme
+0000f710: 6e74 7320 7468 6174 2068 6173 2073 7065  nts that has spe
+0000f720: 6369 6669 6320 7075 6e63 7475 6174 696f  cific punctuatio
+0000f730: 6e73 2069 6e62 6574 7765 656e 2e0d 0a0d  ns inbetween....
+0000f740: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0000f750: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
+0000f760: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+0000f770: 2070 756e 6374 7561 7469 6f6e 203a 206c   punctuation : l
+0000f780: 6973 7420 6f66 2073 7472 206f 6620 6c69  ist of str of li
+0000f790: 7374 206f 6620 7475 706c 6520 6f66 2028  st of tuple of (
+0000f7a0: 7374 722c 2073 7472 2920 6f72 2073 7472  str, str) or str
+0000f7b0: 0d0a 2020 2020 2020 2020 2020 2020 5075  ..            Pu
+0000f7c0: 6e63 7475 6174 696f 6e28 7329 2074 6f20  nctuation(s) to 
+0000f7d0: 6d65 7267 6520 7365 676d 656e 7473 2062  merge segments b
+0000f7e0: 792e 0d0a 2020 2020 2020 2020 6d61 785f  y...        max_
+0000f7f0: 776f 7264 7320 3a20 696e 742c 206f 7074  words : int, opt
+0000f800: 696f 6e61 6c0d 0a20 2020 2020 2020 2020  ional..         
+0000f810: 2020 204d 6178 696d 756d 206e 756d 6265     Maximum numbe
+0000f820: 7220 6f66 2077 6f72 6473 2061 6c6c 6f77  r of words allow
+0000f830: 6564 2069 6e20 6561 6368 2073 6567 6d65  ed in each segme
+0000f840: 6e74 2e0d 0a20 2020 2020 2020 206d 6178  nt...        max
+0000f850: 5f63 6861 7273 203a 2069 6e74 2c20 6f70  _chars : int, op
+0000f860: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+0000f870: 2020 2020 4d61 7869 6d75 6d20 6e75 6d62      Maximum numb
+0000f880: 6572 206f 6620 6368 6172 6163 7465 7273  er of characters
+0000f890: 2061 6c6c 6f77 6564 2069 6e20 6561 6368   allowed in each
+0000f8a0: 2073 6567 6d65 6e74 2e0d 0a20 2020 2020   segment...     
+0000f8b0: 2020 2069 735f 7375 6d5f 6d61 7820 3a20     is_sum_max : 
+0000f8c0: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
+0000f8d0: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+0000f8e0: 2057 6865 7468 6572 2060 606d 6178 5f77   Whether ``max_w
+0000f8f0: 6f72 6473 6060 2061 6e64 2060 606d 6178  ords`` and ``max
+0000f900: 5f63 6861 7273 6060 2069 7320 6170 706c  _chars`` is appl
+0000f910: 6965 6420 746f 2074 6865 206d 6572 6765  ied to the merge
+0000f920: 6420 7365 676d 656e 7420 696e 7374 6561  d segment instea
+0000f930: 6420 6f66 2074 6865 2069 6e64 6976 6964  d of the individ
+0000f940: 7561 6c20 7365 676d 656e 7473 0d0a 2020  ual segments..  
+0000f950: 2020 2020 2020 2020 2020 746f 2062 6520            to be 
+0000f960: 6d65 7267 6564 2e0d 0a20 2020 2020 2020  merged...       
+0000f970: 206c 6f63 6b20 3a20 626f 6f6c 2c20 6465   lock : bool, de
+0000f980: 6661 756c 7420 4661 6c73 650d 0a20 2020  fault False..   
+0000f990: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
+0000f9a0: 2074 6f20 7072 6576 656e 7420 6675 7475   to prevent futu
+0000f9b0: 7265 2073 706c 6974 732f 6d65 7267 6573  re splits/merges
+0000f9c0: 2066 726f 6d20 616c 7465 7269 6e67 2063   from altering c
+0000f9d0: 6861 6e67 6573 206d 6164 6520 6279 2074  hanges made by t
+0000f9e0: 6869 7320 6d65 7468 6f64 2e0d 0a0d 0a20  his method..... 
+0000f9f0: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
+0000fa00: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
+0000fa10: 0a20 2020 2020 2020 2073 7461 626c 655f  .        stable_
+0000fa20: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
+0000fa30: 6869 7370 6572 5265 7375 6c74 0d0a 2020  hisperResult..  
+0000fa40: 2020 2020 2020 2020 2020 5468 6520 6375            The cu
+0000fa50: 7272 656e 7420 696e 7374 616e 6365 2061  rrent instance a
+0000fa60: 6674 6572 2074 6865 2063 6861 6e67 6573  fter the changes
+0000fa70: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+0000fa80: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
+0000fa90: 3d20 7365 6c66 2e67 6574 5f70 756e 6374  = self.get_punct
+0000faa0: 7561 7469 6f6e 5f69 6e64 6963 6573 2870  uation_indices(p
+0000fab0: 756e 6374 7561 7469 6f6e 290d 0a20 2020  unctuation)..   
+0000fac0: 2020 2020 2073 656c 662e 5f6d 6572 6765       self._merge
+0000fad0: 5f73 6567 6d65 6e74 7328 696e 6469 6365  _segments(indice
+0000fae0: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
+0000faf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb00: 206d 6178 5f77 6f72 6473 3d6d 6178 5f77   max_words=max_w
+0000fb10: 6f72 6473 2c20 6d61 785f 6368 6172 733d  ords, max_chars=
+0000fb20: 6d61 785f 6368 6172 732c 2069 735f 7375  max_chars, is_su
+0000fb30: 6d5f 6d61 783d 6973 5f73 756d 5f6d 6178  m_max=is_sum_max
+0000fb40: 2c20 6c6f 636b 3d6c 6f63 6b29 0d0a 2020  , lock=lock)..  
+0000fb50: 2020 2020 2020 6966 2073 656c 662e 5f72        if self._r
+0000fb60: 6567 726f 7570 5f68 6973 746f 7279 3a0d  egroup_history:.
+0000fb70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000fb80: 662e 5f72 6567 726f 7570 5f68 6973 746f  f._regroup_histo
+0000fb90: 7279 202b 3d20 275f 270d 0a20 2020 2020  ry += '_'..     
+0000fba0: 2020 2070 756e 6374 5f73 7472 203d 2027     punct_str = '
+0000fbb0: 2f27 2e6a 6f69 6e28 7020 6966 2069 7369  /'.join(p if isi
+0000fbc0: 6e73 7461 6e63 6528 702c 2073 7472 2920  nstance(p, str) 
+0000fbd0: 656c 7365 2027 2a27 2e6a 6f69 6e28 7029  else '*'.join(p)
+0000fbe0: 2066 6f72 2070 2069 6e20 7075 6e63 7475   for p in punctu
+0000fbf0: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
+0000fc00: 7365 6c66 2e5f 7265 6772 6f75 705f 6869  self._regroup_hi
+0000fc10: 7374 6f72 7920 2b3d 2066 276d 703d 7b70  story += f'mp={p
+0000fc20: 756e 6374 5f73 7472 7d2b 7b6d 6178 5f77  unct_str}+{max_w
+0000fc30: 6f72 6473 206f 7220 2222 7d2b 7b6d 6178  ords or ""}+{max
+0000fc40: 5f63 6861 7273 206f 7220 2222 7d2b 7b69  _chars or ""}+{i
+0000fc50: 6e74 2869 735f 7375 6d5f 6d61 7829 7d2b  nt(is_sum_max)}+
+0000fc60: 7b69 6e74 286c 6f63 6b29 7d27 0d0a 2020  {int(lock)}'..  
+0000fc70: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000fc80: 660d 0a0d 0a20 2020 2064 6566 206d 6572  f....    def mer
+0000fc90: 6765 5f61 6c6c 5f73 6567 6d65 6e74 7328  ge_all_segments(
+0000fca0: 7365 6c66 2920 2d3e 2022 5768 6973 7065  self) -> "Whispe
+0000fcb0: 7252 6573 756c 7422 3a0d 0a20 2020 2020  rResult":..     
+0000fcc0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+0000fcd0: 4d65 7267 6520 616c 6c20 7365 676d 656e  Merge all segmen
+0000fce0: 7473 2069 6e74 6f20 6f6e 6520 7365 676d  ts into one segm
+0000fcf0: 656e 742e 0d0a 0d0a 2020 2020 2020 2020  ent.....        
+0000fd00: 5265 7475 726e 730d 0a20 2020 2020 2020  Returns..       
+0000fd10: 202d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020   -------..      
+0000fd20: 2020 7374 6162 6c65 5f77 6869 7370 6572    stable_whisper
+0000fd30: 2e72 6573 756c 742e 5768 6973 7065 7252  .result.WhisperR
+0000fd40: 6573 756c 740d 0a20 2020 2020 2020 2020  esult..         
+0000fd50: 2020 2054 6865 2063 7572 7265 6e74 2069     The current i
+0000fd60: 6e73 7461 6e63 6520 6166 7465 7220 7468  nstance after th
+0000fd70: 6520 6368 616e 6765 732e 0d0a 2020 2020  e changes...    
+0000fd80: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+0000fd90: 2069 6620 6e6f 7420 7365 6c66 2e73 6567   if not self.seg
+0000fda0: 6d65 6e74 733a 0d0a 2020 2020 2020 2020  ments:..        
+0000fdb0: 2020 2020 7265 7475 726e 2073 656c 660d      return self.
+0000fdc0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000fdd0: 2e68 6173 5f77 6f72 6473 3a0d 0a20 2020  .has_words:..   
+0000fde0: 2020 2020 2020 2020 206e 6577 5f73 6567           new_seg
+0000fdf0: 203d 2073 656c 662e 7365 676d 656e 7473   = self.segments
+0000fe00: 5b30 5d2e 636f 7079 2873 656c 662e 616c  [0].copy(self.al
+0000fe10: 6c5f 776f 7264 7328 292c 206b 6565 705f  l_words(), keep_
+0000fe20: 7265 7375 6c74 3d54 7275 652c 2063 6f70  result=True, cop
+0000fe30: 795f 776f 7264 733d 4661 6c73 6529 0d0a  y_words=False)..
+0000fe40: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0000fe50: 2020 2020 2020 2020 2020 206e 6577 5f73             new_s
+0000fe60: 6567 203d 2073 656c 662e 7365 676d 656e  eg = self.segmen
+0000fe70: 7473 5b30 5d0d 0a20 2020 2020 2020 2020  ts[0]..         
+0000fe80: 2020 206e 6577 5f73 6567 2e5f 6465 6661     new_seg._defa
+0000fe90: 756c 745f 7465 7874 202b 3d20 2727 2e6a  ult_text += ''.j
+0000fea0: 6f69 6e28 732e 7465 7874 2066 6f72 2073  oin(s.text for s
+0000feb0: 2069 6e20 7365 6c66 2e73 6567 6d65 6e74   in self.segment
+0000fec0: 735b 313a 5d29 0d0a 2020 2020 2020 2020  s[1:])..        
+0000fed0: 2020 2020 6966 2061 6c6c 2873 2e74 6f6b      if all(s.tok
+0000fee0: 656e 7320 6973 206e 6f74 204e 6f6e 6520  ens is not None 
+0000fef0: 666f 7220 7320 696e 2073 656c 662e 7365  for s in self.se
+0000ff00: 676d 656e 7473 293a 0d0a 2020 2020 2020  gments):..      
+0000ff10: 2020 2020 2020 2020 2020 6e65 775f 7365            new_se
+0000ff20: 672e 5f64 6566 6175 6c74 5f74 6f6b 656e  g._default_token
+0000ff30: 7320 2b3d 206c 6973 7428 6368 6169 6e2e  s += list(chain.
+0000ff40: 6672 6f6d 5f69 7465 7261 626c 6528 732e  from_iterable(s.
+0000ff50: 746f 6b65 6e73 2066 6f72 2073 2069 6e20  tokens for s in 
+0000ff60: 7365 6c66 2e73 6567 6d65 6e74 735b 313a  self.segments[1:
+0000ff70: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
+0000ff80: 206e 6577 5f73 6567 2e65 6e64 203d 2073   new_seg.end = s
+0000ff90: 656c 662e 7365 676d 656e 7473 5b2d 315d  elf.segments[-1]
+0000ffa0: 2e65 6e64 0d0a 2020 2020 2020 2020 7365  .end..        se
+0000ffb0: 6c66 2e73 6567 6d65 6e74 7320 3d20 5b6e  lf.segments = [n
+0000ffc0: 6577 5f73 6567 5d0d 0a20 2020 2020 2020  ew_seg]..       
+0000ffd0: 2073 656c 662e 7265 6173 7369 676e 5f69   self.reassign_i
+0000ffe0: 6473 2829 0d0a 2020 2020 2020 2020 6966  ds()..        if
 0000fff0: 2073 656c 662e 5f72 6567 726f 7570 5f68   self._regroup_h
-00010000: 6973 746f 7279 202b 3d20 276d 7327 0d0a  istory += 'ms'..
-00010010: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00010020: 656c 660d 0a0d 0a20 2020 2064 6566 2073  elf....    def s
-00010030: 706c 6974 5f62 795f 6c65 6e67 7468 280d  plit_by_length(.
-00010040: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010050: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
-00010060: 6d61 785f 6368 6172 733a 2069 6e74 203d  max_chars: int =
-00010070: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00010080: 2020 2020 6d61 785f 776f 7264 733a 2069      max_words: i
-00010090: 6e74 203d 204e 6f6e 652c 0d0a 2020 2020  nt = None,..    
-000100a0: 2020 2020 2020 2020 6576 656e 5f73 706c          even_spl
-000100b0: 6974 3a20 626f 6f6c 203d 2054 7275 652c  it: bool = True,
-000100c0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-000100d0: 7263 655f 6c65 6e3a 2062 6f6f 6c20 3d20  rce_len: bool = 
-000100e0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-000100f0: 2020 2020 6c6f 636b 3a20 626f 6f6c 203d      lock: bool =
-00010100: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
-00010110: 2020 2020 2069 6e63 6c75 6465 5f6c 6f63       include_loc
-00010120: 6b3a 2062 6f6f 6c20 3d20 4661 6c73 652c  k: bool = False,
-00010130: 0d0a 2020 2020 2020 2020 2020 2020 6e65  ..            ne
-00010140: 776c 696e 653a 2062 6f6f 6c20 3d20 4661  wline: bool = Fa
-00010150: 6c73 650d 0a20 2020 2029 202d 3e20 2257  lse..    ) -> "W
-00010160: 6869 7370 6572 5265 7375 6c74 223a 0d0a  hisperResult":..
-00010170: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00010180: 2020 2020 2053 706c 6974 2028 696e 2d70       Split (in-p
-00010190: 6c61 6365 2920 616e 7920 7365 676d 656e  lace) any segmen
-000101a0: 7420 7468 6174 2065 7863 6565 6473 2060  t that exceeds `
-000101b0: 606d 6178 5f63 6861 7273 6060 206f 7220  `max_chars`` or 
-000101c0: 6060 6d61 785f 776f 7264 7360 6020 696e  ``max_words`` in
-000101d0: 746f 2073 6d61 6c6c 6572 2073 6567 6d65  to smaller segme
-000101e0: 6e74 732e 0d0a 0d0a 2020 2020 2020 2020  nts.....        
-000101f0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
-00010200: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
-00010210: 2020 2020 2020 2020 6d61 785f 6368 6172          max_char
-00010220: 7320 3a20 696e 742c 206f 7074 696f 6e61  s : int, optiona
-00010230: 6c0d 0a20 2020 2020 2020 2020 2020 204d  l..            M
-00010240: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
-00010250: 2063 6861 7261 6374 6572 7320 616c 6c6f   characters allo
-00010260: 7765 6420 696e 2065 6163 6820 7365 676d  wed in each segm
-00010270: 656e 742e 0d0a 2020 2020 2020 2020 6d61  ent...        ma
-00010280: 785f 776f 7264 7320 3a20 696e 742c 206f  x_words : int, o
-00010290: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-000102a0: 2020 2020 204d 6178 696d 756d 206e 756d       Maximum num
-000102b0: 6265 7220 6f66 2077 6f72 6473 2061 6c6c  ber of words all
-000102c0: 6f77 6564 2069 6e20 6561 6368 2073 6567  owed in each seg
-000102d0: 6d65 6e74 2e0d 0a20 2020 2020 2020 2065  ment...        e
-000102e0: 7665 6e5f 7370 6c69 7420 3a20 626f 6f6c  ven_split : bool
-000102f0: 2c20 6465 6661 756c 7420 5472 7565 0d0a  , default True..
-00010300: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
-00010310: 6865 7220 746f 2065 7665 6e6c 7920 7370  her to evenly sp
-00010320: 6c69 7420 6120 7365 676d 656e 7420 696e  lit a segment in
-00010330: 206c 656e 6774 6820 6966 2069 7420 6578   length if it ex
-00010340: 6365 6564 7320 6060 6d61 785f 6368 6172  ceeds ``max_char
-00010350: 7360 6020 6f72 2060 606d 6178 5f77 6f72  s`` or ``max_wor
-00010360: 6473 6060 2e0d 0a20 2020 2020 2020 2066  ds``...        f
-00010370: 6f72 6365 5f6c 656e 203a 2062 6f6f 6c2c  orce_len : bool,
-00010380: 2064 6566 6175 6c74 2046 616c 7365 0d0a   default False..
-00010390: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
-000103a0: 6865 7220 746f 2066 6f72 6365 2061 2063  her to force a c
-000103b0: 6f6e 7374 616e 7420 6c65 6e67 7468 2066  onstant length f
-000103c0: 6f72 2065 6163 6820 7365 676d 656e 7420  or each segment 
-000103d0: 6578 6365 7074 2074 6865 206c 6173 7420  except the last 
-000103e0: 7365 676d 656e 742e 0d0a 2020 2020 2020  segment...      
-000103f0: 2020 2020 2020 5468 6973 2077 696c 6c20        This will 
-00010400: 6967 6e6f 7265 2061 6c6c 2070 7265 7669  ignore all previ
-00010410: 6f75 7320 6e6f 6e2d 6c6f 636b 6564 2073  ous non-locked s
-00010420: 6567 6d65 6e74 2062 6f75 6e64 6172 6965  egment boundarie
-00010430: 732e 0d0a 2020 2020 2020 2020 6c6f 636b  s...        lock
-00010440: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-00010450: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00010460: 2020 2020 5768 6574 6865 7220 746f 2070      Whether to p
-00010470: 7265 7665 6e74 2066 7574 7572 6520 7370  revent future sp
-00010480: 6c69 7473 2f6d 6572 6765 7320 6672 6f6d  lits/merges from
-00010490: 2061 6c74 6572 696e 6720 6368 616e 6765   altering change
-000104a0: 7320 6d61 6465 2062 7920 7468 6973 206d  s made by this m
-000104b0: 6574 686f 642e 0d0a 2020 2020 2020 2020  ethod...        
-000104c0: 696e 636c 7564 655f 6c6f 636b 3a20 626f  include_lock: bo
-000104d0: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
-000104e0: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
-000104f0: 6865 7468 6572 2074 6f20 696e 636c 7564  hether to includ
-00010500: 6520 7072 6576 696f 7573 206c 6f63 6b20  e previous lock 
-00010510: 6265 666f 7265 2073 706c 6974 7469 6e67  before splitting
-00010520: 2062 6173 6564 206f 6e20 6d61 785f 776f   based on max_wo
-00010530: 7264 732c 2069 6620 6060 6576 656e 5f73  rds, if ``even_s
-00010540: 706c 6974 203d 2046 616c 7365 6060 2e0d  plit = False``..
-00010550: 0a20 2020 2020 2020 2020 2020 2053 706c  .            Spl
-00010560: 6974 7469 6e67 2077 696c 6c20 6265 2064  itting will be d
-00010570: 6f6e 6520 6166 7465 7220 7468 6520 6669  one after the fi
-00010580: 7273 7420 6e6f 6e2d 6c6f 636b 6564 2077  rst non-locked w
-00010590: 6f72 6420 3e20 6060 6d61 785f 6368 6172  ord > ``max_char
-000105a0: 7360 6020 2f20 6060 6d61 785f 776f 7264  s`` / ``max_word
-000105b0: 7360 602e 0d0a 2020 2020 2020 2020 6e65  s``...        ne
-000105c0: 776c 696e 653a 2062 6f6f 6c2c 2064 6566  wline: bool, def
-000105d0: 6175 6c74 2046 616c 7365 0d0a 2020 2020  ault False..    
-000105e0: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
-000105f0: 746f 2069 6e73 6572 7420 6c69 6e65 2062  to insert line b
-00010600: 7265 616b 2061 7420 7468 6520 7370 6c69  reak at the spli
-00010610: 7420 706f 696e 7473 2069 6e73 7465 6164  t points instead
-00010620: 206f 6620 7370 6c69 7474 696e 6720 696e   of splitting in
-00010630: 746f 2073 6570 6172 6174 6520 7365 676d  to separate segm
-00010640: 656e 7473 2e0d 0a0d 0a20 2020 2020 2020  ents.....       
-00010650: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
-00010660: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
-00010670: 2020 2073 7461 626c 655f 7768 6973 7065     stable_whispe
-00010680: 722e 7265 7375 6c74 2e57 6869 7370 6572  r.result.Whisper
-00010690: 5265 7375 6c74 0d0a 2020 2020 2020 2020  Result..        
-000106a0: 2020 2020 5468 6520 6375 7272 656e 7420      The current 
-000106b0: 696e 7374 616e 6365 2061 6674 6572 2074  instance after t
-000106c0: 6865 2063 6861 6e67 6573 2e0d 0a0d 0a20  he changes..... 
-000106d0: 2020 2020 2020 204e 6f74 6573 0d0a 2020         Notes..  
-000106e0: 2020 2020 2020 2d2d 2d2d 2d0d 0a20 2020        -----..   
-000106f0: 2020 2020 2049 6620 6060 6576 656e 5f73       If ``even_s
-00010700: 706c 6974 203d 2054 7275 6560 602c 2073  plit = True``, s
-00010710: 6567 6d65 6e74 7320 6361 6e20 7374 696c  egments can stil
-00010720: 6c20 6578 6365 6564 2060 606d 6178 5f63  l exceed ``max_c
-00010730: 6861 7273 6060 2061 6e64 206c 6f63 6b65  hars`` and locke
-00010740: 6420 776f 7264 7320 7769 6c6c 2062 6520  d words will be 
-00010750: 6967 6e6f 7265 6420 746f 2061 766f 6964  ignored to avoid
-00010760: 0d0a 2020 2020 2020 2020 756e 6576 656e  ..        uneven
-00010770: 2073 706c 6974 7469 6e67 2e0d 0a20 2020   splitting...   
-00010780: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00010790: 2020 6966 2066 6f72 6365 5f6c 656e 3a0d    if force_len:.
-000107a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000107b0: 662e 6d65 7267 655f 616c 6c5f 7365 676d  f.merge_all_segm
-000107c0: 656e 7473 2829 0d0a 2020 2020 2020 2020  ents()..        
-000107d0: 7365 6c66 2e5f 7370 6c69 745f 7365 676d  self._split_segm
-000107e0: 656e 7473 280d 0a20 2020 2020 2020 2020  ents(..         
-000107f0: 2020 206c 616d 6264 6120 783a 2078 2e67     lambda x: x.g
-00010800: 6574 5f6c 656e 6774 685f 696e 6469 6365  et_length_indice
-00010810: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
-00010820: 2020 2020 6d61 785f 6368 6172 733d 6d61      max_chars=ma
-00010830: 785f 6368 6172 732c 0d0a 2020 2020 2020  x_chars,..      
-00010840: 2020 2020 2020 2020 2020 6d61 785f 776f            max_wo
-00010850: 7264 733d 6d61 785f 776f 7264 732c 0d0a  rds=max_words,..
-00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010870: 6576 656e 5f73 706c 6974 3d65 7665 6e5f  even_split=even_
-00010880: 7370 6c69 742c 0d0a 2020 2020 2020 2020  split,..        
-00010890: 2020 2020 2020 2020 696e 636c 7564 655f          include_
-000108a0: 6c6f 636b 3d69 6e63 6c75 6465 5f6c 6f63  lock=include_loc
-000108b0: 6b0d 0a20 2020 2020 2020 2020 2020 2029  k..            )
-000108c0: 2c0d 0a20 2020 2020 2020 2020 2020 206c  ,..            l
-000108d0: 6f63 6b3d 6c6f 636b 2c0d 0a20 2020 2020  ock=lock,..     
-000108e0: 2020 2020 2020 206e 6577 6c69 6e65 3d6e         newline=n
-000108f0: 6577 6c69 6e65 0d0a 2020 2020 2020 2020  ewline..        
-00010900: 290d 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-00010910: 6c66 2e5f 7265 6772 6f75 705f 6869 7374  lf._regroup_hist
-00010920: 6f72 793a 0d0a 2020 2020 2020 2020 2020  ory:..          
-00010930: 2020 7365 6c66 2e5f 7265 6772 6f75 705f    self._regroup_
-00010940: 6869 7374 6f72 7920 2b3d 2027 5f27 0d0a  history += '_'..
-00010950: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
-00010960: 6772 6f75 705f 6869 7374 6f72 7920 2b3d  group_history +=
-00010970: 2028 6627 736c 3d7b 6d61 785f 6368 6172   (f'sl={max_char
-00010980: 7320 6f72 2022 227d 2b7b 6d61 785f 776f  s or ""}+{max_wo
-00010990: 7264 7320 6f72 2022 227d 2b7b 696e 7428  rds or ""}+{int(
-000109a0: 6576 656e 5f73 706c 6974 297d 2b7b 696e  even_split)}+{in
-000109b0: 7428 666f 7263 655f 6c65 6e29 7d27 0d0a  t(force_len)}'..
-000109c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109e0: 2020 6627 2b7b 696e 7428 6c6f 636b 297d    f'+{int(lock)}
-000109f0: 2b7b 696e 7428 696e 636c 7564 655f 6c6f  +{int(include_lo
-00010a00: 636b 297d 2b7b 696e 7428 6e65 776c 696e  ck)}+{int(newlin
-00010a10: 6529 7d27 290d 0a20 2020 2020 2020 2072  e)}')..        r
-00010a20: 6574 7572 6e20 7365 6c66 0d0a 0d0a 2020  eturn self....  
-00010a30: 2020 6465 6620 7370 6c69 745f 6279 5f64    def split_by_d
-00010a40: 7572 6174 696f 6e28 0d0a 2020 2020 2020  uration(..      
-00010a50: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
-00010a60: 2020 2020 2020 2020 206d 6178 5f64 7572           max_dur
-00010a70: 3a20 666c 6f61 742c 0d0a 2020 2020 2020  : float,..      
-00010a80: 2020 2020 2020 6576 656e 5f73 706c 6974        even_split
-00010a90: 3a20 626f 6f6c 203d 2054 7275 652c 0d0a  : bool = True,..
-00010aa0: 2020 2020 2020 2020 2020 2020 666f 7263              forc
-00010ab0: 655f 6c65 6e3a 2062 6f6f 6c20 3d20 4661  e_len: bool = Fa
-00010ac0: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
-00010ad0: 2020 6c6f 636b 3a20 626f 6f6c 203d 2046    lock: bool = F
-00010ae0: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
-00010af0: 2020 2069 6e63 6c75 6465 5f6c 6f63 6b3a     include_lock:
+00010000: 6973 746f 7279 3a0d 0a20 2020 2020 2020  istory:..       
+00010010: 2020 2020 2073 656c 662e 5f72 6567 726f       self._regro
+00010020: 7570 5f68 6973 746f 7279 202b 3d20 275f  up_history += '_
+00010030: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
+00010040: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
+00010050: 202b 3d20 276d 7327 0d0a 2020 2020 2020   += 'ms'..      
+00010060: 2020 7265 7475 726e 2073 656c 660d 0a0d    return self...
+00010070: 0a20 2020 2064 6566 2073 706c 6974 5f62  .    def split_b
+00010080: 795f 6c65 6e67 7468 280d 0a20 2020 2020  y_length(..     
+00010090: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
+000100a0: 2020 2020 2020 2020 2020 6d61 785f 6368            max_ch
+000100b0: 6172 733a 2069 6e74 203d 204e 6f6e 652c  ars: int = None,
+000100c0: 0d0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
+000100d0: 785f 776f 7264 733a 2069 6e74 203d 204e  x_words: int = N
+000100e0: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+000100f0: 2020 6576 656e 5f73 706c 6974 3a20 626f    even_split: bo
+00010100: 6f6c 203d 2054 7275 652c 0d0a 2020 2020  ol = True,..    
+00010110: 2020 2020 2020 2020 666f 7263 655f 6c65          force_le
+00010120: 6e3a 2062 6f6f 6c20 3d20 4661 6c73 652c  n: bool = False,
+00010130: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+00010140: 636b 3a20 626f 6f6c 203d 2046 616c 7365  ck: bool = False
+00010150: 2c0d 0a20 2020 2020 2020 2020 2020 2069  ,..            i
+00010160: 6e63 6c75 6465 5f6c 6f63 6b3a 2062 6f6f  nclude_lock: boo
+00010170: 6c20 3d20 4661 6c73 652c 0d0a 2020 2020  l = False,..    
+00010180: 2020 2020 2020 2020 6e65 776c 696e 653a          newline:
+00010190: 2062 6f6f 6c20 3d20 4661 6c73 650d 0a20   bool = False.. 
+000101a0: 2020 2029 202d 3e20 2257 6869 7370 6572     ) -> "Whisper
+000101b0: 5265 7375 6c74 223a 0d0a 2020 2020 2020  Result":..      
+000101c0: 2020 2222 220d 0a20 2020 2020 2020 2053    """..        S
+000101d0: 706c 6974 2028 696e 2d70 6c61 6365 2920  plit (in-place) 
+000101e0: 616e 7920 7365 676d 656e 7420 7468 6174  any segment that
+000101f0: 2065 7863 6565 6473 2060 606d 6178 5f63   exceeds ``max_c
+00010200: 6861 7273 6060 206f 7220 6060 6d61 785f  hars`` or ``max_
+00010210: 776f 7264 7360 6020 696e 746f 2073 6d61  words`` into sma
+00010220: 6c6c 6572 2073 6567 6d65 6e74 732e 0d0a  ller segments...
+00010230: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00010240: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
+00010250: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
+00010260: 2020 6d61 785f 6368 6172 7320 3a20 696e    max_chars : in
+00010270: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
+00010280: 2020 2020 2020 2020 204d 6178 696d 756d           Maximum
+00010290: 206e 756d 6265 7220 6f66 2063 6861 7261   number of chara
+000102a0: 6374 6572 7320 616c 6c6f 7765 6420 696e  cters allowed in
+000102b0: 2065 6163 6820 7365 676d 656e 742e 0d0a   each segment...
+000102c0: 2020 2020 2020 2020 6d61 785f 776f 7264          max_word
+000102d0: 7320 3a20 696e 742c 206f 7074 696f 6e61  s : int, optiona
+000102e0: 6c0d 0a20 2020 2020 2020 2020 2020 204d  l..            M
+000102f0: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
+00010300: 2077 6f72 6473 2061 6c6c 6f77 6564 2069   words allowed i
+00010310: 6e20 6561 6368 2073 6567 6d65 6e74 2e0d  n each segment..
+00010320: 0a20 2020 2020 2020 2065 7665 6e5f 7370  .        even_sp
+00010330: 6c69 7420 3a20 626f 6f6c 2c20 6465 6661  lit : bool, defa
+00010340: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
+00010350: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+00010360: 2065 7665 6e6c 7920 7370 6c69 7420 6120   evenly split a 
+00010370: 7365 676d 656e 7420 696e 206c 656e 6774  segment in lengt
+00010380: 6820 6966 2069 7420 6578 6365 6564 7320  h if it exceeds 
+00010390: 6060 6d61 785f 6368 6172 7360 6020 6f72  ``max_chars`` or
+000103a0: 2060 606d 6178 5f77 6f72 6473 6060 2e0d   ``max_words``..
+000103b0: 0a20 2020 2020 2020 2066 6f72 6365 5f6c  .        force_l
+000103c0: 656e 203a 2062 6f6f 6c2c 2064 6566 6175  en : bool, defau
+000103d0: 6c74 2046 616c 7365 0d0a 2020 2020 2020  lt False..      
+000103e0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+000103f0: 2066 6f72 6365 2061 2063 6f6e 7374 616e   force a constan
+00010400: 7420 6c65 6e67 7468 2066 6f72 2065 6163  t length for eac
+00010410: 6820 7365 676d 656e 7420 6578 6365 7074  h segment except
+00010420: 2074 6865 206c 6173 7420 7365 676d 656e   the last segmen
+00010430: 742e 0d0a 2020 2020 2020 2020 2020 2020  t...            
+00010440: 5468 6973 2077 696c 6c20 6967 6e6f 7265  This will ignore
+00010450: 2061 6c6c 2070 7265 7669 6f75 7320 6e6f   all previous no
+00010460: 6e2d 6c6f 636b 6564 2073 6567 6d65 6e74  n-locked segment
+00010470: 2062 6f75 6e64 6172 6965 732e 0d0a 2020   boundaries...  
+00010480: 2020 2020 2020 6c6f 636b 203a 2062 6f6f        lock : boo
+00010490: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
+000104a0: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
+000104b0: 6574 6865 7220 746f 2070 7265 7665 6e74  ether to prevent
+000104c0: 2066 7574 7572 6520 7370 6c69 7473 2f6d   future splits/m
+000104d0: 6572 6765 7320 6672 6f6d 2061 6c74 6572  erges from alter
+000104e0: 696e 6720 6368 616e 6765 7320 6d61 6465  ing changes made
+000104f0: 2062 7920 7468 6973 206d 6574 686f 642e   by this method.
+00010500: 0d0a 2020 2020 2020 2020 696e 636c 7564  ..        includ
+00010510: 655f 6c6f 636b 3a20 626f 6f6c 2c20 6465  e_lock: bool, de
+00010520: 6661 756c 7420 4661 6c73 650d 0a20 2020  fault False..   
+00010530: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
+00010540: 2074 6f20 696e 636c 7564 6520 7072 6576   to include prev
+00010550: 696f 7573 206c 6f63 6b20 6265 666f 7265  ious lock before
+00010560: 2073 706c 6974 7469 6e67 2062 6173 6564   splitting based
+00010570: 206f 6e20 6d61 785f 776f 7264 732c 2069   on max_words, i
+00010580: 6620 6060 6576 656e 5f73 706c 6974 203d  f ``even_split =
+00010590: 2046 616c 7365 6060 2e0d 0a20 2020 2020   False``...     
+000105a0: 2020 2020 2020 2053 706c 6974 7469 6e67         Splitting
+000105b0: 2077 696c 6c20 6265 2064 6f6e 6520 6166   will be done af
+000105c0: 7465 7220 7468 6520 6669 7273 7420 6e6f  ter the first no
+000105d0: 6e2d 6c6f 636b 6564 2077 6f72 6420 3e20  n-locked word > 
+000105e0: 6060 6d61 785f 6368 6172 7360 6020 2f20  ``max_chars`` / 
+000105f0: 6060 6d61 785f 776f 7264 7360 602e 0d0a  ``max_words``...
+00010600: 2020 2020 2020 2020 6e65 776c 696e 653a          newline:
+00010610: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
+00010620: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
+00010630: 2020 5768 6574 6865 7220 746f 2069 6e73    Whether to ins
+00010640: 6572 7420 6c69 6e65 2062 7265 616b 2061  ert line break a
+00010650: 7420 7468 6520 7370 6c69 7420 706f 696e  t the split poin
+00010660: 7473 2069 6e73 7465 6164 206f 6620 7370  ts instead of sp
+00010670: 6c69 7474 696e 6720 696e 746f 2073 6570  litting into sep
+00010680: 6172 6174 6520 7365 676d 656e 7473 2e0d  arate segments..
+00010690: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+000106a0: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
+000106b0: 2d2d 2d0d 0a20 2020 2020 2020 2073 7461  ---..        sta
+000106c0: 626c 655f 7768 6973 7065 722e 7265 7375  ble_whisper.resu
+000106d0: 6c74 2e57 6869 7370 6572 5265 7375 6c74  lt.WhisperResult
+000106e0: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+000106f0: 6520 6375 7272 656e 7420 696e 7374 616e  e current instan
+00010700: 6365 2061 6674 6572 2074 6865 2063 6861  ce after the cha
+00010710: 6e67 6573 2e0d 0a0d 0a20 2020 2020 2020  nges.....       
+00010720: 204e 6f74 6573 0d0a 2020 2020 2020 2020   Notes..        
+00010730: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2049  -----..        I
+00010740: 6620 6060 6576 656e 5f73 706c 6974 203d  f ``even_split =
+00010750: 2054 7275 6560 602c 2073 6567 6d65 6e74   True``, segment
+00010760: 7320 6361 6e20 7374 696c 6c20 6578 6365  s can still exce
+00010770: 6564 2060 606d 6178 5f63 6861 7273 6060  ed ``max_chars``
+00010780: 2061 6e64 206c 6f63 6b65 6420 776f 7264   and locked word
+00010790: 7320 7769 6c6c 2062 6520 6967 6e6f 7265  s will be ignore
+000107a0: 6420 746f 2061 766f 6964 0d0a 2020 2020  d to avoid..    
+000107b0: 2020 2020 756e 6576 656e 2073 706c 6974      uneven split
+000107c0: 7469 6e67 2e0d 0a20 2020 2020 2020 2022  ting...        "
+000107d0: 2222 0d0a 2020 2020 2020 2020 6966 2066  ""..        if f
+000107e0: 6f72 6365 5f6c 656e 3a0d 0a20 2020 2020  orce_len:..     
+000107f0: 2020 2020 2020 2073 656c 662e 6d65 7267         self.merg
+00010800: 655f 616c 6c5f 7365 676d 656e 7473 2829  e_all_segments()
+00010810: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00010820: 7370 6c69 745f 7365 676d 656e 7473 280d  split_segments(.
+00010830: 0a20 2020 2020 2020 2020 2020 206c 616d  .            lam
+00010840: 6264 6120 783a 2078 2e67 6574 5f6c 656e  bda x: x.get_len
+00010850: 6774 685f 696e 6469 6365 7328 0d0a 2020  gth_indices(..  
+00010860: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00010870: 785f 6368 6172 733d 6d61 785f 6368 6172  x_chars=max_char
+00010880: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
+00010890: 2020 2020 6d61 785f 776f 7264 733d 6d61      max_words=ma
+000108a0: 785f 776f 7264 732c 0d0a 2020 2020 2020  x_words,..      
+000108b0: 2020 2020 2020 2020 2020 6576 656e 5f73            even_s
+000108c0: 706c 6974 3d65 7665 6e5f 7370 6c69 742c  plit=even_split,
+000108d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000108e0: 2020 696e 636c 7564 655f 6c6f 636b 3d69    include_lock=i
+000108f0: 6e63 6c75 6465 5f6c 6f63 6b0d 0a20 2020  nclude_lock..   
+00010900: 2020 2020 2020 2020 2029 2c0d 0a20 2020           ),..   
+00010910: 2020 2020 2020 2020 206c 6f63 6b3d 6c6f           lock=lo
+00010920: 636b 2c0d 0a20 2020 2020 2020 2020 2020  ck,..           
+00010930: 206e 6577 6c69 6e65 3d6e 6577 6c69 6e65   newline=newline
+00010940: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
+00010950: 2020 2020 2069 6620 7365 6c66 2e5f 7265       if self._re
+00010960: 6772 6f75 705f 6869 7374 6f72 793a 0d0a  group_history:..
+00010970: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010980: 2e5f 7265 6772 6f75 705f 6869 7374 6f72  ._regroup_histor
+00010990: 7920 2b3d 2027 5f27 0d0a 2020 2020 2020  y += '_'..      
+000109a0: 2020 7365 6c66 2e5f 7265 6772 6f75 705f    self._regroup_
+000109b0: 6869 7374 6f72 7920 2b3d 2028 6627 736c  history += (f'sl
+000109c0: 3d7b 6d61 785f 6368 6172 7320 6f72 2022  ={max_chars or "
+000109d0: 227d 2b7b 6d61 785f 776f 7264 7320 6f72  "}+{max_words or
+000109e0: 2022 227d 2b7b 696e 7428 6576 656e 5f73   ""}+{int(even_s
+000109f0: 706c 6974 297d 2b7b 696e 7428 666f 7263  plit)}+{int(forc
+00010a00: 655f 6c65 6e29 7d27 0d0a 2020 2020 2020  e_len)}'..      
+00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a20: 2020 2020 2020 2020 2020 2020 6627 2b7b              f'+{
+00010a30: 696e 7428 6c6f 636b 297d 2b7b 696e 7428  int(lock)}+{int(
+00010a40: 696e 636c 7564 655f 6c6f 636b 297d 2b7b  include_lock)}+{
+00010a50: 696e 7428 6e65 776c 696e 6529 7d27 290d  int(newline)}').
+00010a60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00010a70: 7365 6c66 0d0a 0d0a 2020 2020 6465 6620  self....    def 
+00010a80: 7370 6c69 745f 6279 5f64 7572 6174 696f  split_by_duratio
+00010a90: 6e28 0d0a 2020 2020 2020 2020 2020 2020  n(..            
+00010aa0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+00010ab0: 2020 206d 6178 5f64 7572 3a20 666c 6f61     max_dur: floa
+00010ac0: 742c 0d0a 2020 2020 2020 2020 2020 2020  t,..            
+00010ad0: 6576 656e 5f73 706c 6974 3a20 626f 6f6c  even_split: bool
+00010ae0: 203d 2054 7275 652c 0d0a 2020 2020 2020   = True,..      
+00010af0: 2020 2020 2020 666f 7263 655f 6c65 6e3a        force_len:
 00010b00: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
-00010b10: 2020 2020 2020 2020 2020 2020 6e65 776c              newl
-00010b20: 696e 653a 2062 6f6f 6c20 3d20 4661 6c73  ine: bool = Fals
-00010b30: 650d 0a20 2020 2029 202d 3e20 2257 6869  e..    ) -> "Whi
-00010b40: 7370 6572 5265 7375 6c74 223a 0d0a 2020  sperResult":..  
-00010b50: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00010b60: 2020 2053 706c 6974 2028 696e 2d70 6c61     Split (in-pla
-00010b70: 6365 2920 616e 7920 7365 676d 656e 7420  ce) any segment 
-00010b80: 7468 6174 2065 7863 6565 6473 2060 606d  that exceeds ``m
-00010b90: 6178 5f64 7572 6060 2069 6e74 6f20 736d  ax_dur`` into sm
-00010ba0: 616c 6c65 7220 7365 676d 656e 7473 2e0d  aller segments..
-00010bb0: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00010bc0: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
-00010bd0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
-00010be0: 2020 206d 6178 5f64 7572 203a 2066 6c6f     max_dur : flo
-00010bf0: 6174 0d0a 2020 2020 2020 2020 2020 2020  at..            
-00010c00: 4d61 7869 6d75 6d20 6475 7261 7469 6f6e  Maximum duration
-00010c10: 2028 696e 2073 6563 6f6e 6473 2920 7065   (in seconds) pe
-00010c20: 7220 7365 676d 656e 742e 0d0a 2020 2020  r segment...    
-00010c30: 2020 2020 6576 656e 5f73 706c 6974 203a      even_split :
-00010c40: 2062 6f6f 6c2c 2064 6566 6175 6c74 2054   bool, default T
-00010c50: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
-00010c60: 2057 6865 7468 6572 2074 6f20 6576 656e   Whether to even
-00010c70: 6c79 2073 706c 6974 2061 2073 6567 6d65  ly split a segme
-00010c80: 6e74 2069 6e20 6c65 6e67 7468 2069 6620  nt in length if 
-00010c90: 6974 2065 7863 6565 6473 2060 606d 6178  it exceeds ``max
-00010ca0: 5f64 7572 6060 2e0d 0a20 2020 2020 2020  _dur``...       
-00010cb0: 2066 6f72 6365 5f6c 656e 203a 2062 6f6f   force_len : boo
-00010cc0: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
-00010cd0: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-00010ce0: 6574 6865 7220 746f 2066 6f72 6365 2061  ether to force a
-00010cf0: 2063 6f6e 7374 616e 7420 6c65 6e67 7468   constant length
-00010d00: 2066 6f72 2065 6163 6820 7365 676d 656e   for each segmen
-00010d10: 7420 6578 6365 7074 2074 6865 206c 6173  t except the las
-00010d20: 7420 7365 676d 656e 742e 0d0a 2020 2020  t segment...    
-00010d30: 2020 2020 2020 2020 5468 6973 2077 696c          This wil
-00010d40: 6c20 6967 6e6f 7265 2061 6c6c 2070 7265  l ignore all pre
-00010d50: 7669 6f75 7320 6e6f 6e2d 6c6f 636b 6564  vious non-locked
-00010d60: 2073 6567 6d65 6e74 2062 6f75 6e64 6172   segment boundar
-00010d70: 6965 732e 0d0a 2020 2020 2020 2020 6c6f  ies...        lo
-00010d80: 636b 203a 2062 6f6f 6c2c 2064 6566 6175  ck : bool, defau
-00010d90: 6c74 2046 616c 7365 0d0a 2020 2020 2020  lt False..      
-00010da0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
-00010db0: 2070 7265 7665 6e74 2066 7574 7572 6520   prevent future 
-00010dc0: 7370 6c69 7473 2f6d 6572 6765 7320 6672  splits/merges fr
-00010dd0: 6f6d 2061 6c74 6572 696e 6720 6368 616e  om altering chan
-00010de0: 6765 7320 6d61 6465 2062 7920 7468 6973  ges made by this
-00010df0: 206d 6574 686f 642e 0d0a 2020 2020 2020   method...      
-00010e00: 2020 696e 636c 7564 655f 6c6f 636b 3a20    include_lock: 
-00010e10: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-00010e20: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-00010e30: 2057 6865 7468 6572 2074 6f20 696e 636c   Whether to incl
-00010e40: 7564 6520 7072 6576 696f 7573 206c 6f63  ude previous loc
-00010e50: 6b20 6265 666f 7265 2073 706c 6974 7469  k before splitti
-00010e60: 6e67 2062 6173 6564 206f 6e20 6d61 785f  ng based on max_
-00010e70: 776f 7264 732c 2069 6620 6060 6576 656e  words, if ``even
-00010e80: 5f73 706c 6974 203d 2046 616c 7365 6060  _split = False``
-00010e90: 2e0d 0a20 2020 2020 2020 2020 2020 2053  ...            S
-00010ea0: 706c 6974 7469 6e67 2077 696c 6c20 6265  plitting will be
-00010eb0: 2064 6f6e 6520 6166 7465 7220 7468 6520   done after the 
-00010ec0: 6669 7273 7420 6e6f 6e2d 6c6f 636b 6564  first non-locked
-00010ed0: 2077 6f72 6420 3e20 6060 6d61 785f 6475   word > ``max_du
-00010ee0: 7260 602e 0d0a 2020 2020 2020 2020 6e65  r``...        ne
-00010ef0: 776c 696e 653a 2062 6f6f 6c2c 2064 6566  wline: bool, def
-00010f00: 6175 6c74 2046 616c 7365 0d0a 2020 2020  ault False..    
-00010f10: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
-00010f20: 746f 2069 6e73 6572 7420 6c69 6e65 2062  to insert line b
-00010f30: 7265 616b 2061 7420 7468 6520 7370 6c69  reak at the spli
-00010f40: 7420 706f 696e 7473 2069 6e73 7465 6164  t points instead
-00010f50: 206f 6620 7370 6c69 7474 696e 6720 696e   of splitting in
-00010f60: 746f 2073 6570 6172 6174 6520 7365 676d  to separate segm
-00010f70: 656e 7473 2e0d 0a0d 0a20 2020 2020 2020  ents.....       
-00010f80: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
-00010f90: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
-00010fa0: 2020 2073 7461 626c 655f 7768 6973 7065     stable_whispe
-00010fb0: 722e 7265 7375 6c74 2e57 6869 7370 6572  r.result.Whisper
-00010fc0: 5265 7375 6c74 0d0a 2020 2020 2020 2020  Result..        
-00010fd0: 2020 2020 5468 6520 6375 7272 656e 7420      The current 
-00010fe0: 696e 7374 616e 6365 2061 6674 6572 2074  instance after t
-00010ff0: 6865 2063 6861 6e67 6573 2e0d 0a0d 0a20  he changes..... 
-00011000: 2020 2020 2020 204e 6f74 6573 0d0a 2020         Notes..  
-00011010: 2020 2020 2020 2d2d 2d2d 2d0d 0a20 2020        -----..   
-00011020: 2020 2020 2049 6620 6060 6576 656e 5f73       If ``even_s
-00011030: 706c 6974 203d 2054 7275 6560 602c 2073  plit = True``, s
-00011040: 6567 6d65 6e74 7320 6361 6e20 7374 696c  egments can stil
-00011050: 6c20 6578 6365 6564 2060 606d 6178 5f64  l exceed ``max_d
-00011060: 7572 6060 2061 6e64 206c 6f63 6b65 6420  ur`` and locked 
-00011070: 776f 7264 7320 7769 6c6c 2062 6520 6967  words will be ig
-00011080: 6e6f 7265 6420 746f 2061 766f 6964 0d0a  nored to avoid..
-00011090: 2020 2020 2020 2020 756e 6576 656e 2073          uneven s
-000110a0: 706c 6974 7469 6e67 2e0d 0a20 2020 2020  plitting...     
-000110b0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000110c0: 6966 2066 6f72 6365 5f6c 656e 3a0d 0a20  if force_len:.. 
-000110d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000110e0: 6d65 7267 655f 616c 6c5f 7365 676d 656e  merge_all_segmen
-000110f0: 7473 2829 0d0a 2020 2020 2020 2020 7365  ts()..        se
-00011100: 6c66 2e5f 7370 6c69 745f 7365 676d 656e  lf._split_segmen
-00011110: 7473 280d 0a20 2020 2020 2020 2020 2020  ts(..           
-00011120: 206c 616d 6264 6120 783a 2078 2e67 6574   lambda x: x.get
-00011130: 5f64 7572 6174 696f 6e5f 696e 6469 6365  _duration_indice
-00011140: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
-00011150: 2020 2020 6d61 785f 6475 723d 6d61 785f      max_dur=max_
-00011160: 6475 722c 0d0a 2020 2020 2020 2020 2020  dur,..          
-00011170: 2020 2020 2020 6576 656e 5f73 706c 6974        even_split
-00011180: 3d65 7665 6e5f 7370 6c69 742c 0d0a 2020  =even_split,..  
-00011190: 2020 2020 2020 2020 2020 2020 2020 696e                in
-000111a0: 636c 7564 655f 6c6f 636b 3d69 6e63 6c75  clude_lock=inclu
-000111b0: 6465 5f6c 6f63 6b0d 0a20 2020 2020 2020  de_lock..       
-000111c0: 2020 2020 2029 2c0d 0a20 2020 2020 2020       ),..       
-000111d0: 2020 2020 206c 6f63 6b3d 6c6f 636b 2c0d       lock=lock,.
-000111e0: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
-000111f0: 6c69 6e65 3d6e 6577 6c69 6e65 0d0a 2020  line=newline..  
-00011200: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00011210: 2069 6620 7365 6c66 2e5f 7265 6772 6f75   if self._regrou
-00011220: 705f 6869 7374 6f72 793a 0d0a 2020 2020  p_history:..    
-00011230: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
-00011240: 6772 6f75 705f 6869 7374 6f72 7920 2b3d  group_history +=
-00011250: 2027 5f27 0d0a 2020 2020 2020 2020 7365   '_'..        se
+00010b10: 2020 2020 2020 2020 2020 2020 6c6f 636b              lock
+00010b20: 3a20 626f 6f6c 203d 2046 616c 7365 2c0d  : bool = False,.
+00010b30: 0a20 2020 2020 2020 2020 2020 2069 6e63  .            inc
+00010b40: 6c75 6465 5f6c 6f63 6b3a 2062 6f6f 6c20  lude_lock: bool 
+00010b50: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
+00010b60: 2020 2020 2020 6e65 776c 696e 653a 2062        newline: b
+00010b70: 6f6f 6c20 3d20 4661 6c73 650d 0a20 2020  ool = False..   
+00010b80: 2029 202d 3e20 2257 6869 7370 6572 5265   ) -> "WhisperRe
+00010b90: 7375 6c74 223a 0d0a 2020 2020 2020 2020  sult":..        
+00010ba0: 2222 220d 0a20 2020 2020 2020 2053 706c  """..        Spl
+00010bb0: 6974 2028 696e 2d70 6c61 6365 2920 616e  it (in-place) an
+00010bc0: 7920 7365 676d 656e 7420 7468 6174 2065  y segment that e
+00010bd0: 7863 6565 6473 2060 606d 6178 5f64 7572  xceeds ``max_dur
+00010be0: 6060 2069 6e74 6f20 736d 616c 6c65 7220  `` into smaller 
+00010bf0: 7365 676d 656e 7473 2e0d 0a0d 0a20 2020  segments.....   
+00010c00: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
+00010c10: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00010c20: 2d2d 2d0d 0a20 2020 2020 2020 206d 6178  ---..        max
+00010c30: 5f64 7572 203a 2066 6c6f 6174 0d0a 2020  _dur : float..  
+00010c40: 2020 2020 2020 2020 2020 4d61 7869 6d75            Maximu
+00010c50: 6d20 6475 7261 7469 6f6e 2028 696e 2073  m duration (in s
+00010c60: 6563 6f6e 6473 2920 7065 7220 7365 676d  econds) per segm
+00010c70: 656e 742e 0d0a 2020 2020 2020 2020 6576  ent...        ev
+00010c80: 656e 5f73 706c 6974 203a 2062 6f6f 6c2c  en_split : bool,
+00010c90: 2064 6566 6175 6c74 2054 7275 650d 0a20   default True.. 
+00010ca0: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+00010cb0: 6572 2074 6f20 6576 656e 6c79 2073 706c  er to evenly spl
+00010cc0: 6974 2061 2073 6567 6d65 6e74 2069 6e20  it a segment in 
+00010cd0: 6c65 6e67 7468 2069 6620 6974 2065 7863  length if it exc
+00010ce0: 6565 6473 2060 606d 6178 5f64 7572 6060  eeds ``max_dur``
+00010cf0: 2e0d 0a20 2020 2020 2020 2066 6f72 6365  ...        force
+00010d00: 5f6c 656e 203a 2062 6f6f 6c2c 2064 6566  _len : bool, def
+00010d10: 6175 6c74 2046 616c 7365 0d0a 2020 2020  ault False..    
+00010d20: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
+00010d30: 746f 2066 6f72 6365 2061 2063 6f6e 7374  to force a const
+00010d40: 616e 7420 6c65 6e67 7468 2066 6f72 2065  ant length for e
+00010d50: 6163 6820 7365 676d 656e 7420 6578 6365  ach segment exce
+00010d60: 7074 2074 6865 206c 6173 7420 7365 676d  pt the last segm
+00010d70: 656e 742e 0d0a 2020 2020 2020 2020 2020  ent...          
+00010d80: 2020 5468 6973 2077 696c 6c20 6967 6e6f    This will igno
+00010d90: 7265 2061 6c6c 2070 7265 7669 6f75 7320  re all previous 
+00010da0: 6e6f 6e2d 6c6f 636b 6564 2073 6567 6d65  non-locked segme
+00010db0: 6e74 2062 6f75 6e64 6172 6965 732e 0d0a  nt boundaries...
+00010dc0: 2020 2020 2020 2020 6c6f 636b 203a 2062          lock : b
+00010dd0: 6f6f 6c2c 2064 6566 6175 6c74 2046 616c  ool, default Fal
+00010de0: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
+00010df0: 5768 6574 6865 7220 746f 2070 7265 7665  Whether to preve
+00010e00: 6e74 2066 7574 7572 6520 7370 6c69 7473  nt future splits
+00010e10: 2f6d 6572 6765 7320 6672 6f6d 2061 6c74  /merges from alt
+00010e20: 6572 696e 6720 6368 616e 6765 7320 6d61  ering changes ma
+00010e30: 6465 2062 7920 7468 6973 206d 6574 686f  de by this metho
+00010e40: 642e 0d0a 2020 2020 2020 2020 696e 636c  d...        incl
+00010e50: 7564 655f 6c6f 636b 3a20 626f 6f6c 2c20  ude_lock: bool, 
+00010e60: 6465 6661 756c 7420 4661 6c73 650d 0a20  default False.. 
+00010e70: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+00010e80: 6572 2074 6f20 696e 636c 7564 6520 7072  er to include pr
+00010e90: 6576 696f 7573 206c 6f63 6b20 6265 666f  evious lock befo
+00010ea0: 7265 2073 706c 6974 7469 6e67 2062 6173  re splitting bas
+00010eb0: 6564 206f 6e20 6d61 785f 776f 7264 732c  ed on max_words,
+00010ec0: 2069 6620 6060 6576 656e 5f73 706c 6974   if ``even_split
+00010ed0: 203d 2046 616c 7365 6060 2e0d 0a20 2020   = False``...   
+00010ee0: 2020 2020 2020 2020 2053 706c 6974 7469           Splitti
+00010ef0: 6e67 2077 696c 6c20 6265 2064 6f6e 6520  ng will be done 
+00010f00: 6166 7465 7220 7468 6520 6669 7273 7420  after the first 
+00010f10: 6e6f 6e2d 6c6f 636b 6564 2077 6f72 6420  non-locked word 
+00010f20: 3e20 6060 6d61 785f 6475 7260 602e 0d0a  > ``max_dur``...
+00010f30: 2020 2020 2020 2020 6e65 776c 696e 653a          newline:
+00010f40: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
+00010f50: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
+00010f60: 2020 5768 6574 6865 7220 746f 2069 6e73    Whether to ins
+00010f70: 6572 7420 6c69 6e65 2062 7265 616b 2061  ert line break a
+00010f80: 7420 7468 6520 7370 6c69 7420 706f 696e  t the split poin
+00010f90: 7473 2069 6e73 7465 6164 206f 6620 7370  ts instead of sp
+00010fa0: 6c69 7474 696e 6720 696e 746f 2073 6570  litting into sep
+00010fb0: 6172 6174 6520 7365 676d 656e 7473 2e0d  arate segments..
+00010fc0: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00010fd0: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
+00010fe0: 2d2d 2d0d 0a20 2020 2020 2020 2073 7461  ---..        sta
+00010ff0: 626c 655f 7768 6973 7065 722e 7265 7375  ble_whisper.resu
+00011000: 6c74 2e57 6869 7370 6572 5265 7375 6c74  lt.WhisperResult
+00011010: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00011020: 6520 6375 7272 656e 7420 696e 7374 616e  e current instan
+00011030: 6365 2061 6674 6572 2074 6865 2063 6861  ce after the cha
+00011040: 6e67 6573 2e0d 0a0d 0a20 2020 2020 2020  nges.....       
+00011050: 204e 6f74 6573 0d0a 2020 2020 2020 2020   Notes..        
+00011060: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2049  -----..        I
+00011070: 6620 6060 6576 656e 5f73 706c 6974 203d  f ``even_split =
+00011080: 2054 7275 6560 602c 2073 6567 6d65 6e74   True``, segment
+00011090: 7320 6361 6e20 7374 696c 6c20 6578 6365  s can still exce
+000110a0: 6564 2060 606d 6178 5f64 7572 6060 2061  ed ``max_dur`` a
+000110b0: 6e64 206c 6f63 6b65 6420 776f 7264 7320  nd locked words 
+000110c0: 7769 6c6c 2062 6520 6967 6e6f 7265 6420  will be ignored 
+000110d0: 746f 2061 766f 6964 0d0a 2020 2020 2020  to avoid..      
+000110e0: 2020 756e 6576 656e 2073 706c 6974 7469    uneven splitti
+000110f0: 6e67 2e0d 0a20 2020 2020 2020 2022 2222  ng...        """
+00011100: 0d0a 2020 2020 2020 2020 6966 2066 6f72  ..        if for
+00011110: 6365 5f6c 656e 3a0d 0a20 2020 2020 2020  ce_len:..       
+00011120: 2020 2020 2073 656c 662e 6d65 7267 655f       self.merge_
+00011130: 616c 6c5f 7365 676d 656e 7473 2829 0d0a  all_segments()..
+00011140: 2020 2020 2020 2020 7365 6c66 2e5f 7370          self._sp
+00011150: 6c69 745f 7365 676d 656e 7473 280d 0a20  lit_segments(.. 
+00011160: 2020 2020 2020 2020 2020 206c 616d 6264             lambd
+00011170: 6120 783a 2078 2e67 6574 5f64 7572 6174  a x: x.get_durat
+00011180: 696f 6e5f 696e 6469 6365 7328 0d0a 2020  ion_indices(..  
+00011190: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+000111a0: 785f 6475 723d 6d61 785f 6475 722c 0d0a  x_dur=max_dur,..
+000111b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111c0: 6576 656e 5f73 706c 6974 3d65 7665 6e5f  even_split=even_
+000111d0: 7370 6c69 742c 0d0a 2020 2020 2020 2020  split,..        
+000111e0: 2020 2020 2020 2020 696e 636c 7564 655f          include_
+000111f0: 6c6f 636b 3d69 6e63 6c75 6465 5f6c 6f63  lock=include_loc
+00011200: 6b0d 0a20 2020 2020 2020 2020 2020 2029  k..            )
+00011210: 2c0d 0a20 2020 2020 2020 2020 2020 206c  ,..            l
+00011220: 6f63 6b3d 6c6f 636b 2c0d 0a20 2020 2020  ock=lock,..     
+00011230: 2020 2020 2020 206e 6577 6c69 6e65 3d6e         newline=n
+00011240: 6577 6c69 6e65 0d0a 2020 2020 2020 2020  ewline..        
+00011250: 290d 0a20 2020 2020 2020 2069 6620 7365  )..        if se
 00011260: 6c66 2e5f 7265 6772 6f75 705f 6869 7374  lf._regroup_hist
-00011270: 6f72 7920 2b3d 2028 6627 7364 3d7b 6d61  ory += (f'sd={ma
-00011280: 785f 6475 727d 2b7b 696e 7428 6576 656e  x_dur}+{int(even
-00011290: 5f73 706c 6974 297d 2b7b 696e 7428 666f  _split)}+{int(fo
-000112a0: 7263 655f 6c65 6e29 7d27 0d0a 2020 2020  rce_len)}'..    
-000112b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112c0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-000112d0: 2b7b 696e 7428 6c6f 636b 297d 2b7b 696e  +{int(lock)}+{in
-000112e0: 7428 696e 636c 7564 655f 6c6f 636b 297d  t(include_lock)}
-000112f0: 2b7b 696e 7428 6e65 776c 696e 6529 7d27  +{int(newline)}'
-00011300: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00011310: 6e20 7365 6c66 0d0a 0d0a 2020 2020 6465  n self....    de
-00011320: 6620 636c 616d 705f 6d61 7828 0d0a 2020  f clamp_max(..  
-00011330: 2020 2020 2020 2020 2020 7365 6c66 2c0d            self,.
-00011340: 0a20 2020 2020 2020 2020 2020 206d 6564  .            med
-00011350: 6975 6d5f 6661 6374 6f72 3a20 666c 6f61  ium_factor: floa
-00011360: 7420 3d20 322e 352c 0d0a 2020 2020 2020  t = 2.5,..      
-00011370: 2020 2020 2020 6d61 785f 6475 723a 2066        max_dur: f
-00011380: 6c6f 6174 203d 204e 6f6e 652c 0d0a 2020  loat = None,..  
-00011390: 2020 2020 2020 2020 2020 636c 6970 5f73            clip_s
-000113a0: 7461 7274 3a20 4f70 7469 6f6e 616c 5b62  tart: Optional[b
-000113b0: 6f6f 6c5d 203d 204e 6f6e 652c 0d0a 2020  ool] = None,..  
-000113c0: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
-000113d0: 653a 2062 6f6f 6c20 3d20 4661 6c73 650d  e: bool = False.
-000113e0: 0a20 2020 2029 202d 3e20 2257 6869 7370  .    ) -> "Whisp
-000113f0: 6572 5265 7375 6c74 223a 0d0a 2020 2020  erResult":..    
-00011400: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00011410: 2043 6c61 6d70 2061 6c6c 2077 6f72 6420   Clamp all word 
-00011420: 6475 7261 7469 6f6e 7320 6162 6f76 6520  durations above 
-00011430: 6365 7274 6169 6e20 7661 6c75 652e 0d0a  certain value...
-00011440: 0d0a 2020 2020 2020 2020 5468 6973 2069  ..        This i
-00011450: 7320 6d6f 7374 2065 6666 6563 7469 7665  s most effective
-00011460: 2077 6865 6e20 6170 706c 6965 6420 6265   when applied be
-00011470: 666f 7265 2061 6e64 2061 6674 6572 206f  fore and after o
-00011480: 7468 6572 2072 6567 726f 7570 206f 7065  ther regroup ope
-00011490: 7261 7469 6f6e 732e 0d0a 0d0a 2020 2020  rations.....    
-000114a0: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
-000114b0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-000114c0: 2d2d 0d0a 2020 2020 2020 2020 6d65 6469  --..        medi
-000114d0: 756d 5f66 6163 746f 7220 3a20 666c 6f61  um_factor : floa
-000114e0: 742c 2064 6566 6175 6c74 2032 2e35 0d0a  t, default 2.5..
-000114f0: 2020 2020 2020 2020 2020 2020 436c 616d              Clam
-00011500: 7020 6475 7261 7469 6f6e 7320 6162 6f76  p durations abov
-00011510: 6520 2860 606d 6564 6975 6d5f 6661 6374  e (``medium_fact
-00011520: 6f72 6060 202a 206d 6564 6975 6d20 6475  or`` * medium du
-00011530: 7261 7469 6f6e 2920 7065 7220 7365 676d  ration) per segm
-00011540: 656e 742e 0d0a 2020 2020 2020 2020 2020  ent...          
-00011550: 2020 4966 2060 606d 6564 6975 6d5f 6661    If ``medium_fa
-00011560: 6374 6f72 203d 204e 6f6e 652f 3060 6020  ctor = None/0`` 
-00011570: 6f72 2073 6567 6d65 6e74 2068 6173 206c  or segment has l
-00011580: 6573 7320 7468 616e 2033 2077 6f72 6473  ess than 3 words
-00011590: 2c20 6974 2077 696c 6c20 6265 2069 676e  , it will be ign
-000115a0: 6f72 6564 2061 6e64 2075 7365 206f 6e6c  ored and use onl
-000115b0: 7920 6060 6d61 785f 6475 7260 602e 0d0a  y ``max_dur``...
-000115c0: 2020 2020 2020 2020 6d61 785f 6475 7220          max_dur 
-000115d0: 3a20 666c 6f61 742c 206f 7074 696f 6e61  : float, optiona
-000115e0: 6c0d 0a20 2020 2020 2020 2020 2020 2043  l..            C
-000115f0: 6c61 6d70 2064 7572 6174 696f 6e73 2061  lamp durations a
-00011600: 626f 7665 2060 606d 6178 5f64 7572 6060  bove ``max_dur``
-00011610: 2e0d 0a20 2020 2020 2020 2063 6c69 705f  ...        clip_
-00011620: 7374 6172 7420 3a20 626f 6f6c 206f 7220  start : bool or 
-00011630: 4e6f 6e65 2c20 6465 6661 756c 7420 4e6f  None, default No
-00011640: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
-00011650: 5768 6574 6865 7220 746f 2063 6c61 6d70  Whether to clamp
-00011660: 2074 6865 2073 7461 7274 206f 6620 6120   the start of a 
-00011670: 776f 7264 2e20 4966 2060 604e 6f6e 6560  word. If ``None`
-00011680: 602c 2063 6c61 6d70 2074 6865 2073 7461  `, clamp the sta
-00011690: 7274 206f 6620 6669 7273 7420 776f 7264  rt of first word
-000116a0: 2061 6e64 2065 6e64 206f 6620 6c61 7374   and end of last
-000116b0: 2077 6f72 6420 7065 720d 0a20 2020 2020   word per..     
-000116c0: 2020 2020 2020 2073 6567 6d65 6e74 2e0d         segment..
-000116d0: 0a20 2020 2020 2020 2076 6572 626f 7365  .        verbose
-000116e0: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-000116f0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00011700: 2020 2020 5768 6574 6865 7220 746f 2070      Whether to p
-00011710: 7269 6e74 206f 7574 2074 6865 2074 696d  rint out the tim
-00011720: 6573 7461 6d70 2063 6861 6e67 6573 2e0d  estamp changes..
-00011730: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00011740: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
-00011750: 2d2d 2d0d 0a20 2020 2020 2020 2073 7461  ---..        sta
-00011760: 626c 655f 7768 6973 7065 722e 7265 7375  ble_whisper.resu
-00011770: 6c74 2e57 6869 7370 6572 5265 7375 6c74  lt.WhisperResult
-00011780: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00011790: 6520 6375 7272 656e 7420 696e 7374 616e  e current instan
-000117a0: 6365 2061 6674 6572 2074 6865 2063 6861  ce after the cha
-000117b0: 6e67 6573 2e0d 0a20 2020 2020 2020 2022  nges...        "
-000117c0: 2222 0d0a 2020 2020 2020 2020 6966 206e  ""..        if n
-000117d0: 6f74 2028 6d65 6469 756d 5f66 6163 746f  ot (medium_facto
-000117e0: 7220 6f72 206d 6178 5f64 7572 293a 0d0a  r or max_dur):..
-000117f0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00011800: 6520 5661 6c75 6545 7272 6f72 2827 4174  e ValueError('At
-00011810: 206c 6561 7374 206f 6e65 206f 6620 666f   least one of fo
-00011820: 6c6c 6f77 696e 6720 6172 6775 6d65 6e74  llowing argument
-00011830: 7320 7265 7175 6972 6573 206e 6f6e 2d7a  s requires non-z
-00011840: 6572 6f20 7661 6c75 653a 206d 6564 6975  ero value: mediu
-00011850: 6d5f 6661 6374 6f72 3b20 6d61 785f 6475  m_factor; max_du
-00011860: 7227 290d 0a0d 0a20 2020 2020 2020 2069  r')....        i
-00011870: 6620 6e6f 7420 7365 6c66 2e68 6173 5f77  f not self.has_w
-00011880: 6f72 6473 3a0d 0a20 2020 2020 2020 2020  ords:..         
-00011890: 2020 2077 6172 6e69 6e67 732e 7761 726e     warnings.warn
-000118a0: 2827 4361 6e6e 6f74 2063 6c61 6d70 2064  ('Cannot clamp d
-000118b0: 7565 2074 6f20 6d69 7373 696e 672f 6e6f  ue to missing/no
-000118c0: 2077 6f72 642d 7469 6d65 7374 616d 7073   word-timestamps
-000118d0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-000118e0: 7265 7475 726e 2073 656c 660d 0a0d 0a20  return self.... 
-000118f0: 2020 2020 2020 2066 6f72 2073 6567 2069         for seg i
-00011900: 6e20 7365 6c66 2e73 6567 6d65 6e74 733a  n self.segments:
-00011910: 0d0a 2020 2020 2020 2020 2020 2020 6375  ..            cu
-00011920: 7272 5f6d 6178 5f64 7572 203d 204e 6f6e  rr_max_dur = Non
-00011930: 650d 0a20 2020 2020 2020 2020 2020 2069  e..            i
-00011940: 6620 6d65 6469 756d 5f66 6163 746f 7220  f medium_factor 
-00011950: 616e 6420 6c65 6e28 7365 672e 776f 7264  and len(seg.word
-00011960: 7329 203e 2032 3a0d 0a20 2020 2020 2020  s) > 2:..       
-00011970: 2020 2020 2020 2020 2064 7572 6174 696f           duratio
-00011980: 6e73 203d 206e 702e 6172 7261 7928 5b77  ns = np.array([w
-00011990: 6f72 642e 6475 7261 7469 6f6e 2066 6f72  ord.duration for
-000119a0: 2077 6f72 6420 696e 2073 6567 2e77 6f72   word in seg.wor
-000119b0: 6473 5d29 0d0a 2020 2020 2020 2020 2020  ds])..          
-000119c0: 2020 2020 2020 6475 7261 7469 6f6e 732e        durations.
-000119d0: 736f 7274 2829 0d0a 2020 2020 2020 2020  sort()..        
-000119e0: 2020 2020 2020 2020 6375 7272 5f6d 6178          curr_max
-000119f0: 5f64 7572 203d 206d 6564 6975 6d5f 6661  _dur = medium_fa
-00011a00: 6374 6f72 202a 2064 7572 6174 696f 6e73  ctor * durations
-00011a10: 5b6c 656e 2864 7572 6174 696f 6e73 292f  [len(durations)/
-00011a20: 2f32 202b 2031 5d0d 0a0d 0a20 2020 2020  /2 + 1]....     
-00011a30: 2020 2020 2020 2069 6620 6d61 785f 6475         if max_du
-00011a40: 7220 616e 6420 286e 6f74 2063 7572 725f  r and (not curr_
-00011a50: 6d61 785f 6475 7220 6f72 2063 7572 725f  max_dur or curr_
-00011a60: 6d61 785f 6475 7220 3e20 6d61 785f 6475  max_dur > max_du
-00011a70: 7229 3a0d 0a20 2020 2020 2020 2020 2020  r):..           
-00011a80: 2020 2020 2063 7572 725f 6d61 785f 6475       curr_max_du
-00011a90: 7220 3d20 6d61 785f 6475 720d 0a0d 0a20  r = max_dur.... 
-00011aa0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00011ab0: 7420 6375 7272 5f6d 6178 5f64 7572 3a0d  t curr_max_dur:.
-00011ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011ad0: 2063 6f6e 7469 6e75 650d 0a0d 0a20 2020   continue....   
-00011ae0: 2020 2020 2020 2020 2069 6620 636c 6970           if clip
-00011af0: 5f73 7461 7274 2069 7320 4e6f 6e65 3a0d  _start is None:.
-00011b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011b10: 2073 6567 2e77 6f72 6473 5b30 5d2e 636c   seg.words[0].cl
-00011b20: 616d 705f 6d61 7828 6375 7272 5f6d 6178  amp_max(curr_max
-00011b30: 5f64 7572 2c20 636c 6970 5f73 7461 7274  _dur, clip_start
-00011b40: 3d54 7275 652c 2076 6572 626f 7365 3d76  =True, verbose=v
-00011b50: 6572 626f 7365 290d 0a20 2020 2020 2020  erbose)..       
-00011b60: 2020 2020 2020 2020 2073 6567 2e77 6f72           seg.wor
-00011b70: 6473 5b2d 315d 2e63 6c61 6d70 5f6d 6178  ds[-1].clamp_max
-00011b80: 2863 7572 725f 6d61 785f 6475 722c 2063  (curr_max_dur, c
-00011b90: 6c69 705f 7374 6172 743d 4661 6c73 652c  lip_start=False,
-00011ba0: 2076 6572 626f 7365 3d76 6572 626f 7365   verbose=verbose
-00011bb0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00011bc0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00011bd0: 2020 2020 2020 666f 7220 692c 2077 6f72        for i, wor
-00011be0: 6420 696e 2065 6e75 6d65 7261 7465 2873  d in enumerate(s
-00011bf0: 6567 2e77 6f72 6473 293a 0d0a 2020 2020  eg.words):..    
-00011c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c10: 776f 7264 2e63 6c61 6d70 5f6d 6178 2863  word.clamp_max(c
-00011c20: 7572 725f 6d61 785f 6475 722c 2063 6c69  urr_max_dur, cli
-00011c30: 705f 7374 6172 743d 636c 6970 5f73 7461  p_start=clip_sta
-00011c40: 7274 2c20 7665 7262 6f73 653d 7665 7262  rt, verbose=verb
-00011c50: 6f73 6529 0d0a 0d0a 2020 2020 2020 2020  ose)....        
-00011c60: 6966 2073 656c 662e 5f72 6567 726f 7570  if self._regroup
-00011c70: 5f68 6973 746f 7279 3a0d 0a20 2020 2020  _history:..     
-00011c80: 2020 2020 2020 2073 656c 662e 5f72 6567         self._reg
-00011c90: 726f 7570 5f68 6973 746f 7279 202b 3d20  roup_history += 
-00011ca0: 275f 270d 0a20 2020 2020 2020 2073 656c  '_'..        sel
+00011270: 6f72 793a 0d0a 2020 2020 2020 2020 2020  ory:..          
+00011280: 2020 7365 6c66 2e5f 7265 6772 6f75 705f    self._regroup_
+00011290: 6869 7374 6f72 7920 2b3d 2027 5f27 0d0a  history += '_'..
+000112a0: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
+000112b0: 6772 6f75 705f 6869 7374 6f72 7920 2b3d  group_history +=
+000112c0: 2028 6627 7364 3d7b 6d61 785f 6475 727d   (f'sd={max_dur}
+000112d0: 2b7b 696e 7428 6576 656e 5f73 706c 6974  +{int(even_split
+000112e0: 297d 2b7b 696e 7428 666f 7263 655f 6c65  )}+{int(force_le
+000112f0: 6e29 7d27 0d0a 2020 2020 2020 2020 2020  n)}'..          
+00011300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011310: 2020 2020 2020 2020 6627 2b7b 696e 7428          f'+{int(
+00011320: 6c6f 636b 297d 2b7b 696e 7428 696e 636c  lock)}+{int(incl
+00011330: 7564 655f 6c6f 636b 297d 2b7b 696e 7428  ude_lock)}+{int(
+00011340: 6e65 776c 696e 6529 7d27 290d 0a20 2020  newline)}')..   
+00011350: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00011360: 0d0a 0d0a 2020 2020 6465 6620 636c 616d  ....    def clam
+00011370: 705f 6d61 7828 0d0a 2020 2020 2020 2020  p_max(..        
+00011380: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
+00011390: 2020 2020 2020 206d 6564 6975 6d5f 6661         medium_fa
+000113a0: 6374 6f72 3a20 666c 6f61 7420 3d20 322e  ctor: float = 2.
+000113b0: 352c 0d0a 2020 2020 2020 2020 2020 2020  5,..            
+000113c0: 6d61 785f 6475 723a 2066 6c6f 6174 203d  max_dur: float =
+000113d0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+000113e0: 2020 2020 636c 6970 5f73 7461 7274 3a20      clip_start: 
+000113f0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+00011400: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+00011410: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
+00011420: 6c20 3d20 4661 6c73 650d 0a20 2020 2029  l = False..    )
+00011430: 202d 3e20 2257 6869 7370 6572 5265 7375   -> "WhisperResu
+00011440: 6c74 223a 0d0a 2020 2020 2020 2020 2222  lt":..        ""
+00011450: 220d 0a20 2020 2020 2020 2043 6c61 6d70  "..        Clamp
+00011460: 2061 6c6c 2077 6f72 6420 6475 7261 7469   all word durati
+00011470: 6f6e 7320 6162 6f76 6520 6365 7274 6169  ons above certai
+00011480: 6e20 7661 6c75 652e 0d0a 0d0a 2020 2020  n value.....    
+00011490: 2020 2020 5468 6973 2069 7320 6d6f 7374      This is most
+000114a0: 2065 6666 6563 7469 7665 2077 6865 6e20   effective when 
+000114b0: 6170 706c 6965 6420 6265 666f 7265 2061  applied before a
+000114c0: 6e64 2061 6674 6572 206f 7468 6572 2072  nd after other r
+000114d0: 6567 726f 7570 206f 7065 7261 7469 6f6e  egroup operation
+000114e0: 732e 0d0a 0d0a 2020 2020 2020 2020 5061  s.....        Pa
+000114f0: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
+00011500: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
+00011510: 2020 2020 2020 6d65 6469 756d 5f66 6163        medium_fac
+00011520: 746f 7220 3a20 666c 6f61 742c 2064 6566  tor : float, def
+00011530: 6175 6c74 2032 2e35 0d0a 2020 2020 2020  ault 2.5..      
+00011540: 2020 2020 2020 436c 616d 7020 6475 7261        Clamp dura
+00011550: 7469 6f6e 7320 6162 6f76 6520 2860 606d  tions above (``m
+00011560: 6564 6975 6d5f 6661 6374 6f72 6060 202a  edium_factor`` *
+00011570: 206d 6564 6975 6d20 6475 7261 7469 6f6e   medium duration
+00011580: 2920 7065 7220 7365 676d 656e 742e 0d0a  ) per segment...
+00011590: 2020 2020 2020 2020 2020 2020 4966 2060              If `
+000115a0: 606d 6564 6975 6d5f 6661 6374 6f72 203d  `medium_factor =
+000115b0: 204e 6f6e 652f 3060 6020 6f72 2073 6567   None/0`` or seg
+000115c0: 6d65 6e74 2068 6173 206c 6573 7320 7468  ment has less th
+000115d0: 616e 2033 2077 6f72 6473 2c20 6974 2077  an 3 words, it w
+000115e0: 696c 6c20 6265 2069 676e 6f72 6564 2061  ill be ignored a
+000115f0: 6e64 2075 7365 206f 6e6c 7920 6060 6d61  nd use only ``ma
+00011600: 785f 6475 7260 602e 0d0a 2020 2020 2020  x_dur``...      
+00011610: 2020 6d61 785f 6475 7220 3a20 666c 6f61    max_dur : floa
+00011620: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
+00011630: 2020 2020 2020 2020 2043 6c61 6d70 2064           Clamp d
+00011640: 7572 6174 696f 6e73 2061 626f 7665 2060  urations above `
+00011650: 606d 6178 5f64 7572 6060 2e0d 0a20 2020  `max_dur``...   
+00011660: 2020 2020 2063 6c69 705f 7374 6172 7420       clip_start 
+00011670: 3a20 626f 6f6c 206f 7220 4e6f 6e65 2c20  : bool or None, 
+00011680: 6465 6661 756c 7420 4e6f 6e65 0d0a 2020  default None..  
+00011690: 2020 2020 2020 2020 2020 5768 6574 6865            Whethe
+000116a0: 7220 746f 2063 6c61 6d70 2074 6865 2073  r to clamp the s
+000116b0: 7461 7274 206f 6620 6120 776f 7264 2e20  tart of a word. 
+000116c0: 4966 2060 604e 6f6e 6560 602c 2063 6c61  If ``None``, cla
+000116d0: 6d70 2074 6865 2073 7461 7274 206f 6620  mp the start of 
+000116e0: 6669 7273 7420 776f 7264 2061 6e64 2065  first word and e
+000116f0: 6e64 206f 6620 6c61 7374 2077 6f72 6420  nd of last word 
+00011700: 7065 720d 0a20 2020 2020 2020 2020 2020  per..           
+00011710: 2073 6567 6d65 6e74 2e0d 0a20 2020 2020   segment...     
+00011720: 2020 2076 6572 626f 7365 203a 2062 6f6f     verbose : boo
+00011730: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
+00011740: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
+00011750: 6574 6865 7220 746f 2070 7269 6e74 206f  ether to print o
+00011760: 7574 2074 6865 2074 696d 6573 7461 6d70  ut the timestamp
+00011770: 2063 6861 6e67 6573 2e0d 0a0d 0a20 2020   changes.....   
+00011780: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
+00011790: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
+000117a0: 2020 2020 2020 2073 7461 626c 655f 7768         stable_wh
+000117b0: 6973 7065 722e 7265 7375 6c74 2e57 6869  isper.result.Whi
+000117c0: 7370 6572 5265 7375 6c74 0d0a 2020 2020  sperResult..    
+000117d0: 2020 2020 2020 2020 5468 6520 6375 7272          The curr
+000117e0: 656e 7420 696e 7374 616e 6365 2061 6674  ent instance aft
+000117f0: 6572 2074 6865 2063 6861 6e67 6573 2e0d  er the changes..
+00011800: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00011810: 2020 2020 2020 6966 206e 6f74 2028 6d65        if not (me
+00011820: 6469 756d 5f66 6163 746f 7220 6f72 206d  dium_factor or m
+00011830: 6178 5f64 7572 293a 0d0a 2020 2020 2020  ax_dur):..      
+00011840: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00011850: 6545 7272 6f72 2827 4174 206c 6561 7374  eError('At least
+00011860: 206f 6e65 206f 6620 666f 6c6c 6f77 696e   one of followin
+00011870: 6720 6172 6775 6d65 6e74 7320 7265 7175  g arguments requ
+00011880: 6972 6573 206e 6f6e 2d7a 6572 6f20 7661  ires non-zero va
+00011890: 6c75 653a 206d 6564 6975 6d5f 6661 6374  lue: medium_fact
+000118a0: 6f72 3b20 6d61 785f 6475 7227 290d 0a0d  or; max_dur')...
+000118b0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000118c0: 7365 6c66 2e68 6173 5f77 6f72 6473 3a0d  self.has_words:.
+000118d0: 0a20 2020 2020 2020 2020 2020 2077 6172  .            war
+000118e0: 6e69 6e67 732e 7761 726e 2827 4361 6e6e  nings.warn('Cann
+000118f0: 6f74 2063 6c61 6d70 2064 7565 2074 6f20  ot clamp due to 
+00011900: 6d69 7373 696e 672f 6e6f 2077 6f72 642d  missing/no word-
+00011910: 7469 6d65 7374 616d 7073 2729 0d0a 2020  timestamps')..  
+00011920: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00011930: 2073 656c 660d 0a0d 0a20 2020 2020 2020   self....       
+00011940: 2066 6f72 2073 6567 2069 6e20 7365 6c66   for seg in self
+00011950: 2e73 6567 6d65 6e74 733a 0d0a 2020 2020  .segments:..    
+00011960: 2020 2020 2020 2020 6375 7272 5f6d 6178          curr_max
+00011970: 5f64 7572 203d 204e 6f6e 650d 0a20 2020  _dur = None..   
+00011980: 2020 2020 2020 2020 2069 6620 6d65 6469           if medi
+00011990: 756d 5f66 6163 746f 7220 616e 6420 6c65  um_factor and le
+000119a0: 6e28 7365 672e 776f 7264 7329 203e 2032  n(seg.words) > 2
+000119b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000119c0: 2020 2064 7572 6174 696f 6e73 203d 206e     durations = n
+000119d0: 702e 6172 7261 7928 5b77 6f72 642e 6475  p.array([word.du
+000119e0: 7261 7469 6f6e 2066 6f72 2077 6f72 6420  ration for word 
+000119f0: 696e 2073 6567 2e77 6f72 6473 5d29 0d0a  in seg.words])..
+00011a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a10: 6475 7261 7469 6f6e 732e 736f 7274 2829  durations.sort()
+00011a20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011a30: 2020 6375 7272 5f6d 6178 5f64 7572 203d    curr_max_dur =
+00011a40: 206d 6564 6975 6d5f 6661 6374 6f72 202a   medium_factor *
+00011a50: 2064 7572 6174 696f 6e73 5b6c 656e 2864   durations[len(d
+00011a60: 7572 6174 696f 6e73 292f 2f32 202b 2031  urations)//2 + 1
+00011a70: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00011a80: 2069 6620 6d61 785f 6475 7220 616e 6420   if max_dur and 
+00011a90: 286e 6f74 2063 7572 725f 6d61 785f 6475  (not curr_max_du
+00011aa0: 7220 6f72 2063 7572 725f 6d61 785f 6475  r or curr_max_du
+00011ab0: 7220 3e20 6d61 785f 6475 7229 3a0d 0a20  r > max_dur):.. 
+00011ac0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00011ad0: 7572 725f 6d61 785f 6475 7220 3d20 6d61  urr_max_dur = ma
+00011ae0: 785f 6475 720d 0a0d 0a20 2020 2020 2020  x_dur....       
+00011af0: 2020 2020 2069 6620 6e6f 7420 6375 7272       if not curr
+00011b00: 5f6d 6178 5f64 7572 3a0d 0a20 2020 2020  _max_dur:..     
+00011b10: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00011b20: 6e75 650d 0a0d 0a20 2020 2020 2020 2020  nue....         
+00011b30: 2020 2069 6620 636c 6970 5f73 7461 7274     if clip_start
+00011b40: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00011b50: 2020 2020 2020 2020 2020 2073 6567 2e77             seg.w
+00011b60: 6f72 6473 5b30 5d2e 636c 616d 705f 6d61  ords[0].clamp_ma
+00011b70: 7828 6375 7272 5f6d 6178 5f64 7572 2c20  x(curr_max_dur, 
+00011b80: 636c 6970 5f73 7461 7274 3d54 7275 652c  clip_start=True,
+00011b90: 2076 6572 626f 7365 3d76 6572 626f 7365   verbose=verbose
+00011ba0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00011bb0: 2020 2073 6567 2e77 6f72 6473 5b2d 315d     seg.words[-1]
+00011bc0: 2e63 6c61 6d70 5f6d 6178 2863 7572 725f  .clamp_max(curr_
+00011bd0: 6d61 785f 6475 722c 2063 6c69 705f 7374  max_dur, clip_st
+00011be0: 6172 743d 4661 6c73 652c 2076 6572 626f  art=False, verbo
+00011bf0: 7365 3d76 6572 626f 7365 290d 0a20 2020  se=verbose)..   
+00011c00: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00011c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c20: 666f 7220 692c 2077 6f72 6420 696e 2065  for i, word in e
+00011c30: 6e75 6d65 7261 7465 2873 6567 2e77 6f72  numerate(seg.wor
+00011c40: 6473 293a 0d0a 2020 2020 2020 2020 2020  ds):..          
+00011c50: 2020 2020 2020 2020 2020 776f 7264 2e63            word.c
+00011c60: 6c61 6d70 5f6d 6178 2863 7572 725f 6d61  lamp_max(curr_ma
+00011c70: 785f 6475 722c 2063 6c69 705f 7374 6172  x_dur, clip_star
+00011c80: 743d 636c 6970 5f73 7461 7274 2c20 7665  t=clip_start, ve
+00011c90: 7262 6f73 653d 7665 7262 6f73 6529 0d0a  rbose=verbose)..
+00011ca0: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
 00011cb0: 662e 5f72 6567 726f 7570 5f68 6973 746f  f._regroup_histo
-00011cc0: 7279 202b 3d20 6627 636d 3d7b 6d65 6469  ry += f'cm={medi
-00011cd0: 756d 5f66 6163 746f 727d 2b7b 6d61 785f  um_factor}+{max_
-00011ce0: 6475 7220 6f72 2022 227d 2b7b 636c 6970  dur or ""}+{clip
-00011cf0: 5f73 7461 7274 206f 7220 2222 7d2b 7b69  _start or ""}+{i
-00011d00: 6e74 2876 6572 626f 7365 297d 270d 0a20  nt(verbose)}'.. 
-00011d10: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00011d20: 6c66 0d0a 0d0a 2020 2020 6465 6620 6c6f  lf....    def lo
-00011d30: 636b 280d 0a20 2020 2020 2020 2020 2020  ck(..           
-00011d40: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
-00011d50: 2020 2020 7374 6172 7473 7769 7468 3a20      startswith: 
-00011d60: 556e 696f 6e5b 7374 722c 204c 6973 745b  Union[str, List[
-00011d70: 7374 725d 5d20 3d20 4e6f 6e65 2c0d 0a20  str]] = None,.. 
-00011d80: 2020 2020 2020 2020 2020 2065 6e64 7377             endsw
-00011d90: 6974 683a 2055 6e69 6f6e 5b73 7472 2c20  ith: Union[str, 
-00011da0: 4c69 7374 5b73 7472 5d5d 203d 204e 6f6e  List[str]] = Non
-00011db0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00011dc0: 7269 6768 743a 2062 6f6f 6c20 3d20 5472  right: bool = Tr
-00011dd0: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-00011de0: 206c 6566 743a 2062 6f6f 6c20 3d20 4661   left: bool = Fa
-00011df0: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
-00011e00: 2020 6361 7365 5f73 656e 7369 7469 7665    case_sensitive
-00011e10: 3a20 626f 6f6c 203d 2046 616c 7365 2c0d  : bool = False,.
-00011e20: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00011e30: 6970 3a20 626f 6f6c 203d 2054 7275 650d  ip: bool = True.
-00011e40: 0a20 2020 2029 202d 3e20 2257 6869 7370  .    ) -> "Whisp
-00011e50: 6572 5265 7375 6c74 223a 0d0a 2020 2020  erResult":..    
-00011e60: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00011e70: 204c 6f63 6b20 776f 7264 732f 7365 676d   Lock words/segm
-00011e80: 656e 7473 2077 6974 6820 6d61 7463 6869  ents with matchi
-00011e90: 6e67 2070 7265 6669 782f 7375 6666 6978  ng prefix/suffix
-00011ea0: 2074 6f20 7072 6576 656e 7420 7370 6c69   to prevent spli
-00011eb0: 7474 696e 672f 6d65 7267 696e 672e 0d0a  tting/merging...
-00011ec0: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00011ed0: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
-00011ee0: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-00011ef0: 2020 7374 6172 7473 7769 7468 3a20 7374    startswith: st
-00011f00: 7220 6f72 206c 6973 7420 6f66 2073 7472  r or list of str
-00011f10: 0d0a 2020 2020 2020 2020 2020 2020 5072  ..            Pr
-00011f20: 6566 6978 6573 2074 6f20 6c6f 636b 2e0d  efixes to lock..
-00011f30: 0a20 2020 2020 2020 2065 6e64 7377 6974  .        endswit
-00011f40: 683a 2073 7472 206f 7220 6c69 7374 206f  h: str or list o
-00011f50: 6620 7374 720d 0a20 2020 2020 2020 2020  f str..         
-00011f60: 2020 2053 7566 6669 7865 7320 746f 206c     Suffixes to l
-00011f70: 6f63 6b2e 0d0a 2020 2020 2020 2020 7269  ock...        ri
-00011f80: 6768 7420 3a20 626f 6f6c 2c20 6465 6661  ght : bool, defa
-00011f90: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
-00011fa0: 2020 2020 2020 5768 6574 6865 7220 7072        Whether pr
-00011fb0: 6576 656e 7420 7370 6c69 7473 2f6d 6572  event splits/mer
-00011fc0: 6765 7320 7769 7468 2074 6865 206e 6578  ges with the nex
-00011fd0: 7420 776f 7264 2f73 6567 6d65 6e74 2e0d  t word/segment..
-00011fe0: 0a20 2020 2020 2020 206c 6566 7420 3a20  .        left : 
-00011ff0: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-00012000: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-00012010: 2057 6865 7468 6572 2070 7265 7665 6e74   Whether prevent
-00012020: 2073 706c 6974 732f 6d65 7267 6573 2077   splits/merges w
-00012030: 6974 6820 7468 6520 7072 6576 696f 7573  ith the previous
-00012040: 2077 6f72 642f 7365 676d 656e 742e 0d0a   word/segment...
-00012050: 2020 2020 2020 2020 6361 7365 5f73 656e          case_sen
-00012060: 7369 7469 7665 203a 2062 6f6f 6c2c 2064  sitive : bool, d
-00012070: 6566 6175 6c74 2046 616c 7365 0d0a 2020  efault False..  
-00012080: 2020 2020 2020 2020 2020 5768 6574 6865            Whethe
-00012090: 7220 746f 206d 6174 6368 2074 6865 2063  r to match the c
-000120a0: 6173 6520 6f66 2074 6865 2070 7265 6669  ase of the prefi
-000120b0: 7865 732f 7375 6666 6978 6573 2077 6974  xes/suffixes wit
-000120c0: 6820 7468 6520 776f 7264 732f 7365 676d  h the words/segm
-000120d0: 656e 7473 2e0d 0a20 2020 2020 2020 2073  ents...        s
-000120e0: 7472 6970 203a 2062 6f6f 6c2c 2064 6566  trip : bool, def
-000120f0: 6175 6c74 2054 7275 650d 0a20 2020 2020  ault True..     
-00012100: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
-00012110: 6f20 6967 6e6f 7265 2073 7061 6365 7320  o ignore spaces 
-00012120: 6265 666f 7265 2061 6e64 2061 6674 6572  before and after
-00012130: 2062 6f74 6820 776f 7264 732f 7365 676d   both words/segm
-00012140: 656e 7473 2061 6e64 2070 7265 6669 7865  ents and prefixe
-00012150: 732f 7375 6666 6978 6573 2e0d 0a0d 0a20  s/suffixes..... 
-00012160: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
-00012170: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
-00012180: 0a20 2020 2020 2020 2073 7461 626c 655f  .        stable_
-00012190: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
-000121a0: 6869 7370 6572 5265 7375 6c74 0d0a 2020  hisperResult..  
-000121b0: 2020 2020 2020 2020 2020 5468 6520 6375            The cu
-000121c0: 7272 656e 7420 696e 7374 616e 6365 2061  rrent instance a
-000121d0: 6674 6572 2074 6865 2063 6861 6e67 6573  fter the changes
-000121e0: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-000121f0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00012200: 7461 7274 7377 6974 6820 6f72 2065 6e64  tartswith or end
-00012210: 7377 6974 682c 2027 4d75 7374 2073 7065  swith, 'Must spe
-00012220: 6369 6679 205b 7374 6172 7473 7769 7468  cify [startswith
-00012230: 5d20 6f72 2f61 6e64 205b 656e 6473 7769  ] or/and [endswi
-00012240: 7468 5d2e 270d 0a20 2020 2020 2020 2073  th].'..        s
-00012250: 7461 7274 7377 6974 6820 3d20 5b5d 2069  tartswith = [] i
-00012260: 6620 7374 6172 7473 7769 7468 2069 7320  f startswith is 
-00012270: 4e6f 6e65 2065 6c73 6520 285b 7374 6172  None else ([star
-00012280: 7473 7769 7468 5d20 6966 2069 7369 6e73  tswith] if isins
-00012290: 7461 6e63 6528 7374 6172 7473 7769 7468  tance(startswith
-000122a0: 2c20 7374 7229 2065 6c73 6520 7374 6172  , str) else star
-000122b0: 7473 7769 7468 290d 0a20 2020 2020 2020  tswith)..       
-000122c0: 2065 6e64 7377 6974 6820 3d20 5b5d 2069   endswith = [] i
-000122d0: 6620 656e 6473 7769 7468 2069 7320 4e6f  f endswith is No
-000122e0: 6e65 2065 6c73 6520 285b 656e 6473 7769  ne else ([endswi
-000122f0: 7468 5d20 6966 2069 7369 6e73 7461 6e63  th] if isinstanc
-00012300: 6528 656e 6473 7769 7468 2c20 7374 7229  e(endswith, str)
-00012310: 2065 6c73 6520 656e 6473 7769 7468 290d   else endswith).
-00012320: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00012330: 6361 7365 5f73 656e 7369 7469 7665 3a0d  case_sensitive:.
-00012340: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-00012350: 7274 7377 6974 6820 3d20 5b74 2e6c 6f77  rtswith = [t.low
-00012360: 6572 2829 2066 6f72 2074 2069 6e20 7374  er() for t in st
-00012370: 6172 7473 7769 7468 5d0d 0a20 2020 2020  artswith]..     
-00012380: 2020 2020 2020 2065 6e64 7377 6974 6820         endswith 
-00012390: 3d20 5b74 2e6c 6f77 6572 2829 2066 6f72  = [t.lower() for
-000123a0: 2074 2069 6e20 656e 6473 7769 7468 5d0d   t in endswith].
-000123b0: 0a20 2020 2020 2020 2069 6620 7374 7269  .        if stri
-000123c0: 703a 0d0a 2020 2020 2020 2020 2020 2020  p:..            
-000123d0: 7374 6172 7473 7769 7468 203d 205b 742e  startswith = [t.
-000123e0: 7374 7269 7028 2920 666f 7220 7420 696e  strip() for t in
-000123f0: 2073 7461 7274 7377 6974 685d 0d0a 2020   startswith]..  
-00012400: 2020 2020 2020 2020 2020 656e 6473 7769            endswi
-00012410: 7468 203d 205b 742e 7374 7269 7028 2920  th = [t.strip() 
-00012420: 666f 7220 7420 696e 2065 6e64 7377 6974  for t in endswit
-00012430: 685d 0d0a 2020 2020 2020 2020 666f 7220  h]..        for 
-00012440: 7061 7274 2069 6e20 7365 6c66 2e61 6c6c  part in self.all
-00012450: 5f77 6f72 6473 5f6f 725f 7365 676d 656e  _words_or_segmen
-00012460: 7473 2829 3a0d 0a20 2020 2020 2020 2020  ts():..         
-00012470: 2020 2074 6578 7420 3d20 7061 7274 2e77     text = part.w
-00012480: 6f72 6420 6966 2068 6173 6174 7472 2870  ord if hasattr(p
-00012490: 6172 742c 2027 776f 7264 2729 2065 6c73  art, 'word') els
-000124a0: 6520 7061 7274 2e74 6578 740d 0a20 2020  e part.text..   
-000124b0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-000124c0: 6361 7365 5f73 656e 7369 7469 7665 3a0d  case_sensitive:.
-000124d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000124e0: 2074 6578 7420 3d20 7465 7874 2e6c 6f77   text = text.low
-000124f0: 6572 2829 0d0a 2020 2020 2020 2020 2020  er()..          
-00012500: 2020 6966 2073 7472 6970 3a0d 0a20 2020    if strip:..   
-00012510: 2020 2020 2020 2020 2020 2020 2074 6578               tex
-00012520: 7420 3d20 7465 7874 2e73 7472 6970 2829  t = text.strip()
-00012530: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00012540: 7220 7072 6566 6978 2069 6e20 7374 6172  r prefix in star
-00012550: 7473 7769 7468 3a0d 0a20 2020 2020 2020  tswith:..       
-00012560: 2020 2020 2020 2020 2069 6620 7465 7874           if text
-00012570: 2e73 7461 7274 7377 6974 6828 7072 6566  .startswith(pref
-00012580: 6978 293a 0d0a 2020 2020 2020 2020 2020  ix):..          
-00012590: 2020 2020 2020 2020 2020 6966 2072 6967            if rig
-000125a0: 6874 3a0d 0a20 2020 2020 2020 2020 2020  ht:..           
-000125b0: 2020 2020 2020 2020 2020 2020 2070 6172               par
-000125c0: 742e 6c6f 636b 5f72 6967 6874 2829 0d0a  t.lock_right()..
+00011cc0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00011cd0: 2073 656c 662e 5f72 6567 726f 7570 5f68   self._regroup_h
+00011ce0: 6973 746f 7279 202b 3d20 275f 270d 0a20  istory += '_'.. 
+00011cf0: 2020 2020 2020 2073 656c 662e 5f72 6567         self._reg
+00011d00: 726f 7570 5f68 6973 746f 7279 202b 3d20  roup_history += 
+00011d10: 6627 636d 3d7b 6d65 6469 756d 5f66 6163  f'cm={medium_fac
+00011d20: 746f 727d 2b7b 6d61 785f 6475 7220 6f72  tor}+{max_dur or
+00011d30: 2022 227d 2b7b 636c 6970 5f73 7461 7274   ""}+{clip_start
+00011d40: 206f 7220 2222 7d2b 7b69 6e74 2876 6572   or ""}+{int(ver
+00011d50: 626f 7365 297d 270d 0a20 2020 2020 2020  bose)}'..       
+00011d60: 2072 6574 7572 6e20 7365 6c66 0d0a 0d0a   return self....
+00011d70: 2020 2020 6465 6620 6c6f 636b 280d 0a20      def lock(.. 
+00011d80: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00011d90: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00011da0: 6172 7473 7769 7468 3a20 556e 696f 6e5b  artswith: Union[
+00011db0: 7374 722c 204c 6973 745b 7374 725d 5d20  str, List[str]] 
+00011dc0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+00011dd0: 2020 2020 2065 6e64 7377 6974 683a 2055       endswith: U
+00011de0: 6e69 6f6e 5b73 7472 2c20 4c69 7374 5b73  nion[str, List[s
+00011df0: 7472 5d5d 203d 204e 6f6e 652c 0d0a 2020  tr]] = None,..  
+00011e00: 2020 2020 2020 2020 2020 7269 6768 743a            right:
+00011e10: 2062 6f6f 6c20 3d20 5472 7565 2c0d 0a20   bool = True,.. 
+00011e20: 2020 2020 2020 2020 2020 206c 6566 743a             left:
+00011e30: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
+00011e40: 2020 2020 2020 2020 2020 2020 6361 7365              case
+00011e50: 5f73 656e 7369 7469 7665 3a20 626f 6f6c  _sensitive: bool
+00011e60: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
+00011e70: 2020 2020 2020 2073 7472 6970 3a20 626f         strip: bo
+00011e80: 6f6c 203d 2054 7275 650d 0a20 2020 2029  ol = True..    )
+00011e90: 202d 3e20 2257 6869 7370 6572 5265 7375   -> "WhisperResu
+00011ea0: 6c74 223a 0d0a 2020 2020 2020 2020 2222  lt":..        ""
+00011eb0: 220d 0a20 2020 2020 2020 204c 6f63 6b20  "..        Lock 
+00011ec0: 776f 7264 732f 7365 676d 656e 7473 2077  words/segments w
+00011ed0: 6974 6820 6d61 7463 6869 6e67 2070 7265  ith matching pre
+00011ee0: 6669 782f 7375 6666 6978 2074 6f20 7072  fix/suffix to pr
+00011ef0: 6576 656e 7420 7370 6c69 7474 696e 672f  event splitting/
+00011f00: 6d65 7267 696e 672e 0d0a 0d0a 2020 2020  merging.....    
+00011f10: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
+00011f20: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00011f30: 2d2d 0d0a 2020 2020 2020 2020 7374 6172  --..        star
+00011f40: 7473 7769 7468 3a20 7374 7220 6f72 206c  tswith: str or l
+00011f50: 6973 7420 6f66 2073 7472 0d0a 2020 2020  ist of str..    
+00011f60: 2020 2020 2020 2020 5072 6566 6978 6573          Prefixes
+00011f70: 2074 6f20 6c6f 636b 2e0d 0a20 2020 2020   to lock...     
+00011f80: 2020 2065 6e64 7377 6974 683a 2073 7472     endswith: str
+00011f90: 206f 7220 6c69 7374 206f 6620 7374 720d   or list of str.
+00011fa0: 0a20 2020 2020 2020 2020 2020 2053 7566  .            Suf
+00011fb0: 6669 7865 7320 746f 206c 6f63 6b2e 0d0a  fixes to lock...
+00011fc0: 2020 2020 2020 2020 7269 6768 7420 3a20          right : 
+00011fd0: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
+00011fe0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+00011ff0: 5768 6574 6865 7220 7072 6576 656e 7420  Whether prevent 
+00012000: 7370 6c69 7473 2f6d 6572 6765 7320 7769  splits/merges wi
+00012010: 7468 2074 6865 206e 6578 7420 776f 7264  th the next word
+00012020: 2f73 6567 6d65 6e74 2e0d 0a20 2020 2020  /segment...     
+00012030: 2020 206c 6566 7420 3a20 626f 6f6c 2c20     left : bool, 
+00012040: 6465 6661 756c 7420 4661 6c73 650d 0a20  default False.. 
+00012050: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+00012060: 6572 2070 7265 7665 6e74 2073 706c 6974  er prevent split
+00012070: 732f 6d65 7267 6573 2077 6974 6820 7468  s/merges with th
+00012080: 6520 7072 6576 696f 7573 2077 6f72 642f  e previous word/
+00012090: 7365 676d 656e 742e 0d0a 2020 2020 2020  segment...      
+000120a0: 2020 6361 7365 5f73 656e 7369 7469 7665    case_sensitive
+000120b0: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+000120c0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+000120d0: 2020 2020 5768 6574 6865 7220 746f 206d      Whether to m
+000120e0: 6174 6368 2074 6865 2063 6173 6520 6f66  atch the case of
+000120f0: 2074 6865 2070 7265 6669 7865 732f 7375   the prefixes/su
+00012100: 6666 6978 6573 2077 6974 6820 7468 6520  ffixes with the 
+00012110: 776f 7264 732f 7365 676d 656e 7473 2e0d  words/segments..
+00012120: 0a20 2020 2020 2020 2073 7472 6970 203a  .        strip :
+00012130: 2062 6f6f 6c2c 2064 6566 6175 6c74 2054   bool, default T
+00012140: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
+00012150: 2057 6865 7468 6572 2074 6f20 6967 6e6f   Whether to igno
+00012160: 7265 2073 7061 6365 7320 6265 666f 7265  re spaces before
+00012170: 2061 6e64 2061 6674 6572 2062 6f74 6820   and after both 
+00012180: 776f 7264 732f 7365 676d 656e 7473 2061  words/segments a
+00012190: 6e64 2070 7265 6669 7865 732f 7375 6666  nd prefixes/suff
+000121a0: 6978 6573 2e0d 0a0d 0a20 2020 2020 2020  ixes.....       
+000121b0: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
+000121c0: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
+000121d0: 2020 2073 7461 626c 655f 7768 6973 7065     stable_whispe
+000121e0: 722e 7265 7375 6c74 2e57 6869 7370 6572  r.result.Whisper
+000121f0: 5265 7375 6c74 0d0a 2020 2020 2020 2020  Result..        
+00012200: 2020 2020 5468 6520 6375 7272 656e 7420      The current 
+00012210: 696e 7374 616e 6365 2061 6674 6572 2074  instance after t
+00012220: 6865 2063 6861 6e67 6573 2e0d 0a20 2020  he changes...   
+00012230: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00012240: 2020 6173 7365 7274 2073 7461 7274 7377    assert startsw
+00012250: 6974 6820 6f72 2065 6e64 7377 6974 682c  ith or endswith,
+00012260: 2027 4d75 7374 2073 7065 6369 6679 205b   'Must specify [
+00012270: 7374 6172 7473 7769 7468 5d20 6f72 2f61  startswith] or/a
+00012280: 6e64 205b 656e 6473 7769 7468 5d2e 270d  nd [endswith].'.
+00012290: 0a20 2020 2020 2020 2073 7461 7274 7377  .        startsw
+000122a0: 6974 6820 3d20 5b5d 2069 6620 7374 6172  ith = [] if star
+000122b0: 7473 7769 7468 2069 7320 4e6f 6e65 2065  tswith is None e
+000122c0: 6c73 6520 285b 7374 6172 7473 7769 7468  lse ([startswith
+000122d0: 5d20 6966 2069 7369 6e73 7461 6e63 6528  ] if isinstance(
+000122e0: 7374 6172 7473 7769 7468 2c20 7374 7229  startswith, str)
+000122f0: 2065 6c73 6520 7374 6172 7473 7769 7468   else startswith
+00012300: 290d 0a20 2020 2020 2020 2065 6e64 7377  )..        endsw
+00012310: 6974 6820 3d20 5b5d 2069 6620 656e 6473  ith = [] if ends
+00012320: 7769 7468 2069 7320 4e6f 6e65 2065 6c73  with is None els
+00012330: 6520 285b 656e 6473 7769 7468 5d20 6966  e ([endswith] if
+00012340: 2069 7369 6e73 7461 6e63 6528 656e 6473   isinstance(ends
+00012350: 7769 7468 2c20 7374 7229 2065 6c73 6520  with, str) else 
+00012360: 656e 6473 7769 7468 290d 0a20 2020 2020  endswith)..     
+00012370: 2020 2069 6620 6e6f 7420 6361 7365 5f73     if not case_s
+00012380: 656e 7369 7469 7665 3a0d 0a20 2020 2020  ensitive:..     
+00012390: 2020 2020 2020 2073 7461 7274 7377 6974         startswit
+000123a0: 6820 3d20 5b74 2e6c 6f77 6572 2829 2066  h = [t.lower() f
+000123b0: 6f72 2074 2069 6e20 7374 6172 7473 7769  or t in startswi
+000123c0: 7468 5d0d 0a20 2020 2020 2020 2020 2020  th]..           
+000123d0: 2065 6e64 7377 6974 6820 3d20 5b74 2e6c   endswith = [t.l
+000123e0: 6f77 6572 2829 2066 6f72 2074 2069 6e20  ower() for t in 
+000123f0: 656e 6473 7769 7468 5d0d 0a20 2020 2020  endswith]..     
+00012400: 2020 2069 6620 7374 7269 703a 0d0a 2020     if strip:..  
+00012410: 2020 2020 2020 2020 2020 7374 6172 7473            starts
+00012420: 7769 7468 203d 205b 742e 7374 7269 7028  with = [t.strip(
+00012430: 2920 666f 7220 7420 696e 2073 7461 7274  ) for t in start
+00012440: 7377 6974 685d 0d0a 2020 2020 2020 2020  swith]..        
+00012450: 2020 2020 656e 6473 7769 7468 203d 205b      endswith = [
+00012460: 742e 7374 7269 7028 2920 666f 7220 7420  t.strip() for t 
+00012470: 696e 2065 6e64 7377 6974 685d 0d0a 2020  in endswith]..  
+00012480: 2020 2020 2020 666f 7220 7061 7274 2069        for part i
+00012490: 6e20 7365 6c66 2e61 6c6c 5f77 6f72 6473  n self.all_words
+000124a0: 5f6f 725f 7365 676d 656e 7473 2829 3a0d  _or_segments():.
+000124b0: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
+000124c0: 7420 3d20 7061 7274 2e77 6f72 6420 6966  t = part.word if
+000124d0: 2068 6173 6174 7472 2870 6172 742c 2027   hasattr(part, '
+000124e0: 776f 7264 2729 2065 6c73 6520 7061 7274  word') else part
+000124f0: 2e74 6578 740d 0a20 2020 2020 2020 2020  .text..         
+00012500: 2020 2069 6620 6e6f 7420 6361 7365 5f73     if not case_s
+00012510: 656e 7369 7469 7665 3a0d 0a20 2020 2020  ensitive:..     
+00012520: 2020 2020 2020 2020 2020 2074 6578 7420             text 
+00012530: 3d20 7465 7874 2e6c 6f77 6572 2829 0d0a  = text.lower()..
+00012540: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00012550: 7472 6970 3a0d 0a20 2020 2020 2020 2020  trip:..         
+00012560: 2020 2020 2020 2074 6578 7420 3d20 7465         text = te
+00012570: 7874 2e73 7472 6970 2829 0d0a 2020 2020  xt.strip()..    
+00012580: 2020 2020 2020 2020 666f 7220 7072 6566          for pref
+00012590: 6978 2069 6e20 7374 6172 7473 7769 7468  ix in startswith
+000125a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000125b0: 2020 2069 6620 7465 7874 2e73 7461 7274     if text.start
+000125c0: 7377 6974 6828 7072 6566 6978 293a 0d0a  swith(prefix):..
 000125d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125e0: 2020 2020 6966 206c 6566 743a 0d0a 2020      if left:..  
+000125e0: 2020 2020 6966 2072 6967 6874 3a0d 0a20      if right:.. 
 000125f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012600: 2020 2020 2020 7061 7274 2e6c 6f63 6b5f        part.lock_
-00012610: 6c65 6674 2829 0d0a 2020 2020 2020 2020  left()..        
-00012620: 2020 2020 666f 7220 7375 6666 6978 2069      for suffix i
-00012630: 6e20 656e 6473 7769 7468 3a0d 0a20 2020  n endswith:..   
-00012640: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00012650: 7465 7874 2e65 6e64 7377 6974 6828 7375  text.endswith(su
-00012660: 6666 6978 293a 0d0a 2020 2020 2020 2020  ffix):..        
-00012670: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00012680: 6967 6874 3a0d 0a20 2020 2020 2020 2020  ight:..         
-00012690: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000126a0: 6172 742e 6c6f 636b 5f72 6967 6874 2829  art.lock_right()
+00012600: 2020 2020 2020 2070 6172 742e 6c6f 636b         part.lock
+00012610: 5f72 6967 6874 2829 0d0a 2020 2020 2020  _right()..      
+00012620: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00012630: 206c 6566 743a 0d0a 2020 2020 2020 2020   left:..        
+00012640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012650: 7061 7274 2e6c 6f63 6b5f 6c65 6674 2829  part.lock_left()
+00012660: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+00012670: 7220 7375 6666 6978 2069 6e20 656e 6473  r suffix in ends
+00012680: 7769 7468 3a0d 0a20 2020 2020 2020 2020  with:..         
+00012690: 2020 2020 2020 2069 6620 7465 7874 2e65         if text.e
+000126a0: 6e64 7377 6974 6828 7375 6666 6978 293a  ndswith(suffix):
 000126b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000126c0: 2020 2020 2020 6966 206c 6566 743a 0d0a        if left:..
-000126d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126e0: 2020 2020 2020 2020 7061 7274 2e6c 6f63          part.loc
-000126f0: 6b5f 6c65 6674 2829 0d0a 2020 2020 2020  k_left()..      
-00012700: 2020 6966 2073 656c 662e 5f72 6567 726f    if self._regro
-00012710: 7570 5f68 6973 746f 7279 3a0d 0a20 2020  up_history:..   
-00012720: 2020 2020 2020 2020 2073 656c 662e 5f72           self._r
-00012730: 6567 726f 7570 5f68 6973 746f 7279 202b  egroup_history +
-00012740: 3d20 275f 270d 0a20 2020 2020 2020 2073  = '_'..        s
-00012750: 7461 7274 7377 6974 685f 7374 7220 3d20  tartswith_str = 
-00012760: 2873 7461 7274 7377 6974 6820 6966 2069  (startswith if i
-00012770: 7369 6e73 7461 6e63 6528 7374 6172 7473  sinstance(starts
-00012780: 7769 7468 2c20 7374 7229 2065 6c73 6520  with, str) else 
-00012790: 272f 272e 6a6f 696e 2873 7461 7274 7377  '/'.join(startsw
-000127a0: 6974 6829 2920 6966 2073 7461 7274 7377  ith)) if startsw
-000127b0: 6974 6820 656c 7365 2022 220d 0a20 2020  ith else ""..   
-000127c0: 2020 2020 2065 6e64 7377 6974 685f 7374       endswith_st
-000127d0: 7220 3d20 2865 6e64 7377 6974 6820 6966  r = (endswith if
-000127e0: 2069 7369 6e73 7461 6e63 6528 656e 6473   isinstance(ends
-000127f0: 7769 7468 2c20 7374 7229 2065 6c73 6520  with, str) else 
-00012800: 272f 272e 6a6f 696e 2865 6e64 7377 6974  '/'.join(endswit
-00012810: 6829 2920 6966 2065 6e64 7377 6974 6820  h)) if endswith 
-00012820: 656c 7365 2022 220d 0a20 2020 2020 2020  else ""..       
-00012830: 2073 656c 662e 5f72 6567 726f 7570 5f68   self._regroup_h
-00012840: 6973 746f 7279 202b 3d20 2866 276c 3d7b  istory += (f'l={
-00012850: 7374 6172 7473 7769 7468 5f73 7472 7d2b  startswith_str}+
-00012860: 7b65 6e64 7377 6974 685f 7374 727d 270d  {endswith_str}'.
-00012870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012890: 2020 2066 272b 7b69 6e74 2872 6967 6874     f'+{int(right
-000128a0: 297d 2b7b 696e 7428 6c65 6674 297d 2b7b  )}+{int(left)}+{
-000128b0: 696e 7428 6361 7365 5f73 656e 7369 7469  int(case_sensiti
-000128c0: 7665 297d 2b7b 696e 7428 7374 7269 7029  ve)}+{int(strip)
-000128d0: 7d27 290d 0a20 2020 2020 2020 2072 6574  }')..        ret
-000128e0: 7572 6e20 7365 6c66 0d0a 0d0a 2020 2020  urn self....    
-000128f0: 6465 6620 7265 6d6f 7665 5f77 6f72 6428  def remove_word(
-00012900: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00012910: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
-00012920: 2077 6f72 643a 2055 6e69 6f6e 5b57 6f72   word: Union[Wor
-00012930: 6454 696d 696e 672c 2054 7570 6c65 5b69  dTiming, Tuple[i
-00012940: 6e74 2c20 696e 745d 5d2c 0d0a 2020 2020  nt, int]],..    
-00012950: 2020 2020 2020 2020 7265 6173 7369 676e          reassign
-00012960: 5f69 6473 3a20 626f 6f6c 203d 2054 7275  _ids: bool = Tru
-00012970: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00012980: 7665 7262 6f73 653a 2062 6f6f 6c20 3d20  verbose: bool = 
-00012990: 5472 7565 0d0a 2020 2020 2920 2d3e 2027  True..    ) -> '
-000129a0: 5768 6973 7065 7252 6573 756c 7427 3a0d  WhisperResult':.
-000129b0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-000129c0: 2020 2020 2020 5265 6d6f 7665 2061 2077        Remove a w
-000129d0: 6f72 642e 0d0a 0d0a 2020 2020 2020 2020  ord.....        
-000129e0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
-000129f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
-00012a00: 2020 2020 2020 2020 776f 7264 203a 2057          word : W
-00012a10: 6f72 6454 696d 696e 6720 6f72 2074 7570  ordTiming or tup
-00012a20: 6c65 206f 6620 2869 6e74 2c20 696e 7429  le of (int, int)
-00012a30: 0d0a 2020 2020 2020 2020 2020 2020 496e  ..            In
-00012a40: 7374 616e 6365 206f 6620 3a63 6c61 7373  stance of :class
-00012a50: 3a60 7374 6162 6c65 5f77 6869 7370 6572  :`stable_whisper
-00012a60: 2e72 6573 756c 742e 576f 7264 5469 6d69  .result.WordTimi
-00012a70: 6e67 6020 6f72 2074 7570 6c65 206f 6620  ng` or tuple of 
-00012a80: 2873 6567 6d65 6e74 2069 6e64 6578 2c20  (segment index, 
-00012a90: 776f 7264 2069 6e64 6578 292e 0d0a 2020  word index)...  
-00012aa0: 2020 2020 2020 7265 6173 7369 676e 5f69        reassign_i
-00012ab0: 6473 203a 2062 6f6f 6c2c 2064 6566 6175  ds : bool, defau
-00012ac0: 6c74 2054 7275 650d 0a20 2020 2020 2020  lt True..       
-00012ad0: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
-00012ae0: 7265 6173 7369 676e 2073 6567 6d65 6e74  reassign segment
-00012af0: 2061 6e64 2077 6f72 6420 6964 7320 2869   and word ids (i
-00012b00: 6e64 6963 6573 2920 6166 7465 7220 7265  ndices) after re
-00012b10: 6d6f 7669 6e67 2060 6077 6f72 6460 602e  moving ``word``.
-00012b20: 0d0a 2020 2020 2020 2020 7665 7262 6f73  ..        verbos
-00012b30: 6520 3a20 626f 6f6c 2c20 6465 6661 756c  e : bool, defaul
-00012b40: 7420 5472 7565 0d0a 2020 2020 2020 2020  t True..        
-00012b50: 2020 2020 5768 6574 6865 7220 746f 2070      Whether to p
-00012b60: 7269 6e74 2064 6574 6169 6c20 6f66 2074  rint detail of t
-00012b70: 6865 2072 656d 6f76 6564 2077 6f72 642e  he removed word.
-00012b80: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-00012b90: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
-00012ba0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 7374  ----..        st
-00012bb0: 6162 6c65 5f77 6869 7370 6572 2e72 6573  able_whisper.res
-00012bc0: 756c 742e 5768 6973 7065 7252 6573 756c  ult.WhisperResul
-00012bd0: 740d 0a20 2020 2020 2020 2020 2020 2054  t..            T
-00012be0: 6865 2063 7572 7265 6e74 2069 6e73 7461  he current insta
-00012bf0: 6e63 6520 6166 7465 7220 7468 6520 6368  nce after the ch
-00012c00: 616e 6765 732e 0d0a 2020 2020 2020 2020  anges...        
-00012c10: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
-00012c20: 6973 696e 7374 616e 6365 2877 6f72 642c  isinstance(word,
-00012c30: 2057 6f72 6454 696d 696e 6729 3a0d 0a20   WordTiming):.. 
-00012c40: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00012c50: 6c66 5b77 6f72 642e 7365 676d 656e 745f  lf[word.segment_
-00012c60: 6964 5d5b 776f 7264 2e69 645d 2069 7320  id][word.id] is 
-00012c70: 6e6f 7420 776f 7264 3a0d 0a20 2020 2020  not word:..     
-00012c80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012c90: 7265 6173 7369 676e 5f69 6473 2829 0d0a  reassign_ids()..
-00012ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cb0: 6966 2073 656c 665b 776f 7264 2e73 6567  if self[word.seg
-00012cc0: 6d65 6e74 5f69 645d 5b77 6f72 642e 6964  ment_id][word.id
-00012cd0: 5d20 6973 206e 6f74 2077 6f72 643a 0d0a  ] is not word:..
-00012ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cf0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00012d00: 7272 6f72 2827 776f 7264 206e 6f74 2069  rror('word not i
-00012d10: 6e20 7265 7375 6c74 2729 0d0a 2020 2020  n result')..    
-00012d20: 2020 2020 2020 2020 7365 675f 6964 2c20          seg_id, 
-00012d30: 776f 7264 5f69 6420 3d20 776f 7264 2e73  word_id = word.s
-00012d40: 6567 6d65 6e74 5f69 642c 2077 6f72 642e  egment_id, word.
-00012d50: 6964 0d0a 2020 2020 2020 2020 656c 7365  id..        else
-00012d60: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00012d70: 6567 5f69 642c 2077 6f72 645f 6964 203d  eg_id, word_id =
-00012d80: 2077 6f72 640d 0a20 2020 2020 2020 2069   word..        i
-00012d90: 6620 7665 7262 6f73 653a 0d0a 2020 2020  f verbose:..    
-00012da0: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
-00012db0: 5265 6d6f 7665 643a 207b 7365 6c66 5b73  Removed: {self[s
-00012dc0: 6567 5f69 645d 5b77 6f72 645f 6964 5d2e  eg_id][word_id].
-00012dd0: 746f 5f64 6963 7428 297d 2729 0d0a 2020  to_dict()}')..  
-00012de0: 2020 2020 2020 6465 6c20 7365 6c66 2e73        del self.s
-00012df0: 6567 6d65 6e74 735b 7365 675f 6964 5d2e  egments[seg_id].
-00012e00: 776f 7264 735b 776f 7264 5f69 645d 0d0a  words[word_id]..
-00012e10: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
-00012e20: 6561 7373 6967 6e5f 6964 733a 0d0a 2020  eassign_ids:..  
-00012e30: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00012e40: 2073 656c 660d 0a20 2020 2020 2020 2069   self..        i
-00012e50: 6620 7365 6c66 5b73 6567 5f69 645d 2e68  f self[seg_id].h
-00012e60: 6173 5f77 6f72 6473 3a0d 0a20 2020 2020  as_words:..     
-00012e70: 2020 2020 2020 2073 656c 665b 7365 675f         self[seg_
-00012e80: 6964 5d2e 7265 6173 7369 676e 5f69 6473  id].reassign_ids
-00012e90: 2829 0d0a 2020 2020 2020 2020 656c 7365  ()..        else
-00012ea0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00012eb0: 656c 662e 7265 6d6f 7665 5f6e 6f5f 776f  elf.remove_no_wo
-00012ec0: 7264 5f73 6567 6d65 6e74 7328 290d 0a20  rd_segments().. 
-00012ed0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00012ee0: 6c66 0d0a 0d0a 2020 2020 6465 6620 7265  lf....    def re
-00012ef0: 6d6f 7665 5f73 6567 6d65 6e74 280d 0a20  move_segment(.. 
-00012f00: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-00012f10: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00012f20: 676d 656e 743a 2055 6e69 6f6e 5b53 6567  gment: Union[Seg
-00012f30: 6d65 6e74 2c20 696e 745d 2c0d 0a20 2020  ment, int],..   
-00012f40: 2020 2020 2020 2020 2072 6561 7373 6967           reassig
-00012f50: 6e5f 6964 733a 2062 6f6f 6c20 3d20 5472  n_ids: bool = Tr
-00012f60: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-00012f70: 2076 6572 626f 7365 3a20 626f 6f6c 203d   verbose: bool =
-00012f80: 2054 7275 650d 0a20 2020 2029 202d 3e20   True..    ) -> 
-00012f90: 2757 6869 7370 6572 5265 7375 6c74 273a  'WhisperResult':
-00012fa0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00012fb0: 2020 2020 2020 2052 656d 6f76 6520 6120         Remove a 
-00012fc0: 7365 676d 656e 742e 0d0a 0d0a 2020 2020  segment.....    
-00012fd0: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
-00012fe0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00012ff0: 2d2d 0d0a 2020 2020 2020 2020 7365 676d  --..        segm
-00013000: 656e 7420 3a20 5365 676d 656e 7420 6f72  ent : Segment or
-00013010: 2069 6e74 0d0a 2020 2020 2020 2020 2020   int..          
-00013020: 2020 496e 7374 616e 6365 203a 636c 6173    Instance :clas
-00013030: 733a 6073 7461 626c 655f 7768 6973 7065  s:`stable_whispe
-00013040: 722e 7265 7375 6c74 2e53 6567 6d65 6e74  r.result.Segment
-00013050: 6020 6f72 2073 6567 6d65 6e74 2069 6e64  ` or segment ind
-00013060: 6578 2e0d 0a20 2020 2020 2020 2072 6561  ex...        rea
-00013070: 7373 6967 6e5f 6964 7320 3a20 626f 6f6c  ssign_ids : bool
-00013080: 2c20 6465 6661 756c 7420 5472 7565 0d0a  , default True..
-00013090: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
-000130a0: 6865 7220 746f 2072 6561 7373 6967 6e20  her to reassign 
-000130b0: 7365 676d 656e 7420 4944 7320 2869 6e64  segment IDs (ind
-000130c0: 6963 6573 2920 6166 7465 7220 7265 6d6f  ices) after remo
-000130d0: 7669 6e67 2060 6073 6567 6d65 6e74 6060  ving ``segment``
-000130e0: 2e0d 0a20 2020 2020 2020 2076 6572 626f  ...        verbo
-000130f0: 7365 203a 2062 6f6f 6c2c 2064 6566 6175  se : bool, defau
-00013100: 6c74 2054 7275 650d 0a20 2020 2020 2020  lt True..       
-00013110: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
-00013120: 7072 696e 7420 6465 7461 696c 206f 6620  print detail of 
-00013130: 7468 6520 7265 6d6f 7665 6420 776f 7264  the removed word
-00013140: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
-00013150: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
-00013160: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
-00013170: 7461 626c 655f 7768 6973 7065 722e 7265  table_whisper.re
-00013180: 7375 6c74 2e57 6869 7370 6572 5265 7375  sult.WhisperResu
-00013190: 6c74 0d0a 2020 2020 2020 2020 2020 2020  lt..            
-000131a0: 5468 6520 6375 7272 656e 7420 696e 7374  The current inst
-000131b0: 616e 6365 2061 6674 6572 2074 6865 2063  ance after the c
-000131c0: 6861 6e67 6573 2e0d 0a20 2020 2020 2020  hanges...       
-000131d0: 2022 2222 0d0a 2020 2020 2020 2020 6966   """..        if
-000131e0: 2069 7369 6e73 7461 6e63 6528 7365 676d   isinstance(segm
-000131f0: 656e 742c 2053 6567 6d65 6e74 293a 0d0a  ent, Segment):..
-00013200: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00013210: 656c 665b 7365 676d 656e 742e 6964 5d20  elf[segment.id] 
-00013220: 6973 206e 6f74 2073 6567 6d65 6e74 3a0d  is not segment:.
-00013230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013240: 2073 656c 662e 7265 6173 7369 676e 5f69   self.reassign_i
-00013250: 6473 2829 0d0a 2020 2020 2020 2020 2020  ds()..          
-00013260: 2020 2020 2020 6966 2073 656c 665b 7365        if self[se
-00013270: 676d 656e 742e 6964 5d20 6973 206e 6f74  gment.id] is not
-00013280: 2073 6567 6d65 6e74 3a0d 0a20 2020 2020   segment:..     
-00013290: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000132a0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-000132b0: 2773 6567 6d65 6e74 206e 6f74 2069 6e20  'segment not in 
-000132c0: 7265 7375 6c74 2729 0d0a 2020 2020 2020  result')..      
-000132d0: 2020 2020 2020 7365 676d 656e 7420 3d20        segment = 
-000132e0: 7365 676d 656e 742e 6964 0d0a 2020 2020  segment.id..    
-000132f0: 2020 2020 6966 2076 6572 626f 7365 3a0d      if verbose:.
-00013300: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00013310: 6e74 2866 2752 656d 6f76 6564 3a20 5b69  nt(f'Removed: [i
-00013320: 643a 7b73 656c 665b 7365 676d 656e 745d  d:{self[segment]
-00013330: 2e69 647d 5d20 7b73 656c 665b 7365 676d  .id}] {self[segm
-00013340: 656e 745d 2e74 6f5f 6469 7370 6c61 795f  ent].to_display_
-00013350: 7374 7228 5472 7565 297d 2729 0d0a 2020  str(True)}')..  
-00013360: 2020 2020 2020 6465 6c20 7365 6c66 2e73        del self.s
-00013370: 6567 6d65 6e74 735b 7365 676d 656e 745d  egments[segment]
-00013380: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-00013390: 2072 6561 7373 6967 6e5f 6964 733a 0d0a   reassign_ids:..
-000133a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000133b0: 726e 2073 656c 660d 0a20 2020 2020 2020  rn self..       
-000133c0: 2073 656c 662e 7265 6173 7369 676e 5f69   self.reassign_i
-000133d0: 6473 2854 7275 652c 2073 7461 7274 3d73  ds(True, start=s
-000133e0: 6567 6d65 6e74 290d 0a20 2020 2020 2020  egment)..       
-000133f0: 2072 6574 7572 6e20 7365 6c66 0d0a 0d0a   return self....
-00013400: 2020 2020 6465 6620 7265 6d6f 7665 5f72      def remove_r
-00013410: 6570 6574 6974 696f 6e28 0d0a 2020 2020  epetition(..    
-00013420: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-00013430: 2020 2020 2020 2020 2020 206d 6178 5f77             max_w
-00013440: 6f72 6473 3a20 696e 7420 3d20 312c 0d0a  ords: int = 1,..
-00013450: 2020 2020 2020 2020 2020 2020 6361 7365              case
-00013460: 5f73 656e 7369 7469 7665 3a20 626f 6f6c  _sensitive: bool
-00013470: 203d 2046 616c 7365 2c0d 0a20 2020 2020   = False,..     
-00013480: 2020 2020 2020 2073 7472 6970 3a20 626f         strip: bo
-00013490: 6f6c 203d 2054 7275 652c 0d0a 2020 2020  ol = True,..    
-000134a0: 2020 2020 2020 2020 6967 6e6f 7265 5f70          ignore_p
-000134b0: 756e 6374 7561 7469 6f6e 733a 2073 7472  unctuations: str
-000134c0: 203d 2022 5c22 272c 2e3f 2122 2c0d 0a20   = "\"',.?!",.. 
-000134d0: 2020 2020 2020 2020 2020 2065 7874 656e             exten
-000134e0: 645f 6475 7261 7469 6f6e 3a20 626f 6f6c  d_duration: bool
-000134f0: 203d 2054 7275 652c 0d0a 2020 2020 2020   = True,..      
-00013500: 2020 2020 2020 7665 7262 6f73 653a 2062        verbose: b
-00013510: 6f6f 6c20 3d20 5472 7565 0d0a 2020 2020  ool = True..    
-00013520: 2920 2d3e 2027 5768 6973 7065 7252 6573  ) -> 'WhisperRes
-00013530: 756c 7427 3a0d 0a20 2020 2020 2020 2022  ult':..        "
-00013540: 2222 0d0a 2020 2020 2020 2020 5265 6d6f  ""..        Remo
-00013550: 7665 2077 6f72 6473 2074 6861 7420 7265  ve words that re
-00013560: 7065 6174 2063 6f6e 7365 6375 7469 7665  peat consecutive
-00013570: 6c79 2e0d 0a0d 0a20 2020 2020 2020 2050  ly.....        P
-00013580: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
-00013590: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-000135a0: 2020 2020 2020 206d 6178 5f77 6f72 6473         max_words
-000135b0: 203a 2069 6e74 0d0a 2020 2020 2020 2020   : int..        
-000135c0: 2020 2020 4d61 7869 6d75 6d20 6e75 6d62      Maximum numb
-000135d0: 6572 206f 6620 776f 7264 7320 746f 206c  er of words to l
-000135e0: 6f6f 6b20 666f 7220 636f 6e73 6563 7574  ook for consecut
-000135f0: 6976 656c 792e 0d0a 2020 2020 2020 2020  ively...        
-00013600: 6361 7365 5f73 656e 7369 7469 7665 203a  case_sensitive :
-00013610: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
-00013620: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
-00013630: 2020 5768 6574 6865 7220 7468 6520 6361    Whether the ca
-00013640: 7365 206f 6620 776f 7264 7320 6e65 6564  se of words need
-00013650: 2074 6f20 6d61 7463 6820 746f 2062 6520   to match to be 
-00013660: 636f 6e73 6964 6572 6564 2061 7320 7265  considered as re
-00013670: 7065 7469 7469 6f6e 2e0d 0a20 2020 2020  petition...     
-00013680: 2020 2073 7472 6970 203a 2062 6f6f 6c2c     strip : bool,
-00013690: 2064 6566 6175 6c74 2054 7275 650d 0a20   default True.. 
-000136a0: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
-000136b0: 6572 2074 6f20 6967 6e6f 7265 2073 7061  er to ignore spa
-000136c0: 6365 7320 6265 666f 7265 2061 6e64 2061  ces before and a
-000136d0: 6674 6572 2065 6163 6820 776f 7264 2e0d  fter each word..
-000136e0: 0a20 2020 2020 2020 2069 676e 6f72 655f  .        ignore_
-000136f0: 7075 6e63 7475 6174 696f 6e73 203a 2062  punctuations : b
-00013700: 6f6f 6c2c 2064 6566 6175 6c74 2027 2227  ool, default '"'
-00013710: 2c2e 3f21 270d 0a20 2020 2020 2020 2020  ,.?!'..         
-00013720: 2020 2045 6e64 696e 6720 7075 6e63 7475     Ending punctu
-00013730: 6174 696f 6e73 2074 6f20 6967 6e6f 7265  ations to ignore
-00013740: 2e0d 0a20 2020 2020 2020 2065 7874 656e  ...        exten
-00013750: 645f 6475 7261 7469 6f6e 3a20 626f 6f6c  d_duration: bool
-00013760: 2c20 6465 6661 756c 7420 5472 7565 0d0a  , default True..
-00013770: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
-00013780: 6865 7220 746f 2065 7874 656e 6420 7468  her to extend th
-00013790: 6520 6475 7261 7469 6f6e 206f 6620 7468  e duration of th
-000137a0: 6520 7072 6576 696f 7573 2077 6f72 6420  e previous word 
-000137b0: 746f 2063 6f76 6572 2074 6865 2064 7572  to cover the dur
-000137c0: 6174 696f 6e20 6f66 2074 6865 2072 6570  ation of the rep
-000137d0: 6574 6974 696f 6e2e 0d0a 2020 2020 2020  etition...      
-000137e0: 2020 7665 7262 6f73 653a 2062 6f6f 6c2c    verbose: bool,
-000137f0: 2064 6566 6175 6c74 2054 7275 650d 0a20   default True.. 
-00013800: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
-00013810: 6572 2074 6f20 7072 696e 7420 6465 7461  er to print deta
-00013820: 696c 206f 6620 7468 6520 7265 6d6f 7665  il of the remove
-00013830: 6420 7265 7065 7469 7469 6f6e 732e 0d0a  d repetitions...
-00013840: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00013850: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
-00013860: 2d2d 0d0a 2020 2020 2020 2020 7374 6162  --..        stab
-00013870: 6c65 5f77 6869 7370 6572 2e72 6573 756c  le_whisper.resul
-00013880: 742e 5768 6973 7065 7252 6573 756c 740d  t.WhisperResult.
-00013890: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-000138a0: 2063 7572 7265 6e74 2069 6e73 7461 6e63   current instanc
-000138b0: 6520 6166 7465 7220 7468 6520 6368 616e  e after the chan
-000138c0: 6765 732e 0d0a 2020 2020 2020 2020 2222  ges...        ""
-000138d0: 220d 0a20 2020 2020 2020 2069 6620 6e6f  "..        if no
-000138e0: 7420 7365 6c66 2e68 6173 5f77 6f72 6473  t self.has_words
-000138f0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00013900: 6574 7572 6e20 7365 6c66 0d0a 0d0a 2020  eturn self....  
-00013910: 2020 2020 2020 666f 7220 636f 756e 7420        for count 
-00013920: 696e 2072 616e 6765 2831 2c20 6d61 785f  in range(1, max_
-00013930: 776f 7264 7320 2b20 3129 3a0d 0a20 2020  words + 1):..   
-00013940: 2020 2020 2020 2020 2061 6c6c 5f77 6f72           all_wor
-00013950: 6473 203d 2073 656c 662e 616c 6c5f 776f  ds = self.all_wo
-00013960: 7264 7328 290d 0a20 2020 2020 2020 2020  rds()..         
-00013970: 2020 2069 6620 6c65 6e28 616c 6c5f 776f     if len(all_wo
-00013980: 7264 7329 203c 2032 3a0d 0a20 2020 2020  rds) < 2:..     
-00013990: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000139a0: 6e20 7365 6c66 0d0a 2020 2020 2020 2020  n self..        
-000139b0: 2020 2020 616c 6c5f 776f 7264 735f 7374      all_words_st
-000139c0: 7220 3d20 5b77 2e77 6f72 6420 666f 7220  r = [w.word for 
-000139d0: 7720 696e 2061 6c6c 5f77 6f72 6473 5d0d  w in all_words].
-000139e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000139f0: 7374 7269 703a 0d0a 2020 2020 2020 2020  strip:..        
-00013a00: 2020 2020 2020 2020 616c 6c5f 776f 7264          all_word
-00013a10: 735f 7374 7220 3d20 5b77 2e73 7472 6970  s_str = [w.strip
-00013a20: 2829 2066 6f72 2077 2069 6e20 616c 6c5f  () for w in all_
-00013a30: 776f 7264 735f 7374 725d 0d0a 2020 2020  words_str]..    
-00013a40: 2020 2020 2020 2020 6966 2069 676e 6f72          if ignor
-00013a50: 655f 7075 6e63 7475 6174 696f 6e73 3a0d  e_punctuations:.
-00013a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013a70: 2070 746e 203d 2066 275b 7b69 676e 6f72   ptn = f'[{ignor
-00013a80: 655f 7075 6e63 7475 6174 696f 6e73 7d5d  e_punctuations}]
-00013a90: 2b24 270d 0a20 2020 2020 2020 2020 2020  +$'..           
-00013aa0: 2020 2020 2061 6c6c 5f77 6f72 6473 5f73       all_words_s
-00013ab0: 7472 203d 205b 7265 2e73 7562 2870 746e  tr = [re.sub(ptn
-00013ac0: 2c20 2727 2c20 7729 2066 6f72 2077 2069  , '', w) for w i
-00013ad0: 6e20 616c 6c5f 776f 7264 735f 7374 725d  n all_words_str]
-00013ae0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00013af0: 206e 6f74 2063 6173 655f 7365 6e73 6974   not case_sensit
-00013b00: 6976 653a 0d0a 2020 2020 2020 2020 2020  ive:..          
-00013b10: 2020 2020 2020 616c 6c5f 776f 7264 735f        all_words_
-00013b20: 7374 7220 3d20 5b77 2e6c 6f77 6572 2829  str = [w.lower()
-00013b30: 2066 6f72 2077 2069 6e20 616c 6c5f 776f   for w in all_wo
-00013b40: 7264 735f 7374 725d 0d0a 2020 2020 2020  rds_str]..      
-00013b50: 2020 2020 2020 6e65 7874 5f69 203d 204e        next_i = N
-00013b60: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
-00013b70: 2063 6861 6e67 6573 203d 205b 5d0d 0a20   changes = [].. 
-00013b80: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00013b90: 2069 6e20 7265 7665 7273 6564 2872 616e   in reversed(ran
-00013ba0: 6765 2863 6f75 6e74 2a32 2c20 6c65 6e28  ge(count*2, len(
-00013bb0: 616c 6c5f 776f 7264 735f 7374 7229 2b31  all_words_str)+1
-00013bc0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00013bd0: 2020 2020 2069 6620 6e65 7874 5f69 2069       if next_i i
-00013be0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-00013bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c00: 2069 6620 6e65 7874 5f69 2021 3d20 693a   if next_i != i:
-00013c10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013c20: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00013c30: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00013c40: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00013c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c60: 2020 2020 2020 206e 6578 745f 6920 3d20         next_i = 
-00013c70: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
-00013c80: 2020 2020 2020 7320 3d20 6920 2d20 636f        s = i - co
-00013c90: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-00013ca0: 2020 2020 2069 6620 616c 6c5f 776f 7264       if all_word
-00013cb0: 735f 7374 725b 7320 2d20 636f 756e 743a  s_str[s - count:
-00013cc0: 735d 2021 3d20 616c 6c5f 776f 7264 735f  s] != all_words_
-00013cd0: 7374 725b 733a 695d 3a0d 0a20 2020 2020  str[s:i]:..     
-00013ce0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013cf0: 6f6e 7469 6e75 650d 0a20 2020 2020 2020  ontinue..       
-00013d00: 2020 2020 2020 2020 206e 6578 745f 6920           next_i 
-00013d10: 3d20 730d 0a20 2020 2020 2020 2020 2020  = s..           
-00013d20: 2020 2020 2069 6620 6578 7465 6e64 5f64       if extend_d
-00013d30: 7572 6174 696f 6e3a 0d0a 2020 2020 2020  uration:..      
-00013d40: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00013d50: 6c5f 776f 7264 735b 732d 315d 2e65 6e64  l_words[s-1].end
-00013d60: 203d 2061 6c6c 5f77 6f72 6473 5b69 2d31   = all_words[i-1
-00013d70: 5d2e 656e 640d 0a20 2020 2020 2020 2020  ].end..         
-00013d80: 2020 2020 2020 2074 656d 705f 6368 616e         temp_chan
-00013d90: 6765 7320 3d20 5b5d 0d0a 2020 2020 2020  ges = []..      
-00013da0: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
-00013db0: 696e 2072 6576 6572 7365 6428 7261 6e67  in reversed(rang
-00013dc0: 6528 732c 2069 2929 3a0d 0a20 2020 2020  e(s, i)):..     
-00013dd0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00013de0: 6620 7665 7262 6f73 653a 0d0a 2020 2020  f verbose:..    
-00013df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e00: 2020 2020 7465 6d70 5f63 6861 6e67 6573      temp_changes
-00013e10: 2e61 7070 656e 6428 6627 2d20 7b61 6c6c  .append(f'- {all
-00013e20: 5f77 6f72 6473 5b6a 5d2e 746f 5f64 6963  _words[j].to_dic
-00013e30: 7428 297d 2729 0d0a 2020 2020 2020 2020  t()}')..        
-00013e40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013e50: 2e72 656d 6f76 655f 776f 7264 2861 6c6c  .remove_word(all
-00013e60: 5f77 6f72 6473 5b6a 5d2c 2046 616c 7365  _words[j], False
-00013e70: 2c20 7665 7262 6f73 653d 4661 6c73 6529  , verbose=False)
+000126c0: 2020 2020 2020 6966 2072 6967 6874 3a0d        if right:.
+000126d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000126e0: 2020 2020 2020 2020 2070 6172 742e 6c6f           part.lo
+000126f0: 636b 5f72 6967 6874 2829 0d0a 2020 2020  ck_right()..    
+00012700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012710: 6966 206c 6566 743a 0d0a 2020 2020 2020  if left:..      
+00012720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012730: 2020 7061 7274 2e6c 6f63 6b5f 6c65 6674    part.lock_left
+00012740: 2829 0d0a 2020 2020 2020 2020 6966 2073  ()..        if s
+00012750: 656c 662e 5f72 6567 726f 7570 5f68 6973  elf._regroup_his
+00012760: 746f 7279 3a0d 0a20 2020 2020 2020 2020  tory:..         
+00012770: 2020 2073 656c 662e 5f72 6567 726f 7570     self._regroup
+00012780: 5f68 6973 746f 7279 202b 3d20 275f 270d  _history += '_'.
+00012790: 0a20 2020 2020 2020 2073 7461 7274 7377  .        startsw
+000127a0: 6974 685f 7374 7220 3d20 2873 7461 7274  ith_str = (start
+000127b0: 7377 6974 6820 6966 2069 7369 6e73 7461  swith if isinsta
+000127c0: 6e63 6528 7374 6172 7473 7769 7468 2c20  nce(startswith, 
+000127d0: 7374 7229 2065 6c73 6520 272f 272e 6a6f  str) else '/'.jo
+000127e0: 696e 2873 7461 7274 7377 6974 6829 2920  in(startswith)) 
+000127f0: 6966 2073 7461 7274 7377 6974 6820 656c  if startswith el
+00012800: 7365 2022 220d 0a20 2020 2020 2020 2065  se ""..        e
+00012810: 6e64 7377 6974 685f 7374 7220 3d20 2865  ndswith_str = (e
+00012820: 6e64 7377 6974 6820 6966 2069 7369 6e73  ndswith if isins
+00012830: 7461 6e63 6528 656e 6473 7769 7468 2c20  tance(endswith, 
+00012840: 7374 7229 2065 6c73 6520 272f 272e 6a6f  str) else '/'.jo
+00012850: 696e 2865 6e64 7377 6974 6829 2920 6966  in(endswith)) if
+00012860: 2065 6e64 7377 6974 6820 656c 7365 2022   endswith else "
+00012870: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
+00012880: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
+00012890: 202b 3d20 2866 276c 3d7b 7374 6172 7473   += (f'l={starts
+000128a0: 7769 7468 5f73 7472 7d2b 7b65 6e64 7377  with_str}+{endsw
+000128b0: 6974 685f 7374 727d 270d 0a20 2020 2020  ith_str}'..     
+000128c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128d0: 2020 2020 2020 2020 2020 2020 2066 272b               f'+
+000128e0: 7b69 6e74 2872 6967 6874 297d 2b7b 696e  {int(right)}+{in
+000128f0: 7428 6c65 6674 297d 2b7b 696e 7428 6361  t(left)}+{int(ca
+00012900: 7365 5f73 656e 7369 7469 7665 297d 2b7b  se_sensitive)}+{
+00012910: 696e 7428 7374 7269 7029 7d27 290d 0a20  int(strip)}').. 
+00012920: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00012930: 6c66 0d0a 0d0a 2020 2020 6465 6620 7265  lf....    def re
+00012940: 6d6f 7665 5f77 6f72 6428 0d0a 2020 2020  move_word(..    
+00012950: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
+00012960: 2020 2020 2020 2020 2020 2077 6f72 643a             word:
+00012970: 2055 6e69 6f6e 5b57 6f72 6454 696d 696e   Union[WordTimin
+00012980: 672c 2054 7570 6c65 5b69 6e74 2c20 696e  g, Tuple[int, in
+00012990: 745d 5d2c 0d0a 2020 2020 2020 2020 2020  t]],..          
+000129a0: 2020 7265 6173 7369 676e 5f69 6473 3a20    reassign_ids: 
+000129b0: 626f 6f6c 203d 2054 7275 652c 0d0a 2020  bool = True,..  
+000129c0: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
+000129d0: 653a 2062 6f6f 6c20 3d20 5472 7565 0d0a  e: bool = True..
+000129e0: 2020 2020 2920 2d3e 2027 5768 6973 7065      ) -> 'Whispe
+000129f0: 7252 6573 756c 7427 3a0d 0a20 2020 2020  rResult':..     
+00012a00: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00012a10: 5265 6d6f 7665 2061 2077 6f72 642e 0d0a  Remove a word...
+00012a20: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00012a30: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
+00012a40: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
+00012a50: 2020 776f 7264 203a 2057 6f72 6454 696d    word : WordTim
+00012a60: 696e 6720 6f72 2074 7570 6c65 206f 6620  ing or tuple of 
+00012a70: 2869 6e74 2c20 696e 7429 0d0a 2020 2020  (int, int)..    
+00012a80: 2020 2020 2020 2020 496e 7374 616e 6365          Instance
+00012a90: 206f 6620 3a63 6c61 7373 3a60 7374 6162   of :class:`stab
+00012aa0: 6c65 5f77 6869 7370 6572 2e72 6573 756c  le_whisper.resul
+00012ab0: 742e 576f 7264 5469 6d69 6e67 6020 6f72  t.WordTiming` or
+00012ac0: 2074 7570 6c65 206f 6620 2873 6567 6d65   tuple of (segme
+00012ad0: 6e74 2069 6e64 6578 2c20 776f 7264 2069  nt index, word i
+00012ae0: 6e64 6578 292e 0d0a 2020 2020 2020 2020  ndex)...        
+00012af0: 7265 6173 7369 676e 5f69 6473 203a 2062  reassign_ids : b
+00012b00: 6f6f 6c2c 2064 6566 6175 6c74 2054 7275  ool, default Tru
+00012b10: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
+00012b20: 6865 7468 6572 2074 6f20 7265 6173 7369  hether to reassi
+00012b30: 676e 2073 6567 6d65 6e74 2061 6e64 2077  gn segment and w
+00012b40: 6f72 6420 6964 7320 2869 6e64 6963 6573  ord ids (indices
+00012b50: 2920 6166 7465 7220 7265 6d6f 7669 6e67  ) after removing
+00012b60: 2060 6077 6f72 6460 602e 0d0a 2020 2020   ``word``...    
+00012b70: 2020 2020 7665 7262 6f73 6520 3a20 626f      verbose : bo
+00012b80: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
+00012b90: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
+00012ba0: 6574 6865 7220 746f 2070 7269 6e74 2064  ether to print d
+00012bb0: 6574 6169 6c20 6f66 2074 6865 2072 656d  etail of the rem
+00012bc0: 6f76 6564 2077 6f72 642e 0d0a 0d0a 2020  oved word.....  
+00012bd0: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
+00012be0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
+00012bf0: 2020 2020 2020 2020 7374 6162 6c65 5f77          stable_w
+00012c00: 6869 7370 6572 2e72 6573 756c 742e 5768  hisper.result.Wh
+00012c10: 6973 7065 7252 6573 756c 740d 0a20 2020  isperResult..   
+00012c20: 2020 2020 2020 2020 2054 6865 2063 7572           The cur
+00012c30: 7265 6e74 2069 6e73 7461 6e63 6520 6166  rent instance af
+00012c40: 7465 7220 7468 6520 6368 616e 6765 732e  ter the changes.
+00012c50: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00012c60: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00012c70: 616e 6365 2877 6f72 642c 2057 6f72 6454  ance(word, WordT
+00012c80: 696d 696e 6729 3a0d 0a20 2020 2020 2020  iming):..       
+00012c90: 2020 2020 2069 6620 7365 6c66 5b77 6f72       if self[wor
+00012ca0: 642e 7365 676d 656e 745f 6964 5d5b 776f  d.segment_id][wo
+00012cb0: 7264 2e69 645d 2069 7320 6e6f 7420 776f  rd.id] is not wo
+00012cc0: 7264 3a0d 0a20 2020 2020 2020 2020 2020  rd:..           
+00012cd0: 2020 2020 2073 656c 662e 7265 6173 7369       self.reassi
+00012ce0: 676e 5f69 6473 2829 0d0a 2020 2020 2020  gn_ids()..      
+00012cf0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00012d00: 665b 776f 7264 2e73 6567 6d65 6e74 5f69  f[word.segment_i
+00012d10: 645d 5b77 6f72 642e 6964 5d20 6973 206e  d][word.id] is n
+00012d20: 6f74 2077 6f72 643a 0d0a 2020 2020 2020  ot word:..      
+00012d30: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00012d40: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+00012d50: 776f 7264 206e 6f74 2069 6e20 7265 7375  word not in resu
+00012d60: 6c74 2729 0d0a 2020 2020 2020 2020 2020  lt')..          
+00012d70: 2020 7365 675f 6964 2c20 776f 7264 5f69    seg_id, word_i
+00012d80: 6420 3d20 776f 7264 2e73 6567 6d65 6e74  d = word.segment
+00012d90: 5f69 642c 2077 6f72 642e 6964 0d0a 2020  _id, word.id..  
+00012da0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00012db0: 2020 2020 2020 2020 2073 6567 5f69 642c           seg_id,
+00012dc0: 2077 6f72 645f 6964 203d 2077 6f72 640d   word_id = word.
+00012dd0: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
+00012de0: 6f73 653a 0d0a 2020 2020 2020 2020 2020  ose:..          
+00012df0: 2020 7072 696e 7428 6627 5265 6d6f 7665    print(f'Remove
+00012e00: 643a 207b 7365 6c66 5b73 6567 5f69 645d  d: {self[seg_id]
+00012e10: 5b77 6f72 645f 6964 5d2e 746f 5f64 6963  [word_id].to_dic
+00012e20: 7428 297d 2729 0d0a 2020 2020 2020 2020  t()}')..        
+00012e30: 6465 6c20 7365 6c66 2e73 6567 6d65 6e74  del self.segment
+00012e40: 735b 7365 675f 6964 5d2e 776f 7264 735b  s[seg_id].words[
+00012e50: 776f 7264 5f69 645d 0d0a 2020 2020 2020  word_id]..      
+00012e60: 2020 6966 206e 6f74 2072 6561 7373 6967    if not reassig
+00012e70: 6e5f 6964 733a 0d0a 2020 2020 2020 2020  n_ids:..        
+00012e80: 2020 2020 7265 7475 726e 2073 656c 660d      return self.
+00012e90: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00012ea0: 5b73 6567 5f69 645d 2e68 6173 5f77 6f72  [seg_id].has_wor
+00012eb0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+00012ec0: 2073 656c 665b 7365 675f 6964 5d2e 7265   self[seg_id].re
+00012ed0: 6173 7369 676e 5f69 6473 2829 0d0a 2020  assign_ids()..  
+00012ee0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00012ef0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00012f00: 6d6f 7665 5f6e 6f5f 776f 7264 5f73 6567  move_no_word_seg
+00012f10: 6d65 6e74 7328 290d 0a20 2020 2020 2020  ments()..       
+00012f20: 2072 6574 7572 6e20 7365 6c66 0d0a 0d0a   return self....
+00012f30: 2020 2020 6465 6620 7265 6d6f 7665 5f73      def remove_s
+00012f40: 6567 6d65 6e74 280d 0a20 2020 2020 2020  egment(..       
+00012f50: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
+00012f60: 2020 2020 2020 2020 7365 676d 656e 743a          segment:
+00012f70: 2055 6e69 6f6e 5b53 6567 6d65 6e74 2c20   Union[Segment, 
+00012f80: 696e 745d 2c0d 0a20 2020 2020 2020 2020  int],..         
+00012f90: 2020 2072 6561 7373 6967 6e5f 6964 733a     reassign_ids:
+00012fa0: 2062 6f6f 6c20 3d20 5472 7565 2c0d 0a20   bool = True,.. 
+00012fb0: 2020 2020 2020 2020 2020 2076 6572 626f             verbo
+00012fc0: 7365 3a20 626f 6f6c 203d 2054 7275 650d  se: bool = True.
+00012fd0: 0a20 2020 2029 202d 3e20 2757 6869 7370  .    ) -> 'Whisp
+00012fe0: 6572 5265 7375 6c74 273a 0d0a 2020 2020  erResult':..    
+00012ff0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00013000: 2052 656d 6f76 6520 6120 7365 676d 656e   Remove a segmen
+00013010: 742e 0d0a 0d0a 2020 2020 2020 2020 5061  t.....        Pa
+00013020: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
+00013030: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
+00013040: 2020 2020 2020 7365 676d 656e 7420 3a20        segment : 
+00013050: 5365 676d 656e 7420 6f72 2069 6e74 0d0a  Segment or int..
+00013060: 2020 2020 2020 2020 2020 2020 496e 7374              Inst
+00013070: 616e 6365 203a 636c 6173 733a 6073 7461  ance :class:`sta
+00013080: 626c 655f 7768 6973 7065 722e 7265 7375  ble_whisper.resu
+00013090: 6c74 2e53 6567 6d65 6e74 6020 6f72 2073  lt.Segment` or s
+000130a0: 6567 6d65 6e74 2069 6e64 6578 2e0d 0a20  egment index... 
+000130b0: 2020 2020 2020 2072 6561 7373 6967 6e5f         reassign_
+000130c0: 6964 7320 3a20 626f 6f6c 2c20 6465 6661  ids : bool, defa
+000130d0: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
+000130e0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+000130f0: 2072 6561 7373 6967 6e20 7365 676d 656e   reassign segmen
+00013100: 7420 4944 7320 2869 6e64 6963 6573 2920  t IDs (indices) 
+00013110: 6166 7465 7220 7265 6d6f 7669 6e67 2060  after removing `
+00013120: 6073 6567 6d65 6e74 6060 2e0d 0a20 2020  `segment``...   
+00013130: 2020 2020 2076 6572 626f 7365 203a 2062       verbose : b
+00013140: 6f6f 6c2c 2064 6566 6175 6c74 2054 7275  ool, default Tru
+00013150: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
+00013160: 6865 7468 6572 2074 6f20 7072 696e 7420  hether to print 
+00013170: 6465 7461 696c 206f 6620 7468 6520 7265  detail of the re
+00013180: 6d6f 7665 6420 776f 7264 2e0d 0a0d 0a20  moved word..... 
+00013190: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
+000131a0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
+000131b0: 0a20 2020 2020 2020 2073 7461 626c 655f  .        stable_
+000131c0: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
+000131d0: 6869 7370 6572 5265 7375 6c74 0d0a 2020  hisperResult..  
+000131e0: 2020 2020 2020 2020 2020 5468 6520 6375            The cu
+000131f0: 7272 656e 7420 696e 7374 616e 6365 2061  rrent instance a
+00013200: 6674 6572 2074 6865 2063 6861 6e67 6573  fter the changes
+00013210: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+00013220: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00013230: 7461 6e63 6528 7365 676d 656e 742c 2053  tance(segment, S
+00013240: 6567 6d65 6e74 293a 0d0a 2020 2020 2020  egment):..      
+00013250: 2020 2020 2020 6966 2073 656c 665b 7365        if self[se
+00013260: 676d 656e 742e 6964 5d20 6973 206e 6f74  gment.id] is not
+00013270: 2073 6567 6d65 6e74 3a0d 0a20 2020 2020   segment:..     
+00013280: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013290: 7265 6173 7369 676e 5f69 6473 2829 0d0a  reassign_ids()..
+000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132b0: 6966 2073 656c 665b 7365 676d 656e 742e  if self[segment.
+000132c0: 6964 5d20 6973 206e 6f74 2073 6567 6d65  id] is not segme
+000132d0: 6e74 3a0d 0a20 2020 2020 2020 2020 2020  nt:..           
+000132e0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+000132f0: 616c 7565 4572 726f 7228 2773 6567 6d65  alueError('segme
+00013300: 6e74 206e 6f74 2069 6e20 7265 7375 6c74  nt not in result
+00013310: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+00013320: 7365 676d 656e 7420 3d20 7365 676d 656e  segment = segmen
+00013330: 742e 6964 0d0a 2020 2020 2020 2020 6966  t.id..        if
+00013340: 2076 6572 626f 7365 3a0d 0a20 2020 2020   verbose:..     
+00013350: 2020 2020 2020 2070 7269 6e74 2866 2752         print(f'R
+00013360: 656d 6f76 6564 3a20 5b69 643a 7b73 656c  emoved: [id:{sel
+00013370: 665b 7365 676d 656e 745d 2e69 647d 5d20  f[segment].id}] 
+00013380: 7b73 656c 665b 7365 676d 656e 745d 2e74  {self[segment].t
+00013390: 6f5f 6469 7370 6c61 795f 7374 7228 5472  o_display_str(Tr
+000133a0: 7565 297d 2729 0d0a 2020 2020 2020 2020  ue)}')..        
+000133b0: 6465 6c20 7365 6c66 2e73 6567 6d65 6e74  del self.segment
+000133c0: 735b 7365 676d 656e 745d 0d0a 2020 2020  s[segment]..    
+000133d0: 2020 2020 6966 206e 6f74 2072 6561 7373      if not reass
+000133e0: 6967 6e5f 6964 733a 0d0a 2020 2020 2020  ign_ids:..      
+000133f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00013400: 660d 0a20 2020 2020 2020 2073 656c 662e  f..        self.
+00013410: 7265 6173 7369 676e 5f69 6473 2854 7275  reassign_ids(Tru
+00013420: 652c 2073 7461 7274 3d73 6567 6d65 6e74  e, start=segment
+00013430: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00013440: 6e20 7365 6c66 0d0a 0d0a 2020 2020 6465  n self....    de
+00013450: 6620 7265 6d6f 7665 5f72 6570 6574 6974  f remove_repetit
+00013460: 696f 6e28 0d0a 2020 2020 2020 2020 2020  ion(..          
+00013470: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
+00013480: 2020 2020 206d 6178 5f77 6f72 6473 3a20       max_words: 
+00013490: 696e 7420 3d20 312c 0d0a 2020 2020 2020  int = 1,..      
+000134a0: 2020 2020 2020 6361 7365 5f73 656e 7369        case_sensi
+000134b0: 7469 7665 3a20 626f 6f6c 203d 2046 616c  tive: bool = Fal
+000134c0: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
+000134d0: 2073 7472 6970 3a20 626f 6f6c 203d 2054   strip: bool = T
+000134e0: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+000134f0: 2020 6967 6e6f 7265 5f70 756e 6374 7561    ignore_punctua
+00013500: 7469 6f6e 733a 2073 7472 203d 2022 5c22  tions: str = "\"
+00013510: 272c 2e3f 2122 2c0d 0a20 2020 2020 2020  ',.?!",..       
+00013520: 2020 2020 2065 7874 656e 645f 6475 7261       extend_dura
+00013530: 7469 6f6e 3a20 626f 6f6c 203d 2054 7275  tion: bool = Tru
+00013540: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00013550: 7665 7262 6f73 653a 2062 6f6f 6c20 3d20  verbose: bool = 
+00013560: 5472 7565 0d0a 2020 2020 2920 2d3e 2027  True..    ) -> '
+00013570: 5768 6973 7065 7252 6573 756c 7427 3a0d  WhisperResult':.
+00013580: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00013590: 2020 2020 2020 5265 6d6f 7665 2077 6f72        Remove wor
+000135a0: 6473 2074 6861 7420 7265 7065 6174 2063  ds that repeat c
+000135b0: 6f6e 7365 6375 7469 7665 6c79 2e0d 0a0d  onsecutively....
+000135c0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+000135d0: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
+000135e0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+000135f0: 206d 6178 5f77 6f72 6473 203a 2069 6e74   max_words : int
+00013600: 0d0a 2020 2020 2020 2020 2020 2020 4d61  ..            Ma
+00013610: 7869 6d75 6d20 6e75 6d62 6572 206f 6620  ximum number of 
+00013620: 776f 7264 7320 746f 206c 6f6f 6b20 666f  words to look fo
+00013630: 7220 636f 6e73 6563 7574 6976 656c 792e  r consecutively.
+00013640: 0d0a 2020 2020 2020 2020 6361 7365 5f73  ..        case_s
+00013650: 656e 7369 7469 7665 203a 2062 6f6f 6c2c  ensitive : bool,
+00013660: 2064 6566 6175 6c74 2046 616c 7365 0d0a   default False..
+00013670: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
+00013680: 6865 7220 7468 6520 6361 7365 206f 6620  her the case of 
+00013690: 776f 7264 7320 6e65 6564 2074 6f20 6d61  words need to ma
+000136a0: 7463 6820 746f 2062 6520 636f 6e73 6964  tch to be consid
+000136b0: 6572 6564 2061 7320 7265 7065 7469 7469  ered as repetiti
+000136c0: 6f6e 2e0d 0a20 2020 2020 2020 2073 7472  on...        str
+000136d0: 6970 203a 2062 6f6f 6c2c 2064 6566 6175  ip : bool, defau
+000136e0: 6c74 2054 7275 650d 0a20 2020 2020 2020  lt True..       
+000136f0: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
+00013700: 6967 6e6f 7265 2073 7061 6365 7320 6265  ignore spaces be
+00013710: 666f 7265 2061 6e64 2061 6674 6572 2065  fore and after e
+00013720: 6163 6820 776f 7264 2e0d 0a20 2020 2020  ach word...     
+00013730: 2020 2069 676e 6f72 655f 7075 6e63 7475     ignore_punctu
+00013740: 6174 696f 6e73 203a 2062 6f6f 6c2c 2064  ations : bool, d
+00013750: 6566 6175 6c74 2027 2227 2c2e 3f21 270d  efault '"',.?!'.
+00013760: 0a20 2020 2020 2020 2020 2020 2045 6e64  .            End
+00013770: 696e 6720 7075 6e63 7475 6174 696f 6e73  ing punctuations
+00013780: 2074 6f20 6967 6e6f 7265 2e0d 0a20 2020   to ignore...   
+00013790: 2020 2020 2065 7874 656e 645f 6475 7261       extend_dura
+000137a0: 7469 6f6e 3a20 626f 6f6c 2c20 6465 6661  tion: bool, defa
+000137b0: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
+000137c0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+000137d0: 2065 7874 656e 6420 7468 6520 6475 7261   extend the dura
+000137e0: 7469 6f6e 206f 6620 7468 6520 7072 6576  tion of the prev
+000137f0: 696f 7573 2077 6f72 6420 746f 2063 6f76  ious word to cov
+00013800: 6572 2074 6865 2064 7572 6174 696f 6e20  er the duration 
+00013810: 6f66 2074 6865 2072 6570 6574 6974 696f  of the repetitio
+00013820: 6e2e 0d0a 2020 2020 2020 2020 7665 7262  n...        verb
+00013830: 6f73 653a 2062 6f6f 6c2c 2064 6566 6175  ose: bool, defau
+00013840: 6c74 2054 7275 650d 0a20 2020 2020 2020  lt True..       
+00013850: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
+00013860: 7072 696e 7420 6465 7461 696c 206f 6620  print detail of 
+00013870: 7468 6520 7265 6d6f 7665 6420 7265 7065  the removed repe
+00013880: 7469 7469 6f6e 732e 0d0a 0d0a 2020 2020  titions.....    
+00013890: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
+000138a0: 2020 2020 202d 2d2d 2d2d 2d2d 0d0a 2020       -------..  
+000138b0: 2020 2020 2020 7374 6162 6c65 5f77 6869        stable_whi
+000138c0: 7370 6572 2e72 6573 756c 742e 5768 6973  sper.result.Whis
+000138d0: 7065 7252 6573 756c 740d 0a20 2020 2020  perResult..     
+000138e0: 2020 2020 2020 2054 6865 2063 7572 7265         The curre
+000138f0: 6e74 2069 6e73 7461 6e63 6520 6166 7465  nt instance afte
+00013900: 7220 7468 6520 6368 616e 6765 732e 0d0a  r the changes...
+00013910: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00013920: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00013930: 2e68 6173 5f77 6f72 6473 3a0d 0a20 2020  .has_words:..   
+00013940: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00013950: 7365 6c66 0d0a 0d0a 2020 2020 2020 2020  self....        
+00013960: 666f 7220 636f 756e 7420 696e 2072 616e  for count in ran
+00013970: 6765 2831 2c20 6d61 785f 776f 7264 7320  ge(1, max_words 
+00013980: 2b20 3129 3a0d 0a20 2020 2020 2020 2020  + 1):..         
+00013990: 2020 2061 6c6c 5f77 6f72 6473 203d 2073     all_words = s
+000139a0: 656c 662e 616c 6c5f 776f 7264 7328 290d  elf.all_words().
+000139b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000139c0: 6c65 6e28 616c 6c5f 776f 7264 7329 203c  len(all_words) <
+000139d0: 2032 3a0d 0a20 2020 2020 2020 2020 2020   2:..           
+000139e0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000139f0: 0d0a 2020 2020 2020 2020 2020 2020 616c  ..            al
+00013a00: 6c5f 776f 7264 735f 7374 7220 3d20 5b77  l_words_str = [w
+00013a10: 2e77 6f72 6420 666f 7220 7720 696e 2061  .word for w in a
+00013a20: 6c6c 5f77 6f72 6473 5d0d 0a20 2020 2020  ll_words]..     
+00013a30: 2020 2020 2020 2069 6620 7374 7269 703a         if strip:
+00013a40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013a50: 2020 616c 6c5f 776f 7264 735f 7374 7220    all_words_str 
+00013a60: 3d20 5b77 2e73 7472 6970 2829 2066 6f72  = [w.strip() for
+00013a70: 2077 2069 6e20 616c 6c5f 776f 7264 735f   w in all_words_
+00013a80: 7374 725d 0d0a 2020 2020 2020 2020 2020  str]..          
+00013a90: 2020 6966 2069 676e 6f72 655f 7075 6e63    if ignore_punc
+00013aa0: 7475 6174 696f 6e73 3a0d 0a20 2020 2020  tuations:..     
+00013ab0: 2020 2020 2020 2020 2020 2070 746e 203d             ptn =
+00013ac0: 2066 275b 7b69 676e 6f72 655f 7075 6e63   f'[{ignore_punc
+00013ad0: 7475 6174 696f 6e73 7d5d 2b24 270d 0a20  tuations}]+$'.. 
+00013ae0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00013af0: 6c6c 5f77 6f72 6473 5f73 7472 203d 205b  ll_words_str = [
+00013b00: 7265 2e73 7562 2870 746e 2c20 2727 2c20  re.sub(ptn, '', 
+00013b10: 7729 2066 6f72 2077 2069 6e20 616c 6c5f  w) for w in all_
+00013b20: 776f 7264 735f 7374 725d 0d0a 2020 2020  words_str]..    
+00013b30: 2020 2020 2020 2020 6966 206e 6f74 2063          if not c
+00013b40: 6173 655f 7365 6e73 6974 6976 653a 0d0a  ase_sensitive:..
+00013b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b60: 616c 6c5f 776f 7264 735f 7374 7220 3d20  all_words_str = 
+00013b70: 5b77 2e6c 6f77 6572 2829 2066 6f72 2077  [w.lower() for w
+00013b80: 2069 6e20 616c 6c5f 776f 7264 735f 7374   in all_words_st
+00013b90: 725d 0d0a 2020 2020 2020 2020 2020 2020  r]..            
+00013ba0: 6e65 7874 5f69 203d 204e 6f6e 650d 0a20  next_i = None.. 
+00013bb0: 2020 2020 2020 2020 2020 2063 6861 6e67             chang
+00013bc0: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
+00013bd0: 2020 2020 2066 6f72 2069 2069 6e20 7265       for i in re
+00013be0: 7665 7273 6564 2872 616e 6765 2863 6f75  versed(range(cou
+00013bf0: 6e74 2a32 2c20 6c65 6e28 616c 6c5f 776f  nt*2, len(all_wo
+00013c00: 7264 735f 7374 7229 2b31 2929 3a0d 0a20  rds_str)+1)):.. 
+00013c10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00013c20: 6620 6e65 7874 5f69 2069 7320 6e6f 7420  f next_i is not 
+00013c30: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00013c40: 2020 2020 2020 2020 2020 2069 6620 6e65             if ne
+00013c50: 7874 5f69 2021 3d20 693a 0d0a 2020 2020  xt_i != i:..    
+00013c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c70: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
+00013c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c90: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00013ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cb0: 206e 6578 745f 6920 3d20 4e6f 6e65 0d0a   next_i = None..
+00013cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cd0: 7320 3d20 6920 2d20 636f 756e 740d 0a20  s = i - count.. 
+00013ce0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00013cf0: 6620 616c 6c5f 776f 7264 735f 7374 725b  f all_words_str[
+00013d00: 7320 2d20 636f 756e 743a 735d 2021 3d20  s - count:s] != 
+00013d10: 616c 6c5f 776f 7264 735f 7374 725b 733a  all_words_str[s:
+00013d20: 695d 3a0d 0a20 2020 2020 2020 2020 2020  i]:..           
+00013d30: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00013d40: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00013d50: 2020 206e 6578 745f 6920 3d20 730d 0a20     next_i = s.. 
+00013d60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00013d70: 6620 6578 7465 6e64 5f64 7572 6174 696f  f extend_duratio
+00013d80: 6e3a 0d0a 2020 2020 2020 2020 2020 2020  n:..            
+00013d90: 2020 2020 2020 2020 616c 6c5f 776f 7264          all_word
+00013da0: 735b 732d 315d 2e65 6e64 203d 2061 6c6c  s[s-1].end = all
+00013db0: 5f77 6f72 6473 5b69 2d31 5d2e 656e 640d  _words[i-1].end.
+00013dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013dd0: 2074 656d 705f 6368 616e 6765 7320 3d20   temp_changes = 
+00013de0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00013df0: 2020 2020 666f 7220 6a20 696e 2072 6576      for j in rev
+00013e00: 6572 7365 6428 7261 6e67 6528 732c 2069  ersed(range(s, i
+00013e10: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00013e20: 2020 2020 2020 2020 2069 6620 7665 7262           if verb
+00013e30: 6f73 653a 0d0a 2020 2020 2020 2020 2020  ose:..          
+00013e40: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00013e50: 6d70 5f63 6861 6e67 6573 2e61 7070 656e  mp_changes.appen
+00013e60: 6428 6627 2d20 7b61 6c6c 5f77 6f72 6473  d(f'- {all_words
+00013e70: 5b6a 5d2e 746f 5f64 6963 7428 297d 2729  [j].to_dict()}')
 00013e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013e90: 2020 6966 2074 656d 705f 6368 616e 6765    if temp_change
-00013ea0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00013eb0: 2020 2020 2020 2020 6368 616e 6765 732e          changes.
-00013ec0: 6170 7065 6e64 280d 0a20 2020 2020 2020  append(..       
-00013ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ee0: 2066 2752 656d 6f76 653a 205b 7b66 6f72   f'Remove: [{for
-00013ef0: 6d61 745f 7469 6d65 7374 616d 7028 616c  mat_timestamp(al
-00013f00: 6c5f 776f 7264 735b 735d 2e73 7461 7274  l_words[s].start
-00013f10: 297d 202d 3e20 7b66 6f72 6d61 745f 7469  )} -> {format_ti
-00013f20: 6d65 7374 616d 7028 616c 6c5f 776f 7264  mestamp(all_word
-00013f30: 735b 692d 315d 2e65 6e64 297d 5d20 270d  s[i-1].end)}] '.
-00013f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013f50: 2020 2020 2020 2020 202b 2027 272e 6a6f           + ''.jo
-00013f60: 696e 285f 772e 776f 7264 2066 6f72 205f  in(_w.word for _
-00013f70: 7720 696e 2061 6c6c 5f77 6f72 6473 5b73  w in all_words[s
-00013f80: 3a69 5d29 202b 2027 5c6e 270d 0a20 2020  :i]) + '\n'..   
+00013e90: 2020 2020 2020 7365 6c66 2e72 656d 6f76        self.remov
+00013ea0: 655f 776f 7264 2861 6c6c 5f77 6f72 6473  e_word(all_words
+00013eb0: 5b6a 5d2c 2046 616c 7365 2c20 7665 7262  [j], False, verb
+00013ec0: 6f73 653d 4661 6c73 6529 0d0a 2020 2020  ose=False)..    
+00013ed0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00013ee0: 656d 705f 6368 616e 6765 733a 0d0a 2020  emp_changes:..  
+00013ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f00: 2020 6368 616e 6765 732e 6170 7065 6e64    changes.append
+00013f10: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00013f20: 2020 2020 2020 2020 2020 2066 2752 656d             f'Rem
+00013f30: 6f76 653a 205b 7b66 6f72 6d61 745f 7469  ove: [{format_ti
+00013f40: 6d65 7374 616d 7028 616c 6c5f 776f 7264  mestamp(all_word
+00013f50: 735b 735d 2e73 7461 7274 297d 202d 3e20  s[s].start)} -> 
+00013f60: 7b66 6f72 6d61 745f 7469 6d65 7374 616d  {format_timestam
+00013f70: 7028 616c 6c5f 776f 7264 735b 692d 315d  p(all_words[i-1]
+00013f80: 2e65 6e64 297d 5d20 270d 0a20 2020 2020  .end)}] '..     
 00013f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fa0: 2020 2020 202b 2027 5c6e 272e 6a6f 696e       + '\n'.join
-00013fb0: 2872 6576 6572 7365 6428 7465 6d70 5f63  (reversed(temp_c
-00013fc0: 6861 6e67 6573 2929 202b 2027 5c6e 270d  hanges)) + '\n'.
-00013fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013fe0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00013ff0: 2020 2020 2020 2020 666f 7220 6930 2c20          for i0, 
-00014000: 6931 2069 6e20 7a69 7028 7261 6e67 6528  i1 in zip(range(
-00014010: 7320 2d20 636f 756e 742c 2073 292c 2072  s - count, s), r
-00014020: 616e 6765 2873 2c20 6929 293a 0d0a 2020  ange(s, i)):..  
-00014030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014040: 2020 6966 206c 656e 2861 6c6c 5f77 6f72    if len(all_wor
-00014050: 6473 5b69 305d 2e77 6f72 6429 203c 206c  ds[i0].word) < l
-00014060: 656e 2861 6c6c 5f77 6f72 6473 5b69 315d  en(all_words[i1]
-00014070: 2e77 6f72 6429 3a0d 0a20 2020 2020 2020  .word):..       
-00014080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014090: 2061 6c6c 5f77 6f72 6473 5b69 315d 2e73   all_words[i1].s
-000140a0: 7461 7274 203d 2061 6c6c 5f77 6f72 6473  tart = all_words
-000140b0: 5b69 305d 2e73 7461 7274 0d0a 2020 2020  [i0].start..    
-000140c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140d0: 2020 2020 616c 6c5f 776f 7264 735b 6931      all_words[i1
-000140e0: 5d2e 656e 6420 3d20 616c 6c5f 776f 7264  ].end = all_word
-000140f0: 735b 6930 5d2e 656e 640d 0a20 2020 2020  s[i0].end..     
-00014100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014110: 2020 205f 7369 642c 205f 7769 6420 3d20     _sid, _wid = 
-00014120: 616c 6c5f 776f 7264 735b 6930 5d2e 7365  all_words[i0].se
-00014130: 676d 656e 745f 6964 2c20 616c 6c5f 776f  gment_id, all_wo
-00014140: 7264 735b 6930 5d2e 6964 0d0a 2020 2020  rds[i0].id..    
-00014150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014160: 2020 2020 7365 6c66 2e73 6567 6d65 6e74      self.segment
-00014170: 735b 5f73 6964 5d2e 776f 7264 735b 5f77  s[_sid].words[_w
-00014180: 6964 5d20 3d20 616c 6c5f 776f 7264 735b  id] = all_words[
-00014190: 6931 5d0d 0a0d 0a20 2020 2020 2020 2020  i1]....         
-000141a0: 2020 2069 6620 6368 616e 6765 733a 0d0a     if changes:..
-000141b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141c0: 7072 696e 7428 275c 6e27 2e6a 6f69 6e28  print('\n'.join(
-000141d0: 7265 7665 7273 6564 2863 6861 6e67 6573  reversed(changes
-000141e0: 2929 290d 0a0d 0a20 2020 2020 2020 2020  )))....         
-000141f0: 2020 2073 656c 662e 7265 6d6f 7665 5f6e     self.remove_n
-00014200: 6f5f 776f 7264 5f73 6567 6d65 6e74 7328  o_word_segments(
-00014210: 7265 6173 7369 676e 5f69 6473 3d46 616c  reassign_ids=Fal
-00014220: 7365 290d 0a20 2020 2020 2020 2073 656c  se)..        sel
-00014230: 662e 7265 6173 7369 676e 5f69 6473 2829  f.reassign_ids()
-00014240: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
-00014250: 726e 2073 656c 660d 0a0d 0a20 2020 2064  rn self....    d
-00014260: 6566 2072 656d 6f76 655f 776f 7264 735f  ef remove_words_
-00014270: 6279 5f73 7472 280d 0a20 2020 2020 2020  by_str(..       
-00014280: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
-00014290: 2020 2020 2020 2020 776f 7264 733a 2055          words: U
-000142a0: 6e69 6f6e 5b73 7472 2c20 4c69 7374 5b73  nion[str, List[s
-000142b0: 7472 5d2c 204e 6f6e 655d 2c0d 0a20 2020  tr], None],..   
-000142c0: 2020 2020 2020 2020 2063 6173 655f 7365           case_se
-000142d0: 6e73 6974 6976 653a 2062 6f6f 6c20 3d20  nsitive: bool = 
-000142e0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-000142f0: 2020 2020 7374 7269 703a 2062 6f6f 6c20      strip: bool 
-00014300: 3d20 5472 7565 2c0d 0a20 2020 2020 2020  = True,..       
-00014310: 2020 2020 2069 676e 6f72 655f 7075 6e63       ignore_punc
-00014320: 7475 6174 696f 6e73 3a20 7374 7220 3d20  tuations: str = 
-00014330: 225c 2227 2c2e 3f21 222c 0d0a 2020 2020  "\"',.?!",..    
-00014340: 2020 2020 2020 2020 6d69 6e5f 7072 6f62          min_prob
-00014350: 3a20 666c 6f61 7420 3d20 4e6f 6e65 2c0d  : float = None,.
-00014360: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-00014370: 7465 7273 3a20 4361 6c6c 6162 6c65 203d  ters: Callable =
-00014380: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00014390: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
-000143a0: 6c20 3d20 5472 7565 0d0a 2020 2020 2920  l = True..    ) 
-000143b0: 2d3e 2027 5768 6973 7065 7252 6573 756c  -> 'WhisperResul
-000143c0: 7427 3a0d 0a20 2020 2020 2020 2022 2222  t':..        """
-000143d0: 0d0a 2020 2020 2020 2020 5265 6d6f 7665  ..        Remove
-000143e0: 2077 6f72 6473 2074 6861 7420 6d61 7463   words that matc
-000143f0: 6820 6060 776f 7264 7360 602e 0d0a 0d0a  h ``words``.....
-00014400: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00014410: 7273 0d0a 2020 2020 2020 2020 2d2d 2d2d  rs..        ----
-00014420: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
-00014430: 776f 7264 7320 3a20 7374 7220 6f72 206c  words : str or l
-00014440: 6973 7420 6f66 2073 7472 206f 7220 4e6f  ist of str or No
-00014450: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
-00014460: 4120 776f 7264 206f 7220 6c69 7374 206f  A word or list o
-00014470: 6620 776f 7264 7320 746f 2072 656d 6f76  f words to remov
-00014480: 652e 6060 4e6f 6e65 6060 2066 6f72 2061  e.``None`` for a
-00014490: 6c6c 2077 6f72 6473 2074 6f20 6265 2070  ll words to be p
-000144a0: 6173 7365 6420 696e 746f 2060 6066 696c  assed into ``fil
-000144b0: 7465 7273 6060 2e0d 0a20 2020 2020 2020  ters``...       
-000144c0: 2063 6173 655f 7365 6e73 6974 6976 6520   case_sensitive 
-000144d0: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-000144e0: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
-000144f0: 2020 2057 6865 7468 6572 2074 6865 2063     Whether the c
-00014500: 6173 6520 6f66 2077 6f72 6473 206e 6565  ase of words nee
-00014510: 6420 746f 206d 6174 6368 2074 6f20 6265  d to match to be
-00014520: 2063 6f6e 7369 6465 7265 6420 6173 2072   considered as r
-00014530: 6570 6574 6974 696f 6e2e 0d0a 2020 2020  epetition...    
-00014540: 2020 2020 7374 7269 7020 3a20 626f 6f6c      strip : bool
-00014550: 2c20 6465 6661 756c 7420 5472 7565 0d0a  , default True..
-00014560: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
-00014570: 6865 7220 746f 2069 676e 6f72 6520 7370  her to ignore sp
-00014580: 6163 6573 2062 6566 6f72 6520 616e 6420  aces before and 
-00014590: 6166 7465 7220 6561 6368 2077 6f72 642e  after each word.
-000145a0: 0d0a 2020 2020 2020 2020 6967 6e6f 7265  ..        ignore
-000145b0: 5f70 756e 6374 7561 7469 6f6e 7320 3a20  _punctuations : 
-000145c0: 626f 6f6c 2c20 6465 6661 756c 7420 2722  bool, default '"
-000145d0: 272c 2e3f 2127 0d0a 2020 2020 2020 2020  ',.?!'..        
-000145e0: 2020 2020 456e 6469 6e67 2070 756e 6374      Ending punct
-000145f0: 7561 7469 6f6e 7320 746f 2069 676e 6f72  uations to ignor
-00014600: 652e 0d0a 2020 2020 2020 2020 6d69 6e5f  e...        min_
-00014610: 7072 6f62 203a 2066 6c6f 6174 2c20 6f70  prob : float, op
-00014620: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-00014630: 2020 2020 4163 7473 2061 7320 7468 6520      Acts as the 
-00014640: 6669 7273 7420 6669 6c74 6572 2074 6865  first filter the
-00014650: 2066 6f72 2074 6865 2077 6f72 6473 2074   for the words t
-00014660: 6861 7420 6d61 7463 6820 6060 776f 7264  hat match ``word
-00014670: 7360 602e 2057 6f72 6473 2077 6974 6820  s``. Words with 
-00014680: 7072 6f62 6162 696c 6974 7920 3c20 6060  probability < ``
-00014690: 6d69 6e5f 7072 6f62 6060 2077 696c 6c0d  min_prob`` will.
-000146a0: 0a20 2020 2020 2020 2020 2020 2062 6520  .            be 
-000146b0: 7265 6d6f 7665 6420 6966 2060 6066 696c  removed if ``fil
-000146c0: 7465 7273 6060 2069 7320 6060 4e6f 6e65  ters`` is ``None
-000146d0: 6060 2c20 656c 7365 2070 6173 7320 7468  ``, else pass th
-000146e0: 6520 776f 7264 7320 696e 746f 2060 6066  e words into ``f
-000146f0: 696c 7465 7273 6060 2e20 576f 7264 7320  ilters``. Words 
-00014700: 7769 7468 6f75 7420 7072 6f62 6162 696c  without probabil
-00014710: 6974 7920 7769 6c6c 0d0a 2020 2020 2020  ity will..      
-00014720: 2020 2020 2020 6265 2074 7265 6174 6564        be treated
-00014730: 2061 7320 6861 7669 6e67 2070 726f 6261   as having proba
-00014740: 6269 6c69 7479 203c 2060 606d 696e 5f70  bility < ``min_p
-00014750: 726f 6260 602e 0d0a 2020 2020 2020 2020  rob``...        
-00014760: 6669 6c74 6572 7320 3a20 4361 6c6c 6162  filters : Callab
-00014770: 6c65 2c20 6f70 7469 6f6e 616c 0d0a 2020  le, optional..  
-00014780: 2020 2020 2020 2020 2020 4120 6675 6e63            A func
-00014790: 7469 6f6e 2074 6861 7420 7461 6b65 7320  tion that takes 
-000147a0: 616e 2069 6e73 7461 6e63 6520 6f66 203a  an instance of :
-000147b0: 636c 6173 733a 6073 7461 626c 655f 7768  class:`stable_wh
-000147c0: 6973 7065 722e 7265 7375 6c74 2e57 6f72  isper.result.Wor
-000147d0: 6454 696d 696e 6760 2061 7320 6974 7320  dTiming` as its 
-000147e0: 6f6e 6c79 2061 7267 756d 656e 742e 0d0a  only argument...
-000147f0: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00014800: 2066 756e 6374 696f 6e20 6973 2063 7573   function is cus
-00014810: 746f 6d20 6669 6c74 6572 2066 6f72 2074  tom filter for t
-00014820: 6865 2077 6f72 6473 2074 6861 7420 6d61  he words that ma
-00014830: 7463 6820 6060 776f 7264 7360 6020 616e  tch ``words`` an
-00014840: 6420 7765 7265 206e 6f74 2063 6175 6768  d were not caugh
-00014850: 7420 6279 2060 606d 696e 5f70 726f 6260  t by ``min_prob`
-00014860: 602e 0d0a 2020 2020 2020 2020 7665 7262  `...        verb
-00014870: 6f73 653a 0d0a 2020 2020 2020 2020 2020  ose:..          
-00014880: 2020 5768 6574 6865 7220 746f 2070 7269    Whether to pri
-00014890: 6e74 2064 6574 6169 6c20 6f66 2074 6865  nt detail of the
-000148a0: 2072 656d 6f76 6564 2077 6f72 6473 2e0d   removed words..
-000148b0: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-000148c0: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
-000148d0: 2d2d 2d0d 0a20 2020 2020 2020 2073 7461  ---..        sta
-000148e0: 626c 655f 7768 6973 7065 722e 7265 7375  ble_whisper.resu
-000148f0: 6c74 2e57 6869 7370 6572 5265 7375 6c74  lt.WhisperResult
-00014900: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00014910: 6520 6375 7272 656e 7420 696e 7374 616e  e current instan
-00014920: 6365 2061 6674 6572 2074 6865 2063 6861  ce after the cha
-00014930: 6e67 6573 2e0d 0a20 2020 2020 2020 2022  nges...        "
-00014940: 2222 0d0a 2020 2020 2020 2020 6966 206e  ""..        if n
-00014950: 6f74 2073 656c 662e 6861 735f 776f 7264  ot self.has_word
-00014960: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00014970: 7265 7475 726e 2073 656c 660d 0a20 2020  return self..   
-00014980: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00014990: 6365 2877 6f72 6473 2c20 7374 7229 3a0d  ce(words, str):.
-000149a0: 0a20 2020 2020 2020 2020 2020 2077 6f72  .            wor
-000149b0: 6473 203d 205b 776f 7264 735d 0d0a 2020  ds = [words]..  
-000149c0: 2020 2020 2020 616c 6c5f 776f 7264 7320        all_words 
-000149d0: 3d20 7365 6c66 2e61 6c6c 5f77 6f72 6473  = self.all_words
-000149e0: 2829 0d0a 2020 2020 2020 2020 616c 6c5f  ()..        all_
-000149f0: 776f 7264 735f 7374 7220 3d20 5b77 2e77  words_str = [w.w
-00014a00: 6f72 6420 666f 7220 7720 696e 2061 6c6c  ord for w in all
-00014a10: 5f77 6f72 6473 5d0d 0a20 2020 2020 2020  _words]..       
-00014a20: 2069 6620 7374 7269 703a 0d0a 2020 2020   if strip:..    
-00014a30: 2020 2020 2020 2020 616c 6c5f 776f 7264          all_word
-00014a40: 735f 7374 7220 3d20 5b77 2e73 7472 6970  s_str = [w.strip
-00014a50: 2829 2066 6f72 2077 2069 6e20 616c 6c5f  () for w in all_
-00014a60: 776f 7264 735f 7374 725d 0d0a 2020 2020  words_str]..    
-00014a70: 2020 2020 2020 2020 776f 7264 7320 3d20          words = 
-00014a80: 5b77 2e73 7472 6970 2829 2066 6f72 2077  [w.strip() for w
-00014a90: 2069 6e20 776f 7264 735d 0d0a 2020 2020   in words]..    
-00014aa0: 2020 2020 6966 2069 676e 6f72 655f 7075      if ignore_pu
-00014ab0: 6e63 7475 6174 696f 6e73 3a0d 0a20 2020  nctuations:..   
-00014ac0: 2020 2020 2020 2020 2070 746e 203d 2066           ptn = f
-00014ad0: 275b 7b69 676e 6f72 655f 7075 6e63 7475  '[{ignore_punctu
-00014ae0: 6174 696f 6e73 7d5d 2b24 270d 0a20 2020  ations}]+$'..   
-00014af0: 2020 2020 2020 2020 2061 6c6c 5f77 6f72           all_wor
-00014b00: 6473 5f73 7472 203d 205b 7265 2e73 7562  ds_str = [re.sub
-00014b10: 2870 746e 2c20 2727 2c20 7729 2066 6f72  (ptn, '', w) for
-00014b20: 2077 2069 6e20 616c 6c5f 776f 7264 735f   w in all_words_
-00014b30: 7374 725d 0d0a 2020 2020 2020 2020 2020  str]..          
-00014b40: 2020 776f 7264 7320 3d20 5b72 652e 7375    words = [re.su
-00014b50: 6228 7074 6e2c 2027 272c 2077 2920 666f  b(ptn, '', w) fo
-00014b60: 7220 7720 696e 2077 6f72 6473 5d0d 0a20  r w in words].. 
-00014b70: 2020 2020 2020 2069 6620 6e6f 7420 6361         if not ca
-00014b80: 7365 5f73 656e 7369 7469 7665 3a0d 0a20  se_sensitive:.. 
-00014b90: 2020 2020 2020 2020 2020 2061 6c6c 5f77             all_w
-00014ba0: 6f72 6473 5f73 7472 203d 205b 772e 6c6f  ords_str = [w.lo
-00014bb0: 7765 7228 2920 666f 7220 7720 696e 2061  wer() for w in a
-00014bc0: 6c6c 5f77 6f72 6473 5f73 7472 5d0d 0a20  ll_words_str].. 
-00014bd0: 2020 2020 2020 2020 2020 2077 6f72 6473             words
-00014be0: 203d 205b 772e 6c6f 7765 7228 2920 666f   = [w.lower() fo
-00014bf0: 7220 7720 696e 2077 6f72 6473 5d0d 0a0d  r w in words]...
-00014c00: 0a20 2020 2020 2020 2063 6861 6e67 6573  .        changes
-00014c10: 203d 205b 5d0d 0a20 2020 2020 2020 2066   = []..        f
-00014c20: 6f72 2069 2c20 7720 696e 2072 6576 6572  or i, w in rever
-00014c30: 7365 6428 6c69 7374 2865 6e75 6d65 7261  sed(list(enumera
-00014c40: 7465 2861 6c6c 5f77 6f72 6473 5f73 7472  te(all_words_str
-00014c50: 2929 293a 0d0a 2020 2020 2020 2020 2020  ))):..          
-00014c60: 2020 6966 206e 6f74 2028 776f 7264 7320    if not (words 
-00014c70: 6973 204e 6f6e 6520 6f72 2061 6e79 2877  is None or any(w
-00014c80: 203d 3d20 5f77 2066 6f72 205f 7720 696e   == _w for _w in
-00014c90: 2077 6f72 6473 2929 3a0d 0a20 2020 2020   words)):..     
-00014ca0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-00014cb0: 6e75 650d 0a20 2020 2020 2020 2020 2020  nue..           
-00014cc0: 2069 6620 280d 0a20 2020 2020 2020 2020   if (..         
-00014cd0: 2020 2020 2020 2020 2020 2028 6d69 6e5f             (min_
-00014ce0: 7072 6f62 2069 7320 4e6f 6e65 206f 7220  prob is None or 
-00014cf0: 616c 6c5f 776f 7264 735b 695d 2e70 726f  all_words[i].pro
-00014d00: 6261 6269 6c69 7479 2069 7320 4e6f 6e65  bability is None
-00014d10: 206f 7220 6d69 6e5f 7072 6f62 203e 2061   or min_prob > a
-00014d20: 6c6c 5f77 6f72 6473 5b69 5d2e 7072 6f62  ll_words[i].prob
-00014d30: 6162 696c 6974 7929 2061 6e64 0d0a 2020  ability) and..  
-00014d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d50: 2020 2866 696c 7465 7273 2069 7320 4e6f    (filters is No
-00014d60: 6e65 206f 7220 6669 6c74 6572 7328 616c  ne or filters(al
-00014d70: 6c5f 776f 7264 735b 695d 2929 0d0a 2020  l_words[i]))..  
-00014d80: 2020 2020 2020 2020 2020 293a 0d0a 2020            ):..  
-00014d90: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00014da0: 2076 6572 626f 7365 3a0d 0a20 2020 2020   verbose:..     
-00014db0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00014dc0: 6861 6e67 6573 2e61 7070 656e 6428 6627  hanges.append(f'
-00014dd0: 5265 6d6f 7665 643a 207b 616c 6c5f 776f  Removed: {all_wo
-00014de0: 7264 735b 695d 2e74 6f5f 6469 6374 2829  rds[i].to_dict()
-00014df0: 7d27 290d 0a20 2020 2020 2020 2020 2020  }')..           
-00014e00: 2020 2020 2073 656c 662e 7265 6d6f 7665       self.remove
-00014e10: 5f77 6f72 6428 616c 6c5f 776f 7264 735b  _word(all_words[
-00014e20: 695d 2c20 4661 6c73 652c 2076 6572 626f  i], False, verbo
-00014e30: 7365 3d46 616c 7365 290d 0a20 2020 2020  se=False)..     
-00014e40: 2020 2069 6620 6368 616e 6765 733a 0d0a     if changes:..
-00014e50: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00014e60: 7428 275c 6e27 2e6a 6f69 6e28 7265 7665  t('\n'.join(reve
-00014e70: 7273 6564 2863 6861 6e67 6573 2929 290d  rsed(changes))).
-00014e80: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00014e90: 6d6f 7665 5f6e 6f5f 776f 7264 5f73 6567  move_no_word_seg
-00014ea0: 6d65 6e74 7328 290d 0a0d 0a20 2020 2020  ments()....     
-00014eb0: 2020 2072 6574 7572 6e20 7365 6c66 0d0a     return self..
-00014ec0: 0d0a 2020 2020 6465 6620 6669 6c6c 5f69  ..    def fill_i
-00014ed0: 6e5f 6761 7073 280d 0a20 2020 2020 2020  n_gaps(..       
-00014ee0: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
-00014ef0: 2020 2020 2020 2020 6f74 6865 725f 7265          other_re
-00014f00: 7375 6c74 3a20 556e 696f 6e5b 2757 6869  sult: Union['Whi
-00014f10: 7370 6572 5265 7375 6c74 272c 2073 7472  sperResult', str
-00014f20: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00014f30: 6d69 6e5f 6761 703a 2066 6c6f 6174 203d  min_gap: float =
-00014f40: 2030 2e31 2c0d 0a20 2020 2020 2020 2020   0.1,..         
-00014f50: 2020 2063 6173 655f 7365 6e73 6974 6976     case_sensitiv
-00014f60: 653a 2062 6f6f 6c20 3d20 4661 6c73 652c  e: bool = False,
-00014f70: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00014f80: 7269 703a 2062 6f6f 6c20 3d20 5472 7565  rip: bool = True
-00014f90: 2c0d 0a20 2020 2020 2020 2020 2020 2069  ,..            i
-00014fa0: 676e 6f72 655f 7075 6e63 7475 6174 696f  gnore_punctuatio
-00014fb0: 6e73 3a20 7374 7220 3d20 225c 2227 2c2e  ns: str = "\"',.
-00014fc0: 3f21 222c 0d0a 2020 2020 2020 2020 2020  ?!",..          
-00014fd0: 2020 7665 7262 6f73 653a 2062 6f6f 6c20    verbose: bool 
-00014fe0: 3d20 5472 7565 0d0a 2020 2020 2920 2d3e  = True..    ) ->
-00014ff0: 2027 5768 6973 7065 7252 6573 756c 7427   'WhisperResult'
-00015000: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00015010: 2020 2020 2020 2020 4669 6c6c 2069 6e20          Fill in 
-00015020: 7365 676d 656e 7420 6761 7073 206c 6172  segment gaps lar
-00015030: 6765 7220 7468 616e 2060 606d 696e 5f67  ger than ``min_g
-00015040: 6170 6060 2077 6974 6820 636f 6e74 656e  ap`` with conten
-00015050: 7420 6672 6f6d 2060 606f 7468 6572 5f72  t from ``other_r
-00015060: 6573 756c 7460 6020 6174 2074 6865 2074  esult`` at the t
-00015070: 696d 6573 206f 6620 6761 7073 2e0d 0a0d  imes of gaps....
-00015080: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00015090: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
-000150a0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-000150b0: 206f 7468 6572 5f72 6573 756c 7420 3a20   other_result : 
-000150c0: 5768 6973 7065 7252 6573 756c 7420 6f72  WhisperResult or
-000150d0: 2073 7472 0d0a 2020 2020 2020 2020 2020   str..          
-000150e0: 2020 416e 6f74 6865 7220 7472 616e 7363    Another transc
-000150f0: 7269 7074 696f 6e20 7265 7375 6c74 2061  ription result a
-00015100: 7320 616e 2069 6e73 7461 6e63 6520 6f66  s an instance of
-00015110: 203a 636c 6173 733a 6073 7461 626c 655f   :class:`stable_
-00015120: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
-00015130: 6869 7370 6572 5265 7375 6c74 6020 6f72  hisperResult` or
-00015140: 2070 6174 6820 746f 2074 6865 0d0a 2020   path to the..  
-00015150: 2020 2020 2020 2020 2020 4a53 4f4e 206f            JSON o
-00015160: 6620 7468 6520 7265 7375 6c74 2e0d 0a20  f the result... 
-00015170: 2020 2020 2020 206d 696e 5f67 6170 203a         min_gap :
-00015180: 2066 6c6f 6174 2c20 6465 6661 756c 7420   float, default 
-00015190: 302e 310d 0a20 2020 2020 2020 2020 2020  0.1..           
-000151a0: 2054 6865 206d 696e 696d 756d 2073 6563   The minimum sec
-000151b0: 6f6e 6473 206f 6620 6120 6761 7020 6265  onds of a gap be
-000151c0: 7477 6565 6e20 7365 676d 656e 7473 2074  tween segments t
-000151d0: 6861 7420 6d75 7374 2062 6520 6578 6365  hat must be exce
-000151e0: 6564 6564 2074 6f20 6265 2066 696c 6c65  eded to be fille
-000151f0: 6420 696e 2e0d 0a20 2020 2020 2020 2063  d in...        c
-00015200: 6173 655f 7365 6e73 6974 6976 6520 3a20  ase_sensitive : 
-00015210: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-00015220: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-00015230: 2057 6865 7468 6572 2074 6f20 636f 6e73   Whether to cons
-00015240: 6964 6572 2074 6865 2063 6173 6520 6f66  ider the case of
-00015250: 2074 6865 2066 6972 7374 2061 6e64 206c   the first and l
-00015260: 6173 7420 776f 7264 206f 6620 7468 6520  ast word of the 
-00015270: 6761 7020 746f 2064 6574 6572 6d69 6e65  gap to determine
-00015280: 206f 7665 726c 6170 7069 6e67 2077 6f72   overlapping wor
-00015290: 6473 2074 6f20 7265 6d6f 7665 0d0a 2020  ds to remove..  
-000152a0: 2020 2020 2020 2020 2020 6265 666f 7265            before
-000152b0: 2066 696c 6c69 6e67 2069 6e2e 0d0a 2020   filling in...  
-000152c0: 2020 2020 2020 7374 7269 7020 3a20 626f        strip : bo
-000152d0: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
-000152e0: 0d0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-000152f0: 6574 6865 7220 746f 2069 676e 6f72 6520  ether to ignore 
-00015300: 7370 6163 6573 2062 6566 6f72 6520 616e  spaces before an
-00015310: 6420 6166 7465 7220 7468 6520 6669 7273  d after the firs
-00015320: 7420 616e 6420 6c61 7374 2077 6f72 6420  t and last word 
-00015330: 6f66 2074 6865 2067 6170 2074 6f20 6465  of the gap to de
-00015340: 7465 726d 696e 6520 6f76 6572 6c61 7070  termine overlapp
-00015350: 696e 6720 776f 7264 730d 0a20 2020 2020  ing words..     
-00015360: 2020 2020 2020 2074 6f20 7265 6d6f 7665         to remove
-00015370: 2062 6566 6f72 6520 6669 6c6c 696e 6720   before filling 
-00015380: 696e 2e0d 0a20 2020 2020 2020 2069 676e  in...        ign
-00015390: 6f72 655f 7075 6e63 7475 6174 696f 6e73  ore_punctuations
-000153a0: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-000153b0: 2027 2227 2c2e 3f21 270d 0a20 2020 2020   '"',.?!'..     
-000153c0: 2020 2020 2020 2045 6e64 696e 6720 7075         Ending pu
-000153d0: 6e63 7475 6174 696f 6e73 2074 6f20 6967  nctuations to ig
-000153e0: 6e6f 7265 2069 6e20 7468 6520 6669 7273  nore in the firs
-000153f0: 7420 616e 6420 6c61 7374 2077 6f72 6420  t and last word 
-00015400: 6f66 2074 6865 2067 6170 2074 6f20 6465  of the gap to de
-00015410: 7465 726d 696e 6520 6f76 6572 6c61 7070  termine overlapp
-00015420: 696e 6720 776f 7264 7320 746f 0d0a 2020  ing words to..  
-00015430: 2020 2020 2020 2020 2020 7265 6d6f 7665            remove
-00015440: 2062 6566 6f72 6520 6669 6c6c 696e 6720   before filling 
-00015450: 696e 2e0d 0a20 2020 2020 2020 2076 6572  in...        ver
-00015460: 626f 7365 3a0d 0a20 2020 2020 2020 2020  bose:..         
-00015470: 2020 2057 6865 7468 6572 2074 6f20 7072     Whether to pr
-00015480: 696e 7420 6465 7461 696c 206f 6620 7468  int detail of th
-00015490: 6520 6669 6c6c 6564 2063 6f6e 7465 6e74  e filled content
-000154a0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
-000154b0: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
-000154c0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
-000154d0: 7461 626c 655f 7768 6973 7065 722e 7265  table_whisper.re
-000154e0: 7375 6c74 2e57 6869 7370 6572 5265 7375  sult.WhisperResu
-000154f0: 6c74 0d0a 2020 2020 2020 2020 2020 2020  lt..            
-00015500: 5468 6520 6375 7272 656e 7420 696e 7374  The current inst
-00015510: 616e 6365 2061 6674 6572 2074 6865 2063  ance after the c
-00015520: 6861 6e67 6573 2e0d 0a20 2020 2020 2020  hanges...       
-00015530: 2022 2222 0d0a 2020 2020 2020 2020 6966   """..        if
-00015540: 206c 656e 2873 656c 662e 7365 676d 656e   len(self.segmen
-00015550: 7473 2920 3c20 323a 0d0a 2020 2020 2020  ts) < 2:..      
-00015560: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00015570: 660d 0a20 2020 2020 2020 2069 6620 6973  f..        if is
-00015580: 696e 7374 616e 6365 286f 7468 6572 5f72  instance(other_r
-00015590: 6573 756c 742c 2073 7472 293a 0d0a 2020  esult, str):..  
-000155a0: 2020 2020 2020 2020 2020 6f74 6865 725f            other_
-000155b0: 7265 7375 6c74 203d 2057 6869 7370 6572  result = Whisper
-000155c0: 5265 7375 6c74 286f 7468 6572 5f72 6573  Result(other_res
-000155d0: 756c 7429 0d0a 0d0a 2020 2020 2020 2020  ult)....        
-000155e0: 6966 2073 7472 6970 3a0d 0a20 2020 2020  if strip:..     
-000155f0: 2020 2020 2020 2064 6566 2073 7472 6970         def strip
-00015600: 5f73 7061 6365 2877 293a 0d0a 2020 2020  _space(w):..    
-00015610: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00015620: 726e 2077 2e73 7472 6970 2829 0d0a 2020  rn w.strip()..  
-00015630: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00015640: 2020 2020 2020 2020 2064 6566 2073 7472           def str
-00015650: 6970 5f73 7061 6365 2877 293a 0d0a 2020  ip_space(w):..  
-00015660: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00015670: 7475 726e 2077 0d0a 0d0a 2020 2020 2020  turn w....      
-00015680: 2020 6966 2069 676e 6f72 655f 7075 6e63    if ignore_punc
-00015690: 7475 6174 696f 6e73 3a0d 0a20 2020 2020  tuations:..     
-000156a0: 2020 2020 2020 2070 746e 203d 2066 275b         ptn = f'[
-000156b0: 7b69 676e 6f72 655f 7075 6e63 7475 6174  {ignore_punctuat
-000156c0: 696f 6e73 7d5d 2b24 270d 0a0d 0a20 2020  ions}]+$'....   
-000156d0: 2020 2020 2020 2020 2064 6566 2073 7472           def str
-000156e0: 6970 5f70 756e 6374 7561 7469 6f6e 7328  ip_punctuations(
-000156f0: 7729 3a0d 0a20 2020 2020 2020 2020 2020  w):..           
-00015700: 2020 2020 2072 6574 7572 6e20 7265 2e73       return re.s
-00015710: 7562 2870 746e 2c20 2727 2c20 7374 7269  ub(ptn, '', stri
-00015720: 705f 7370 6163 6528 7729 290d 0a20 2020  p_space(w))..   
-00015730: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00015740: 2020 2020 2020 2020 7374 7269 705f 7075          strip_pu
-00015750: 6e63 7475 6174 696f 6e73 203d 2073 7472  nctuations = str
-00015760: 6970 5f73 7061 6365 0d0a 0d0a 2020 2020  ip_space....    
-00015770: 2020 2020 6966 2063 6173 655f 7365 6e73      if case_sens
-00015780: 6974 6976 653a 0d0a 2020 2020 2020 2020  itive:..        
-00015790: 2020 2020 7374 7269 7020 3d20 7374 7269      strip = stri
-000157a0: 705f 7075 6e63 7475 6174 696f 6e73 0d0a  p_punctuations..
-000157b0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-000157c0: 2020 2020 2020 2020 2020 2064 6566 2073             def s
-000157d0: 7472 6970 2877 293a 0d0a 2020 2020 2020  trip(w):..      
-000157e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000157f0: 2073 7472 6970 5f70 756e 6374 7561 7469   strip_punctuati
-00015800: 6f6e 7328 7729 2e6c 6f77 6572 2829 0d0a  ons(w).lower()..
-00015810: 0d0a 2020 2020 2020 2020 7365 675f 7061  ..        seg_pa
-00015820: 6972 7320 3d20 6c69 7374 2865 6e75 6d65  irs = list(enume
-00015830: 7261 7465 287a 6970 2873 656c 662e 7365  rate(zip(self.se
-00015840: 676d 656e 7473 5b3a 2d31 5d2c 2073 656c  gments[:-1], sel
-00015850: 662e 7365 676d 656e 7473 5b31 3a5d 2929  f.segments[1:]))
-00015860: 290d 0a20 2020 2020 2020 2073 6567 5f70  )..        seg_p
-00015870: 6169 7273 2e69 6e73 6572 7428 302c 2028  airs.insert(0, (
-00015880: 2d31 2c20 284e 6f6e 652c 2073 656c 662e  -1, (None, self.
-00015890: 7365 676d 656e 7473 5b30 5d29 2929 0d0a  segments[0])))..
-000158a0: 2020 2020 2020 2020 7365 675f 7061 6972          seg_pair
-000158b0: 732e 6170 7065 6e64 2828 7365 675f 7061  s.append((seg_pa
-000158c0: 6972 735b 2d31 5d5b 305d 2b31 2c20 2873  irs[-1][0]+1, (s
-000158d0: 656c 662e 7365 676d 656e 7473 5b2d 315d  elf.segments[-1]
-000158e0: 2c20 4e6f 6e65 2929 290d 0a0d 0a20 2020  , None)))....   
-000158f0: 2020 2020 2063 6861 6e67 6573 203d 205b       changes = [
-00015900: 5d0d 0a20 2020 2020 2020 2066 6f72 2069  ]..        for i
-00015910: 2c20 2873 6567 302c 2073 6567 3129 2069  , (seg0, seg1) i
-00015920: 6e20 7265 7665 7273 6564 2873 6567 5f70  n reversed(seg_p
-00015930: 6169 7273 293a 0d0a 2020 2020 2020 2020  airs):..        
-00015940: 2020 2020 6669 7273 745f 776f 7264 203d      first_word =
-00015950: 204e 6f6e 6520 6966 2073 6567 3020 6973   None if seg0 is
-00015960: 204e 6f6e 6520 656c 7365 2073 6567 302e   None else seg0.
-00015970: 776f 7264 735b 2d31 5d0d 0a20 2020 2020  words[-1]..     
-00015980: 2020 2020 2020 206c 6173 745f 776f 7264         last_word
-00015990: 203d 204e 6f6e 6520 6966 2073 6567 3120   = None if seg1 
-000159a0: 6973 204e 6f6e 6520 656c 7365 2073 6567  is None else seg
-000159b0: 312e 776f 7264 735b 305d 0d0a 2020 2020  1.words[0]..    
-000159c0: 2020 2020 2020 2020 7374 6172 7420 3d20          start = 
-000159d0: 286f 7468 6572 5f72 6573 756c 745b 305d  (other_result[0]
-000159e0: 2e73 7461 7274 2069 6620 6669 7273 745f  .start if first_
-000159f0: 776f 7264 2069 7320 4e6f 6e65 2065 6c73  word is None els
-00015a00: 6520 6669 7273 745f 776f 7264 2e65 6e64  e first_word.end
-00015a10: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00015a20: 6e64 203d 206f 7468 6572 5f72 6573 756c  nd = other_resul
-00015a30: 745b 2d31 5d2e 656e 6420 6966 206c 6173  t[-1].end if las
-00015a40: 745f 776f 7264 2069 7320 4e6f 6e65 2065  t_word is None e
-00015a50: 6c73 6520 6c61 7374 5f77 6f72 642e 7374  lse last_word.st
-00015a60: 6172 740d 0a20 2020 2020 2020 2020 2020  art..           
-00015a70: 2069 6620 656e 6420 2d20 7374 6172 7420   if end - start 
-00015a80: 3c3d 206d 696e 5f67 6170 3a0d 0a20 2020  <= min_gap:..   
-00015a90: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00015aa0: 7469 6e75 650d 0a20 2020 2020 2020 2020  tinue..         
-00015ab0: 2020 2067 6170 5f77 6f72 6473 203d 206f     gap_words = o
-00015ac0: 7468 6572 5f72 6573 756c 742e 6765 745f  ther_result.get_
-00015ad0: 636f 6e74 656e 745f 6279 5f74 696d 6528  content_by_time(
-00015ae0: 2873 7461 7274 2c20 656e 6429 290d 0a20  (start, end)).. 
-00015af0: 2020 2020 2020 2020 2020 2069 6620 6669             if fi
-00015b00: 7273 745f 776f 7264 2069 7320 6e6f 7420  rst_word is not 
-00015b10: 4e6f 6e65 2061 6e64 2067 6170 5f77 6f72  None and gap_wor
-00015b20: 6473 2061 6e64 2073 7472 6970 2866 6972  ds and strip(fir
-00015b30: 7374 5f77 6f72 642e 776f 7264 2920 3d3d  st_word.word) ==
-00015b40: 2073 7472 6970 2867 6170 5f77 6f72 6473   strip(gap_words
-00015b50: 5b30 5d2e 776f 7264 293a 0d0a 2020 2020  [0].word):..    
-00015b60: 2020 2020 2020 2020 2020 2020 6669 7273              firs
-00015b70: 745f 776f 7264 2e65 6e64 203d 2067 6170  t_word.end = gap
-00015b80: 5f77 6f72 6473 5b30 5d2e 656e 640d 0a20  _words[0].end.. 
-00015b90: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00015ba0: 6170 5f77 6f72 6473 203d 2067 6170 5f77  ap_words = gap_w
-00015bb0: 6f72 6473 5b31 3a5d 0d0a 2020 2020 2020  ords[1:]..      
-00015bc0: 2020 2020 2020 6966 206c 6173 745f 776f        if last_wo
-00015bd0: 7264 2069 7320 6e6f 7420 4e6f 6e65 2061  rd is not None a
-00015be0: 6e64 2067 6170 5f77 6f72 6473 2061 6e64  nd gap_words and
-00015bf0: 2073 7472 6970 286c 6173 745f 776f 7264   strip(last_word
-00015c00: 2e77 6f72 6429 203d 3d20 7374 7269 7028  .word) == strip(
-00015c10: 6761 705f 776f 7264 735b 2d31 5d2e 776f  gap_words[-1].wo
-00015c20: 7264 293a 0d0a 2020 2020 2020 2020 2020  rd):..          
-00015c30: 2020 2020 2020 6c61 7374 5f77 6f72 642e        last_word.
-00015c40: 7374 6172 7420 3d20 6761 705f 776f 7264  start = gap_word
-00015c50: 735b 2d31 5d2e 7374 6172 740d 0a20 2020  s[-1].start..   
-00015c60: 2020 2020 2020 2020 2020 2020 2067 6170               gap
-00015c70: 5f77 6f72 6473 203d 2067 6170 5f77 6f72  _words = gap_wor
-00015c80: 6473 5b3a 2d31 5d0d 0a20 2020 2020 2020  ds[:-1]..       
-00015c90: 2020 2020 2069 6620 6e6f 7420 6761 705f       if not gap_
-00015ca0: 776f 7264 733a 0d0a 2020 2020 2020 2020  words:..        
-00015cb0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00015cc0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00015cd0: 206c 6173 745f 776f 7264 2069 7320 6e6f   last_word is no
-00015ce0: 7420 4e6f 6e65 2061 6e64 206c 6173 745f  t None and last_
-00015cf0: 776f 7264 2e73 7461 7274 203c 2067 6170  word.start < gap
-00015d00: 5f77 6f72 6473 5b2d 315d 2e65 6e64 3a0d  _words[-1].end:.
-00015d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015d20: 206c 6173 745f 776f 7264 2e73 7461 7274   last_word.start
-00015d30: 203d 2067 6170 5f77 6f72 6473 5b2d 315d   = gap_words[-1]
-00015d40: 2e65 6e64 0d0a 2020 2020 2020 2020 2020  .end..          
-00015d50: 2020 6e65 775f 7365 676d 656e 7473 203d    new_segments =
-00015d60: 205b 6f74 6865 725f 7265 7375 6c74 5b67   [other_result[g
-00015d70: 6170 5f77 6f72 6473 5b30 5d2e 7365 676d  ap_words[0].segm
-00015d80: 656e 745f 6964 5d2e 636f 7079 285b 5d29  ent_id].copy([])
-00015d90: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
-00015da0: 6f72 206a 2c20 6e65 775f 776f 7264 2069  or j, new_word i
-00015db0: 6e20 656e 756d 6572 6174 6528 6761 705f  n enumerate(gap_
-00015dc0: 776f 7264 7329 3a0d 0a20 2020 2020 2020  words):..       
-00015dd0: 2020 2020 2020 2020 206e 6577 5f77 6f72           new_wor
-00015de0: 645f 636f 7079 203d 206e 6577 5f77 6f72  d_copy = new_wor
-00015df0: 642e 636f 7079 2863 6f70 795f 746f 6b65  d.copy(copy_toke
-00015e00: 6e73 3d54 7275 6529 0d0a 2020 2020 2020  ns=True)..      
-00015e10: 2020 2020 2020 2020 2020 6966 206a 203d            if j =
-00015e20: 3d20 3020 616e 6420 6669 7273 745f 776f  = 0 and first_wo
-00015e30: 7264 2069 7320 6e6f 7420 4e6f 6e65 2061  rd is not None a
-00015e40: 6e64 2066 6972 7374 5f77 6f72 642e 656e  nd first_word.en
-00015e50: 6420 3e20 6761 705f 776f 7264 735b 305d  d > gap_words[0]
-00015e60: 2e73 7461 7274 3a0d 0a20 2020 2020 2020  .start:..       
-00015e70: 2020 2020 2020 2020 2020 2020 206e 6577               new
-00015e80: 5f77 6f72 645f 636f 7079 2e73 7461 7274  _word_copy.start
-00015e90: 203d 2066 6972 7374 5f77 6f72 642e 656e   = first_word.en
-00015ea0: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
-00015eb0: 2020 2069 6620 6e65 775f 7365 676d 656e     if new_segmen
-00015ec0: 7473 5b2d 315d 2e69 6420 213d 206e 6577  ts[-1].id != new
-00015ed0: 5f77 6f72 642e 7365 676d 656e 745f 6964  _word.segment_id
-00015ee0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00015ef0: 2020 2020 2020 206e 6577 5f73 6567 6d65         new_segme
-00015f00: 6e74 732e 6170 7065 6e64 286f 7468 6572  nts.append(other
-00015f10: 5f72 6573 756c 745b 6e65 775f 776f 7264  _result[new_word
-00015f20: 2e73 6567 6d65 6e74 5f69 645d 2e63 6f70  .segment_id].cop
-00015f30: 7928 5b5d 2929 0d0a 2020 2020 2020 2020  y([]))..        
-00015f40: 2020 2020 2020 2020 6e65 775f 7365 676d          new_segm
-00015f50: 656e 7473 5b2d 315d 2e77 6f72 6473 2e61  ents[-1].words.a
-00015f60: 7070 656e 6428 6e65 775f 776f 7264 5f63  ppend(new_word_c
-00015f70: 6f70 7929 0d0a 2020 2020 2020 2020 2020  opy)..          
-00015f80: 2020 6966 2076 6572 626f 7365 3a0d 0a20    if verbose:.. 
-00015f90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00015fa0: 6861 6e67 6573 2e61 7070 656e 6428 275c  hanges.append('\
-00015fb0: 6e27 2e6a 6f69 6e28 2741 6464 6564 3a20  n'.join('Added: 
-00015fc0: 2720 2b20 732e 746f 5f64 6973 706c 6179  ' + s.to_display
-00015fd0: 5f73 7472 2854 7275 6529 2066 6f72 2073  _str(True) for s
-00015fe0: 2069 6e20 6e65 775f 7365 676d 656e 7473   in new_segments
-00015ff0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00016000: 7365 6c66 2e73 6567 6d65 6e74 7320 3d20  self.segments = 
-00016010: 7365 6c66 2e73 6567 6d65 6e74 735b 3a69  self.segments[:i
-00016020: 2b31 5d20 2b20 6e65 775f 7365 676d 656e  +1] + new_segmen
-00016030: 7473 202b 2073 656c 662e 7365 676d 656e  ts + self.segmen
-00016040: 7473 5b69 2b31 3a5d 0d0a 2020 2020 2020  ts[i+1:]..      
-00016050: 2020 6966 2063 6861 6e67 6573 3a0d 0a20    if changes:.. 
-00016060: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00016070: 2827 5c6e 272e 6a6f 696e 2872 6576 6572  ('\n'.join(rever
-00016080: 7365 6428 6368 616e 6765 7329 2929 0d0a  sed(changes)))..
-00016090: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
-000160a0: 7373 6967 6e5f 6964 7328 290d 0a0d 0a20  ssign_ids().... 
-000160b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000160c0: 6c66 0d0a 0d0a 2020 2020 6465 6620 7265  lf....    def re
-000160d0: 6772 6f75 7028 0d0a 2020 2020 2020 2020  group(..        
-000160e0: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
-000160f0: 2020 2020 2020 2072 6567 726f 7570 5f61         regroup_a
-00016100: 6c67 6f3a 2055 6e69 6f6e 5b73 7472 2c20  lgo: Union[str, 
-00016110: 626f 6f6c 5d20 3d20 4e6f 6e65 2c0d 0a20  bool] = None,.. 
-00016120: 2020 2020 2020 2020 2020 2076 6572 626f             verbo
-00016130: 7365 3a20 626f 6f6c 203d 2046 616c 7365  se: bool = False
-00016140: 2c0d 0a20 2020 2020 2020 2020 2020 206f  ,..            o
-00016150: 6e6c 795f 7368 6f77 3a20 626f 6f6c 203d  nly_show: bool =
-00016160: 2046 616c 7365 0d0a 2020 2020 2920 2d3e   False..    ) ->
-00016170: 2022 5768 6973 7065 7252 6573 756c 7422   "WhisperResult"
-00016180: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00016190: 2020 2020 2020 2020 5265 6772 6f75 7020          Regroup 
-000161a0: 2869 6e2d 706c 6163 6529 2077 6f72 6473  (in-place) words
-000161b0: 2069 6e74 6f20 7365 676d 656e 7473 2e0d   into segments..
-000161c0: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-000161d0: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
-000161e0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
-000161f0: 2020 2072 6567 726f 7570 5f61 6c67 6f3a     regroup_algo:
-00016200: 2073 7472 206f 7220 626f 6f6c 2c20 6465   str or bool, de
-00016210: 6661 756c 7420 2764 6127 0d0a 2020 2020  fault 'da'..    
-00016220: 2020 2020 2020 2020 2053 7472 696e 6720           String 
-00016230: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
-00016240: 6620 6120 6375 7374 6f6d 2072 6567 726f  f a custom regro
-00016250: 7570 696e 6720 616c 676f 7269 7468 6d20  uping algorithm 
-00016260: 6f72 2060 6054 7275 6560 6020 7573 6520  or ``True`` use 
-00016270: 746f 2074 6865 2064 6566 6175 6c74 2061  to the default a
-00016280: 6c67 6f72 6974 686d 2027 6461 272e 0d0a  lgorithm 'da'...
-00016290: 2020 2020 2020 2020 7665 7262 6f73 6520          verbose 
-000162a0: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-000162b0: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
-000162c0: 2020 2057 6865 7468 6572 2074 6f20 7368     Whether to sh
-000162d0: 6f77 2061 6c6c 2074 6865 206d 6574 686f  ow all the metho
-000162e0: 6473 2061 6e64 2061 7267 756d 656e 7473  ds and arguments
-000162f0: 2070 6172 7365 6420 6672 6f6d 2060 6072   parsed from ``r
-00016300: 6567 726f 7570 5f61 6c67 6f60 602e 0d0a  egroup_algo``...
-00016310: 2020 2020 2020 2020 6f6e 6c79 5f73 686f          only_sho
-00016320: 7720 3a20 626f 6f6c 2c20 6465 6661 756c  w : bool, defaul
-00016330: 7420 4661 6c73 650d 0a20 2020 2020 2020  t False..       
-00016340: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
-00016350: 7368 6f77 2074 6865 2061 6c6c 206d 6574  show the all met
-00016360: 686f 6473 2061 6e64 2061 7267 756d 656e  hods and argumen
-00016370: 7473 2070 6172 7365 6420 6672 6f6d 2060  ts parsed from `
-00016380: 6072 6567 726f 7570 5f61 6c67 6f60 6020  `regroup_algo`` 
-00016390: 7769 7468 6f75 7420 7275 6e6e 696e 6720  without running 
-000163a0: 7468 6520 6d65 7468 6f64 730d 0a0d 0a20  the methods.... 
-000163b0: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
-000163c0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
-000163d0: 0a20 2020 2020 2020 2073 7461 626c 655f  .        stable_
-000163e0: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
-000163f0: 6869 7370 6572 5265 7375 6c74 0d0a 2020  hisperResult..  
-00016400: 2020 2020 2020 2020 2020 5468 6520 6375            The cu
-00016410: 7272 656e 7420 696e 7374 616e 6365 2061  rrent instance a
-00016420: 6674 6572 2074 6865 2063 6861 6e67 6573  fter the changes
-00016430: 2e0d 0a0d 0a20 2020 2020 2020 204e 6f74  .....        Not
-00016440: 6573 0d0a 2020 2020 2020 2020 2d2d 2d2d  es..        ----
-00016450: 2d0d 0a20 2020 2020 2020 2053 796e 7461  -..        Synta
-00016460: 7820 666f 7220 7374 7269 6e67 2072 6570  x for string rep
-00016470: 7265 7365 6e74 6174 696f 6e20 6f66 2063  resentation of c
-00016480: 7573 746f 6d20 7265 6772 6f75 7069 6e67  ustom regrouping
-00016490: 2061 6c67 6f72 6974 686d 2e0d 0a20 2020   algorithm...   
-000164a0: 2020 2020 2020 2020 204d 6574 686f 6420           Method 
-000164b0: 6b65 7973 3a0d 0a20 2020 2020 2020 2020  keys:..         
-000164c0: 2020 2020 2020 2073 673a 2073 706c 6974         sg: split
-000164d0: 5f62 795f 6761 700d 0a20 2020 2020 2020  _by_gap..       
-000164e0: 2020 2020 2020 2020 2073 703a 2073 706c           sp: spl
-000164f0: 6974 5f62 795f 7075 6e63 7475 6174 696f  it_by_punctuatio
-00016500: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00016510: 2020 2073 6c3a 2073 706c 6974 5f62 795f     sl: split_by_
-00016520: 6c65 6e67 7468 0d0a 2020 2020 2020 2020  length..        
-00016530: 2020 2020 2020 2020 7364 3a20 7370 6c69          sd: spli
-00016540: 745f 6279 5f64 7572 6174 696f 6e0d 0a20  t_by_duration.. 
-00016550: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00016560: 673a 206d 6572 6765 5f62 795f 6761 700d  g: merge_by_gap.
-00016570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016580: 206d 703a 206d 6572 6765 5f62 795f 7075   mp: merge_by_pu
-00016590: 6e63 7475 6174 696f 6e0d 0a20 2020 2020  nctuation..     
-000165a0: 2020 2020 2020 2020 2020 206d 733a 206d             ms: m
-000165b0: 6572 6765 5f61 6c6c 5f73 6567 6d65 6e74  erge_all_segment
-000165c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000165d0: 2020 636d 3a20 636c 616d 705f 6d61 780d    cm: clamp_max.
-000165e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000165f0: 206c 3a20 6c6f 636b 0d0a 2020 2020 2020   l: lock..      
-00016600: 2020 2020 2020 2020 2020 7573 3a20 756e            us: un
-00016610: 6c6f 636b 5f61 6c6c 5f73 6567 6d65 6e74  lock_all_segment
-00016620: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-00016630: 2020 2064 613a 2064 6566 6175 6c74 2061     da: default a
-00016640: 6c67 6f72 6974 686d 2028 636d 5f73 703d  lgorithm (cm_sp=
-00016650: 2c2a 202f efbc 8c5f 7367 3d2e 355f 6d67  ,* /..._sg=.5_mg
-00016660: 3d2e 332b 335f 7370 3d2e 2a20 2fe3 8082  =.3+3_sp=.* /...
-00016670: 2f3f 2fef bc9f 290d 0a20 2020 2020 2020  /?/...)..       
-00016680: 2020 2020 2020 2020 2072 773a 2072 656d           rw: rem
-00016690: 6f76 655f 776f 7264 0d0a 2020 2020 2020  ove_word..      
-000166a0: 2020 2020 2020 2020 2020 7273 3a20 7265            rs: re
-000166b0: 6d6f 7665 5f73 6567 6d65 6e74 0d0a 2020  move_segment..  
-000166c0: 2020 2020 2020 2020 2020 2020 2020 7270                rp
-000166d0: 3a20 7265 6d6f 7665 5f72 6570 6574 6974  : remove_repetit
-000166e0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-000166f0: 2020 2020 2072 7773 3a20 7265 6d6f 7665       rws: remove
-00016700: 5f77 6f72 6473 5f62 795f 7374 720d 0a20  _words_by_str.. 
-00016710: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00016720: 673a 2066 696c 6c5f 696e 5f67 6170 730d  g: fill_in_gaps.
-00016730: 0a20 2020 2020 2020 2020 2020 204d 6574  .            Met
-00016740: 6163 6861 7261 6374 6572 733a 0d0a 2020  acharacters:..  
-00016750: 2020 2020 2020 2020 2020 2020 2020 3d20                = 
-00016760: 7365 7061 7261 7465 7320 6120 6d65 7468  separates a meth
-00016770: 6f64 206b 6579 2061 6e64 2069 7473 2061  od key and its a
-00016780: 7267 756d 656e 7473 2028 6e6f 7420 7573  rguments (not us
-00016790: 6564 2069 6620 6e6f 2061 7267 756d 656e  ed if no argumen
-000167a0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-000167b0: 2020 2020 5f20 7365 7061 7261 7465 7320      _ separates 
-000167c0: 6d65 7468 6f64 206b 6579 7320 2861 6674  method keys (aft
-000167d0: 6572 2061 7267 756d 656e 7473 2069 6620  er arguments if 
-000167e0: 7468 6572 6520 6172 6520 616e 7929 0d0a  there are any)..
-000167f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016800: 2b20 7365 7061 7261 7465 7320 6172 6775  + separates argu
-00016810: 6d65 6e74 7320 666f 7220 6120 6d65 7468  ments for a meth
-00016820: 6f64 206b 6579 0d0a 2020 2020 2020 2020  od key..        
-00016830: 2020 2020 2020 2020 2f20 7365 7061 7261          / separa
-00016840: 7465 7320 616e 2061 7267 756d 656e 7420  tes an argument 
-00016850: 696e 746f 206c 6973 7420 6f66 2073 7472  into list of str
-00016860: 696e 6773 0d0a 2020 2020 2020 2020 2020  ings..          
-00016870: 2020 2020 2020 2a20 7365 7061 7261 7465        * separate
-00016880: 7320 616e 2069 7465 6d20 696e 206c 6973  s an item in lis
-00016890: 7420 6f66 2073 7472 696e 6773 2069 6e74  t of strings int
-000168a0: 6f20 6120 6e65 7374 6564 206c 6973 7420  o a nested list 
-000168b0: 6f66 2073 7472 696e 6773 0d0a 2020 2020  of strings..    
-000168c0: 2020 2020 2020 2020 4e6f 7465 733a 0d0a          Notes:..
-000168d0: 2020 2020 2020 2020 2020 2020 2d61 7267              -arg
-000168e0: 756d 656e 7473 2061 7265 2070 6172 7365  uments are parse
-000168f0: 6420 706f 7369 7469 6f6e 616c 6c79 0d0a  d positionally..
-00016900: 2020 2020 2020 2020 2020 2020 2d69 6620              -if 
-00016910: 6e6f 2061 7267 756d 656e 7420 6973 2070  no argument is p
-00016920: 726f 7669 6465 642c 2074 6865 2064 6566  rovided, the def
-00016930: 6175 6c74 206f 6e65 7320 7769 6c6c 2062  ault ones will b
-00016940: 6520 7573 6564 0d0a 2020 2020 2020 2020  e used..        
-00016950: 2020 2020 2d75 7365 2031 206f 7220 3020      -use 1 or 0 
-00016960: 746f 2072 6570 7265 7365 6e74 2054 7275  to represent Tru
-00016970: 6520 6f72 2046 616c 7365 0d0a 2020 2020  e or False..    
-00016980: 2020 2020 2020 2020 4578 616d 706c 6520          Example 
-00016990: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
-000169a0: 2020 2020 6d65 7267 655f 6279 5f67 6170      merge_by_gap
-000169b0: 282e 322c 2031 302c 206c 6f63 6b3d 5472  (.2, 10, lock=Tr
-000169c0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-000169d0: 2020 2020 206d 673d 2e32 2b31 302b 2b2b       mg=.2+10+++
-000169e0: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
-000169f0: 2020 204e 6f74 653a 205b 6c6f 636b 5d20     Note: [lock] 
-00016a00: 6973 2074 6865 2035 7468 2061 7267 756d  is the 5th argum
-00016a10: 656e 7420 6865 6e63 6520 7468 6520 3220  ent hence the 2 
-00016a20: 6d69 7373 696e 6720 6172 6775 6d65 6e74  missing argument
-00016a30: 7320 696e 6265 7477 6565 6e20 7468 6520  s inbetween the 
-00016a40: 7468 7265 6520 2b20 6265 666f 7265 2031  three + before 1
-00016a50: 0d0a 2020 2020 2020 2020 2020 2020 4578  ..            Ex
-00016a60: 616d 706c 6520 323a 0d0a 2020 2020 2020  ample 2:..      
-00016a70: 2020 2020 2020 2020 2020 7370 6c69 745f            split_
-00016a80: 6279 5f70 756e 6374 7561 7469 6f6e 285b  by_punctuation([
-00016a90: 2827 2e27 2c20 2720 2729 2c20 27e3 8082  ('.', ' '), '...
-00016aa0: 272c 2027 3f27 2c20 27ef bc9f 275d 2c20  ', '?', '...'], 
-00016ab0: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
-00016ac0: 2020 2020 2020 2073 703d 2e2a 202f e380         sp=.* /..
-00016ad0: 822f 3f2f efbc 9f2b 310d 0a20 2020 2020  ./?/...+1..     
-00016ae0: 2020 2020 2020 2045 7861 6d70 6c65 2033         Example 3
-00016af0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00016b00: 2020 206d 6572 6765 5f61 6c6c 5f73 6567     merge_all_seg
-00016b10: 6d65 6e74 7328 292e 7370 6c69 745f 6279  ments().split_by
-00016b20: 5f67 6170 282e 3529 2e6d 6572 6765 5f62  _gap(.5).merge_b
-00016b30: 795f 6761 7028 2e31 352c 2033 290d 0a20  y_gap(.15, 3).. 
-00016b40: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00016b50: 735f 7367 3d2e 355f 6d67 3d2e 3135 2b33  s_sg=.5_mg=.15+3
-00016b60: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00016b70: 2020 2020 2020 2069 6620 7265 6772 6f75         if regrou
-00016b80: 705f 616c 676f 2069 7320 4661 6c73 653a  p_algo is False:
-00016b90: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00016ba0: 7475 726e 2073 656c 660d 0a20 2020 2020  turn self..     
-00016bb0: 2020 2069 6620 7265 6772 6f75 705f 616c     if regroup_al
-00016bc0: 676f 2069 7320 4e6f 6e65 206f 7220 7265  go is None or re
-00016bd0: 6772 6f75 705f 616c 676f 2069 7320 5472  group_algo is Tr
-00016be0: 7565 3a0d 0a20 2020 2020 2020 2020 2020  ue:..           
-00016bf0: 2072 6567 726f 7570 5f61 6c67 6f20 3d20   regroup_algo = 
-00016c00: 2764 6127 0d0a 0d0a 2020 2020 2020 2020  'da'....        
-00016c10: 666f 7220 6d65 7468 6f64 2c20 6b77 6172  for method, kwar
-00016c20: 6773 2c20 6d73 6720 696e 2073 656c 662e  gs, msg in self.
-00016c30: 7061 7273 655f 7265 6772 6f75 705f 616c  parse_regroup_al
-00016c40: 676f 2872 6567 726f 7570 5f61 6c67 6f2c  go(regroup_algo,
-00016c50: 2069 6e63 6c75 6465 5f73 7472 3d76 6572   include_str=ver
-00016c60: 626f 7365 206f 7220 6f6e 6c79 5f73 686f  bose or only_sho
-00016c70: 7729 3a0d 0a20 2020 2020 2020 2020 2020  w):..           
-00016c80: 2069 6620 6d73 673a 0d0a 2020 2020 2020   if msg:..      
-00016c90: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00016ca0: 6d73 6729 0d0a 2020 2020 2020 2020 2020  msg)..          
-00016cb0: 2020 6966 206e 6f74 206f 6e6c 795f 7368    if not only_sh
-00016cc0: 6f77 3a0d 0a20 2020 2020 2020 2020 2020  ow:..           
-00016cd0: 2020 2020 206d 6574 686f 6428 2a2a 6b77       method(**kw
-00016ce0: 6172 6773 290d 0a0d 0a20 2020 2020 2020  args)....       
-00016cf0: 2072 6574 7572 6e20 7365 6c66 0d0a 0d0a   return self....
-00016d00: 2020 2020 6465 6620 7061 7273 655f 7265      def parse_re
-00016d10: 6772 6f75 705f 616c 676f 2873 656c 662c  group_algo(self,
-00016d20: 2072 6567 726f 7570 5f61 6c67 6f3a 2073   regroup_algo: s
-00016d30: 7472 2c20 696e 636c 7564 655f 7374 723a  tr, include_str:
-00016d40: 2062 6f6f 6c20 3d20 5472 7565 2920 2d3e   bool = True) ->
-00016d50: 204c 6973 745b 5475 706c 655b 4361 6c6c   List[Tuple[Call
-00016d60: 6162 6c65 2c20 6469 6374 2c20 7374 725d  able, dict, str]
-00016d70: 5d3a 0d0a 2020 2020 2020 2020 6d65 7468  ]:..        meth
-00016d80: 6f64 7320 3d20 6469 6374 280d 0a20 2020  ods = dict(..   
-00016d90: 2020 2020 2020 2020 2073 673d 7365 6c66           sg=self
-00016da0: 2e73 706c 6974 5f62 795f 6761 702c 0d0a  .split_by_gap,..
-00016db0: 2020 2020 2020 2020 2020 2020 7370 3d73              sp=s
-00016dc0: 656c 662e 7370 6c69 745f 6279 5f70 756e  elf.split_by_pun
-00016dd0: 6374 7561 7469 6f6e 2c0d 0a20 2020 2020  ctuation,..     
-00016de0: 2020 2020 2020 2073 6c3d 7365 6c66 2e73         sl=self.s
-00016df0: 706c 6974 5f62 795f 6c65 6e67 7468 2c0d  plit_by_length,.
-00016e00: 0a20 2020 2020 2020 2020 2020 2073 643d  .            sd=
-00016e10: 7365 6c66 2e73 706c 6974 5f62 795f 6475  self.split_by_du
-00016e20: 7261 7469 6f6e 2c0d 0a20 2020 2020 2020  ration,..       
-00016e30: 2020 2020 206d 673d 7365 6c66 2e6d 6572       mg=self.mer
-00016e40: 6765 5f62 795f 6761 702c 0d0a 2020 2020  ge_by_gap,..    
-00016e50: 2020 2020 2020 2020 6d70 3d73 656c 662e          mp=self.
-00016e60: 6d65 7267 655f 6279 5f70 756e 6374 7561  merge_by_punctua
-00016e70: 7469 6f6e 2c0d 0a20 2020 2020 2020 2020  tion,..         
-00016e80: 2020 206d 733d 7365 6c66 2e6d 6572 6765     ms=self.merge
-00016e90: 5f61 6c6c 5f73 6567 6d65 6e74 732c 0d0a  _all_segments,..
-00016ea0: 2020 2020 2020 2020 2020 2020 636d 3d73              cm=s
-00016eb0: 656c 662e 636c 616d 705f 6d61 782c 0d0a  elf.clamp_max,..
-00016ec0: 2020 2020 2020 2020 2020 2020 7573 3d73              us=s
-00016ed0: 656c 662e 756e 6c6f 636b 5f61 6c6c 5f73  elf.unlock_all_s
+00013fa0: 2020 202b 2027 272e 6a6f 696e 285f 772e     + ''.join(_w.
+00013fb0: 776f 7264 2066 6f72 205f 7720 696e 2061  word for _w in a
+00013fc0: 6c6c 5f77 6f72 6473 5b73 3a69 5d29 202b  ll_words[s:i]) +
+00013fd0: 2027 5c6e 270d 0a20 2020 2020 2020 2020   '\n'..         
+00013fe0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00013ff0: 2027 5c6e 272e 6a6f 696e 2872 6576 6572   '\n'.join(rever
+00014000: 7365 6428 7465 6d70 5f63 6861 6e67 6573  sed(temp_changes
+00014010: 2929 202b 2027 5c6e 270d 0a20 2020 2020  )) + '\n'..     
+00014020: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00014030: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014040: 2020 666f 7220 6930 2c20 6931 2069 6e20    for i0, i1 in 
+00014050: 7a69 7028 7261 6e67 6528 7320 2d20 636f  zip(range(s - co
+00014060: 756e 742c 2073 292c 2072 616e 6765 2873  unt, s), range(s
+00014070: 2c20 6929 293a 0d0a 2020 2020 2020 2020  , i)):..        
+00014080: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00014090: 656e 2861 6c6c 5f77 6f72 6473 5b69 305d  en(all_words[i0]
+000140a0: 2e77 6f72 6429 203c 206c 656e 2861 6c6c  .word) < len(all
+000140b0: 5f77 6f72 6473 5b69 315d 2e77 6f72 6429  _words[i1].word)
+000140c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000140d0: 2020 2020 2020 2020 2020 2061 6c6c 5f77             all_w
+000140e0: 6f72 6473 5b69 315d 2e73 7461 7274 203d  ords[i1].start =
+000140f0: 2061 6c6c 5f77 6f72 6473 5b69 305d 2e73   all_words[i0].s
+00014100: 7461 7274 0d0a 2020 2020 2020 2020 2020  tart..          
+00014110: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00014120: 6c5f 776f 7264 735b 6931 5d2e 656e 6420  l_words[i1].end 
+00014130: 3d20 616c 6c5f 776f 7264 735b 6930 5d2e  = all_words[i0].
+00014140: 656e 640d 0a20 2020 2020 2020 2020 2020  end..           
+00014150: 2020 2020 2020 2020 2020 2020 205f 7369               _si
+00014160: 642c 205f 7769 6420 3d20 616c 6c5f 776f  d, _wid = all_wo
+00014170: 7264 735b 6930 5d2e 7365 676d 656e 745f  rds[i0].segment_
+00014180: 6964 2c20 616c 6c5f 776f 7264 735b 6930  id, all_words[i0
+00014190: 5d2e 6964 0d0a 2020 2020 2020 2020 2020  ].id..          
+000141a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000141b0: 6c66 2e73 6567 6d65 6e74 735b 5f73 6964  lf.segments[_sid
+000141c0: 5d2e 776f 7264 735b 5f77 6964 5d20 3d20  ].words[_wid] = 
+000141d0: 616c 6c5f 776f 7264 735b 6931 5d0d 0a0d  all_words[i1]...
+000141e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000141f0: 6368 616e 6765 733a 0d0a 2020 2020 2020  changes:..      
+00014200: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00014210: 275c 6e27 2e6a 6f69 6e28 7265 7665 7273  '\n'.join(revers
+00014220: 6564 2863 6861 6e67 6573 2929 290d 0a0d  ed(changes)))...
+00014230: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00014240: 662e 7265 6d6f 7665 5f6e 6f5f 776f 7264  f.remove_no_word
+00014250: 5f73 6567 6d65 6e74 7328 7265 6173 7369  _segments(reassi
+00014260: 676e 5f69 6473 3d46 616c 7365 290d 0a20  gn_ids=False).. 
+00014270: 2020 2020 2020 2073 656c 662e 7265 6173         self.reas
+00014280: 7369 676e 5f69 6473 2829 0d0a 0d0a 2020  sign_ids()....  
+00014290: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000142a0: 660d 0a0d 0a20 2020 2064 6566 2072 656d  f....    def rem
+000142b0: 6f76 655f 776f 7264 735f 6279 5f73 7472  ove_words_by_str
+000142c0: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
+000142d0: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
+000142e0: 2020 776f 7264 733a 2055 6e69 6f6e 5b73    words: Union[s
+000142f0: 7472 2c20 4c69 7374 5b73 7472 5d2c 204e  tr, List[str], N
+00014300: 6f6e 655d 2c0d 0a20 2020 2020 2020 2020  one],..         
+00014310: 2020 2063 6173 655f 7365 6e73 6974 6976     case_sensitiv
+00014320: 653a 2062 6f6f 6c20 3d20 4661 6c73 652c  e: bool = False,
+00014330: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00014340: 7269 703a 2062 6f6f 6c20 3d20 5472 7565  rip: bool = True
+00014350: 2c0d 0a20 2020 2020 2020 2020 2020 2069  ,..            i
+00014360: 676e 6f72 655f 7075 6e63 7475 6174 696f  gnore_punctuatio
+00014370: 6e73 3a20 7374 7220 3d20 225c 2227 2c2e  ns: str = "\"',.
+00014380: 3f21 222c 0d0a 2020 2020 2020 2020 2020  ?!",..          
+00014390: 2020 6d69 6e5f 7072 6f62 3a20 666c 6f61    min_prob: floa
+000143a0: 7420 3d20 4e6f 6e65 2c0d 0a20 2020 2020  t = None,..     
+000143b0: 2020 2020 2020 2066 696c 7465 7273 3a20         filters: 
+000143c0: 4361 6c6c 6162 6c65 203d 204e 6f6e 652c  Callable = None,
+000143d0: 0d0a 2020 2020 2020 2020 2020 2020 7665  ..            ve
+000143e0: 7262 6f73 653a 2062 6f6f 6c20 3d20 5472  rbose: bool = Tr
+000143f0: 7565 0d0a 2020 2020 2920 2d3e 2027 5768  ue..    ) -> 'Wh
+00014400: 6973 7065 7252 6573 756c 7427 3a0d 0a20  isperResult':.. 
+00014410: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00014420: 2020 2020 5265 6d6f 7665 2077 6f72 6473      Remove words
+00014430: 2074 6861 7420 6d61 7463 6820 6060 776f   that match ``wo
+00014440: 7264 7360 602e 0d0a 0d0a 2020 2020 2020  rds``.....      
+00014450: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
+00014460: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00014470: 0d0a 2020 2020 2020 2020 776f 7264 7320  ..        words 
+00014480: 3a20 7374 7220 6f72 206c 6973 7420 6f66  : str or list of
+00014490: 2073 7472 206f 7220 4e6f 6e65 0d0a 2020   str or None..  
+000144a0: 2020 2020 2020 2020 2020 4120 776f 7264            A word
+000144b0: 206f 7220 6c69 7374 206f 6620 776f 7264   or list of word
+000144c0: 7320 746f 2072 656d 6f76 652e 6060 4e6f  s to remove.``No
+000144d0: 6e65 6060 2066 6f72 2061 6c6c 2077 6f72  ne`` for all wor
+000144e0: 6473 2074 6f20 6265 2070 6173 7365 6420  ds to be passed 
+000144f0: 696e 746f 2060 6066 696c 7465 7273 6060  into ``filters``
+00014500: 2e0d 0a20 2020 2020 2020 2063 6173 655f  ...        case_
+00014510: 7365 6e73 6974 6976 6520 3a20 626f 6f6c  sensitive : bool
+00014520: 2c20 6465 6661 756c 7420 4661 6c73 650d  , default False.
+00014530: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
+00014540: 7468 6572 2074 6865 2063 6173 6520 6f66  ther the case of
+00014550: 2077 6f72 6473 206e 6565 6420 746f 206d   words need to m
+00014560: 6174 6368 2074 6f20 6265 2063 6f6e 7369  atch to be consi
+00014570: 6465 7265 6420 6173 2072 6570 6574 6974  dered as repetit
+00014580: 696f 6e2e 0d0a 2020 2020 2020 2020 7374  ion...        st
+00014590: 7269 7020 3a20 626f 6f6c 2c20 6465 6661  rip : bool, defa
+000145a0: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
+000145b0: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+000145c0: 2069 676e 6f72 6520 7370 6163 6573 2062   ignore spaces b
+000145d0: 6566 6f72 6520 616e 6420 6166 7465 7220  efore and after 
+000145e0: 6561 6368 2077 6f72 642e 0d0a 2020 2020  each word...    
+000145f0: 2020 2020 6967 6e6f 7265 5f70 756e 6374      ignore_punct
+00014600: 7561 7469 6f6e 7320 3a20 626f 6f6c 2c20  uations : bool, 
+00014610: 6465 6661 756c 7420 2722 272c 2e3f 2127  default '"',.?!'
+00014620: 0d0a 2020 2020 2020 2020 2020 2020 456e  ..            En
+00014630: 6469 6e67 2070 756e 6374 7561 7469 6f6e  ding punctuation
+00014640: 7320 746f 2069 676e 6f72 652e 0d0a 2020  s to ignore...  
+00014650: 2020 2020 2020 6d69 6e5f 7072 6f62 203a        min_prob :
+00014660: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
+00014670: 0d0a 2020 2020 2020 2020 2020 2020 4163  ..            Ac
+00014680: 7473 2061 7320 7468 6520 6669 7273 7420  ts as the first 
+00014690: 6669 6c74 6572 2074 6865 2066 6f72 2074  filter the for t
+000146a0: 6865 2077 6f72 6473 2074 6861 7420 6d61  he words that ma
+000146b0: 7463 6820 6060 776f 7264 7360 602e 2057  tch ``words``. W
+000146c0: 6f72 6473 2077 6974 6820 7072 6f62 6162  ords with probab
+000146d0: 696c 6974 7920 3c20 6060 6d69 6e5f 7072  ility < ``min_pr
+000146e0: 6f62 6060 2077 696c 6c0d 0a20 2020 2020  ob`` will..     
+000146f0: 2020 2020 2020 2062 6520 7265 6d6f 7665         be remove
+00014700: 6420 6966 2060 6066 696c 7465 7273 6060  d if ``filters``
+00014710: 2069 7320 6060 4e6f 6e65 6060 2c20 656c   is ``None``, el
+00014720: 7365 2070 6173 7320 7468 6520 776f 7264  se pass the word
+00014730: 7320 696e 746f 2060 6066 696c 7465 7273  s into ``filters
+00014740: 6060 2e20 576f 7264 7320 7769 7468 6f75  ``. Words withou
+00014750: 7420 7072 6f62 6162 696c 6974 7920 7769  t probability wi
+00014760: 6c6c 0d0a 2020 2020 2020 2020 2020 2020  ll..            
+00014770: 6265 2074 7265 6174 6564 2061 7320 6861  be treated as ha
+00014780: 7669 6e67 2070 726f 6261 6269 6c69 7479  ving probability
+00014790: 203c 2060 606d 696e 5f70 726f 6260 602e   < ``min_prob``.
+000147a0: 0d0a 2020 2020 2020 2020 6669 6c74 6572  ..        filter
+000147b0: 7320 3a20 4361 6c6c 6162 6c65 2c20 6f70  s : Callable, op
+000147c0: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+000147d0: 2020 2020 4120 6675 6e63 7469 6f6e 2074      A function t
+000147e0: 6861 7420 7461 6b65 7320 616e 2069 6e73  hat takes an ins
+000147f0: 7461 6e63 6520 6f66 203a 636c 6173 733a  tance of :class:
+00014800: 6073 7461 626c 655f 7768 6973 7065 722e  `stable_whisper.
+00014810: 7265 7375 6c74 2e57 6f72 6454 696d 696e  result.WordTimin
+00014820: 6760 2061 7320 6974 7320 6f6e 6c79 2061  g` as its only a
+00014830: 7267 756d 656e 742e 0d0a 2020 2020 2020  rgument...      
+00014840: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
+00014850: 696f 6e20 6973 2063 7573 746f 6d20 6669  ion is custom fi
+00014860: 6c74 6572 2066 6f72 2074 6865 2077 6f72  lter for the wor
+00014870: 6473 2074 6861 7420 6d61 7463 6820 6060  ds that match ``
+00014880: 776f 7264 7360 6020 616e 6420 7765 7265  words`` and were
+00014890: 206e 6f74 2063 6175 6768 7420 6279 2060   not caught by `
+000148a0: 606d 696e 5f70 726f 6260 602e 0d0a 2020  `min_prob``...  
+000148b0: 2020 2020 2020 7665 7262 6f73 653a 0d0a        verbose:..
+000148c0: 2020 2020 2020 2020 2020 2020 5768 6574              Whet
+000148d0: 6865 7220 746f 2070 7269 6e74 2064 6574  her to print det
+000148e0: 6169 6c20 6f66 2074 6865 2072 656d 6f76  ail of the remov
+000148f0: 6564 2077 6f72 6473 2e0d 0a0d 0a20 2020  ed words.....   
+00014900: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
+00014910: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
+00014920: 2020 2020 2020 2073 7461 626c 655f 7768         stable_wh
+00014930: 6973 7065 722e 7265 7375 6c74 2e57 6869  isper.result.Whi
+00014940: 7370 6572 5265 7375 6c74 0d0a 2020 2020  sperResult..    
+00014950: 2020 2020 2020 2020 5468 6520 6375 7272          The curr
+00014960: 656e 7420 696e 7374 616e 6365 2061 6674  ent instance aft
+00014970: 6572 2074 6865 2063 6861 6e67 6573 2e0d  er the changes..
+00014980: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00014990: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+000149a0: 662e 6861 735f 776f 7264 733a 0d0a 2020  f.has_words:..  
+000149b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000149c0: 2073 656c 660d 0a20 2020 2020 2020 2069   self..        i
+000149d0: 6620 6973 696e 7374 616e 6365 2877 6f72  f isinstance(wor
+000149e0: 6473 2c20 7374 7229 3a0d 0a20 2020 2020  ds, str):..     
+000149f0: 2020 2020 2020 2077 6f72 6473 203d 205b         words = [
+00014a00: 776f 7264 735d 0d0a 2020 2020 2020 2020  words]..        
+00014a10: 616c 6c5f 776f 7264 7320 3d20 7365 6c66  all_words = self
+00014a20: 2e61 6c6c 5f77 6f72 6473 2829 0d0a 2020  .all_words()..  
+00014a30: 2020 2020 2020 616c 6c5f 776f 7264 735f        all_words_
+00014a40: 7374 7220 3d20 5b77 2e77 6f72 6420 666f  str = [w.word fo
+00014a50: 7220 7720 696e 2061 6c6c 5f77 6f72 6473  r w in all_words
+00014a60: 5d0d 0a20 2020 2020 2020 2069 6620 7374  ]..        if st
+00014a70: 7269 703a 0d0a 2020 2020 2020 2020 2020  rip:..          
+00014a80: 2020 616c 6c5f 776f 7264 735f 7374 7220    all_words_str 
+00014a90: 3d20 5b77 2e73 7472 6970 2829 2066 6f72  = [w.strip() for
+00014aa0: 2077 2069 6e20 616c 6c5f 776f 7264 735f   w in all_words_
+00014ab0: 7374 725d 0d0a 2020 2020 2020 2020 2020  str]..          
+00014ac0: 2020 776f 7264 7320 3d20 5b77 2e73 7472    words = [w.str
+00014ad0: 6970 2829 2066 6f72 2077 2069 6e20 776f  ip() for w in wo
+00014ae0: 7264 735d 0d0a 2020 2020 2020 2020 6966  rds]..        if
+00014af0: 2069 676e 6f72 655f 7075 6e63 7475 6174   ignore_punctuat
+00014b00: 696f 6e73 3a0d 0a20 2020 2020 2020 2020  ions:..         
+00014b10: 2020 2070 746e 203d 2066 275b 7b69 676e     ptn = f'[{ign
+00014b20: 6f72 655f 7075 6e63 7475 6174 696f 6e73  ore_punctuations
+00014b30: 7d5d 2b24 270d 0a20 2020 2020 2020 2020  }]+$'..         
+00014b40: 2020 2061 6c6c 5f77 6f72 6473 5f73 7472     all_words_str
+00014b50: 203d 205b 7265 2e73 7562 2870 746e 2c20   = [re.sub(ptn, 
+00014b60: 2727 2c20 7729 2066 6f72 2077 2069 6e20  '', w) for w in 
+00014b70: 616c 6c5f 776f 7264 735f 7374 725d 0d0a  all_words_str]..
+00014b80: 2020 2020 2020 2020 2020 2020 776f 7264              word
+00014b90: 7320 3d20 5b72 652e 7375 6228 7074 6e2c  s = [re.sub(ptn,
+00014ba0: 2027 272c 2077 2920 666f 7220 7720 696e   '', w) for w in
+00014bb0: 2077 6f72 6473 5d0d 0a20 2020 2020 2020   words]..       
+00014bc0: 2069 6620 6e6f 7420 6361 7365 5f73 656e   if not case_sen
+00014bd0: 7369 7469 7665 3a0d 0a20 2020 2020 2020  sitive:..       
+00014be0: 2020 2020 2061 6c6c 5f77 6f72 6473 5f73       all_words_s
+00014bf0: 7472 203d 205b 772e 6c6f 7765 7228 2920  tr = [w.lower() 
+00014c00: 666f 7220 7720 696e 2061 6c6c 5f77 6f72  for w in all_wor
+00014c10: 6473 5f73 7472 5d0d 0a20 2020 2020 2020  ds_str]..       
+00014c20: 2020 2020 2077 6f72 6473 203d 205b 772e       words = [w.
+00014c30: 6c6f 7765 7228 2920 666f 7220 7720 696e  lower() for w in
+00014c40: 2077 6f72 6473 5d0d 0a0d 0a20 2020 2020   words]....     
+00014c50: 2020 2063 6861 6e67 6573 203d 205b 5d0d     changes = [].
+00014c60: 0a20 2020 2020 2020 2066 6f72 2069 2c20  .        for i, 
+00014c70: 7720 696e 2072 6576 6572 7365 6428 6c69  w in reversed(li
+00014c80: 7374 2865 6e75 6d65 7261 7465 2861 6c6c  st(enumerate(all
+00014c90: 5f77 6f72 6473 5f73 7472 2929 293a 0d0a  _words_str))):..
+00014ca0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00014cb0: 6f74 2028 776f 7264 7320 6973 204e 6f6e  ot (words is Non
+00014cc0: 6520 6f72 2061 6e79 2877 203d 3d20 5f77  e or any(w == _w
+00014cd0: 2066 6f72 205f 7720 696e 2077 6f72 6473   for _w in words
+00014ce0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00014cf0: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
+00014d00: 2020 2020 2020 2020 2020 2069 6620 280d             if (.
+00014d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014d20: 2020 2020 2028 6d69 6e5f 7072 6f62 2069       (min_prob i
+00014d30: 7320 4e6f 6e65 206f 7220 616c 6c5f 776f  s None or all_wo
+00014d40: 7264 735b 695d 2e70 726f 6261 6269 6c69  rds[i].probabili
+00014d50: 7479 2069 7320 4e6f 6e65 206f 7220 6d69  ty is None or mi
+00014d60: 6e5f 7072 6f62 203e 2061 6c6c 5f77 6f72  n_prob > all_wor
+00014d70: 6473 5b69 5d2e 7072 6f62 6162 696c 6974  ds[i].probabilit
+00014d80: 7929 2061 6e64 0d0a 2020 2020 2020 2020  y) and..        
+00014d90: 2020 2020 2020 2020 2020 2020 2866 696c              (fil
+00014da0: 7465 7273 2069 7320 4e6f 6e65 206f 7220  ters is None or 
+00014db0: 6669 6c74 6572 7328 616c 6c5f 776f 7264  filters(all_word
+00014dc0: 735b 695d 2929 0d0a 2020 2020 2020 2020  s[i]))..        
+00014dd0: 2020 2020 293a 0d0a 2020 2020 2020 2020      ):..        
+00014de0: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
+00014df0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00014e00: 2020 2020 2020 2020 2063 6861 6e67 6573           changes
+00014e10: 2e61 7070 656e 6428 6627 5265 6d6f 7665  .append(f'Remove
+00014e20: 643a 207b 616c 6c5f 776f 7264 735b 695d  d: {all_words[i]
+00014e30: 2e74 6f5f 6469 6374 2829 7d27 290d 0a20  .to_dict()}').. 
+00014e40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014e50: 656c 662e 7265 6d6f 7665 5f77 6f72 6428  elf.remove_word(
+00014e60: 616c 6c5f 776f 7264 735b 695d 2c20 4661  all_words[i], Fa
+00014e70: 6c73 652c 2076 6572 626f 7365 3d46 616c  lse, verbose=Fal
+00014e80: 7365 290d 0a20 2020 2020 2020 2069 6620  se)..        if 
+00014e90: 6368 616e 6765 733a 0d0a 2020 2020 2020  changes:..      
+00014ea0: 2020 2020 2020 7072 696e 7428 275c 6e27        print('\n'
+00014eb0: 2e6a 6f69 6e28 7265 7665 7273 6564 2863  .join(reversed(c
+00014ec0: 6861 6e67 6573 2929 290d 0a20 2020 2020  hanges)))..     
+00014ed0: 2020 2073 656c 662e 7265 6d6f 7665 5f6e     self.remove_n
+00014ee0: 6f5f 776f 7264 5f73 6567 6d65 6e74 7328  o_word_segments(
+00014ef0: 290d 0a0d 0a20 2020 2020 2020 2072 6574  )....        ret
+00014f00: 7572 6e20 7365 6c66 0d0a 0d0a 2020 2020  urn self....    
+00014f10: 6465 6620 6669 6c6c 5f69 6e5f 6761 7073  def fill_in_gaps
+00014f20: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
+00014f30: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
+00014f40: 2020 6f74 6865 725f 7265 7375 6c74 3a20    other_result: 
+00014f50: 556e 696f 6e5b 2757 6869 7370 6572 5265  Union['WhisperRe
+00014f60: 7375 6c74 272c 2073 7472 5d2c 0d0a 2020  sult', str],..  
+00014f70: 2020 2020 2020 2020 2020 6d69 6e5f 6761            min_ga
+00014f80: 703a 2066 6c6f 6174 203d 2030 2e31 2c0d  p: float = 0.1,.
+00014f90: 0a20 2020 2020 2020 2020 2020 2063 6173  .            cas
+00014fa0: 655f 7365 6e73 6974 6976 653a 2062 6f6f  e_sensitive: boo
+00014fb0: 6c20 3d20 4661 6c73 652c 0d0a 2020 2020  l = False,..    
+00014fc0: 2020 2020 2020 2020 7374 7269 703a 2062          strip: b
+00014fd0: 6f6f 6c20 3d20 5472 7565 2c0d 0a20 2020  ool = True,..   
+00014fe0: 2020 2020 2020 2020 2069 676e 6f72 655f           ignore_
+00014ff0: 7075 6e63 7475 6174 696f 6e73 3a20 7374  punctuations: st
+00015000: 7220 3d20 225c 2227 2c2e 3f21 222c 0d0a  r = "\"',.?!",..
+00015010: 2020 2020 2020 2020 2020 2020 7665 7262              verb
+00015020: 6f73 653a 2062 6f6f 6c20 3d20 5472 7565  ose: bool = True
+00015030: 0d0a 2020 2020 2920 2d3e 2027 5768 6973  ..    ) -> 'Whis
+00015040: 7065 7252 6573 756c 7427 3a0d 0a20 2020  perResult':..   
+00015050: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00015060: 2020 4669 6c6c 2069 6e20 7365 676d 656e    Fill in segmen
+00015070: 7420 6761 7073 206c 6172 6765 7220 7468  t gaps larger th
+00015080: 616e 2060 606d 696e 5f67 6170 6060 2077  an ``min_gap`` w
+00015090: 6974 6820 636f 6e74 656e 7420 6672 6f6d  ith content from
+000150a0: 2060 606f 7468 6572 5f72 6573 756c 7460   ``other_result`
+000150b0: 6020 6174 2074 6865 2074 696d 6573 206f  ` at the times o
+000150c0: 6620 6761 7073 2e0d 0a0d 0a20 2020 2020  f gaps.....     
+000150d0: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+000150e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+000150f0: 2d0d 0a20 2020 2020 2020 206f 7468 6572  -..        other
+00015100: 5f72 6573 756c 7420 3a20 5768 6973 7065  _result : Whispe
+00015110: 7252 6573 756c 7420 6f72 2073 7472 0d0a  rResult or str..
+00015120: 2020 2020 2020 2020 2020 2020 416e 6f74              Anot
+00015130: 6865 7220 7472 616e 7363 7269 7074 696f  her transcriptio
+00015140: 6e20 7265 7375 6c74 2061 7320 616e 2069  n result as an i
+00015150: 6e73 7461 6e63 6520 6f66 203a 636c 6173  nstance of :clas
+00015160: 733a 6073 7461 626c 655f 7768 6973 7065  s:`stable_whispe
+00015170: 722e 7265 7375 6c74 2e57 6869 7370 6572  r.result.Whisper
+00015180: 5265 7375 6c74 6020 6f72 2070 6174 6820  Result` or path 
+00015190: 746f 2074 6865 0d0a 2020 2020 2020 2020  to the..        
+000151a0: 2020 2020 4a53 4f4e 206f 6620 7468 6520      JSON of the 
+000151b0: 7265 7375 6c74 2e0d 0a20 2020 2020 2020  result...       
+000151c0: 206d 696e 5f67 6170 203a 2066 6c6f 6174   min_gap : float
+000151d0: 2c20 6465 6661 756c 7420 302e 310d 0a20  , default 0.1.. 
+000151e0: 2020 2020 2020 2020 2020 2054 6865 206d             The m
+000151f0: 696e 696d 756d 2073 6563 6f6e 6473 206f  inimum seconds o
+00015200: 6620 6120 6761 7020 6265 7477 6565 6e20  f a gap between 
+00015210: 7365 676d 656e 7473 2074 6861 7420 6d75  segments that mu
+00015220: 7374 2062 6520 6578 6365 6564 6564 2074  st be exceeded t
+00015230: 6f20 6265 2066 696c 6c65 6420 696e 2e0d  o be filled in..
+00015240: 0a20 2020 2020 2020 2063 6173 655f 7365  .        case_se
+00015250: 6e73 6974 6976 6520 3a20 626f 6f6c 2c20  nsitive : bool, 
+00015260: 6465 6661 756c 7420 4661 6c73 650d 0a20  default False.. 
+00015270: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+00015280: 6572 2074 6f20 636f 6e73 6964 6572 2074  er to consider t
+00015290: 6865 2063 6173 6520 6f66 2074 6865 2066  he case of the f
+000152a0: 6972 7374 2061 6e64 206c 6173 7420 776f  irst and last wo
+000152b0: 7264 206f 6620 7468 6520 6761 7020 746f  rd of the gap to
+000152c0: 2064 6574 6572 6d69 6e65 206f 7665 726c   determine overl
+000152d0: 6170 7069 6e67 2077 6f72 6473 2074 6f20  apping words to 
+000152e0: 7265 6d6f 7665 0d0a 2020 2020 2020 2020  remove..        
+000152f0: 2020 2020 6265 666f 7265 2066 696c 6c69      before filli
+00015300: 6e67 2069 6e2e 0d0a 2020 2020 2020 2020  ng in...        
+00015310: 7374 7269 7020 3a20 626f 6f6c 2c20 6465  strip : bool, de
+00015320: 6661 756c 7420 5472 7565 0d0a 2020 2020  fault True..    
+00015330: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
+00015340: 746f 2069 676e 6f72 6520 7370 6163 6573  to ignore spaces
+00015350: 2062 6566 6f72 6520 616e 6420 6166 7465   before and afte
+00015360: 7220 7468 6520 6669 7273 7420 616e 6420  r the first and 
+00015370: 6c61 7374 2077 6f72 6420 6f66 2074 6865  last word of the
+00015380: 2067 6170 2074 6f20 6465 7465 726d 696e   gap to determin
+00015390: 6520 6f76 6572 6c61 7070 696e 6720 776f  e overlapping wo
+000153a0: 7264 730d 0a20 2020 2020 2020 2020 2020  rds..           
+000153b0: 2074 6f20 7265 6d6f 7665 2062 6566 6f72   to remove befor
+000153c0: 6520 6669 6c6c 696e 6720 696e 2e0d 0a20  e filling in... 
+000153d0: 2020 2020 2020 2069 676e 6f72 655f 7075         ignore_pu
+000153e0: 6e63 7475 6174 696f 6e73 203a 2062 6f6f  nctuations : boo
+000153f0: 6c2c 2064 6566 6175 6c74 2027 2227 2c2e  l, default '"',.
+00015400: 3f21 270d 0a20 2020 2020 2020 2020 2020  ?!'..           
+00015410: 2045 6e64 696e 6720 7075 6e63 7475 6174   Ending punctuat
+00015420: 696f 6e73 2074 6f20 6967 6e6f 7265 2069  ions to ignore i
+00015430: 6e20 7468 6520 6669 7273 7420 616e 6420  n the first and 
+00015440: 6c61 7374 2077 6f72 6420 6f66 2074 6865  last word of the
+00015450: 2067 6170 2074 6f20 6465 7465 726d 696e   gap to determin
+00015460: 6520 6f76 6572 6c61 7070 696e 6720 776f  e overlapping wo
+00015470: 7264 7320 746f 0d0a 2020 2020 2020 2020  rds to..        
+00015480: 2020 2020 7265 6d6f 7665 2062 6566 6f72      remove befor
+00015490: 6520 6669 6c6c 696e 6720 696e 2e0d 0a20  e filling in... 
+000154a0: 2020 2020 2020 2076 6572 626f 7365 3a0d         verbose:.
+000154b0: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
+000154c0: 7468 6572 2074 6f20 7072 696e 7420 6465  ther to print de
+000154d0: 7461 696c 206f 6620 7468 6520 6669 6c6c  tail of the fill
+000154e0: 6564 2063 6f6e 7465 6e74 2e0d 0a0d 0a20  ed content..... 
+000154f0: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
+00015500: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
+00015510: 0a20 2020 2020 2020 2073 7461 626c 655f  .        stable_
+00015520: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
+00015530: 6869 7370 6572 5265 7375 6c74 0d0a 2020  hisperResult..  
+00015540: 2020 2020 2020 2020 2020 5468 6520 6375            The cu
+00015550: 7272 656e 7420 696e 7374 616e 6365 2061  rrent instance a
+00015560: 6674 6572 2074 6865 2063 6861 6e67 6573  fter the changes
+00015570: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+00015580: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
+00015590: 656c 662e 7365 676d 656e 7473 2920 3c20  elf.segments) < 
+000155a0: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
+000155b0: 7265 7475 726e 2073 656c 660d 0a20 2020  return self..   
+000155c0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+000155d0: 6365 286f 7468 6572 5f72 6573 756c 742c  ce(other_result,
+000155e0: 2073 7472 293a 0d0a 2020 2020 2020 2020   str):..        
+000155f0: 2020 2020 6f74 6865 725f 7265 7375 6c74      other_result
+00015600: 203d 2057 6869 7370 6572 5265 7375 6c74   = WhisperResult
+00015610: 286f 7468 6572 5f72 6573 756c 7429 0d0a  (other_result)..
+00015620: 0d0a 2020 2020 2020 2020 6966 2073 7472  ..        if str
+00015630: 6970 3a0d 0a20 2020 2020 2020 2020 2020  ip:..           
+00015640: 2064 6566 2073 7472 6970 5f73 7061 6365   def strip_space
+00015650: 2877 293a 0d0a 2020 2020 2020 2020 2020  (w):..          
+00015660: 2020 2020 2020 7265 7475 726e 2077 2e73        return w.s
+00015670: 7472 6970 2829 0d0a 2020 2020 2020 2020  trip()..        
+00015680: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00015690: 2020 2064 6566 2073 7472 6970 5f73 7061     def strip_spa
+000156a0: 6365 2877 293a 0d0a 2020 2020 2020 2020  ce(w):..        
+000156b0: 2020 2020 2020 2020 7265 7475 726e 2077          return w
+000156c0: 0d0a 0d0a 2020 2020 2020 2020 6966 2069  ....        if i
+000156d0: 676e 6f72 655f 7075 6e63 7475 6174 696f  gnore_punctuatio
+000156e0: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
+000156f0: 2070 746e 203d 2066 275b 7b69 676e 6f72   ptn = f'[{ignor
+00015700: 655f 7075 6e63 7475 6174 696f 6e73 7d5d  e_punctuations}]
+00015710: 2b24 270d 0a0d 0a20 2020 2020 2020 2020  +$'....         
+00015720: 2020 2064 6566 2073 7472 6970 5f70 756e     def strip_pun
+00015730: 6374 7561 7469 6f6e 7328 7729 3a0d 0a20  ctuations(w):.. 
+00015740: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00015750: 6574 7572 6e20 7265 2e73 7562 2870 746e  eturn re.sub(ptn
+00015760: 2c20 2727 2c20 7374 7269 705f 7370 6163  , '', strip_spac
+00015770: 6528 7729 290d 0a20 2020 2020 2020 2065  e(w))..        e
+00015780: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00015790: 2020 7374 7269 705f 7075 6e63 7475 6174    strip_punctuat
+000157a0: 696f 6e73 203d 2073 7472 6970 5f73 7061  ions = strip_spa
+000157b0: 6365 0d0a 0d0a 2020 2020 2020 2020 6966  ce....        if
+000157c0: 2063 6173 655f 7365 6e73 6974 6976 653a   case_sensitive:
+000157d0: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+000157e0: 7269 7020 3d20 7374 7269 705f 7075 6e63  rip = strip_punc
+000157f0: 7475 6174 696f 6e73 0d0a 2020 2020 2020  tuations..      
+00015800: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00015810: 2020 2020 2064 6566 2073 7472 6970 2877       def strip(w
+00015820: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00015830: 2020 2020 7265 7475 726e 2073 7472 6970      return strip
+00015840: 5f70 756e 6374 7561 7469 6f6e 7328 7729  _punctuations(w)
+00015850: 2e6c 6f77 6572 2829 0d0a 0d0a 2020 2020  .lower()....    
+00015860: 2020 2020 7365 675f 7061 6972 7320 3d20      seg_pairs = 
+00015870: 6c69 7374 2865 6e75 6d65 7261 7465 287a  list(enumerate(z
+00015880: 6970 2873 656c 662e 7365 676d 656e 7473  ip(self.segments
+00015890: 5b3a 2d31 5d2c 2073 656c 662e 7365 676d  [:-1], self.segm
+000158a0: 656e 7473 5b31 3a5d 2929 290d 0a20 2020  ents[1:])))..   
+000158b0: 2020 2020 2073 6567 5f70 6169 7273 2e69       seg_pairs.i
+000158c0: 6e73 6572 7428 302c 2028 2d31 2c20 284e  nsert(0, (-1, (N
+000158d0: 6f6e 652c 2073 656c 662e 7365 676d 656e  one, self.segmen
+000158e0: 7473 5b30 5d29 2929 0d0a 2020 2020 2020  ts[0])))..      
+000158f0: 2020 7365 675f 7061 6972 732e 6170 7065    seg_pairs.appe
+00015900: 6e64 2828 7365 675f 7061 6972 735b 2d31  nd((seg_pairs[-1
+00015910: 5d5b 305d 2b31 2c20 2873 656c 662e 7365  ][0]+1, (self.se
+00015920: 676d 656e 7473 5b2d 315d 2c20 4e6f 6e65  gments[-1], None
+00015930: 2929 290d 0a0d 0a20 2020 2020 2020 2063  )))....        c
+00015940: 6861 6e67 6573 203d 205b 5d0d 0a20 2020  hanges = []..   
+00015950: 2020 2020 2066 6f72 2069 2c20 2873 6567       for i, (seg
+00015960: 302c 2073 6567 3129 2069 6e20 7265 7665  0, seg1) in reve
+00015970: 7273 6564 2873 6567 5f70 6169 7273 293a  rsed(seg_pairs):
+00015980: 0d0a 2020 2020 2020 2020 2020 2020 6669  ..            fi
+00015990: 7273 745f 776f 7264 203d 204e 6f6e 6520  rst_word = None 
+000159a0: 6966 2073 6567 3020 6973 204e 6f6e 6520  if seg0 is None 
+000159b0: 656c 7365 2073 6567 302e 776f 7264 735b  else seg0.words[
+000159c0: 2d31 5d0d 0a20 2020 2020 2020 2020 2020  -1]..           
+000159d0: 206c 6173 745f 776f 7264 203d 204e 6f6e   last_word = Non
+000159e0: 6520 6966 2073 6567 3120 6973 204e 6f6e  e if seg1 is Non
+000159f0: 6520 656c 7365 2073 6567 312e 776f 7264  e else seg1.word
+00015a00: 735b 305d 0d0a 2020 2020 2020 2020 2020  s[0]..          
+00015a10: 2020 7374 6172 7420 3d20 286f 7468 6572    start = (other
+00015a20: 5f72 6573 756c 745b 305d 2e73 7461 7274  _result[0].start
+00015a30: 2069 6620 6669 7273 745f 776f 7264 2069   if first_word i
+00015a40: 7320 4e6f 6e65 2065 6c73 6520 6669 7273  s None else firs
+00015a50: 745f 776f 7264 2e65 6e64 290d 0a20 2020  t_word.end)..   
+00015a60: 2020 2020 2020 2020 2065 6e64 203d 206f           end = o
+00015a70: 7468 6572 5f72 6573 756c 745b 2d31 5d2e  ther_result[-1].
+00015a80: 656e 6420 6966 206c 6173 745f 776f 7264  end if last_word
+00015a90: 2069 7320 4e6f 6e65 2065 6c73 6520 6c61   is None else la
+00015aa0: 7374 5f77 6f72 642e 7374 6172 740d 0a20  st_word.start.. 
+00015ab0: 2020 2020 2020 2020 2020 2069 6620 656e             if en
+00015ac0: 6420 2d20 7374 6172 7420 3c3d 206d 696e  d - start <= min
+00015ad0: 5f67 6170 3a0d 0a20 2020 2020 2020 2020  _gap:..         
+00015ae0: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00015af0: 0a20 2020 2020 2020 2020 2020 2067 6170  .            gap
+00015b00: 5f77 6f72 6473 203d 206f 7468 6572 5f72  _words = other_r
+00015b10: 6573 756c 742e 6765 745f 636f 6e74 656e  esult.get_conten
+00015b20: 745f 6279 5f74 696d 6528 2873 7461 7274  t_by_time((start
+00015b30: 2c20 656e 6429 290d 0a20 2020 2020 2020  , end))..       
+00015b40: 2020 2020 2069 6620 6669 7273 745f 776f       if first_wo
+00015b50: 7264 2069 7320 6e6f 7420 4e6f 6e65 2061  rd is not None a
+00015b60: 6e64 2067 6170 5f77 6f72 6473 2061 6e64  nd gap_words and
+00015b70: 2073 7472 6970 2866 6972 7374 5f77 6f72   strip(first_wor
+00015b80: 642e 776f 7264 2920 3d3d 2073 7472 6970  d.word) == strip
+00015b90: 2867 6170 5f77 6f72 6473 5b30 5d2e 776f  (gap_words[0].wo
+00015ba0: 7264 293a 0d0a 2020 2020 2020 2020 2020  rd):..          
+00015bb0: 2020 2020 2020 6669 7273 745f 776f 7264        first_word
+00015bc0: 2e65 6e64 203d 2067 6170 5f77 6f72 6473  .end = gap_words
+00015bd0: 5b30 5d2e 656e 640d 0a20 2020 2020 2020  [0].end..       
+00015be0: 2020 2020 2020 2020 2067 6170 5f77 6f72           gap_wor
+00015bf0: 6473 203d 2067 6170 5f77 6f72 6473 5b31  ds = gap_words[1
+00015c00: 3a5d 0d0a 2020 2020 2020 2020 2020 2020  :]..            
+00015c10: 6966 206c 6173 745f 776f 7264 2069 7320  if last_word is 
+00015c20: 6e6f 7420 4e6f 6e65 2061 6e64 2067 6170  not None and gap
+00015c30: 5f77 6f72 6473 2061 6e64 2073 7472 6970  _words and strip
+00015c40: 286c 6173 745f 776f 7264 2e77 6f72 6429  (last_word.word)
+00015c50: 203d 3d20 7374 7269 7028 6761 705f 776f   == strip(gap_wo
+00015c60: 7264 735b 2d31 5d2e 776f 7264 293a 0d0a  rds[-1].word):..
+00015c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c80: 6c61 7374 5f77 6f72 642e 7374 6172 7420  last_word.start 
+00015c90: 3d20 6761 705f 776f 7264 735b 2d31 5d2e  = gap_words[-1].
+00015ca0: 7374 6172 740d 0a20 2020 2020 2020 2020  start..         
+00015cb0: 2020 2020 2020 2067 6170 5f77 6f72 6473         gap_words
+00015cc0: 203d 2067 6170 5f77 6f72 6473 5b3a 2d31   = gap_words[:-1
+00015cd0: 5d0d 0a20 2020 2020 2020 2020 2020 2069  ]..            i
+00015ce0: 6620 6e6f 7420 6761 705f 776f 7264 733a  f not gap_words:
+00015cf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015d00: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
+00015d10: 2020 2020 2020 2020 6966 206c 6173 745f          if last_
+00015d20: 776f 7264 2069 7320 6e6f 7420 4e6f 6e65  word is not None
+00015d30: 2061 6e64 206c 6173 745f 776f 7264 2e73   and last_word.s
+00015d40: 7461 7274 203c 2067 6170 5f77 6f72 6473  tart < gap_words
+00015d50: 5b2d 315d 2e65 6e64 3a0d 0a20 2020 2020  [-1].end:..     
+00015d60: 2020 2020 2020 2020 2020 206c 6173 745f             last_
+00015d70: 776f 7264 2e73 7461 7274 203d 2067 6170  word.start = gap
+00015d80: 5f77 6f72 6473 5b2d 315d 2e65 6e64 0d0a  _words[-1].end..
+00015d90: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00015da0: 7365 676d 656e 7473 203d 205b 6f74 6865  segments = [othe
+00015db0: 725f 7265 7375 6c74 5b67 6170 5f77 6f72  r_result[gap_wor
+00015dc0: 6473 5b30 5d2e 7365 676d 656e 745f 6964  ds[0].segment_id
+00015dd0: 5d2e 636f 7079 285b 5d29 5d0d 0a20 2020  ].copy([])]..   
+00015de0: 2020 2020 2020 2020 2066 6f72 206a 2c20           for j, 
+00015df0: 6e65 775f 776f 7264 2069 6e20 656e 756d  new_word in enum
+00015e00: 6572 6174 6528 6761 705f 776f 7264 7329  erate(gap_words)
+00015e10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00015e20: 2020 206e 6577 5f77 6f72 645f 636f 7079     new_word_copy
+00015e30: 203d 206e 6577 5f77 6f72 642e 636f 7079   = new_word.copy
+00015e40: 2863 6f70 795f 746f 6b65 6e73 3d54 7275  (copy_tokens=Tru
+00015e50: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00015e60: 2020 2020 6966 206a 203d 3d20 3020 616e      if j == 0 an
+00015e70: 6420 6669 7273 745f 776f 7264 2069 7320  d first_word is 
+00015e80: 6e6f 7420 4e6f 6e65 2061 6e64 2066 6972  not None and fir
+00015e90: 7374 5f77 6f72 642e 656e 6420 3e20 6761  st_word.end > ga
+00015ea0: 705f 776f 7264 735b 305d 2e73 7461 7274  p_words[0].start
+00015eb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00015ec0: 2020 2020 2020 206e 6577 5f77 6f72 645f         new_word_
+00015ed0: 636f 7079 2e73 7461 7274 203d 2066 6972  copy.start = fir
+00015ee0: 7374 5f77 6f72 642e 656e 640d 0a20 2020  st_word.end..   
+00015ef0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00015f00: 6e65 775f 7365 676d 656e 7473 5b2d 315d  new_segments[-1]
+00015f10: 2e69 6420 213d 206e 6577 5f77 6f72 642e  .id != new_word.
+00015f20: 7365 676d 656e 745f 6964 3a0d 0a20 2020  segment_id:..   
+00015f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f40: 206e 6577 5f73 6567 6d65 6e74 732e 6170   new_segments.ap
+00015f50: 7065 6e64 286f 7468 6572 5f72 6573 756c  pend(other_resul
+00015f60: 745b 6e65 775f 776f 7264 2e73 6567 6d65  t[new_word.segme
+00015f70: 6e74 5f69 645d 2e63 6f70 7928 5b5d 2929  nt_id].copy([]))
+00015f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015f90: 2020 6e65 775f 7365 676d 656e 7473 5b2d    new_segments[-
+00015fa0: 315d 2e77 6f72 6473 2e61 7070 656e 6428  1].words.append(
+00015fb0: 6e65 775f 776f 7264 5f63 6f70 7929 0d0a  new_word_copy)..
+00015fc0: 2020 2020 2020 2020 2020 2020 6966 2076              if v
+00015fd0: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
+00015fe0: 2020 2020 2020 2020 2063 6861 6e67 6573           changes
+00015ff0: 2e61 7070 656e 6428 275c 6e27 2e6a 6f69  .append('\n'.joi
+00016000: 6e28 2741 6464 6564 3a20 2720 2b20 732e  n('Added: ' + s.
+00016010: 746f 5f64 6973 706c 6179 5f73 7472 2854  to_display_str(T
+00016020: 7275 6529 2066 6f72 2073 2069 6e20 6e65  rue) for s in ne
+00016030: 775f 7365 676d 656e 7473 2929 0d0a 2020  w_segments))..  
+00016040: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00016050: 6567 6d65 6e74 7320 3d20 7365 6c66 2e73  egments = self.s
+00016060: 6567 6d65 6e74 735b 3a69 2b31 5d20 2b20  egments[:i+1] + 
+00016070: 6e65 775f 7365 676d 656e 7473 202b 2073  new_segments + s
+00016080: 656c 662e 7365 676d 656e 7473 5b69 2b31  elf.segments[i+1
+00016090: 3a5d 0d0a 2020 2020 2020 2020 6966 2063  :]..        if c
+000160a0: 6861 6e67 6573 3a0d 0a20 2020 2020 2020  hanges:..       
+000160b0: 2020 2020 2070 7269 6e74 2827 5c6e 272e       print('\n'.
+000160c0: 6a6f 696e 2872 6576 6572 7365 6428 6368  join(reversed(ch
+000160d0: 616e 6765 7329 2929 0d0a 2020 2020 2020  anges)))..      
+000160e0: 2020 7365 6c66 2e72 6561 7373 6967 6e5f    self.reassign_
+000160f0: 6964 7328 290d 0a0d 0a20 2020 2020 2020  ids()....       
+00016100: 2072 6574 7572 6e20 7365 6c66 0d0a 0d0a   return self....
+00016110: 2020 2020 6465 6620 7265 6772 6f75 7028      def regroup(
+00016120: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00016130: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
+00016140: 2072 6567 726f 7570 5f61 6c67 6f3a 2055   regroup_algo: U
+00016150: 6e69 6f6e 5b73 7472 2c20 626f 6f6c 5d20  nion[str, bool] 
+00016160: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+00016170: 2020 2020 2076 6572 626f 7365 3a20 626f       verbose: bo
+00016180: 6f6c 203d 2046 616c 7365 2c0d 0a20 2020  ol = False,..   
+00016190: 2020 2020 2020 2020 206f 6e6c 795f 7368           only_sh
+000161a0: 6f77 3a20 626f 6f6c 203d 2046 616c 7365  ow: bool = False
+000161b0: 0d0a 2020 2020 2920 2d3e 2022 5768 6973  ..    ) -> "Whis
+000161c0: 7065 7252 6573 756c 7422 3a0d 0a20 2020  perResult":..   
+000161d0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000161e0: 2020 5265 6772 6f75 7020 2869 6e2d 706c    Regroup (in-pl
+000161f0: 6163 6529 2077 6f72 6473 2069 6e74 6f20  ace) words into 
+00016200: 7365 676d 656e 7473 2e0d 0a0d 0a20 2020  segments.....   
+00016210: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
+00016220: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00016230: 2d2d 2d0d 0a20 2020 2020 2020 2072 6567  ---..        reg
+00016240: 726f 7570 5f61 6c67 6f3a 2073 7472 206f  roup_algo: str o
+00016250: 7220 626f 6f6c 2c20 6465 6661 756c 7420  r bool, default 
+00016260: 2764 6127 0d0a 2020 2020 2020 2020 2020  'da'..          
+00016270: 2020 2053 7472 696e 6720 7265 7072 6573     String repres
+00016280: 656e 7461 7469 6f6e 206f 6620 6120 6375  entation of a cu
+00016290: 7374 6f6d 2072 6567 726f 7570 696e 6720  stom regrouping 
+000162a0: 616c 676f 7269 7468 6d20 6f72 2060 6054  algorithm or ``T
+000162b0: 7275 6560 6020 7573 6520 746f 2074 6865  rue`` use to the
+000162c0: 2064 6566 6175 6c74 2061 6c67 6f72 6974   default algorit
+000162d0: 686d 2027 6461 272e 0d0a 2020 2020 2020  hm 'da'...      
+000162e0: 2020 7665 7262 6f73 6520 3a20 626f 6f6c    verbose : bool
+000162f0: 2c20 6465 6661 756c 7420 4661 6c73 650d  , default False.
+00016300: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
+00016310: 7468 6572 2074 6f20 7368 6f77 2061 6c6c  ther to show all
+00016320: 2074 6865 206d 6574 686f 6473 2061 6e64   the methods and
+00016330: 2061 7267 756d 656e 7473 2070 6172 7365   arguments parse
+00016340: 6420 6672 6f6d 2060 6072 6567 726f 7570  d from ``regroup
+00016350: 5f61 6c67 6f60 602e 0d0a 2020 2020 2020  _algo``...      
+00016360: 2020 6f6e 6c79 5f73 686f 7720 3a20 626f    only_show : bo
+00016370: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
+00016380: 650d 0a20 2020 2020 2020 2020 2020 2057  e..            W
+00016390: 6865 7468 6572 2074 6f20 7368 6f77 2074  hether to show t
+000163a0: 6865 2061 6c6c 206d 6574 686f 6473 2061  he all methods a
+000163b0: 6e64 2061 7267 756d 656e 7473 2070 6172  nd arguments par
+000163c0: 7365 6420 6672 6f6d 2060 6072 6567 726f  sed from ``regro
+000163d0: 7570 5f61 6c67 6f60 6020 7769 7468 6f75  up_algo`` withou
+000163e0: 7420 7275 6e6e 696e 6720 7468 6520 6d65  t running the me
+000163f0: 7468 6f64 730d 0a0d 0a20 2020 2020 2020  thods....       
+00016400: 2052 6574 7572 6e73 0d0a 2020 2020 2020   Returns..      
+00016410: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020    -------..     
+00016420: 2020 2073 7461 626c 655f 7768 6973 7065     stable_whispe
+00016430: 722e 7265 7375 6c74 2e57 6869 7370 6572  r.result.Whisper
+00016440: 5265 7375 6c74 0d0a 2020 2020 2020 2020  Result..        
+00016450: 2020 2020 5468 6520 6375 7272 656e 7420      The current 
+00016460: 696e 7374 616e 6365 2061 6674 6572 2074  instance after t
+00016470: 6865 2063 6861 6e67 6573 2e0d 0a0d 0a20  he changes..... 
+00016480: 2020 2020 2020 204e 6f74 6573 0d0a 2020         Notes..  
+00016490: 2020 2020 2020 2d2d 2d2d 2d0d 0a20 2020        -----..   
+000164a0: 2020 2020 2053 796e 7461 7820 666f 7220       Syntax for 
+000164b0: 7374 7269 6e67 2072 6570 7265 7365 6e74  string represent
+000164c0: 6174 696f 6e20 6f66 2063 7573 746f 6d20  ation of custom 
+000164d0: 7265 6772 6f75 7069 6e67 2061 6c67 6f72  regrouping algor
+000164e0: 6974 686d 2e0d 0a20 2020 2020 2020 2020  ithm...         
+000164f0: 2020 204d 6574 686f 6420 6b65 7973 3a0d     Method keys:.
+00016500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016510: 2073 673a 2073 706c 6974 5f62 795f 6761   sg: split_by_ga
+00016520: 700d 0a20 2020 2020 2020 2020 2020 2020  p..             
+00016530: 2020 2073 703a 2073 706c 6974 5f62 795f     sp: split_by_
+00016540: 7075 6e63 7475 6174 696f 6e0d 0a20 2020  punctuation..   
+00016550: 2020 2020 2020 2020 2020 2020 2073 6c3a               sl:
+00016560: 2073 706c 6974 5f62 795f 6c65 6e67 7468   split_by_length
+00016570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016580: 2020 7364 3a20 7370 6c69 745f 6279 5f64    sd: split_by_d
+00016590: 7572 6174 696f 6e0d 0a20 2020 2020 2020  uration..       
+000165a0: 2020 2020 2020 2020 206d 673a 206d 6572           mg: mer
+000165b0: 6765 5f62 795f 6761 700d 0a20 2020 2020  ge_by_gap..     
+000165c0: 2020 2020 2020 2020 2020 206d 703a 206d             mp: m
+000165d0: 6572 6765 5f62 795f 7075 6e63 7475 6174  erge_by_punctuat
+000165e0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+000165f0: 2020 2020 206d 733a 206d 6572 6765 5f61       ms: merge_a
+00016600: 6c6c 5f73 6567 6d65 6e74 0d0a 2020 2020  ll_segment..    
+00016610: 2020 2020 2020 2020 2020 2020 636d 3a20              cm: 
+00016620: 636c 616d 705f 6d61 780d 0a20 2020 2020  clamp_max..     
+00016630: 2020 2020 2020 2020 2020 206c 3a20 6c6f             l: lo
+00016640: 636b 0d0a 2020 2020 2020 2020 2020 2020  ck..            
+00016650: 2020 2020 7573 3a20 756e 6c6f 636b 5f61      us: unlock_a
+00016660: 6c6c 5f73 6567 6d65 6e74 730d 0a20 2020  ll_segments..   
+00016670: 2020 2020 2020 2020 2020 2020 2064 613a               da:
+00016680: 2064 6566 6175 6c74 2061 6c67 6f72 6974   default algorit
+00016690: 686d 2028 636d 5f73 703d 2c2a 202f efbc  hm (cm_sp=,* /..
+000166a0: 8c5f 7367 3d2e 355f 6d67 3d2e 332b 335f  ._sg=.5_mg=.3+3_
+000166b0: 7370 3d2e 2a20 2fe3 8082 2f3f 2fef bc9f  sp=.* /.../?/...
+000166c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000166d0: 2020 2072 773a 2072 656d 6f76 655f 776f     rw: remove_wo
+000166e0: 7264 0d0a 2020 2020 2020 2020 2020 2020  rd..            
+000166f0: 2020 2020 7273 3a20 7265 6d6f 7665 5f73      rs: remove_s
+00016700: 6567 6d65 6e74 0d0a 2020 2020 2020 2020  egment..        
+00016710: 2020 2020 2020 2020 7270 3a20 7265 6d6f          rp: remo
+00016720: 7665 5f72 6570 6574 6974 696f 6e0d 0a20  ve_repetition.. 
+00016730: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00016740: 7773 3a20 7265 6d6f 7665 5f77 6f72 6473  ws: remove_words
+00016750: 5f62 795f 7374 720d 0a20 2020 2020 2020  _by_str..       
+00016760: 2020 2020 2020 2020 2066 673a 2066 696c           fg: fil
+00016770: 6c5f 696e 5f67 6170 730d 0a20 2020 2020  l_in_gaps..     
+00016780: 2020 2020 2020 204d 6574 6163 6861 7261         Metachara
+00016790: 6374 6572 733a 0d0a 2020 2020 2020 2020  cters:..        
+000167a0: 2020 2020 2020 2020 3d20 7365 7061 7261          = separa
+000167b0: 7465 7320 6120 6d65 7468 6f64 206b 6579  tes a method key
+000167c0: 2061 6e64 2069 7473 2061 7267 756d 656e   and its argumen
+000167d0: 7473 2028 6e6f 7420 7573 6564 2069 6620  ts (not used if 
+000167e0: 6e6f 2061 7267 756d 656e 7429 0d0a 2020  no argument)..  
+000167f0: 2020 2020 2020 2020 2020 2020 2020 5f20                _ 
+00016800: 7365 7061 7261 7465 7320 6d65 7468 6f64  separates method
+00016810: 206b 6579 7320 2861 6674 6572 2061 7267   keys (after arg
+00016820: 756d 656e 7473 2069 6620 7468 6572 6520  uments if there 
+00016830: 6172 6520 616e 7929 0d0a 2020 2020 2020  are any)..      
+00016840: 2020 2020 2020 2020 2020 2b20 7365 7061            + sepa
+00016850: 7261 7465 7320 6172 6775 6d65 6e74 7320  rates arguments 
+00016860: 666f 7220 6120 6d65 7468 6f64 206b 6579  for a method key
+00016870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016880: 2020 2f20 7365 7061 7261 7465 7320 616e    / separates an
+00016890: 2061 7267 756d 656e 7420 696e 746f 206c   argument into l
+000168a0: 6973 7420 6f66 2073 7472 696e 6773 0d0a  ist of strings..
+000168b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168c0: 2a20 7365 7061 7261 7465 7320 616e 2069  * separates an i
+000168d0: 7465 6d20 696e 206c 6973 7420 6f66 2073  tem in list of s
+000168e0: 7472 696e 6773 2069 6e74 6f20 6120 6e65  trings into a ne
+000168f0: 7374 6564 206c 6973 7420 6f66 2073 7472  sted list of str
+00016900: 696e 6773 0d0a 2020 2020 2020 2020 2020  ings..          
+00016910: 2020 4e6f 7465 733a 0d0a 2020 2020 2020    Notes:..      
+00016920: 2020 2020 2020 2d61 7267 756d 656e 7473        -arguments
+00016930: 2061 7265 2070 6172 7365 6420 706f 7369   are parsed posi
+00016940: 7469 6f6e 616c 6c79 0d0a 2020 2020 2020  tionally..      
+00016950: 2020 2020 2020 2d69 6620 6e6f 2061 7267        -if no arg
+00016960: 756d 656e 7420 6973 2070 726f 7669 6465  ument is provide
+00016970: 642c 2074 6865 2064 6566 6175 6c74 206f  d, the default o
+00016980: 6e65 7320 7769 6c6c 2062 6520 7573 6564  nes will be used
+00016990: 0d0a 2020 2020 2020 2020 2020 2020 2d75  ..            -u
+000169a0: 7365 2031 206f 7220 3020 746f 2072 6570  se 1 or 0 to rep
+000169b0: 7265 7365 6e74 2054 7275 6520 6f72 2046  resent True or F
+000169c0: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
+000169d0: 2020 4578 616d 706c 6520 313a 0d0a 2020    Example 1:..  
+000169e0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+000169f0: 7267 655f 6279 5f67 6170 282e 322c 2031  rge_by_gap(.2, 1
+00016a00: 302c 206c 6f63 6b3d 5472 7565 290d 0a20  0, lock=True).. 
+00016a10: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00016a20: 673d 2e32 2b31 302b 2b2b 310d 0a20 2020  g=.2+10+++1..   
+00016a30: 2020 2020 2020 2020 2020 2020 204e 6f74               Not
+00016a40: 653a 205b 6c6f 636b 5d20 6973 2074 6865  e: [lock] is the
+00016a50: 2035 7468 2061 7267 756d 656e 7420 6865   5th argument he
+00016a60: 6e63 6520 7468 6520 3220 6d69 7373 696e  nce the 2 missin
+00016a70: 6720 6172 6775 6d65 6e74 7320 696e 6265  g arguments inbe
+00016a80: 7477 6565 6e20 7468 6520 7468 7265 6520  tween the three 
+00016a90: 2b20 6265 666f 7265 2031 0d0a 2020 2020  + before 1..    
+00016aa0: 2020 2020 2020 2020 4578 616d 706c 6520          Example 
+00016ab0: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
+00016ac0: 2020 2020 7370 6c69 745f 6279 5f70 756e      split_by_pun
+00016ad0: 6374 7561 7469 6f6e 285b 2827 2e27 2c20  ctuation([('.', 
+00016ae0: 2720 2729 2c20 27e3 8082 272c 2027 3f27  ' '), '...', '?'
+00016af0: 2c20 27ef bc9f 275d 2c20 5472 7565 290d  , '...'], True).
+00016b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016b10: 2073 703d 2e2a 202f e380 822f 3f2f efbc   sp=.* /.../?/..
+00016b20: 9f2b 310d 0a20 2020 2020 2020 2020 2020  .+1..           
+00016b30: 2045 7861 6d70 6c65 2033 3a0d 0a20 2020   Example 3:..   
+00016b40: 2020 2020 2020 2020 2020 2020 206d 6572               mer
+00016b50: 6765 5f61 6c6c 5f73 6567 6d65 6e74 7328  ge_all_segments(
+00016b60: 292e 7370 6c69 745f 6279 5f67 6170 282e  ).split_by_gap(.
+00016b70: 3529 2e6d 6572 6765 5f62 795f 6761 7028  5).merge_by_gap(
+00016b80: 2e31 352c 2033 290d 0a20 2020 2020 2020  .15, 3)..       
+00016b90: 2020 2020 2020 2020 206d 735f 7367 3d2e           ms_sg=.
+00016ba0: 355f 6d67 3d2e 3135 2b33 0d0a 2020 2020  5_mg=.15+3..    
+00016bb0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00016bc0: 2069 6620 7265 6772 6f75 705f 616c 676f   if regroup_algo
+00016bd0: 2069 7320 4661 6c73 653a 0d0a 2020 2020   is False:..    
+00016be0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00016bf0: 656c 660d 0a20 2020 2020 2020 2069 6620  elf..        if 
+00016c00: 7265 6772 6f75 705f 616c 676f 2069 7320  regroup_algo is 
+00016c10: 4e6f 6e65 206f 7220 7265 6772 6f75 705f  None or regroup_
+00016c20: 616c 676f 2069 7320 5472 7565 3a0d 0a20  algo is True:.. 
+00016c30: 2020 2020 2020 2020 2020 2072 6567 726f             regro
+00016c40: 7570 5f61 6c67 6f20 3d20 2764 6127 0d0a  up_algo = 'da'..
+00016c50: 0d0a 2020 2020 2020 2020 666f 7220 6d65  ..        for me
+00016c60: 7468 6f64 2c20 6b77 6172 6773 2c20 6d73  thod, kwargs, ms
+00016c70: 6720 696e 2073 656c 662e 7061 7273 655f  g in self.parse_
+00016c80: 7265 6772 6f75 705f 616c 676f 2872 6567  regroup_algo(reg
+00016c90: 726f 7570 5f61 6c67 6f2c 2069 6e63 6c75  roup_algo, inclu
+00016ca0: 6465 5f73 7472 3d76 6572 626f 7365 206f  de_str=verbose o
+00016cb0: 7220 6f6e 6c79 5f73 686f 7729 3a0d 0a20  r only_show):.. 
+00016cc0: 2020 2020 2020 2020 2020 2069 6620 6d73             if ms
+00016cd0: 673a 0d0a 2020 2020 2020 2020 2020 2020  g:..            
+00016ce0: 2020 2020 7072 696e 7428 6d73 6729 0d0a      print(msg)..
+00016cf0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00016d00: 6f74 206f 6e6c 795f 7368 6f77 3a0d 0a20  ot only_show:.. 
+00016d10: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00016d20: 6574 686f 6428 2a2a 6b77 6172 6773 290d  ethod(**kwargs).
+00016d30: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+00016d40: 6e20 7365 6c66 0d0a 0d0a 2020 2020 6465  n self....    de
+00016d50: 6620 7061 7273 655f 7265 6772 6f75 705f  f parse_regroup_
+00016d60: 616c 676f 2873 656c 662c 2072 6567 726f  algo(self, regro
+00016d70: 7570 5f61 6c67 6f3a 2073 7472 2c20 696e  up_algo: str, in
+00016d80: 636c 7564 655f 7374 723a 2062 6f6f 6c20  clude_str: bool 
+00016d90: 3d20 5472 7565 2920 2d3e 204c 6973 745b  = True) -> List[
+00016da0: 5475 706c 655b 4361 6c6c 6162 6c65 2c20  Tuple[Callable, 
+00016db0: 6469 6374 2c20 7374 725d 5d3a 0d0a 2020  dict, str]]:..  
+00016dc0: 2020 2020 2020 6d65 7468 6f64 7320 3d20        methods = 
+00016dd0: 6469 6374 280d 0a20 2020 2020 2020 2020  dict(..         
+00016de0: 2020 2073 673d 7365 6c66 2e73 706c 6974     sg=self.split
+00016df0: 5f62 795f 6761 702c 0d0a 2020 2020 2020  _by_gap,..      
+00016e00: 2020 2020 2020 7370 3d73 656c 662e 7370        sp=self.sp
+00016e10: 6c69 745f 6279 5f70 756e 6374 7561 7469  lit_by_punctuati
+00016e20: 6f6e 2c0d 0a20 2020 2020 2020 2020 2020  on,..           
+00016e30: 2073 6c3d 7365 6c66 2e73 706c 6974 5f62   sl=self.split_b
+00016e40: 795f 6c65 6e67 7468 2c0d 0a20 2020 2020  y_length,..     
+00016e50: 2020 2020 2020 2073 643d 7365 6c66 2e73         sd=self.s
+00016e60: 706c 6974 5f62 795f 6475 7261 7469 6f6e  plit_by_duration
+00016e70: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
+00016e80: 673d 7365 6c66 2e6d 6572 6765 5f62 795f  g=self.merge_by_
+00016e90: 6761 702c 0d0a 2020 2020 2020 2020 2020  gap,..          
+00016ea0: 2020 6d70 3d73 656c 662e 6d65 7267 655f    mp=self.merge_
+00016eb0: 6279 5f70 756e 6374 7561 7469 6f6e 2c0d  by_punctuation,.
+00016ec0: 0a20 2020 2020 2020 2020 2020 206d 733d  .            ms=
+00016ed0: 7365 6c66 2e6d 6572 6765 5f61 6c6c 5f73  self.merge_all_s
 00016ee0: 6567 6d65 6e74 732c 0d0a 2020 2020 2020  egments,..      
-00016ef0: 2020 2020 2020 6c3d 7365 6c66 2e6c 6f63        l=self.loc
-00016f00: 6b2c 0d0a 2020 2020 2020 2020 2020 2020  k,..            
-00016f10: 7277 3d73 656c 662e 7265 6d6f 7665 5f77  rw=self.remove_w
-00016f20: 6f72 642c 0d0a 2020 2020 2020 2020 2020  ord,..          
-00016f30: 2020 7273 3d73 656c 662e 7265 6d6f 7665    rs=self.remove
-00016f40: 5f73 6567 6d65 6e74 2c0d 0a20 2020 2020  _segment,..     
-00016f50: 2020 2020 2020 2072 703d 7365 6c66 2e72         rp=self.r
-00016f60: 656d 6f76 655f 7265 7065 7469 7469 6f6e  emove_repetition
-00016f70: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
-00016f80: 7773 3d73 656c 662e 7265 6d6f 7665 5f77  ws=self.remove_w
-00016f90: 6f72 6473 5f62 795f 7374 722c 0d0a 2020  ords_by_str,..  
-00016fa0: 2020 2020 2020 2020 2020 6667 3d73 656c            fg=sel
-00016fb0: 662e 6669 6c6c 5f69 6e5f 6761 7073 2c0d  f.fill_in_gaps,.
-00016fc0: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
-00016fd0: 2020 2020 6966 206e 6f74 2072 6567 726f      if not regro
-00016fe0: 7570 5f61 6c67 6f3a 0d0a 2020 2020 2020  up_algo:..      
-00016ff0: 2020 2020 2020 7265 7475 726e 205b 5d0d        return [].
-00017000: 0a0d 0a20 2020 2020 2020 2063 616c 6c73  ...        calls
-00017010: 203d 2072 6567 726f 7570 5f61 6c67 6f2e   = regroup_algo.
-00017020: 7370 6c69 7428 275f 2729 0d0a 2020 2020  split('_')..    
-00017030: 2020 2020 6966 2027 6461 2720 696e 2063      if 'da' in c
-00017040: 616c 6c73 3a0d 0a20 2020 2020 2020 2020  alls:..         
-00017050: 2020 2064 6566 6175 6c74 5f63 616c 6c73     default_calls
-00017060: 203d 2027 636d 5f73 703d 2c2a 202f efbc   = 'cm_sp=,* /..
-00017070: 8c5f 7367 3d2e 355f 6d67 3d2e 332b 335f  ._sg=.5_mg=.3+3_
-00017080: 7370 3d2e 2a20 2fe3 8082 2f3f 2fef bc9f  sp=.* /.../?/...
-00017090: 272e 7370 6c69 7428 275f 2729 0d0a 2020  '.split('_')..  
-000170a0: 2020 2020 2020 2020 2020 6361 6c6c 7320            calls 
-000170b0: 3d20 6368 6169 6e2e 6672 6f6d 5f69 7465  = chain.from_ite
-000170c0: 7261 626c 6528 6465 6661 756c 745f 6361  rable(default_ca
-000170d0: 6c6c 7320 6966 206d 6574 686f 6420 3d3d  lls if method ==
-000170e0: 2027 6461 2720 656c 7365 205b 6d65 7468   'da' else [meth
-000170f0: 6f64 5d20 666f 7220 6d65 7468 6f64 2069  od] for method i
-00017100: 6e20 6361 6c6c 7329 0d0a 2020 2020 2020  n calls)..      
-00017110: 2020 6f70 6572 6174 696f 6e73 203d 205b    operations = [
-00017120: 5d0d 0a20 2020 2020 2020 2066 6f72 206d  ]..        for m
-00017130: 6574 686f 6420 696e 2063 616c 6c73 3a0d  ethod in calls:.
-00017140: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
-00017150: 686f 642c 2061 7267 7320 3d20 6d65 7468  hod, args = meth
-00017160: 6f64 2e73 706c 6974 2827 3d27 2c20 6d61  od.split('=', ma
-00017170: 7873 706c 6974 3d31 2920 6966 2027 3d27  xsplit=1) if '='
-00017180: 2069 6e20 6d65 7468 6f64 2065 6c73 6520   in method else 
-00017190: 286d 6574 686f 642c 2027 2729 0d0a 2020  (method, '')..  
-000171a0: 2020 2020 2020 2020 2020 6966 206d 6574            if met
-000171b0: 686f 6420 6e6f 7420 696e 206d 6574 686f  hod not in metho
-000171c0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-000171d0: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
-000171e0: 706c 656d 656e 7465 6445 7272 6f72 2866  plementedError(f
-000171f0: 277b 6d65 7468 6f64 7d20 6973 206e 6f74  '{method} is not
-00017200: 206f 6e65 206f 6620 7468 6520 6176 6169   one of the avai
-00017210: 6c61 626c 6520 6d65 7468 6f64 733a 207b  lable methods: {
-00017220: 7475 706c 6528 6d65 7468 6f64 732e 6b65  tuple(methods.ke
-00017230: 7973 2829 297d 2729 0d0a 2020 2020 2020  ys())}')..      
-00017240: 2020 2020 2020 6172 6773 203d 205b 5d20        args = [] 
-00017250: 6966 206c 656e 2861 7267 7329 203d 3d20  if len(args) == 
-00017260: 3020 656c 7365 206c 6973 7428 6d61 7028  0 else list(map(
-00017270: 7374 725f 746f 5f76 616c 6964 5f74 7970  str_to_valid_typ
-00017280: 652c 2061 7267 732e 7370 6c69 7428 272b  e, args.split('+
-00017290: 2729 2929 0d0a 2020 2020 2020 2020 2020  ')))..          
-000172a0: 2020 6b77 6172 6773 203d 207b 6b3a 2076    kwargs = {k: v
-000172b0: 2066 6f72 206b 2c20 7620 696e 207a 6970   for k, v in zip
-000172c0: 286d 6574 686f 6473 5b6d 6574 686f 645d  (methods[method]
-000172d0: 2e5f 5f63 6f64 655f 5f2e 636f 5f76 6172  .__code__.co_var
-000172e0: 6e61 6d65 735b 313a 5d2c 2061 7267 7329  names[1:], args)
-000172f0: 2069 6620 7620 6973 206e 6f74 204e 6f6e   if v is not Non
-00017300: 657d 0d0a 2020 2020 2020 2020 2020 2020  e}..            
-00017310: 6966 2069 6e63 6c75 6465 5f73 7472 3a0d  if include_str:.
-00017320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017330: 206b 7761 7267 735f 7374 7220 3d20 272c   kwargs_str = ',
-00017340: 2027 2e6a 6f69 6e28 6627 7b6b 7d3d 227b   '.join(f'{k}="{
-00017350: 767d 2227 2069 6620 6973 696e 7374 616e  v}"' if isinstan
-00017360: 6365 2876 2c20 7374 7229 2065 6c73 6520  ce(v, str) else 
-00017370: 6627 7b6b 7d3d 7b76 7d27 2066 6f72 206b  f'{k}={v}' for k
-00017380: 2c20 7620 696e 206b 7761 7267 732e 6974  , v in kwargs.it
-00017390: 656d 7328 2929 0d0a 2020 2020 2020 2020  ems())..        
-000173a0: 2020 2020 2020 2020 6f70 5f73 7472 203d          op_str =
-000173b0: 2066 277b 6d65 7468 6f64 735b 6d65 7468   f'{methods[meth
-000173c0: 6f64 5d2e 5f5f 6e61 6d65 5f5f 7d28 7b6b  od].__name__}({k
-000173d0: 7761 7267 735f 7374 727d 2927 0d0a 2020  wargs_str})'..  
-000173e0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-000173f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017400: 206f 705f 7374 7220 3d20 4e6f 6e65 0d0a   op_str = None..
-00017410: 2020 2020 2020 2020 2020 2020 6f70 6572              oper
-00017420: 6174 696f 6e73 2e61 7070 656e 6428 286d  ations.append((m
-00017430: 6574 686f 6473 5b6d 6574 686f 645d 2c20  ethods[method], 
-00017440: 6b77 6172 6773 2c20 6f70 5f73 7472 2929  kwargs, op_str))
-00017450: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
-00017460: 726e 206f 7065 7261 7469 6f6e 730d 0a0d  rn operations...
-00017470: 0a20 2020 2064 6566 2066 696e 6428 7365  .    def find(se
-00017480: 6c66 2c20 7061 7474 6572 6e3a 2073 7472  lf, pattern: str
-00017490: 2c20 776f 7264 5f6c 6576 656c 3d54 7275  , word_level=Tru
-000174a0: 652c 2066 6c61 6773 3d4e 6f6e 6529 202d  e, flags=None) -
-000174b0: 3e20 2257 6869 7370 6572 5265 7375 6c74  > "WhisperResult
-000174c0: 4d61 7463 6865 7322 3a0d 0a20 2020 2020  Matches":..     
-000174d0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000174e0: 4669 6e64 2073 6567 6d65 6e74 732f 776f  Find segments/wo
-000174f0: 7264 7320 616e 6420 7469 6d65 7374 616d  rds and timestam
-00017500: 7073 2077 6974 6820 7265 6775 6c61 7220  ps with regular 
-00017510: 6578 7072 6573 7369 6f6e 2e0d 0a0d 0a20  expression..... 
-00017520: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00017530: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
-00017540: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2070  -----..        p
-00017550: 6174 7465 726e 203a 2073 7472 0d0a 2020  attern : str..  
-00017560: 2020 2020 2020 2020 2020 5265 6745 7820            RegEx 
-00017570: 7061 7474 6572 6e20 746f 2073 6561 7263  pattern to searc
-00017580: 6820 666f 722e 0d0a 2020 2020 2020 2020  h for...        
-00017590: 776f 7264 5f6c 6576 656c 203a 2062 6f6f  word_level : boo
-000175a0: 6c2c 2064 6566 6175 6c74 2054 7275 650d  l, default True.
-000175b0: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
-000175c0: 7468 6572 2074 6f20 7365 6172 6368 2061  ther to search a
-000175d0: 7420 776f 7264 2d6c 6576 656c 2e0d 0a20  t word-level... 
-000175e0: 2020 2020 2020 2066 6c61 6773 203a 206f         flags : o
-000175f0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-00017600: 2020 2020 2052 6567 4578 2066 6c61 6773       RegEx flags
-00017610: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
-00017620: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
-00017630: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2073  -----..        s
-00017640: 7461 626c 655f 7768 6973 7065 722e 7265  table_whisper.re
-00017650: 7375 6c74 2e57 6869 7370 6572 5265 7375  sult.WhisperResu
-00017660: 6c74 4d61 7463 6865 730d 0a20 2020 2020  ltMatches..     
-00017670: 2020 2020 2020 2041 6e20 696e 7374 616e         An instan
-00017680: 6365 206f 6620 3a63 6c61 7373 3a60 7374  ce of :class:`st
-00017690: 6162 6c65 5f77 6869 7370 6572 2e72 6573  able_whisper.res
-000176a0: 756c 742e 5768 6973 7065 7252 6573 756c  ult.WhisperResul
-000176b0: 744d 6174 6368 6573 6020 7769 7468 2077  tMatches` with w
-000176c0: 6f72 642f 7365 676d 656e 7420 7468 6174  ord/segment that
-000176d0: 206d 6174 6368 2060 6070 6174 7465 726e   match ``pattern
-000176e0: 6060 2e0d 0a20 2020 2020 2020 2022 2222  ``...        """
-000176f0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00017700: 2057 6869 7370 6572 5265 7375 6c74 4d61   WhisperResultMa
-00017710: 7463 6865 7328 7365 6c66 292e 6669 6e64  tches(self).find
-00017720: 2870 6174 7465 726e 2c20 776f 7264 5f6c  (pattern, word_l
-00017730: 6576 656c 3d77 6f72 645f 6c65 7665 6c2c  evel=word_level,
-00017740: 2066 6c61 6773 3d66 6c61 6773 290d 0a0d   flags=flags)...
-00017750: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
-00017760: 2020 2020 6465 6620 7465 7874 2873 656c      def text(sel
-00017770: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
-00017780: 7572 6e20 2727 2e6a 6f69 6e28 732e 7465  urn ''.join(s.te
-00017790: 7874 2066 6f72 2073 2069 6e20 7365 6c66  xt for s in self
-000177a0: 2e73 6567 6d65 6e74 7329 0d0a 0d0a 2020  .segments)....  
-000177b0: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
-000177c0: 2064 6566 2072 6567 726f 7570 5f68 6973   def regroup_his
-000177d0: 746f 7279 2873 656c 6629 3a0d 0a20 2020  tory(self):..   
-000177e0: 2020 2020 2023 2073 616d 6520 7379 6e74       # same synt
-000177f0: 6178 2061 7320 6060 7265 6772 6f75 705f  ax as ``regroup_
-00017800: 616c 676f 6060 2066 6f72 203a 6d65 7468  algo`` for :meth
-00017810: 3a60 6072 6573 756c 742e 5768 6973 7065  :``result.Whispe
-00017820: 7252 6573 756c 742e 7265 6772 6f75 7060  rResult.regroup`
-00017830: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00017840: 2073 656c 662e 5f72 6567 726f 7570 5f68   self._regroup_h
-00017850: 6973 746f 7279 0d0a 0d0a 2020 2020 4070  istory....    @p
-00017860: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
-00017870: 206e 6f6e 7370 6565 6368 5f73 6563 7469   nonspeech_secti
-00017880: 6f6e 7328 7365 6c66 293a 0d0a 2020 2020  ons(self):..    
-00017890: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000178a0: 5f6e 6f6e 7370 6565 6368 5f73 6563 7469  _nonspeech_secti
-000178b0: 6f6e 730d 0a0d 0a20 2020 2064 6566 2073  ons....    def s
-000178c0: 686f 775f 7265 6772 6f75 705f 6869 7374  how_regroup_hist
-000178d0: 6f72 7928 7365 6c66 293a 0d0a 2020 2020  ory(self):..    
-000178e0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-000178f0: 2050 7269 6e74 2064 6574 6169 6c73 206f   Print details o
-00017900: 6620 616c 6c20 7265 6772 6f75 7069 6e67  f all regrouping
-00017910: 206f 7065 7261 7469 6f6e 7320 7468 6174   operations that
-00017920: 2062 6565 6e20 7065 7266 6f72 6d65 6420   been performed 
-00017930: 6f6e 2064 6174 612e 0d0a 2020 2020 2020  on data...      
-00017940: 2020 2222 220d 0a20 2020 2020 2020 2069    """..        i
-00017950: 6620 6e6f 7420 7365 6c66 2e5f 7265 6772  f not self._regr
-00017960: 6f75 705f 6869 7374 6f72 793a 0d0a 2020  oup_history:..  
-00017970: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00017980: 2752 6573 756c 7420 6861 7320 6e6f 2068  'Result has no h
-00017990: 6973 746f 7279 2e27 290d 0a20 2020 2020  istory.')..     
-000179a0: 2020 2066 6f72 202a 5f2c 206d 7367 2069     for *_, msg i
-000179b0: 6e20 7365 6c66 2e70 6172 7365 5f72 6567  n self.parse_reg
-000179c0: 726f 7570 5f61 6c67 6f28 7365 6c66 2e5f  roup_algo(self._
-000179d0: 7265 6772 6f75 705f 6869 7374 6f72 7929  regroup_history)
-000179e0: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-000179f0: 7269 6e74 2866 272e 7b6d 7367 7d27 290d  rint(f'.{msg}').
-00017a00: 0a0d 0a20 2020 2064 6566 205f 5f6c 656e  ...    def __len
-00017a10: 5f5f 2873 656c 6629 3a0d 0a20 2020 2020  __(self):..     
-00017a20: 2020 2072 6574 7572 6e20 6c65 6e28 7365     return len(se
-00017a30: 6c66 2e73 6567 6d65 6e74 7329 0d0a 0d0a  lf.segments)....
-00017a40: 2020 2020 6465 6620 756e 6c6f 636b 5f61      def unlock_a
-00017a50: 6c6c 5f73 6567 6d65 6e74 7328 7365 6c66  ll_segments(self
-00017a60: 293a 0d0a 2020 2020 2020 2020 666f 7220  ):..        for 
-00017a70: 7320 696e 2073 656c 662e 7365 676d 656e  s in self.segmen
-00017a80: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
-00017a90: 2073 2e75 6e6c 6f63 6b5f 616c 6c5f 776f   s.unlock_all_wo
-00017aa0: 7264 7328 290d 0a20 2020 2020 2020 2072  rds()..        r
-00017ab0: 6574 7572 6e20 7365 6c66 0d0a 0d0a 2020  eturn self....  
-00017ac0: 2020 6465 6620 7265 7365 7428 7365 6c66    def reset(self
-00017ad0: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
-00017ae0: 0a20 2020 2020 2020 2052 6573 746f 7265  .        Restore
-00017af0: 2061 6c6c 2076 616c 7565 7320 746f 2074   all values to t
-00017b00: 6861 7420 6174 2069 6e69 7469 616c 697a  hat at initializ
-00017b10: 6174 696f 6e2e 0d0a 2020 2020 2020 2020  ation...        
-00017b20: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
-00017b30: 662e 6c61 6e67 7561 6765 203d 2073 656c  f.language = sel
-00017b40: 662e 6f72 695f 6469 6374 2e67 6574 2827  f.ori_dict.get('
-00017b50: 6c61 6e67 7561 6765 2729 0d0a 2020 2020  language')..    
-00017b60: 2020 2020 7365 6c66 2e5f 7265 6772 6f75      self._regrou
-00017b70: 705f 6869 7374 6f72 7920 3d20 2727 0d0a  p_history = ''..
-00017b80: 2020 2020 2020 2020 7365 676d 656e 7473          segments
-00017b90: 203d 2073 656c 662e 6f72 695f 6469 6374   = self.ori_dict
-00017ba0: 2e67 6574 2827 7365 676d 656e 7473 2729  .get('segments')
-00017bb0: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-00017bc0: 6567 6d65 6e74 7320 3d20 5b53 6567 6d65  egments = [Segme
-00017bd0: 6e74 282a 2a73 2c20 6967 6e6f 7265 5f75  nt(**s, ignore_u
-00017be0: 6e75 7365 645f 6172 6773 3d54 7275 6529  nused_args=True)
-00017bf0: 2066 6f72 2073 2069 6e20 7365 676d 656e   for s in segmen
-00017c00: 7473 5d20 6966 2073 6567 6d65 6e74 7320  ts] if segments 
-00017c10: 656c 7365 205b 5d0d 0a20 2020 2020 2020  else []..       
-00017c20: 2069 6620 7365 6c66 2e5f 666f 7263 6564   if self._forced
-00017c30: 5f6f 7264 6572 3a0d 0a20 2020 2020 2020  _order:..       
-00017c40: 2020 2020 2073 656c 662e 666f 7263 655f       self.force_
-00017c50: 6f72 6465 7228 290d 0a20 2020 2020 2020  order()..       
-00017c60: 2073 656c 662e 7265 6d6f 7665 5f6e 6f5f   self.remove_no_
-00017c70: 776f 7264 5f73 6567 6d65 6e74 7328 616e  word_segments(an
-00017c80: 7928 7365 672e 6861 735f 776f 7264 7320  y(seg.has_words 
-00017c90: 666f 7220 7365 6720 696e 2073 656c 662e  for seg in self.
-00017ca0: 7365 676d 656e 7473 2929 0d0a 0d0a 2020  segments))....  
-00017cb0: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
-00017cc0: 2064 6566 2068 6173 5f77 6f72 6473 2873   def has_words(s
-00017cd0: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00017ce0: 6574 7572 6e20 626f 6f6c 2873 656c 662e  eturn bool(self.
-00017cf0: 7365 676d 656e 7473 2920 616e 6420 616c  segments) and al
-00017d00: 6c28 7365 672e 6861 735f 776f 7264 7320  l(seg.has_words 
-00017d10: 666f 7220 7365 6720 696e 2073 656c 662e  for seg in self.
-00017d20: 7365 676d 656e 7473 290d 0a0d 0a20 2020  segments)....   
-00017d30: 2074 6f5f 7372 745f 7674 7420 3d20 7265   to_srt_vtt = re
-00017d40: 7375 6c74 5f74 6f5f 7372 745f 7674 740d  sult_to_srt_vtt.
-00017d50: 0a20 2020 2074 6f5f 6173 7320 3d20 7265  .    to_ass = re
-00017d60: 7375 6c74 5f74 6f5f 6173 730d 0a20 2020  sult_to_ass..   
-00017d70: 2074 6f5f 7473 7620 3d20 7265 7375 6c74   to_tsv = result
-00017d80: 5f74 6f5f 7473 760d 0a20 2020 2074 6f5f  _to_tsv..    to_
-00017d90: 7478 7420 3d20 7265 7375 6c74 5f74 6f5f  txt = result_to_
-00017da0: 7478 740d 0a20 2020 2073 6176 655f 6173  txt..    save_as
-00017db0: 5f6a 736f 6e20 3d20 7361 7665 5f61 735f  _json = save_as_
-00017dc0: 6a73 6f6e 0d0a 0d0a 0d0a 636c 6173 7320  json......class 
-00017dd0: 5365 676d 656e 744d 6174 6368 3a0d 0a0d  SegmentMatch:...
-00017de0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00017df0: 5f28 0d0a 2020 2020 2020 2020 2020 2020  _(..            
-00017e00: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-00017e10: 2020 2073 6567 6d65 6e74 733a 2055 6e69     segments: Uni
-00017e20: 6f6e 5b4c 6973 745b 5365 676d 656e 745d  on[List[Segment]
-00017e30: 2c20 5365 676d 656e 745d 2c0d 0a20 2020  , Segment],..   
-00017e40: 2020 2020 2020 2020 205f 776f 7264 5f69           _word_i
-00017e50: 6e64 6963 6573 3a20 4c69 7374 5b4c 6973  ndices: List[Lis
-00017e60: 745b 696e 745d 5d20 3d20 4e6f 6e65 2c0d  t[int]] = None,.
-00017e70: 0a20 2020 2020 2020 2020 2020 205f 7465  .            _te
-00017e80: 7874 5f6d 6174 6368 3a20 7374 7220 3d20  xt_match: str = 
-00017e90: 4e6f 6e65 0d0a 2020 2020 293a 0d0a 2020  None..    ):..  
-00017ea0: 2020 2020 2020 7365 6c66 2e73 6567 6d65        self.segme
-00017eb0: 6e74 7320 3d20 5b73 6567 6d65 6e74 735d  nts = [segments]
-00017ec0: 2069 6620 6973 696e 7374 616e 6365 2873   if isinstance(s
-00017ed0: 6567 6d65 6e74 732c 2053 6567 6d65 6e74  egments, Segment
-00017ee0: 2920 656c 7365 2073 6567 6d65 6e74 730d  ) else segments.
-00017ef0: 0a20 2020 2020 2020 2073 656c 662e 776f  .        self.wo
-00017f00: 7264 5f69 6e64 6963 6573 203d 205b 5d20  rd_indices = [] 
-00017f10: 6966 205f 776f 7264 5f69 6e64 6963 6573  if _word_indices
-00017f20: 2069 7320 4e6f 6e65 2065 6c73 6520 5f77   is None else _w
-00017f30: 6f72 645f 696e 6469 6365 730d 0a20 2020  ord_indices..   
-00017f40: 2020 2020 2073 656c 662e 776f 7264 7320       self.words 
-00017f50: 3d20 5b73 656c 662e 7365 676d 656e 7473  = [self.segments
-00017f60: 5b69 5d2e 776f 7264 735b 6a5d 2066 6f72  [i].words[j] for
-00017f70: 2069 2c20 696e 6469 6365 7320 696e 2065   i, indices in e
-00017f80: 6e75 6d65 7261 7465 2873 656c 662e 776f  numerate(self.wo
-00017f90: 7264 5f69 6e64 6963 6573 2920 666f 7220  rd_indices) for 
-00017fa0: 6a20 696e 2069 6e64 6963 6573 5d0d 0a20  j in indices].. 
-00017fb0: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
-00017fc0: 6c66 2e77 6f72 6473 2920 213d 2030 3a0d  lf.words) != 0:.
-00017fd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00017fe0: 662e 7465 7874 203d 2027 272e 6a6f 696e  f.text = ''.join
-00017ff0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00018000: 2020 2073 656c 662e 7365 676d 656e 7473     self.segments
-00018010: 5b69 5d2e 776f 7264 735b 6a5d 2e77 6f72  [i].words[j].wor
-00018020: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
-00018030: 2020 2066 6f72 2069 2c20 696e 6469 6365     for i, indice
-00018040: 7320 696e 2065 6e75 6d65 7261 7465 2873  s in enumerate(s
-00018050: 656c 662e 776f 7264 5f69 6e64 6963 6573  elf.word_indices
-00018060: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018070: 2020 2066 6f72 206a 2069 6e20 696e 6469     for j in indi
-00018080: 6365 730d 0a20 2020 2020 2020 2020 2020  ces..           
-00018090: 2029 0d0a 2020 2020 2020 2020 656c 7365   )..        else
-000180a0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-000180b0: 656c 662e 7465 7874 203d 2027 272e 6a6f  elf.text = ''.jo
-000180c0: 696e 2873 6567 2e74 6578 7420 666f 7220  in(seg.text for 
-000180d0: 7365 6720 696e 2073 656c 662e 7365 676d  seg in self.segm
-000180e0: 656e 7473 290d 0a20 2020 2020 2020 2073  ents)..        s
-000180f0: 656c 662e 7465 7874 5f6d 6174 6368 203d  elf.text_match =
-00018100: 205f 7465 7874 5f6d 6174 6368 0d0a 0d0a   _text_match....
-00018110: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-00018120: 2020 2064 6566 2073 7461 7274 2873 656c     def start(sel
-00018130: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
-00018140: 7572 6e20 280d 0a20 2020 2020 2020 2020  urn (..         
-00018150: 2020 2073 656c 662e 776f 7264 735b 305d     self.words[0]
-00018160: 2e73 7461 7274 0d0a 2020 2020 2020 2020  .start..        
-00018170: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
-00018180: 776f 7264 7329 2021 3d20 3020 656c 7365  words) != 0 else
-00018190: 0d0a 2020 2020 2020 2020 2020 2020 2873  ..            (s
-000181a0: 656c 662e 7365 676d 656e 7473 5b30 5d2e  elf.segments[0].
-000181b0: 7374 6172 7420 6966 206c 656e 2873 656c  start if len(sel
-000181c0: 662e 7365 676d 656e 7473 2920 213d 2030  f.segments) != 0
-000181d0: 2065 6c73 6520 4e6f 6e65 290d 0a20 2020   else None)..   
-000181e0: 2020 2020 2029 0d0a 0d0a 2020 2020 4070       )....    @p
-000181f0: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
-00018200: 2065 6e64 2873 656c 6629 3a0d 0a20 2020   end(self):..   
-00018210: 2020 2020 2072 6574 7572 6e20 280d 0a20       return (.. 
-00018220: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018230: 776f 7264 735b 2d31 5d2e 656e 640d 0a20  words[-1].end.. 
-00018240: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00018250: 6e28 7365 6c66 2e77 6f72 6473 2920 213d  n(self.words) !=
-00018260: 2030 2065 6c73 650d 0a20 2020 2020 2020   0 else..       
-00018270: 2020 2020 2028 7365 6c66 2e73 6567 6d65       (self.segme
-00018280: 6e74 735b 2d31 5d2e 656e 6420 6966 206c  nts[-1].end if l
-00018290: 656e 2873 656c 662e 7365 676d 656e 7473  en(self.segments
-000182a0: 2920 213d 2030 2065 6c73 6520 4e6f 6e65  ) != 0 else None
-000182b0: 290d 0a20 2020 2020 2020 2029 0d0a 0d0a  )..        )....
-000182c0: 2020 2020 6465 6620 5f5f 6c65 6e5f 5f28      def __len__(
-000182d0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000182e0: 7265 7475 726e 206c 656e 2873 656c 662e  return len(self.
-000182f0: 7365 676d 656e 7473 290d 0a0d 0a20 2020  segments)....   
-00018300: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
-00018310: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
-00018320: 7475 726e 2073 656c 662e 5f5f 6469 6374  turn self.__dict
-00018330: 5f5f 2e5f 5f72 6570 725f 5f28 290d 0a0d  __.__repr__()...
-00018340: 0a20 2020 2064 6566 205f 5f73 7472 5f5f  .    def __str__
-00018350: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00018360: 2072 6574 7572 6e20 7365 6c66 2e5f 5f64   return self.__d
-00018370: 6963 745f 5f2e 5f5f 7374 725f 5f28 290d  ict__.__str__().
-00018380: 0a0d 0a0d 0a63 6c61 7373 2057 6869 7370  .....class Whisp
-00018390: 6572 5265 7375 6c74 4d61 7463 6865 733a  erResultMatches:
-000183a0: 0d0a 2020 2020 2222 220d 0a20 2020 2052  ..    """..    R
-000183b0: 6567 4578 206d 6174 6368 6573 2066 6f72  egEx matches for
-000183c0: 2057 6869 7370 6572 5265 7375 6c74 732e   WhisperResults.
-000183d0: 0d0a 2020 2020 2222 220d 0a20 2020 2023  ..    """..    #
-000183e0: 2055 7365 2057 6869 7370 6572 5265 7375   Use WhisperResu
-000183f0: 6c74 2e66 696e 6428 2920 696e 7374 6561  lt.find() instea
-00018400: 6420 6f66 2069 6e73 7461 6e74 6961 7469  d of instantiati
-00018410: 6e67 2074 6869 7320 636c 6173 7320 6469  ng this class di
-00018420: 7265 6374 6c79 2e0d 0a20 2020 2064 6566  rectly...    def
-00018430: 205f 5f69 6e69 745f 5f28 0d0a 2020 2020   __init__(..    
-00018440: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-00018450: 2020 2020 2020 2020 2020 206d 6174 6368             match
-00018460: 6573 3a20 556e 696f 6e5b 4c69 7374 5b53  es: Union[List[S
-00018470: 6567 6d65 6e74 4d61 7463 685d 2c20 5768  egmentMatch], Wh
-00018480: 6973 7065 7252 6573 756c 745d 2c0d 0a20  isperResult],.. 
-00018490: 2020 2020 2020 2020 2020 205f 7365 676d             _segm
-000184a0: 656e 745f 696e 6469 6365 733a 204c 6973  ent_indices: Lis
-000184b0: 745b 4c69 7374 5b69 6e74 5d5d 203d 204e  t[List[int]] = N
-000184c0: 6f6e 650d 0a20 2020 2029 3a0d 0a20 2020  one..    ):..   
-000184d0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-000184e0: 6365 286d 6174 6368 6573 2c20 5768 6973  ce(matches, Whis
-000184f0: 7065 7252 6573 756c 7429 3a0d 0a20 2020  perResult):..   
-00018500: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-00018510: 7463 6865 7320 3d20 6c69 7374 286d 6170  tches = list(map
-00018520: 2853 6567 6d65 6e74 4d61 7463 682c 206d  (SegmentMatch, m
-00018530: 6174 6368 6573 2e73 6567 6d65 6e74 7329  atches.segments)
-00018540: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00018550: 656c 662e 5f73 6567 6d65 6e74 5f69 6e64  elf._segment_ind
-00018560: 6963 6573 203d 205b 5b69 5d20 666f 7220  ices = [[i] for 
-00018570: 6920 696e 2072 616e 6765 286c 656e 286d  i in range(len(m
-00018580: 6174 6368 6573 2e73 6567 6d65 6e74 7329  atches.segments)
-00018590: 295d 0d0a 2020 2020 2020 2020 656c 7365  )]..        else
-000185a0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-000185b0: 656c 662e 6d61 7463 6865 7320 3d20 6d61  elf.matches = ma
-000185c0: 7463 6865 730d 0a20 2020 2020 2020 2020  tches..         
-000185d0: 2020 2061 7373 6572 7420 5f73 6567 6d65     assert _segme
-000185e0: 6e74 5f69 6e64 6963 6573 2069 7320 6e6f  nt_indices is no
-000185f0: 7420 4e6f 6e65 0d0a 2020 2020 2020 2020  t None..        
-00018600: 2020 2020 6173 7365 7274 206c 656e 2873      assert len(s
-00018610: 656c 662e 6d61 7463 6865 7329 203d 3d20  elf.matches) == 
-00018620: 6c65 6e28 5f73 6567 6d65 6e74 5f69 6e64  len(_segment_ind
-00018630: 6963 6573 290d 0a20 2020 2020 2020 2020  ices)..         
-00018640: 2020 2061 7373 6572 7420 616c 6c28 6c65     assert all(le
-00018650: 6e28 6d61 7463 682e 7365 676d 656e 7473  n(match.segments
-00018660: 2920 3d3d 206c 656e 285f 7365 676d 656e  ) == len(_segmen
-00018670: 745f 696e 6469 6365 735b 695d 2920 666f  t_indices[i]) fo
-00018680: 7220 692c 206d 6174 6368 2069 6e20 656e  r i, match in en
-00018690: 756d 6572 6174 6528 7365 6c66 2e6d 6174  umerate(self.mat
-000186a0: 6368 6573 2929 0d0a 2020 2020 2020 2020  ches))..        
-000186b0: 2020 2020 7365 6c66 2e5f 7365 676d 656e      self._segmen
-000186c0: 745f 696e 6469 6365 7320 3d20 5f73 6567  t_indices = _seg
-000186d0: 6d65 6e74 5f69 6e64 6963 6573 0d0a 0d0a  ment_indices....
-000186e0: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-000186f0: 2020 2064 6566 2073 6567 6d65 6e74 5f69     def segment_i
-00018700: 6e64 6963 6573 2873 656c 6629 3a0d 0a20  ndices(self):.. 
-00018710: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00018720: 6c66 2e5f 7365 676d 656e 745f 696e 6469  lf._segment_indi
-00018730: 6365 730d 0a0d 0a20 2020 2064 6566 205f  ces....    def _
-00018740: 6375 7272 5f73 6567 5f67 726f 7570 7328  curr_seg_groups(
-00018750: 7365 6c66 2920 2d3e 204c 6973 745b 4c69  self) -> List[Li
-00018760: 7374 5b54 7570 6c65 5b69 6e74 2c20 5365  st[Tuple[int, Se
-00018770: 676d 656e 745d 5d5d 3a0d 0a20 2020 2020  gment]]]:..     
-00018780: 2020 2073 6567 5f67 726f 7570 732c 2063     seg_groups, c
-00018790: 7572 725f 7365 6773 203d 205b 5d2c 205b  urr_segs = [], [
-000187a0: 5d0d 0a20 2020 2020 2020 2063 7572 725f  ]..        curr_
-000187b0: 6d61 7820 3d20 2d31 0d0a 2020 2020 2020  max = -1..      
-000187c0: 2020 666f 7220 7365 675f 696e 6469 6365    for seg_indice
-000187d0: 732c 206d 6174 6368 2069 6e20 7a69 7028  s, match in zip(
-000187e0: 7365 6c66 2e5f 7365 676d 656e 745f 696e  self._segment_in
-000187f0: 6469 6365 732c 2073 656c 662e 6d61 7463  dices, self.matc
-00018800: 6865 7329 3a0d 0a20 2020 2020 2020 2020  hes):..         
-00018810: 2020 2066 6f72 2069 2c20 7365 6720 696e     for i, seg in
-00018820: 207a 6970 2873 6f72 7465 6428 7365 675f   zip(sorted(seg_
-00018830: 696e 6469 6365 7329 2c20 6d61 7463 682e  indices), match.
-00018840: 7365 676d 656e 7473 293a 0d0a 2020 2020  segments):..    
-00018850: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00018860: 203e 2063 7572 725f 6d61 783a 0d0a 2020   > curr_max:..  
-00018870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018880: 2020 6375 7272 5f73 6567 732e 6170 7065    curr_segs.appe
-00018890: 6e64 2828 692c 2073 6567 2929 0d0a 2020  nd((i, seg))..  
-000188a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188b0: 2020 6966 2069 202d 2031 2021 3d20 6375    if i - 1 != cu
-000188c0: 7272 5f6d 6178 3a0d 0a20 2020 2020 2020  rr_max:..       
-000188d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188e0: 2073 6567 5f67 726f 7570 732e 6170 7065   seg_groups.appe
-000188f0: 6e64 2863 7572 725f 7365 6773 290d 0a20  nd(curr_segs).. 
-00018900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018910: 2020 2020 2020 2063 7572 725f 7365 6773         curr_segs
-00018920: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00018930: 2020 2020 2020 2020 2020 2063 7572 725f             curr_
-00018940: 6d61 7820 3d20 690d 0a0d 0a20 2020 2020  max = i....     
-00018950: 2020 2069 6620 6375 7272 5f73 6567 733a     if curr_segs:
-00018960: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00018970: 675f 6772 6f75 7073 2e61 7070 656e 6428  g_groups.append(
-00018980: 6375 7272 5f73 6567 7329 0d0a 2020 2020  curr_segs)..    
-00018990: 2020 2020 7265 7475 726e 2073 6567 5f67      return seg_g
-000189a0: 726f 7570 730d 0a0d 0a20 2020 2064 6566  roups....    def
-000189b0: 2066 696e 6428 7365 6c66 2c20 7061 7474   find(self, patt
-000189c0: 6572 6e3a 2073 7472 2c20 776f 7264 5f6c  ern: str, word_l
-000189d0: 6576 656c 3d54 7275 652c 2066 6c61 6773  evel=True, flags
-000189e0: 3d4e 6f6e 6529 202d 3e20 2257 6869 7370  =None) -> "Whisp
-000189f0: 6572 5265 7375 6c74 4d61 7463 6865 7322  erResultMatches"
-00018a00: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00018a10: 2020 2020 2020 2020 4669 6e64 2073 6567          Find seg
-00018a20: 6d65 6e74 732f 776f 7264 7320 616e 6420  ments/words and 
-00018a30: 7469 6d65 7374 616d 7073 2077 6974 6820  timestamps with 
-00018a40: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
-00018a50: 6f6e 2e0d 0a0d 0a20 2020 2020 2020 2050  on.....        P
-00018a60: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
-00018a70: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-00018a80: 2020 2020 2020 2070 6174 7465 726e 203a         pattern :
-00018a90: 2073 7472 0d0a 2020 2020 2020 2020 2020   str..          
-00018aa0: 2020 5265 6745 7820 7061 7474 6572 6e20    RegEx pattern 
-00018ab0: 746f 2073 6561 7263 6820 666f 722e 0d0a  to search for...
-00018ac0: 2020 2020 2020 2020 776f 7264 5f6c 6576          word_lev
-00018ad0: 656c 203a 2062 6f6f 6c2c 2064 6566 6175  el : bool, defau
-00018ae0: 6c74 2054 7275 650d 0a20 2020 2020 2020  lt True..       
-00018af0: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
-00018b00: 7365 6172 6368 2061 7420 776f 7264 2d6c  search at word-l
-00018b10: 6576 656c 2e0d 0a20 2020 2020 2020 2066  evel...        f
-00018b20: 6c61 6773 203a 206f 7074 696f 6e61 6c0d  lags : optional.
-00018b30: 0a20 2020 2020 2020 2020 2020 2052 6567  .            Reg
-00018b40: 4578 2066 6c61 6773 2e0d 0a0d 0a20 2020  Ex flags.....   
-00018b50: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
-00018b60: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
-00018b70: 2020 2020 2020 2073 7461 626c 655f 7768         stable_wh
-00018b80: 6973 7065 722e 7265 7375 6c74 2e57 6869  isper.result.Whi
-00018b90: 7370 6572 5265 7375 6c74 4d61 7463 6865  sperResultMatche
-00018ba0: 730d 0a20 2020 2020 2020 2020 2020 2041  s..            A
-00018bb0: 6e20 696e 7374 616e 6365 206f 6620 3a63  n instance of :c
-00018bc0: 6c61 7373 3a60 7374 6162 6c65 5f77 6869  lass:`stable_whi
-00018bd0: 7370 6572 2e72 6573 756c 742e 5768 6973  sper.result.Whis
-00018be0: 7065 7252 6573 756c 744d 6174 6368 6573  perResultMatches
-00018bf0: 6020 7769 7468 2077 6f72 642f 7365 676d  ` with word/segm
-00018c00: 656e 7420 7468 6174 206d 6174 6368 2060  ent that match `
-00018c10: 6070 6174 7465 726e 6060 2e0d 0a20 2020  `pattern``...   
-00018c20: 2020 2020 2022 2222 0d0a 0d0a 2020 2020       """....    
-00018c30: 2020 2020 7365 675f 6772 6f75 7073 203d      seg_groups =
-00018c40: 2073 656c 662e 5f63 7572 725f 7365 675f   self._curr_seg_
-00018c50: 6772 6f75 7073 2829 0d0a 2020 2020 2020  groups()..      
-00018c60: 2020 6d61 7463 6865 733a 204c 6973 745b    matches: List[
-00018c70: 5365 676d 656e 744d 6174 6368 5d20 3d20  SegmentMatch] = 
-00018c80: 5b5d 0d0a 2020 2020 2020 2020 6d61 7463  []..        matc
-00018c90: 685f 7365 675f 696e 6469 6365 733a 204c  h_seg_indices: L
-00018ca0: 6973 745b 4c69 7374 5b69 6e74 5d5d 203d  ist[List[int]] =
-00018cb0: 205b 5d0d 0a20 2020 2020 2020 2069 6620   []..        if 
-00018cc0: 776f 7264 5f6c 6576 656c 3a0d 0a20 2020  word_level:..   
-00018cd0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00018ce0: 616c 6c28 616c 6c28 7365 672e 6861 735f  all(all(seg.has_
-00018cf0: 776f 7264 7320 666f 7220 7365 6720 696e  words for seg in
-00018d00: 206d 6174 6368 2e73 6567 6d65 6e74 7329   match.segments)
-00018d10: 2066 6f72 206d 6174 6368 2069 6e20 7365   for match in se
-00018d20: 6c66 2e6d 6174 6368 6573 293a 0d0a 2020  lf.matches):..  
-00018d30: 2020 2020 2020 2020 2020 2020 2020 7761                wa
-00018d40: 726e 696e 6773 2e77 6172 6e28 2743 616e  rnings.warn('Can
-00018d50: 6e6f 7420 7065 7266 6f72 6d20 776f 7264  not perform word
-00018d60: 2d6c 6576 656c 2073 6561 7263 6820 7769  -level search wi
-00018d70: 7468 2073 6567 6d65 6e74 2873 2920 6d69  th segment(s) mi
-00018d80: 7373 696e 6720 776f 7264 2074 696d 6573  ssing word times
-00018d90: 7461 6d70 732e 2729 0d0a 2020 2020 2020  tamps.')..      
-00018da0: 2020 2020 2020 2020 2020 776f 7264 5f6c            word_l
-00018db0: 6576 656c 203d 2046 616c 7365 0d0a 0d0a  evel = False....
-00018dc0: 2020 2020 2020 2020 666f 7220 7365 6773          for segs
-00018dd0: 2069 6e20 7365 675f 6772 6f75 7073 3a0d   in seg_groups:.
-00018de0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00018df0: 776f 7264 5f6c 6576 656c 3a0d 0a20 2020  word_level:..   
-00018e00: 2020 2020 2020 2020 2020 2020 2069 6478               idx
-00018e10: 7320 3d20 6c69 7374 2863 6861 696e 2e66  s = list(chain.f
-00018e20: 726f 6d5f 6974 6572 6162 6c65 280d 0a20  rom_iterable(.. 
-00018e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e40: 2020 205b 2869 2c20 6a29 5d2a 6c65 6e28     [(i, j)]*len(
-00018e50: 776f 7264 2e77 6f72 6429 2066 6f72 2028  word.word) for (
-00018e60: 692c 2073 6567 2920 696e 2073 6567 7320  i, seg) in segs 
-00018e70: 666f 7220 6a2c 2077 6f72 6420 696e 2065  for j, word in e
-00018e80: 6e75 6d65 7261 7465 2873 6567 2e77 6f72  numerate(seg.wor
-00018e90: 6473 290d 0a20 2020 2020 2020 2020 2020  ds)..           
-00018ea0: 2020 2020 2029 290d 0a20 2020 2020 2020       ))..       
-00018eb0: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
-00018ec0: 2727 2e6a 6f69 6e28 776f 7264 2e77 6f72  ''.join(word.wor
-00018ed0: 6420 666f 7220 285f 2c20 7365 6729 2069  d for (_, seg) i
-00018ee0: 6e20 7365 6773 2066 6f72 2077 6f72 6420  n segs for word 
-00018ef0: 696e 2073 6567 2e77 6f72 6473 290d 0a20  in seg.words).. 
-00018f00: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00018f10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018f20: 2020 6964 7873 203d 206c 6973 7428 6368    idxs = list(ch
-00018f30: 6169 6e2e 6672 6f6d 5f69 7465 7261 626c  ain.from_iterabl
-00018f40: 6528 5b28 692c 204e 6f6e 6529 5d2a 6c65  e([(i, None)]*le
-00018f50: 6e28 7365 672e 7465 7874 2920 666f 7220  n(seg.text) for 
-00018f60: 2869 2c20 7365 6729 2069 6e20 7365 6773  (i, seg) in segs
-00018f70: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00018f80: 2020 2020 7465 7874 203d 2027 272e 6a6f      text = ''.jo
-00018f90: 696e 2873 6567 2e74 6578 7420 666f 7220  in(seg.text for 
-00018fa0: 285f 2c20 7365 6729 2069 6e20 7365 6773  (_, seg) in segs
-00018fb0: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
-00018fc0: 7373 6572 7420 6c65 6e28 6964 7873 2920  ssert len(idxs) 
-00018fd0: 3d3d 206c 656e 2874 6578 7429 0d0a 2020  == len(text)..  
-00018fe0: 2020 2020 2020 2020 2020 666f 7220 6375            for cu
-00018ff0: 7272 5f6d 6174 6368 2069 6e20 7265 2e66  rr_match in re.f
-00019000: 696e 6469 7465 7228 7061 7474 6572 6e2c  inditer(pattern,
-00019010: 2074 6578 742c 2066 6c61 6773 3d66 6c61   text, flags=fla
-00019020: 6773 206f 7220 3029 3a0d 0a20 2020 2020  gs or 0):..     
-00019030: 2020 2020 2020 2020 2020 2073 7461 7274             start
-00019040: 2c20 656e 6420 3d20 6375 7272 5f6d 6174  , end = curr_mat
-00019050: 6368 2e73 7061 6e28 290d 0a20 2020 2020  ch.span()..     
-00019060: 2020 2020 2020 2020 2020 2063 7572 725f             curr_
-00019070: 6964 7873 203d 2069 6478 735b 7374 6172  idxs = idxs[star
-00019080: 743a 2065 6e64 5d0d 0a20 2020 2020 2020  t: end]..       
-00019090: 2020 2020 2020 2020 2063 7572 725f 7365           curr_se
-000190a0: 675f 6964 7873 203d 2073 6f72 7465 6428  g_idxs = sorted(
-000190b0: 7365 7428 695b 305d 2066 6f72 2069 2069  set(i[0] for i i
-000190c0: 6e20 6375 7272 5f69 6478 7329 290d 0a20  n curr_idxs)).. 
-000190d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000190e0: 6620 776f 7264 5f6c 6576 656c 3a0d 0a20  f word_level:.. 
-000190f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019100: 2020 2063 7572 725f 776f 7264 5f69 6478     curr_word_idx
-00019110: 7320 3d20 5b0d 0a20 2020 2020 2020 2020  s = [..         
-00019120: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019130: 6f72 7465 6428 7365 7428 6a20 666f 7220  orted(set(j for 
-00019140: 692c 206a 2069 6e20 6375 7272 5f69 6478  i, j in curr_idx
-00019150: 7320 6966 2069 203d 3d20 7365 675f 6964  s if i == seg_id
-00019160: 7829 290d 0a20 2020 2020 2020 2020 2020  x))..           
-00019170: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00019180: 2073 6567 5f69 6478 2069 6e20 6375 7272   seg_idx in curr
-00019190: 5f73 6567 5f69 6478 730d 0a20 2020 2020  _seg_idxs..     
-000191a0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-000191b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000191c0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-000191d0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-000191e0: 725f 776f 7264 5f69 6478 7320 3d20 4e6f  r_word_idxs = No
-000191f0: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
-00019200: 2020 2020 6d61 7463 6865 732e 6170 7065      matches.appe
-00019210: 6e64 2853 6567 6d65 6e74 4d61 7463 6828  nd(SegmentMatch(
-00019220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019230: 2020 2020 2020 7365 676d 656e 7473 3d5b        segments=[
-00019240: 7320 666f 7220 692c 2073 2069 6e20 7365  s for i, s in se
-00019250: 6773 2069 6620 6920 696e 2063 7572 725f  gs if i in curr_
-00019260: 7365 675f 6964 7873 5d2c 0d0a 2020 2020  seg_idxs],..    
-00019270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019280: 5f77 6f72 645f 696e 6469 6365 733d 6375  _word_indices=cu
-00019290: 7272 5f77 6f72 645f 6964 7873 2c0d 0a20  rr_word_idxs,.. 
-000192a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192b0: 2020 205f 7465 7874 5f6d 6174 6368 3d63     _text_match=c
-000192c0: 7572 725f 6d61 7463 682e 6772 6f75 7028  urr_match.group(
-000192d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000192e0: 2020 2029 290d 0a20 2020 2020 2020 2020     ))..         
-000192f0: 2020 2020 2020 206d 6174 6368 5f73 6567         match_seg
-00019300: 5f69 6e64 6963 6573 2e61 7070 656e 6428  _indices.append(
-00019310: 6375 7272 5f73 6567 5f69 6478 7329 0d0a  curr_seg_idxs)..
-00019320: 2020 2020 2020 2020 7265 7475 726e 2057          return W
-00019330: 6869 7370 6572 5265 7375 6c74 4d61 7463  hisperResultMatc
-00019340: 6865 7328 6d61 7463 6865 732c 206d 6174  hes(matches, mat
-00019350: 6368 5f73 6567 5f69 6e64 6963 6573 290d  ch_seg_indices).
-00019360: 0a0d 0a20 2020 2064 6566 205f 5f6c 656e  ...    def __len
-00019370: 5f5f 2873 656c 6629 3a0d 0a20 2020 2020  __(self):..     
-00019380: 2020 2072 6574 7572 6e20 6c65 6e28 7365     return len(se
-00019390: 6c66 2e6d 6174 6368 6573 290d 0a0d 0a20  lf.matches).... 
-000193a0: 2020 2064 6566 205f 5f62 6f6f 6c5f 5f28     def __bool__(
-000193b0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000193c0: 7265 7475 726e 2073 656c 662e 5f5f 6c65  return self.__le
-000193d0: 6e5f 5f28 2920 213d 2030 0d0a 0d0a 2020  n__() != 0....  
-000193e0: 2020 6465 6620 5f5f 6765 7469 7465 6d5f    def __getitem_
-000193f0: 5f28 7365 6c66 2c20 6964 7829 3a0d 0a20  _(self, idx):.. 
-00019400: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00019410: 6c66 2e6d 6174 6368 6573 5b69 6478 5d0d  lf.matches[idx].
-00019420: 0a                                       .
+00016ef0: 2020 2020 2020 636d 3d73 656c 662e 636c        cm=self.cl
+00016f00: 616d 705f 6d61 782c 0d0a 2020 2020 2020  amp_max,..      
+00016f10: 2020 2020 2020 7573 3d73 656c 662e 756e        us=self.un
+00016f20: 6c6f 636b 5f61 6c6c 5f73 6567 6d65 6e74  lock_all_segment
+00016f30: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
+00016f40: 6c3d 7365 6c66 2e6c 6f63 6b2c 0d0a 2020  l=self.lock,..  
+00016f50: 2020 2020 2020 2020 2020 7277 3d73 656c            rw=sel
+00016f60: 662e 7265 6d6f 7665 5f77 6f72 642c 0d0a  f.remove_word,..
+00016f70: 2020 2020 2020 2020 2020 2020 7273 3d73              rs=s
+00016f80: 656c 662e 7265 6d6f 7665 5f73 6567 6d65  elf.remove_segme
+00016f90: 6e74 2c0d 0a20 2020 2020 2020 2020 2020  nt,..           
+00016fa0: 2072 703d 7365 6c66 2e72 656d 6f76 655f   rp=self.remove_
+00016fb0: 7265 7065 7469 7469 6f6e 2c0d 0a20 2020  repetition,..   
+00016fc0: 2020 2020 2020 2020 2072 7773 3d73 656c           rws=sel
+00016fd0: 662e 7265 6d6f 7665 5f77 6f72 6473 5f62  f.remove_words_b
+00016fe0: 795f 7374 722c 0d0a 2020 2020 2020 2020  y_str,..        
+00016ff0: 2020 2020 6667 3d73 656c 662e 6669 6c6c      fg=self.fill
+00017000: 5f69 6e5f 6761 7073 2c0d 0a20 2020 2020  _in_gaps,..     
+00017010: 2020 2029 0d0a 2020 2020 2020 2020 6966     )..        if
+00017020: 206e 6f74 2072 6567 726f 7570 5f61 6c67   not regroup_alg
+00017030: 6f3a 0d0a 2020 2020 2020 2020 2020 2020  o:..            
+00017040: 7265 7475 726e 205b 5d0d 0a0d 0a20 2020  return []....   
+00017050: 2020 2020 2063 616c 6c73 203d 2072 6567       calls = reg
+00017060: 726f 7570 5f61 6c67 6f2e 7370 6c69 7428  roup_algo.split(
+00017070: 275f 2729 0d0a 2020 2020 2020 2020 6966  '_')..        if
+00017080: 2027 6461 2720 696e 2063 616c 6c73 3a0d   'da' in calls:.
+00017090: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
+000170a0: 6175 6c74 5f63 616c 6c73 203d 2027 636d  ault_calls = 'cm
+000170b0: 5f73 703d 2c2a 202f efbc 8c5f 7367 3d2e  _sp=,* /..._sg=.
+000170c0: 355f 6d67 3d2e 332b 335f 7370 3d2e 2a20  5_mg=.3+3_sp=.* 
+000170d0: 2fe3 8082 2f3f 2fef bc9f 272e 7370 6c69  /.../?/...'.spli
+000170e0: 7428 275f 2729 0d0a 2020 2020 2020 2020  t('_')..        
+000170f0: 2020 2020 6361 6c6c 7320 3d20 6368 6169      calls = chai
+00017100: 6e2e 6672 6f6d 5f69 7465 7261 626c 6528  n.from_iterable(
+00017110: 6465 6661 756c 745f 6361 6c6c 7320 6966  default_calls if
+00017120: 206d 6574 686f 6420 3d3d 2027 6461 2720   method == 'da' 
+00017130: 656c 7365 205b 6d65 7468 6f64 5d20 666f  else [method] fo
+00017140: 7220 6d65 7468 6f64 2069 6e20 6361 6c6c  r method in call
+00017150: 7329 0d0a 2020 2020 2020 2020 6f70 6572  s)..        oper
+00017160: 6174 696f 6e73 203d 205b 5d0d 0a20 2020  ations = []..   
+00017170: 2020 2020 2066 6f72 206d 6574 686f 6420       for method 
+00017180: 696e 2063 616c 6c73 3a0d 0a20 2020 2020  in calls:..     
+00017190: 2020 2020 2020 206d 6574 686f 642c 2061         method, a
+000171a0: 7267 7320 3d20 6d65 7468 6f64 2e73 706c  rgs = method.spl
+000171b0: 6974 2827 3d27 2c20 6d61 7873 706c 6974  it('=', maxsplit
+000171c0: 3d31 2920 6966 2027 3d27 2069 6e20 6d65  =1) if '=' in me
+000171d0: 7468 6f64 2065 6c73 6520 286d 6574 686f  thod else (metho
+000171e0: 642c 2027 2729 0d0a 2020 2020 2020 2020  d, '')..        
+000171f0: 2020 2020 6966 206d 6574 686f 6420 6e6f      if method no
+00017200: 7420 696e 206d 6574 686f 6473 3a0d 0a20  t in methods:.. 
+00017210: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00017220: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
+00017230: 7465 6445 7272 6f72 2866 277b 6d65 7468  tedError(f'{meth
+00017240: 6f64 7d20 6973 206e 6f74 206f 6e65 206f  od} is not one o
+00017250: 6620 7468 6520 6176 6169 6c61 626c 6520  f the available 
+00017260: 6d65 7468 6f64 733a 207b 7475 706c 6528  methods: {tuple(
+00017270: 6d65 7468 6f64 732e 6b65 7973 2829 297d  methods.keys())}
+00017280: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+00017290: 6172 6773 203d 205b 5d20 6966 206c 656e  args = [] if len
+000172a0: 2861 7267 7329 203d 3d20 3020 656c 7365  (args) == 0 else
+000172b0: 206c 6973 7428 6d61 7028 7374 725f 746f   list(map(str_to
+000172c0: 5f76 616c 6964 5f74 7970 652c 2061 7267  _valid_type, arg
+000172d0: 732e 7370 6c69 7428 272b 2729 2929 0d0a  s.split('+')))..
+000172e0: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
+000172f0: 6773 203d 207b 6b3a 2076 2066 6f72 206b  gs = {k: v for k
+00017300: 2c20 7620 696e 207a 6970 286d 6574 686f  , v in zip(metho
+00017310: 6473 5b6d 6574 686f 645d 2e5f 5f63 6f64  ds[method].__cod
+00017320: 655f 5f2e 636f 5f76 6172 6e61 6d65 735b  e__.co_varnames[
+00017330: 313a 5d2c 2061 7267 7329 2069 6620 7620  1:], args) if v 
+00017340: 6973 206e 6f74 204e 6f6e 657d 0d0a 2020  is not None}..  
+00017350: 2020 2020 2020 2020 2020 6966 2069 6e63            if inc
+00017360: 6c75 6465 5f73 7472 3a0d 0a20 2020 2020  lude_str:..     
+00017370: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
+00017380: 735f 7374 7220 3d20 272c 2027 2e6a 6f69  s_str = ', '.joi
+00017390: 6e28 6627 7b6b 7d3d 227b 767d 2227 2069  n(f'{k}="{v}"' i
+000173a0: 6620 6973 696e 7374 616e 6365 2876 2c20  f isinstance(v, 
+000173b0: 7374 7229 2065 6c73 6520 6627 7b6b 7d3d  str) else f'{k}=
+000173c0: 7b76 7d27 2066 6f72 206b 2c20 7620 696e  {v}' for k, v in
+000173d0: 206b 7761 7267 732e 6974 656d 7328 2929   kwargs.items())
+000173e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000173f0: 2020 6f70 5f73 7472 203d 2066 277b 6d65    op_str = f'{me
+00017400: 7468 6f64 735b 6d65 7468 6f64 5d2e 5f5f  thods[method].__
+00017410: 6e61 6d65 5f5f 7d28 7b6b 7761 7267 735f  name__}({kwargs_
+00017420: 7374 727d 2927 0d0a 2020 2020 2020 2020  str})'..        
+00017430: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00017440: 2020 2020 2020 2020 2020 206f 705f 7374             op_st
+00017450: 7220 3d20 4e6f 6e65 0d0a 2020 2020 2020  r = None..      
+00017460: 2020 2020 2020 6f70 6572 6174 696f 6e73        operations
+00017470: 2e61 7070 656e 6428 286d 6574 686f 6473  .append((methods
+00017480: 5b6d 6574 686f 645d 2c20 6b77 6172 6773  [method], kwargs
+00017490: 2c20 6f70 5f73 7472 2929 0d0a 0d0a 2020  , op_str))....  
+000174a0: 2020 2020 2020 7265 7475 726e 206f 7065        return ope
+000174b0: 7261 7469 6f6e 730d 0a0d 0a20 2020 2064  rations....    d
+000174c0: 6566 2066 696e 6428 7365 6c66 2c20 7061  ef find(self, pa
+000174d0: 7474 6572 6e3a 2073 7472 2c20 776f 7264  ttern: str, word
+000174e0: 5f6c 6576 656c 3d54 7275 652c 2066 6c61  _level=True, fla
+000174f0: 6773 3d4e 6f6e 6529 202d 3e20 2257 6869  gs=None) -> "Whi
+00017500: 7370 6572 5265 7375 6c74 4d61 7463 6865  sperResultMatche
+00017510: 7322 3a0d 0a20 2020 2020 2020 2022 2222  s":..        """
+00017520: 0d0a 2020 2020 2020 2020 4669 6e64 2073  ..        Find s
+00017530: 6567 6d65 6e74 732f 776f 7264 7320 616e  egments/words an
+00017540: 6420 7469 6d65 7374 616d 7073 2077 6974  d timestamps wit
+00017550: 6820 7265 6775 6c61 7220 6578 7072 6573  h regular expres
+00017560: 7369 6f6e 2e0d 0a0d 0a20 2020 2020 2020  sion.....       
+00017570: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
+00017580: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d       ----------.
+00017590: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
+000175a0: 203a 2073 7472 0d0a 2020 2020 2020 2020   : str..        
+000175b0: 2020 2020 5265 6745 7820 7061 7474 6572      RegEx patter
+000175c0: 6e20 746f 2073 6561 7263 6820 666f 722e  n to search for.
+000175d0: 0d0a 2020 2020 2020 2020 776f 7264 5f6c  ..        word_l
+000175e0: 6576 656c 203a 2062 6f6f 6c2c 2064 6566  evel : bool, def
+000175f0: 6175 6c74 2054 7275 650d 0a20 2020 2020  ault True..     
+00017600: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
+00017610: 6f20 7365 6172 6368 2061 7420 776f 7264  o search at word
+00017620: 2d6c 6576 656c 2e0d 0a20 2020 2020 2020  -level...       
+00017630: 2066 6c61 6773 203a 206f 7074 696f 6e61   flags : optiona
+00017640: 6c0d 0a20 2020 2020 2020 2020 2020 2052  l..            R
+00017650: 6567 4578 2066 6c61 6773 2e0d 0a0d 0a20  egEx flags..... 
+00017660: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
+00017670: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
+00017680: 0a20 2020 2020 2020 2073 7461 626c 655f  .        stable_
+00017690: 7768 6973 7065 722e 7265 7375 6c74 2e57  whisper.result.W
+000176a0: 6869 7370 6572 5265 7375 6c74 4d61 7463  hisperResultMatc
+000176b0: 6865 730d 0a20 2020 2020 2020 2020 2020  hes..           
+000176c0: 2041 6e20 696e 7374 616e 6365 206f 6620   An instance of 
+000176d0: 3a63 6c61 7373 3a60 7374 6162 6c65 5f77  :class:`stable_w
+000176e0: 6869 7370 6572 2e72 6573 756c 742e 5768  hisper.result.Wh
+000176f0: 6973 7065 7252 6573 756c 744d 6174 6368  isperResultMatch
+00017700: 6573 6020 7769 7468 2077 6f72 642f 7365  es` with word/se
+00017710: 676d 656e 7420 7468 6174 206d 6174 6368  gment that match
+00017720: 2060 6070 6174 7465 726e 6060 2e0d 0a20   ``pattern``... 
+00017730: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00017740: 2020 2020 7265 7475 726e 2057 6869 7370      return Whisp
+00017750: 6572 5265 7375 6c74 4d61 7463 6865 7328  erResultMatches(
+00017760: 7365 6c66 292e 6669 6e64 2870 6174 7465  self).find(patte
+00017770: 726e 2c20 776f 7264 5f6c 6576 656c 3d77  rn, word_level=w
+00017780: 6f72 645f 6c65 7665 6c2c 2066 6c61 6773  ord_level, flags
+00017790: 3d66 6c61 6773 290d 0a0d 0a20 2020 2040  =flags)....    @
+000177a0: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
+000177b0: 6620 7465 7874 2873 656c 6629 3a0d 0a20  f text(self):.. 
+000177c0: 2020 2020 2020 2072 6574 7572 6e20 2727         return ''
+000177d0: 2e6a 6f69 6e28 732e 7465 7874 2066 6f72  .join(s.text for
+000177e0: 2073 2069 6e20 7365 6c66 2e73 6567 6d65   s in self.segme
+000177f0: 6e74 7329 0d0a 0d0a 2020 2020 4070 726f  nts)....    @pro
+00017800: 7065 7274 790d 0a20 2020 2064 6566 2072  perty..    def r
+00017810: 6567 726f 7570 5f68 6973 746f 7279 2873  egroup_history(s
+00017820: 656c 6629 3a0d 0a20 2020 2020 2020 2023  elf):..        #
+00017830: 2073 616d 6520 7379 6e74 6178 2061 7320   same syntax as 
+00017840: 6060 7265 6772 6f75 705f 616c 676f 6060  ``regroup_algo``
+00017850: 2066 6f72 203a 6d65 7468 3a60 6072 6573   for :meth:``res
+00017860: 756c 742e 5768 6973 7065 7252 6573 756c  ult.WhisperResul
+00017870: 742e 7265 6772 6f75 7060 0d0a 2020 2020  t.regroup`..    
+00017880: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00017890: 5f72 6567 726f 7570 5f68 6973 746f 7279  _regroup_history
+000178a0: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
+000178b0: 790d 0a20 2020 2064 6566 206e 6f6e 7370  y..    def nonsp
+000178c0: 6565 6368 5f73 6563 7469 6f6e 7328 7365  eech_sections(se
+000178d0: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
+000178e0: 7475 726e 2073 656c 662e 5f6e 6f6e 7370  turn self._nonsp
+000178f0: 6565 6368 5f73 6563 7469 6f6e 730d 0a0d  eech_sections...
+00017900: 0a20 2020 2064 6566 2073 686f 775f 7265  .    def show_re
+00017910: 6772 6f75 705f 6869 7374 6f72 7928 7365  group_history(se
+00017920: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
+00017930: 220d 0a20 2020 2020 2020 2050 7269 6e74  "..        Print
+00017940: 2064 6574 6169 6c73 206f 6620 616c 6c20   details of all 
+00017950: 7265 6772 6f75 7069 6e67 206f 7065 7261  regrouping opera
+00017960: 7469 6f6e 7320 7468 6174 2062 6565 6e20  tions that been 
+00017970: 7065 7266 6f72 6d65 6420 6f6e 2064 6174  performed on dat
+00017980: 612e 0d0a 2020 2020 2020 2020 2222 220d  a...        """.
+00017990: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000179a0: 7365 6c66 2e5f 7265 6772 6f75 705f 6869  self._regroup_hi
+000179b0: 7374 6f72 793a 0d0a 2020 2020 2020 2020  story:..        
+000179c0: 2020 2020 7072 696e 7428 2752 6573 756c      print('Resul
+000179d0: 7420 6861 7320 6e6f 2068 6973 746f 7279  t has no history
+000179e0: 2e27 290d 0a20 2020 2020 2020 2066 6f72  .')..        for
+000179f0: 202a 5f2c 206d 7367 2069 6e20 7365 6c66   *_, msg in self
+00017a00: 2e70 6172 7365 5f72 6567 726f 7570 5f61  .parse_regroup_a
+00017a10: 6c67 6f28 7365 6c66 2e5f 7265 6772 6f75  lgo(self._regrou
+00017a20: 705f 6869 7374 6f72 7929 3a0d 0a20 2020  p_history):..   
+00017a30: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+00017a40: 272e 7b6d 7367 7d27 290d 0a0d 0a20 2020  '.{msg}')....   
+00017a50: 2064 6566 205f 5f6c 656e 5f5f 2873 656c   def __len__(sel
+00017a60: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
+00017a70: 7572 6e20 6c65 6e28 7365 6c66 2e73 6567  urn len(self.seg
+00017a80: 6d65 6e74 7329 0d0a 0d0a 2020 2020 6465  ments)....    de
+00017a90: 6620 756e 6c6f 636b 5f61 6c6c 5f73 6567  f unlock_all_seg
+00017aa0: 6d65 6e74 7328 7365 6c66 293a 0d0a 2020  ments(self):..  
+00017ab0: 2020 2020 2020 666f 7220 7320 696e 2073        for s in s
+00017ac0: 656c 662e 7365 676d 656e 7473 3a0d 0a20  elf.segments:.. 
+00017ad0: 2020 2020 2020 2020 2020 2073 2e75 6e6c             s.unl
+00017ae0: 6f63 6b5f 616c 6c5f 776f 7264 7328 290d  ock_all_words().
+00017af0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00017b00: 7365 6c66 0d0a 0d0a 2020 2020 6465 6620  self....    def 
+00017b10: 7365 745f 6375 7272 656e 745f 6173 5f6f  set_current_as_o
+00017b20: 7269 6728 7365 6c66 2c20 6b65 6570 5f6f  rig(self, keep_o
+00017b30: 7269 673a 2062 6f6f 6c20 3d20 4661 6c73  rig: bool = Fals
+00017b40: 6529 3a0d 0a20 2020 2020 2020 2022 2222  e):..        """
+00017b50: 0d0a 2020 2020 2020 2020 4f76 6572 7772  ..        Overwr
+00017b60: 6974 6520 616c 6c20 7661 6c75 6573 2069  ite all values i
+00017b70: 6e20 6060 6f72 695f 6469 6374 6060 2077  n ``ori_dict`` w
+00017b80: 6974 6820 6375 7272 656e 7420 7661 6c75  ith current valu
+00017b90: 6573 2e0d 0a20 2020 2020 2020 2022 2222  es...        """
+00017ba0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
+00017bb0: 7269 5f64 6963 7420 3d20 7365 6c66 2e74  ri_dict = self.t
+00017bc0: 6f5f 6469 6374 286b 6565 705f 6f72 6967  o_dict(keep_orig
+00017bd0: 3d6b 6565 705f 6f72 6967 290d 0a0d 0a20  =keep_orig).... 
+00017be0: 2020 2064 6566 2072 6573 6574 2873 656c     def reset(sel
+00017bf0: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
+00017c00: 0d0a 2020 2020 2020 2020 5265 7374 6f72  ..        Restor
+00017c10: 6520 616c 6c20 7661 6c75 6573 2074 6f20  e all values to 
+00017c20: 7468 6174 2061 7420 696e 6974 6961 6c69  that at initiali
+00017c30: 7a61 7469 6f6e 2069 6e20 6060 6f72 695f  zation in ``ori_
+00017c40: 6469 6374 6060 2e0d 0a20 2020 2020 2020  dict``...       
+00017c50: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
+00017c60: 6c66 2e6c 616e 6775 6167 6520 3d20 7365  lf.language = se
+00017c70: 6c66 2e6f 7269 5f64 6963 742e 6765 7428  lf.ori_dict.get(
+00017c80: 276c 616e 6775 6167 6527 290d 0a20 2020  'language')..   
+00017c90: 2020 2020 2073 656c 662e 5f72 6567 726f       self._regro
+00017ca0: 7570 5f68 6973 746f 7279 203d 2027 270d  up_history = ''.
+00017cb0: 0a20 2020 2020 2020 2073 6567 6d65 6e74  .        segment
+00017cc0: 7320 3d20 7365 6c66 2e6f 7269 5f64 6963  s = self.ori_dic
+00017cd0: 742e 6765 7428 2773 6567 6d65 6e74 7327  t.get('segments'
+00017ce0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00017cf0: 7365 676d 656e 7473 203d 205b 5365 676d  segments = [Segm
+00017d00: 656e 7428 2a2a 732c 2069 676e 6f72 655f  ent(**s, ignore_
+00017d10: 756e 7573 6564 5f61 7267 733d 5472 7565  unused_args=True
+00017d20: 2920 666f 7220 7320 696e 2073 6567 6d65  ) for s in segme
+00017d30: 6e74 735d 2069 6620 7365 676d 656e 7473  nts] if segments
+00017d40: 2065 6c73 6520 5b5d 0d0a 2020 2020 2020   else []..      
+00017d50: 2020 6966 2073 656c 662e 5f66 6f72 6365    if self._force
+00017d60: 645f 6f72 6465 723a 0d0a 2020 2020 2020  d_order:..      
+00017d70: 2020 2020 2020 7365 6c66 2e66 6f72 6365        self.force
+00017d80: 5f6f 7264 6572 2829 0d0a 2020 2020 2020  _order()..      
+00017d90: 2020 7365 6c66 2e72 656d 6f76 655f 6e6f    self.remove_no
+00017da0: 5f77 6f72 645f 7365 676d 656e 7473 2861  _word_segments(a
+00017db0: 6e79 2873 6567 2e68 6173 5f77 6f72 6473  ny(seg.has_words
+00017dc0: 2066 6f72 2073 6567 2069 6e20 7365 6c66   for seg in self
+00017dd0: 2e73 6567 6d65 6e74 7329 290d 0a0d 0a20  .segments)).... 
+00017de0: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
+00017df0: 2020 6465 6620 6861 735f 776f 7264 7328    def has_words(
+00017e00: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00017e10: 7265 7475 726e 2062 6f6f 6c28 7365 6c66  return bool(self
+00017e20: 2e73 6567 6d65 6e74 7329 2061 6e64 2061  .segments) and a
+00017e30: 6c6c 2873 6567 2e68 6173 5f77 6f72 6473  ll(seg.has_words
+00017e40: 2066 6f72 2073 6567 2069 6e20 7365 6c66   for seg in self
+00017e50: 2e73 6567 6d65 6e74 7329 0d0a 0d0a 2020  .segments)....  
+00017e60: 2020 746f 5f73 7274 5f76 7474 203d 2072    to_srt_vtt = r
+00017e70: 6573 756c 745f 746f 5f73 7274 5f76 7474  esult_to_srt_vtt
+00017e80: 0d0a 2020 2020 746f 5f61 7373 203d 2072  ..    to_ass = r
+00017e90: 6573 756c 745f 746f 5f61 7373 0d0a 2020  esult_to_ass..  
+00017ea0: 2020 746f 5f74 7376 203d 2072 6573 756c    to_tsv = resul
+00017eb0: 745f 746f 5f74 7376 0d0a 2020 2020 746f  t_to_tsv..    to
+00017ec0: 5f74 7874 203d 2072 6573 756c 745f 746f  _txt = result_to
+00017ed0: 5f74 7874 0d0a 2020 2020 7361 7665 5f61  _txt..    save_a
+00017ee0: 735f 6a73 6f6e 203d 2073 6176 655f 6173  s_json = save_as
+00017ef0: 5f6a 736f 6e0d 0a0d 0a0d 0a63 6c61 7373  _json......class
+00017f00: 2053 6567 6d65 6e74 4d61 7463 683a 0d0a   SegmentMatch:..
+00017f10: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00017f20: 5f5f 280d 0a20 2020 2020 2020 2020 2020  __(..           
+00017f30: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
+00017f40: 2020 2020 7365 676d 656e 7473 3a20 556e      segments: Un
+00017f50: 696f 6e5b 4c69 7374 5b53 6567 6d65 6e74  ion[List[Segment
+00017f60: 5d2c 2053 6567 6d65 6e74 5d2c 0d0a 2020  ], Segment],..  
+00017f70: 2020 2020 2020 2020 2020 5f77 6f72 645f            _word_
+00017f80: 696e 6469 6365 733a 204c 6973 745b 4c69  indices: List[Li
+00017f90: 7374 5b69 6e74 5d5d 203d 204e 6f6e 652c  st[int]] = None,
+00017fa0: 0d0a 2020 2020 2020 2020 2020 2020 5f74  ..            _t
+00017fb0: 6578 745f 6d61 7463 683a 2073 7472 203d  ext_match: str =
+00017fc0: 204e 6f6e 650d 0a20 2020 2029 3a0d 0a20   None..    ):.. 
+00017fd0: 2020 2020 2020 2073 656c 662e 7365 676d         self.segm
+00017fe0: 656e 7473 203d 205b 7365 676d 656e 7473  ents = [segments
+00017ff0: 5d20 6966 2069 7369 6e73 7461 6e63 6528  ] if isinstance(
+00018000: 7365 676d 656e 7473 2c20 5365 676d 656e  segments, Segmen
+00018010: 7429 2065 6c73 6520 7365 676d 656e 7473  t) else segments
+00018020: 0d0a 2020 2020 2020 2020 7365 6c66 2e77  ..        self.w
+00018030: 6f72 645f 696e 6469 6365 7320 3d20 5b5d  ord_indices = []
+00018040: 2069 6620 5f77 6f72 645f 696e 6469 6365   if _word_indice
+00018050: 7320 6973 204e 6f6e 6520 656c 7365 205f  s is None else _
+00018060: 776f 7264 5f69 6e64 6963 6573 0d0a 2020  word_indices..  
+00018070: 2020 2020 2020 7365 6c66 2e77 6f72 6473        self.words
+00018080: 203d 205b 7365 6c66 2e73 6567 6d65 6e74   = [self.segment
+00018090: 735b 695d 2e77 6f72 6473 5b6a 5d20 666f  s[i].words[j] fo
+000180a0: 7220 692c 2069 6e64 6963 6573 2069 6e20  r i, indices in 
+000180b0: 656e 756d 6572 6174 6528 7365 6c66 2e77  enumerate(self.w
+000180c0: 6f72 645f 696e 6469 6365 7329 2066 6f72  ord_indices) for
+000180d0: 206a 2069 6e20 696e 6469 6365 735d 0d0a   j in indices]..
+000180e0: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
+000180f0: 656c 662e 776f 7264 7329 2021 3d20 303a  elf.words) != 0:
+00018100: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00018110: 6c66 2e74 6578 7420 3d20 2727 2e6a 6f69  lf.text = ''.joi
+00018120: 6e28 0d0a 2020 2020 2020 2020 2020 2020  n(..            
+00018130: 2020 2020 7365 6c66 2e73 6567 6d65 6e74      self.segment
+00018140: 735b 695d 2e77 6f72 6473 5b6a 5d2e 776f  s[i].words[j].wo
+00018150: 7264 0d0a 2020 2020 2020 2020 2020 2020  rd..            
+00018160: 2020 2020 666f 7220 692c 2069 6e64 6963      for i, indic
+00018170: 6573 2069 6e20 656e 756d 6572 6174 6528  es in enumerate(
+00018180: 7365 6c66 2e77 6f72 645f 696e 6469 6365  self.word_indice
+00018190: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+000181a0: 2020 2020 666f 7220 6a20 696e 2069 6e64      for j in ind
+000181b0: 6963 6573 0d0a 2020 2020 2020 2020 2020  ices..          
+000181c0: 2020 290d 0a20 2020 2020 2020 2065 6c73    )..        els
+000181d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000181e0: 7365 6c66 2e74 6578 7420 3d20 2727 2e6a  self.text = ''.j
+000181f0: 6f69 6e28 7365 672e 7465 7874 2066 6f72  oin(seg.text for
+00018200: 2073 6567 2069 6e20 7365 6c66 2e73 6567   seg in self.seg
+00018210: 6d65 6e74 7329 0d0a 2020 2020 2020 2020  ments)..        
+00018220: 7365 6c66 2e74 6578 745f 6d61 7463 6820  self.text_match 
+00018230: 3d20 5f74 6578 745f 6d61 7463 680d 0a0d  = _text_match...
+00018240: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
+00018250: 2020 2020 6465 6620 7374 6172 7428 7365      def start(se
+00018260: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
+00018270: 7475 726e 2028 0d0a 2020 2020 2020 2020  turn (..        
+00018280: 2020 2020 7365 6c66 2e77 6f72 6473 5b30      self.words[0
+00018290: 5d2e 7374 6172 740d 0a20 2020 2020 2020  ].start..       
+000182a0: 2020 2020 2069 6620 6c65 6e28 7365 6c66       if len(self
+000182b0: 2e77 6f72 6473 2920 213d 2030 2065 6c73  .words) != 0 els
+000182c0: 650d 0a20 2020 2020 2020 2020 2020 2028  e..            (
+000182d0: 7365 6c66 2e73 6567 6d65 6e74 735b 305d  self.segments[0]
+000182e0: 2e73 7461 7274 2069 6620 6c65 6e28 7365  .start if len(se
+000182f0: 6c66 2e73 6567 6d65 6e74 7329 2021 3d20  lf.segments) != 
+00018300: 3020 656c 7365 204e 6f6e 6529 0d0a 2020  0 else None)..  
+00018310: 2020 2020 2020 290d 0a0d 0a20 2020 2040        )....    @
+00018320: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
+00018330: 6620 656e 6428 7365 6c66 293a 0d0a 2020  f end(self):..  
+00018340: 2020 2020 2020 7265 7475 726e 2028 0d0a        return (..
+00018350: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018360: 2e77 6f72 6473 5b2d 315d 2e65 6e64 0d0a  .words[-1].end..
+00018370: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00018380: 656e 2873 656c 662e 776f 7264 7329 2021  en(self.words) !
+00018390: 3d20 3020 656c 7365 0d0a 2020 2020 2020  = 0 else..      
+000183a0: 2020 2020 2020 2873 656c 662e 7365 676d        (self.segm
+000183b0: 656e 7473 5b2d 315d 2e65 6e64 2069 6620  ents[-1].end if 
+000183c0: 6c65 6e28 7365 6c66 2e73 6567 6d65 6e74  len(self.segment
+000183d0: 7329 2021 3d20 3020 656c 7365 204e 6f6e  s) != 0 else Non
+000183e0: 6529 0d0a 2020 2020 2020 2020 290d 0a0d  e)..        )...
+000183f0: 0a20 2020 2064 6566 205f 5f6c 656e 5f5f  .    def __len__
+00018400: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00018410: 2072 6574 7572 6e20 6c65 6e28 7365 6c66   return len(self
+00018420: 2e73 6567 6d65 6e74 7329 0d0a 0d0a 2020  .segments)....  
+00018430: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
+00018440: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
+00018450: 6574 7572 6e20 7365 6c66 2e5f 5f64 6963  eturn self.__dic
+00018460: 745f 5f2e 5f5f 7265 7072 5f5f 2829 0d0a  t__.__repr__()..
+00018470: 0d0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
+00018480: 5f28 7365 6c66 293a 0d0a 2020 2020 2020  _(self):..      
+00018490: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
+000184a0: 6469 6374 5f5f 2e5f 5f73 7472 5f5f 2829  dict__.__str__()
+000184b0: 0d0a 0d0a 0d0a 636c 6173 7320 5768 6973  ......class Whis
+000184c0: 7065 7252 6573 756c 744d 6174 6368 6573  perResultMatches
+000184d0: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
+000184e0: 5265 6745 7820 6d61 7463 6865 7320 666f  RegEx matches fo
+000184f0: 7220 5768 6973 7065 7252 6573 756c 7473  r WhisperResults
+00018500: 2e0d 0a20 2020 2022 2222 0d0a 2020 2020  ...    """..    
+00018510: 2320 5573 6520 5768 6973 7065 7252 6573  # Use WhisperRes
+00018520: 756c 742e 6669 6e64 2829 2069 6e73 7465  ult.find() inste
+00018530: 6164 206f 6620 696e 7374 616e 7469 6174  ad of instantiat
+00018540: 696e 6720 7468 6973 2063 6c61 7373 2064  ing this class d
+00018550: 6972 6563 746c 792e 0d0a 2020 2020 6465  irectly...    de
+00018560: 6620 5f5f 696e 6974 5f5f 280d 0a20 2020  f __init__(..   
+00018570: 2020 2020 2020 2020 2073 656c 662c 0d0a           self,..
+00018580: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
+00018590: 6865 733a 2055 6e69 6f6e 5b4c 6973 745b  hes: Union[List[
+000185a0: 5365 676d 656e 744d 6174 6368 5d2c 2057  SegmentMatch], W
+000185b0: 6869 7370 6572 5265 7375 6c74 5d2c 0d0a  hisperResult],..
+000185c0: 2020 2020 2020 2020 2020 2020 5f73 6567              _seg
+000185d0: 6d65 6e74 5f69 6e64 6963 6573 3a20 4c69  ment_indices: Li
+000185e0: 7374 5b4c 6973 745b 696e 745d 5d20 3d20  st[List[int]] = 
+000185f0: 4e6f 6e65 0d0a 2020 2020 293a 0d0a 2020  None..    ):..  
+00018600: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00018610: 6e63 6528 6d61 7463 6865 732c 2057 6869  nce(matches, Whi
+00018620: 7370 6572 5265 7375 6c74 293a 0d0a 2020  sperResult):..  
+00018630: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00018640: 6174 6368 6573 203d 206c 6973 7428 6d61  atches = list(ma
+00018650: 7028 5365 676d 656e 744d 6174 6368 2c20  p(SegmentMatch, 
+00018660: 6d61 7463 6865 732e 7365 676d 656e 7473  matches.segments
+00018670: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018680: 7365 6c66 2e5f 7365 676d 656e 745f 696e  self._segment_in
+00018690: 6469 6365 7320 3d20 5b5b 695d 2066 6f72  dices = [[i] for
+000186a0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+000186b0: 6d61 7463 6865 732e 7365 676d 656e 7473  matches.segments
+000186c0: 2929 5d0d 0a20 2020 2020 2020 2065 6c73  ))]..        els
+000186d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000186e0: 7365 6c66 2e6d 6174 6368 6573 203d 206d  self.matches = m
+000186f0: 6174 6368 6573 0d0a 2020 2020 2020 2020  atches..        
+00018700: 2020 2020 6173 7365 7274 205f 7365 676d      assert _segm
+00018710: 656e 745f 696e 6469 6365 7320 6973 206e  ent_indices is n
+00018720: 6f74 204e 6f6e 650d 0a20 2020 2020 2020  ot None..       
+00018730: 2020 2020 2061 7373 6572 7420 6c65 6e28       assert len(
+00018740: 7365 6c66 2e6d 6174 6368 6573 2920 3d3d  self.matches) ==
+00018750: 206c 656e 285f 7365 676d 656e 745f 696e   len(_segment_in
+00018760: 6469 6365 7329 0d0a 2020 2020 2020 2020  dices)..        
+00018770: 2020 2020 6173 7365 7274 2061 6c6c 286c      assert all(l
+00018780: 656e 286d 6174 6368 2e73 6567 6d65 6e74  en(match.segment
+00018790: 7329 203d 3d20 6c65 6e28 5f73 6567 6d65  s) == len(_segme
+000187a0: 6e74 5f69 6e64 6963 6573 5b69 5d29 2066  nt_indices[i]) f
+000187b0: 6f72 2069 2c20 6d61 7463 6820 696e 2065  or i, match in e
+000187c0: 6e75 6d65 7261 7465 2873 656c 662e 6d61  numerate(self.ma
+000187d0: 7463 6865 7329 290d 0a20 2020 2020 2020  tches))..       
+000187e0: 2020 2020 2073 656c 662e 5f73 6567 6d65       self._segme
+000187f0: 6e74 5f69 6e64 6963 6573 203d 205f 7365  nt_indices = _se
+00018800: 676d 656e 745f 696e 6469 6365 730d 0a0d  gment_indices...
+00018810: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
+00018820: 2020 2020 6465 6620 7365 676d 656e 745f      def segment_
+00018830: 696e 6469 6365 7328 7365 6c66 293a 0d0a  indices(self):..
+00018840: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00018850: 656c 662e 5f73 6567 6d65 6e74 5f69 6e64  elf._segment_ind
+00018860: 6963 6573 0d0a 0d0a 2020 2020 6465 6620  ices....    def 
+00018870: 5f63 7572 725f 7365 675f 6772 6f75 7073  _curr_seg_groups
+00018880: 2873 656c 6629 202d 3e20 4c69 7374 5b4c  (self) -> List[L
+00018890: 6973 745b 5475 706c 655b 696e 742c 2053  ist[Tuple[int, S
+000188a0: 6567 6d65 6e74 5d5d 5d3a 0d0a 2020 2020  egment]]]:..    
+000188b0: 2020 2020 7365 675f 6772 6f75 7073 2c20      seg_groups, 
+000188c0: 6375 7272 5f73 6567 7320 3d20 5b5d 2c20  curr_segs = [], 
+000188d0: 5b5d 0d0a 2020 2020 2020 2020 6375 7272  []..        curr
+000188e0: 5f6d 6178 203d 202d 310d 0a20 2020 2020  _max = -1..     
+000188f0: 2020 2066 6f72 2073 6567 5f69 6e64 6963     for seg_indic
+00018900: 6573 2c20 6d61 7463 6820 696e 207a 6970  es, match in zip
+00018910: 2873 656c 662e 5f73 6567 6d65 6e74 5f69  (self._segment_i
+00018920: 6e64 6963 6573 2c20 7365 6c66 2e6d 6174  ndices, self.mat
+00018930: 6368 6573 293a 0d0a 2020 2020 2020 2020  ches):..        
+00018940: 2020 2020 666f 7220 692c 2073 6567 2069      for i, seg i
+00018950: 6e20 7a69 7028 736f 7274 6564 2873 6567  n zip(sorted(seg
+00018960: 5f69 6e64 6963 6573 292c 206d 6174 6368  _indices), match
+00018970: 2e73 6567 6d65 6e74 7329 3a0d 0a20 2020  .segments):..   
+00018980: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00018990: 6920 3e20 6375 7272 5f6d 6178 3a0d 0a20  i > curr_max:.. 
+000189a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189b0: 2020 2063 7572 725f 7365 6773 2e61 7070     curr_segs.app
+000189c0: 656e 6428 2869 2c20 7365 6729 290d 0a20  end((i, seg)).. 
+000189d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189e0: 2020 2069 6620 6920 2d20 3120 213d 2063     if i - 1 != c
+000189f0: 7572 725f 6d61 783a 0d0a 2020 2020 2020  urr_max:..      
+00018a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a10: 2020 7365 675f 6772 6f75 7073 2e61 7070    seg_groups.app
+00018a20: 656e 6428 6375 7272 5f73 6567 7329 0d0a  end(curr_segs)..
+00018a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a40: 2020 2020 2020 2020 6375 7272 5f73 6567          curr_seg
+00018a50: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00018a60: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00018a70: 5f6d 6178 203d 2069 0d0a 0d0a 2020 2020  _max = i....    
+00018a80: 2020 2020 6966 2063 7572 725f 7365 6773      if curr_segs
+00018a90: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00018aa0: 6567 5f67 726f 7570 732e 6170 7065 6e64  eg_groups.append
+00018ab0: 2863 7572 725f 7365 6773 290d 0a20 2020  (curr_segs)..   
+00018ac0: 2020 2020 2072 6574 7572 6e20 7365 675f       return seg_
+00018ad0: 6772 6f75 7073 0d0a 0d0a 2020 2020 6465  groups....    de
+00018ae0: 6620 6669 6e64 2873 656c 662c 2070 6174  f find(self, pat
+00018af0: 7465 726e 3a20 7374 722c 2077 6f72 645f  tern: str, word_
+00018b00: 6c65 7665 6c3d 5472 7565 2c20 666c 6167  level=True, flag
+00018b10: 733d 4e6f 6e65 2920 2d3e 2022 5768 6973  s=None) -> "Whis
+00018b20: 7065 7252 6573 756c 744d 6174 6368 6573  perResultMatches
+00018b30: 223a 0d0a 2020 2020 2020 2020 2222 220d  ":..        """.
+00018b40: 0a20 2020 2020 2020 2046 696e 6420 7365  .        Find se
+00018b50: 676d 656e 7473 2f77 6f72 6473 2061 6e64  gments/words and
+00018b60: 2074 696d 6573 7461 6d70 7320 7769 7468   timestamps with
+00018b70: 2072 6567 756c 6172 2065 7870 7265 7373   regular express
+00018b80: 696f 6e2e 0d0a 0d0a 2020 2020 2020 2020  ion.....        
+00018b90: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+00018ba0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+00018bb0: 2020 2020 2020 2020 7061 7474 6572 6e20          pattern 
+00018bc0: 3a20 7374 720d 0a20 2020 2020 2020 2020  : str..         
+00018bd0: 2020 2052 6567 4578 2070 6174 7465 726e     RegEx pattern
+00018be0: 2074 6f20 7365 6172 6368 2066 6f72 2e0d   to search for..
+00018bf0: 0a20 2020 2020 2020 2077 6f72 645f 6c65  .        word_le
+00018c00: 7665 6c20 3a20 626f 6f6c 2c20 6465 6661  vel : bool, defa
+00018c10: 756c 7420 5472 7565 0d0a 2020 2020 2020  ult True..      
+00018c20: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+00018c30: 2073 6561 7263 6820 6174 2077 6f72 642d   search at word-
+00018c40: 6c65 7665 6c2e 0d0a 2020 2020 2020 2020  level...        
+00018c50: 666c 6167 7320 3a20 6f70 7469 6f6e 616c  flags : optional
+00018c60: 0d0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
+00018c70: 6745 7820 666c 6167 732e 0d0a 0d0a 2020  gEx flags.....  
+00018c80: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
+00018c90: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
+00018ca0: 2020 2020 2020 2020 7374 6162 6c65 5f77          stable_w
+00018cb0: 6869 7370 6572 2e72 6573 756c 742e 5768  hisper.result.Wh
+00018cc0: 6973 7065 7252 6573 756c 744d 6174 6368  isperResultMatch
+00018cd0: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
+00018ce0: 416e 2069 6e73 7461 6e63 6520 6f66 203a  An instance of :
+00018cf0: 636c 6173 733a 6073 7461 626c 655f 7768  class:`stable_wh
+00018d00: 6973 7065 722e 7265 7375 6c74 2e57 6869  isper.result.Whi
+00018d10: 7370 6572 5265 7375 6c74 4d61 7463 6865  sperResultMatche
+00018d20: 7360 2077 6974 6820 776f 7264 2f73 6567  s` with word/seg
+00018d30: 6d65 6e74 2074 6861 7420 6d61 7463 6820  ment that match 
+00018d40: 6060 7061 7474 6572 6e60 602e 0d0a 2020  ``pattern``...  
+00018d50: 2020 2020 2020 2222 220d 0a0d 0a20 2020        """....   
+00018d60: 2020 2020 2073 6567 5f67 726f 7570 7320       seg_groups 
+00018d70: 3d20 7365 6c66 2e5f 6375 7272 5f73 6567  = self._curr_seg
+00018d80: 5f67 726f 7570 7328 290d 0a20 2020 2020  _groups()..     
+00018d90: 2020 206d 6174 6368 6573 3a20 4c69 7374     matches: List
+00018da0: 5b53 6567 6d65 6e74 4d61 7463 685d 203d  [SegmentMatch] =
+00018db0: 205b 5d0d 0a20 2020 2020 2020 206d 6174   []..        mat
+00018dc0: 6368 5f73 6567 5f69 6e64 6963 6573 3a20  ch_seg_indices: 
+00018dd0: 4c69 7374 5b4c 6973 745b 696e 745d 5d20  List[List[int]] 
+00018de0: 3d20 5b5d 0d0a 2020 2020 2020 2020 6966  = []..        if
+00018df0: 2077 6f72 645f 6c65 7665 6c3a 0d0a 2020   word_level:..  
+00018e00: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00018e10: 2061 6c6c 2861 6c6c 2873 6567 2e68 6173   all(all(seg.has
+00018e20: 5f77 6f72 6473 2066 6f72 2073 6567 2069  _words for seg i
+00018e30: 6e20 6d61 7463 682e 7365 676d 656e 7473  n match.segments
+00018e40: 2920 666f 7220 6d61 7463 6820 696e 2073  ) for match in s
+00018e50: 656c 662e 6d61 7463 6865 7329 3a0d 0a20  elf.matches):.. 
+00018e60: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00018e70: 6172 6e69 6e67 732e 7761 726e 2827 4361  arnings.warn('Ca
+00018e80: 6e6e 6f74 2070 6572 666f 726d 2077 6f72  nnot perform wor
+00018e90: 642d 6c65 7665 6c20 7365 6172 6368 2077  d-level search w
+00018ea0: 6974 6820 7365 676d 656e 7428 7329 206d  ith segment(s) m
+00018eb0: 6973 7369 6e67 2077 6f72 6420 7469 6d65  issing word time
+00018ec0: 7374 616d 7073 2e27 290d 0a20 2020 2020  stamps.')..     
+00018ed0: 2020 2020 2020 2020 2020 2077 6f72 645f             word_
+00018ee0: 6c65 7665 6c20 3d20 4661 6c73 650d 0a0d  level = False...
+00018ef0: 0a20 2020 2020 2020 2066 6f72 2073 6567  .        for seg
+00018f00: 7320 696e 2073 6567 5f67 726f 7570 733a  s in seg_groups:
+00018f10: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00018f20: 2077 6f72 645f 6c65 7665 6c3a 0d0a 2020   word_level:..  
+00018f30: 2020 2020 2020 2020 2020 2020 2020 6964                id
+00018f40: 7873 203d 206c 6973 7428 6368 6169 6e2e  xs = list(chain.
+00018f50: 6672 6f6d 5f69 7465 7261 626c 6528 0d0a  from_iterable(..
+00018f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f70: 2020 2020 5b28 692c 206a 295d 2a6c 656e      [(i, j)]*len
+00018f80: 2877 6f72 642e 776f 7264 2920 666f 7220  (word.word) for 
+00018f90: 2869 2c20 7365 6729 2069 6e20 7365 6773  (i, seg) in segs
+00018fa0: 2066 6f72 206a 2c20 776f 7264 2069 6e20   for j, word in 
+00018fb0: 656e 756d 6572 6174 6528 7365 672e 776f  enumerate(seg.wo
+00018fc0: 7264 7329 0d0a 2020 2020 2020 2020 2020  rds)..          
+00018fd0: 2020 2020 2020 2929 0d0a 2020 2020 2020        ))..      
+00018fe0: 2020 2020 2020 2020 2020 7465 7874 203d            text =
+00018ff0: 2027 272e 6a6f 696e 2877 6f72 642e 776f   ''.join(word.wo
+00019000: 7264 2066 6f72 2028 5f2c 2073 6567 2920  rd for (_, seg) 
+00019010: 696e 2073 6567 7320 666f 7220 776f 7264  in segs for word
+00019020: 2069 6e20 7365 672e 776f 7264 7329 0d0a   in seg.words)..
+00019030: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00019040: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00019050: 2020 2069 6478 7320 3d20 6c69 7374 2863     idxs = list(c
+00019060: 6861 696e 2e66 726f 6d5f 6974 6572 6162  hain.from_iterab
+00019070: 6c65 285b 2869 2c20 4e6f 6e65 295d 2a6c  le([(i, None)]*l
+00019080: 656e 2873 6567 2e74 6578 7429 2066 6f72  en(seg.text) for
+00019090: 2028 692c 2073 6567 2920 696e 2073 6567   (i, seg) in seg
+000190a0: 7329 290d 0a20 2020 2020 2020 2020 2020  s))..           
+000190b0: 2020 2020 2074 6578 7420 3d20 2727 2e6a       text = ''.j
+000190c0: 6f69 6e28 7365 672e 7465 7874 2066 6f72  oin(seg.text for
+000190d0: 2028 5f2c 2073 6567 2920 696e 2073 6567   (_, seg) in seg
+000190e0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+000190f0: 6173 7365 7274 206c 656e 2869 6478 7329  assert len(idxs)
+00019100: 203d 3d20 6c65 6e28 7465 7874 290d 0a20   == len(text).. 
+00019110: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
+00019120: 7572 725f 6d61 7463 6820 696e 2072 652e  urr_match in re.
+00019130: 6669 6e64 6974 6572 2870 6174 7465 726e  finditer(pattern
+00019140: 2c20 7465 7874 2c20 666c 6167 733d 666c  , text, flags=fl
+00019150: 6167 7320 6f72 2030 293a 0d0a 2020 2020  ags or 0):..    
+00019160: 2020 2020 2020 2020 2020 2020 7374 6172              star
+00019170: 742c 2065 6e64 203d 2063 7572 725f 6d61  t, end = curr_ma
+00019180: 7463 682e 7370 616e 2829 0d0a 2020 2020  tch.span()..    
+00019190: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+000191a0: 5f69 6478 7320 3d20 6964 7873 5b73 7461  _idxs = idxs[sta
+000191b0: 7274 3a20 656e 645d 0d0a 2020 2020 2020  rt: end]..      
+000191c0: 2020 2020 2020 2020 2020 6375 7272 5f73            curr_s
+000191d0: 6567 5f69 6478 7320 3d20 736f 7274 6564  eg_idxs = sorted
+000191e0: 2873 6574 2869 5b30 5d20 666f 7220 6920  (set(i[0] for i 
+000191f0: 696e 2063 7572 725f 6964 7873 2929 0d0a  in curr_idxs))..
+00019200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019210: 6966 2077 6f72 645f 6c65 7665 6c3a 0d0a  if word_level:..
+00019220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019230: 2020 2020 6375 7272 5f77 6f72 645f 6964      curr_word_id
+00019240: 7873 203d 205b 0d0a 2020 2020 2020 2020  xs = [..        
+00019250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019260: 736f 7274 6564 2873 6574 286a 2066 6f72  sorted(set(j for
+00019270: 2069 2c20 6a20 696e 2063 7572 725f 6964   i, j in curr_id
+00019280: 7873 2069 6620 6920 3d3d 2073 6567 5f69  xs if i == seg_i
+00019290: 6478 2929 0d0a 2020 2020 2020 2020 2020  dx))..          
+000192a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000192b0: 7220 7365 675f 6964 7820 696e 2063 7572  r seg_idx in cur
+000192c0: 725f 7365 675f 6964 7873 0d0a 2020 2020  r_seg_idxs..    
+000192d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000192f0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00019300: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00019310: 7272 5f77 6f72 645f 6964 7873 203d 204e  rr_word_idxs = N
+00019320: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
+00019330: 2020 2020 206d 6174 6368 6573 2e61 7070       matches.app
+00019340: 656e 6428 5365 676d 656e 744d 6174 6368  end(SegmentMatch
+00019350: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00019360: 2020 2020 2020 2073 6567 6d65 6e74 733d         segments=
+00019370: 5b73 2066 6f72 2069 2c20 7320 696e 2073  [s for i, s in s
+00019380: 6567 7320 6966 2069 2069 6e20 6375 7272  egs if i in curr
+00019390: 5f73 6567 5f69 6478 735d 2c0d 0a20 2020  _seg_idxs],..   
+000193a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193b0: 205f 776f 7264 5f69 6e64 6963 6573 3d63   _word_indices=c
+000193c0: 7572 725f 776f 7264 5f69 6478 732c 0d0a  urr_word_idxs,..
+000193d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193e0: 2020 2020 5f74 6578 745f 6d61 7463 683d      _text_match=
+000193f0: 6375 7272 5f6d 6174 6368 2e67 726f 7570  curr_match.group
+00019400: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00019410: 2020 2020 2929 0d0a 2020 2020 2020 2020      ))..        
+00019420: 2020 2020 2020 2020 6d61 7463 685f 7365          match_se
+00019430: 675f 696e 6469 6365 732e 6170 7065 6e64  g_indices.append
+00019440: 2863 7572 725f 7365 675f 6964 7873 290d  (curr_seg_idxs).
+00019450: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00019460: 5768 6973 7065 7252 6573 756c 744d 6174  WhisperResultMat
+00019470: 6368 6573 286d 6174 6368 6573 2c20 6d61  ches(matches, ma
+00019480: 7463 685f 7365 675f 696e 6469 6365 7329  tch_seg_indices)
+00019490: 0d0a 0d0a 2020 2020 6465 6620 5f5f 6c65  ....    def __le
+000194a0: 6e5f 5f28 7365 6c66 293a 0d0a 2020 2020  n__(self):..    
+000194b0: 2020 2020 7265 7475 726e 206c 656e 2873      return len(s
+000194c0: 656c 662e 6d61 7463 6865 7329 0d0a 0d0a  elf.matches)....
+000194d0: 2020 2020 6465 6620 5f5f 626f 6f6c 5f5f      def __bool__
+000194e0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+000194f0: 2072 6574 7572 6e20 7365 6c66 2e5f 5f6c   return self.__l
+00019500: 656e 5f5f 2829 2021 3d20 300d 0a0d 0a20  en__() != 0.... 
+00019510: 2020 2064 6566 205f 5f67 6574 6974 656d     def __getitem
+00019520: 5f5f 2873 656c 662c 2069 6478 293a 0d0a  __(self, idx):..
+00019530: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00019540: 656c 662e 6d61 7463 6865 735b 6964 785d  elf.matches[idx]
+00019550: 0d0a                                     ..
```

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/stabilization/__init__.py` & `stable-ts-whisperless-2.17.2/stable_whisper/stabilization/__init__.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/stabilization/nonvad.py` & `stable-ts-whisperless-2.17.2/stable_whisper/stabilization/nonvad.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/stabilization/silero_vad.py` & `stable-ts-whisperless-2.17.2/stable_whisper/stabilization/silero_vad.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/stabilization/utils.py` & `stable-ts-whisperless-2.17.2/stable_whisper/stabilization/utils.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/text_output.py` & `stable-ts-whisperless-2.17.2/stable_whisper/text_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
     elif word_level:
         segments = to_word_level(segments)
 
     if not valid_ts(segments, warn=False):
         warnings.warn(message='Result contains out of order timestamp(s). Output file may not playback properly.')
 
     if segments2blocks is None:
-        sub_str = '\n\n'.join(segment2srtblock(s, i, strip=strip) for i, s in enumerate(segments))
+        sub_str = '\n\n'.join(segment2srtblock(s, i, strip=strip) for i, s in enumerate(segments, 1))
     else:
         sub_str = segments2blocks(segments)
 
     if filepath:
         _save_as_file(sub_str, filepath)
     else:
         return sub_str
```

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/timing.py` & `stable-ts-whisperless-2.17.2/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/utils.py` & `stable-ts-whisperless-2.17.2/stable_whisper/utils.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/video_output.py` & `stable-ts-whisperless-2.17.2/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/whisper_compatibility.py` & `stable-ts-whisperless-2.17.2/stable_whisper/whisper_compatibility.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/cli.py` & `stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/cli.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/faster_whisper.py` & `stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/faster_whisper.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/hf_whisper.py` & `stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/hf_whisper.py`

 * *Files identical despite different names*

### Comparing `stable-ts-whisperless-2.17.1/stable_whisper/whisper_word_level/original_whisper.py` & `stable-ts-whisperless-2.17.2/stable_whisper/whisper_word_level/original_whisper.py`

 * *Files identical despite different names*

