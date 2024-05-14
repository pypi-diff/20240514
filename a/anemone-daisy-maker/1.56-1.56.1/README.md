# Comparing `tmp/anemone_daisy_maker-1.56.tar.gz` & `tmp/anemone_daisy_maker-1.56.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemone_daisy_maker-1.56.tar", last modified: Tue May 14 06:57:25 2024, max compression
+gzip compressed data, was "anemone_daisy_maker-1.56.1.tar", last modified: Tue May 14 07:14:18 2024, max compression
```

## Comparing `anemone_daisy_maker-1.56.tar` & `anemone_daisy_maker-1.56.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 06:57:25.385494 anemone_daisy_maker-1.56/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11357 2024-05-14 06:45:18.000000 anemone_daisy_maker-1.56/LICENSE
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6889 2024-05-14 06:57:25.385494 anemone_daisy_maker-1.56/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    10238 2024-05-14 06:45:20.000000 anemone_daisy_maker-1.56/README.md
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 06:57:25.385494 anemone_daisy_maker-1.56/anemone/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    75174 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       33 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone/__main__.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 06:57:25.385494 anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6889 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      326 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       54 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2024-05-14 06:57:25.385494 anemone_daisy_maker-1.56/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6987 2024-05-14 06:57:25.000000 anemone_daisy_maker-1.56/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 07:14:18.441958 anemone_daisy_maker-1.56.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11357 2024-05-14 07:13:31.000000 anemone_daisy_maker-1.56.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6892 2024-05-14 07:14:18.441958 anemone_daisy_maker-1.56.1/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 07:14:18.437958 anemone_daisy_maker-1.56.1/anemone/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    75174 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       33 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone/__main__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-14 07:14:18.437958 anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6892 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      316 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       54 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2024-05-14 07:14:18.441958 anemone_daisy_maker-1.56.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7094 2024-05-14 07:14:18.000000 anemone_daisy_maker-1.56.1/setup.py
```

### Comparing `anemone_daisy_maker-1.56/LICENSE` & `anemone_daisy_maker-1.56.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anemone_daisy_maker-1.56/PKG-INFO` & `anemone_daisy_maker-1.56.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: anemone_daisy_maker
-Version: 1.56
+Version: 1.56.1
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
 Home-page: UNKNOWN
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
-License: UNKNOWN
+License: Apache 2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `anemone_daisy_maker-1.56/README.md` & `anemone_daisy_maker-1.56.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,12 @@
-# indexer
-This repository contains various indexing utilities from http://ssb22.user.srcf.net/indexer/
-(also mirrored at http://ssb22.gitlab.io/indexer/ just in case)
-the main ones being:
-1. Offline HTML Indexer
-2. Online version of OHI
-3. LaTeX book and dictionary builder (print OHI)
-4. Anemone DAISY maker
-
-Offline HTML Indexer
---------------------
-
-This is a Python program (compatible with both Python 2 and Python 3), for creating large indices of HTML text which can be queried using simple Javascript that works on many mobile phone browsers without needing an Internet connection or a Web server. This is useful if you want to load a dictionary or other reference onto your phone (or computer) for use when connectivity is not available.
-
-The input HTML should be interspersed with anchors like this: `<a name="xyz"></a>` where xyz is the index heading for the following text. There should be one such anchor before each entry and an extra anchor at the end of the text; everything before the first anchor is counted as the “header” and everything after the last as the “footer”. If these are empty, a default “mobile friendly” HTML header and footer specifying UTF-8 encoding will be added. Anchors may be linked from other entries; these links are changed as necessary.
-
-By default, the input HTML is read from standard input, and the output is written to the current directory as a set of HTML files, each limited to 64 Kb so as not to overload a mobile browser. Opening any of these HTML files should display a textbox that lets you type the first few letters of the word you wish to look up; the browser will then jump to whatever heading is alphabetically nearest to the typed-in text. (By default, only alphabetical letters are significant and diacritical marks are stripped from the index, but this can be changed.)
-
-As an example, `c2h.py` is a simple CEDICT to HTML script can produce offline HTML files for CEDICT.
-
-Users of the Android platform might also wish to make an APK from the HTML. `ohi-addCopy.sh` is a shell script to add Copy buttons to any hanzi strings to the HTML files, which should work when it’s put into an APK using [html2apk](http://ssb22.user.srcf.net/indexer/html2apk.html) (but they won’t work in standalone HTML).
-
-Online version
---------------
-
-Although the offline files will also work online, in bandwidth-limited situations you might be better using the `ohi_online.py` lookup CGI which works from the same input as ohi.py (see start of file for configuration, and there are options for running it as a [Web Adjuster](http://ssb22.user.srcf.net/adjuster/) extension if desired). This version can also take multiple adjacent anchors, giving alternate labels to the same fragment; there should not be any whitespace between adjacent anchors.
-
-Print version
--------------
-The script `ohi_latex.py` works from the same input as `ohi.py` and can be used to help make a printed reference. It includes a simple HTML to LaTeX converter with support for CJK (including Pinyin), Greek, Braille, IPA, Latin diacritics, miscellaneous symbols etc, and PDF features such as cross-referencing should work. Line breaks are automatically added between entries, unless their anchor names end with `*` in which case they are separated by semicolons for saving paper when adding large numbers of short “see” entries. If the input has no anchors then `ohi_latex` will just convert simple HTML/Unicode into LaTeX.
-
-Anemone DAISY maker
--------------------
+from setuptools import setup, find_packages;setup(name='anemone_daisy_maker',version='1.56.1',entry_points={'console_scripts':['anemone=anemone.__init__:anemone']},license='Apache 2',platform='cross-platform',home_page='http://ssb22.user.srcf.net/indexer/anemone.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data',long_description='''Anemone DAISY maker
+-----------------
 from http://ssb22.user.srcf.net/indexer/anemone.html
-(also mirrored at http://ssb22.gitlab.io/indexer/anemone.html just in case, plus you can access Anemone via `pip install anemone-daisy-maker` or `pipx run anemone-daisy-maker`)
 
-`anemone.py` is a Python 3 script to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce one of two different types of digital talking book:
+`anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce one of two different types of digital talking book:
 
 1. Full audio with basic Navigation Control Centre only: this requires a list of MP3 or WAV files for the audio, one per section, and the title of each section can be placed either in a separate text file or in the filename of the audio file.
 
 2. Full audio with full text: this requires MP3 or WAV files for the audio, corresponding XHTML files for the text, and corresponding JSON files for the timing synchronisation.  Each JSON file is expected to contain a list called `"markers"` whose items contain `"id"` (or `"paragraphId"` or anything else ending id) and `"time"` (or `"startTime"` or anything else ending time), which can be in seconds, minutes:seconds or hours:minutes:seconds (fractions of a second are allowed in each case).  The IDs in these JSON files should have corresponding attributes in the XHTML, by default data-pid but this can be changed with an option.
 
 All files are placed on the command line (or in parameters if you're using Anemone as a module), and Anemone assumes the correspondences are ordered.  So for example if MP3, HTML and JSON files are given, Anemone assumes the first-listed MP3 file corresponds with the first-listed HTML file and the first-listed JSON file, and so on for the second, third, etc.  With most sensible file naming schemes, you should be able to use shell wildcards like `*` when passing the files to Anemone.  You may also set the name of an output file ending `zip`; the suffix `_daisy.zip` is common.  The title, publisher, language etc of the book should be set via options: run the program with `--help` to see all.
 
@@ -48,45 +16,39 @@
 
 * Dolphin EasyReader 10 (iOS, Android and Chromebook): is able to open the ZIP and play the audio while highlighting the paragraphs in a ‘full audio plus full text’ book, both Daisy 2 and Daisy 3.  In very large books (over 1&nbsp;GB), loading and navigation becomes unreliable.
 
 * EDRLab Thorium Reader (Windows, Mac and GNU/Linux): is able to open the ZIP and play the audio while highlighting the paragraphs in a ‘full audio plus full text’ book, both Daisy 2 and Daisy 3.  Still works in very large books but loading is slow.
 
 * Dolphin EasyReader 10 (Windows): is able to play audio while highlighting paragraphs in both Daisy 2 and Daisy 3, but ZIP needs to be unpacked separately and NCC or OPF file opened.  Very large (1 GB+) books can cause the program to crash when Search is used.
 
-* JAWS FSReader 3 (Windows): is able to play audio while highlighting paragraphs in both Daisy 2 and Daisy 3, but ZIP needs to be unpacked separately and NCC or OPF file opened; may work better without JAWS running; synchronisation with audio seems to require `--mp3-recode`; images are not scaled to fit; tested working with a Braille display and audio speed changes; not tested with very large books (1GB+)
+* JAWS FSReader 3 (Windows): is able to play audio while highlighting paragraphs in both Daisy 2 and Daisy 3, but ZIP needs to be unpacked separately and NCC or OPF file opened; may work better without JAWS running; synchronisation with audio seems to require `mp3_recode`; images are not scaled to fit; tested working with a Braille display and audio speed changes; not tested with very large books (1GB+)
 
 * HumanWare Brailliant: does not show text if there is audio (hopefully it can still be used for navigation) in both Daisy 2 and Daisy 3
 
 * Pronto Notetaker: ZIP needs to be unpacked to a “Daisy” folder on SD or USB, and the device just plays the audio; tested only with Daisy 2
 
-* US Library of Congress NLS Player: unpack the ZIP onto a blank USB stick of capacity 4 GB or less—plays; navigation works if you use `--mp3-recode`; tested only with Daisy 2 but the documentation says Daisy 3 should work
+* US Library of Congress NLS Player: unpack the ZIP onto a blank USB stick of capacity 4 GB or less—plays; navigation works if you use `mp3_recode`; tested only with Daisy 2 but the documentation says Daisy 3 should work
 
 * HumanWare Victor Reader Stream: ZIP needs to be unpacked, either to the top level of a USB device, or into a subfolder of a `$VRDTB` folder on the SD card (different books will be listed alphabetically).  If it's unpacked at the top level of the SD card, the device can still play the MP3s and allow track or time based navigation but not section navigation, so you should use either the folder structure of the SD card or else a USB device.  If correctly set up then audio plays and device can navigate by section.  Tested with both Daisy 2 and Daisy 3.
 
 * HumanWare Victor Reader Stratus4: When unpacking the ZIP to CD, please ensure that your CD writer does *not* create a *folder* with the same name as the ZIP: this default behaviour of Microsoft Windows does *not* result in a valid Daisy CD.  The individual *files* of the ZIP need to be written to the *top level* of the CD, *not* to a folder on it.  Otherwise, the Stratus4 will not recognise the CD as a Daisy CD and will just play the MP3s, resulting in only time and track based navigation being available.  Tested with both Daisy 2 and Daisy 3.
 
 * HIMS QBraille XL: can display the text (after opening with Space and Enter); does not play audio; tested only with Daisy 2
 
 * Daisy Consortium Simply Reading 3 (app available for Android 7 and below): is able to open the ZIP and play the audio while highlighting the paragraphs in a 'full audio plus full text' book, although fonts for some languages might be missing on earlier Android devices
 
-* DAISY Pipeline (2023): Please do not use this to convert an Anemone-produced Daisy 2 book to Daisy 3.  The resulting Daisy 3 is not likely to play on anything.  If Daisy 3 is required, use Anemone's `--daisy3` option to produce it directly.
+* DAISY Pipeline (2023): Please do not use this to convert an Anemone-produced Daisy 2 book to Daisy 3.  The resulting Daisy 3 is not likely to play on anything.  If Daisy 3 is required, use Anemone's `daisy3` option to produce it directly.
 
 Copyright and Trademarks
-------------------------
+----------------------
 
 © Silas S. Brown, licensed under Apache 2.
 
-* Android is a trademark of Google LLC.
-
 * Apache is a registered trademark of The Apache Software Foundation.
 
-* Javascript is a trademark of Oracle Corporation in the US.
-
 * MP3 is a trademark that was registered in Europe to Hypermedia GmbH Webcasting but I was unable to confirm its current holder.
 
 * Python is a trademark of the Python Software Foundation.
 
-* Unicode is a registered trademark of Unicode, Inc. in the United States and other countries.
-
 * Windows is a registered trademark of Microsoft Corp.
 
-* Any other trademarks I mentioned without realising are trademarks of their respective holders.
+* Any other trademarks I mentioned without realising are trademarks of their respective holders.''',long_description_content_type='text/markdown',packages=find_packages(),classifiers=['Programming Language :: Python :: 3','License :: OSI Approved :: Apache Software License','Operating System :: OS Independent'],python_requires='>=3.7',install_requires=['mutagen'])
```

### Comparing `anemone_daisy_maker-1.56/anemone/__init__.py` & `anemone_daisy_maker-1.56.1/anemone/__init__.py`

 * *Files identical despite different names*

### Comparing `anemone_daisy_maker-1.56/anemone_daisy_maker.egg-info/PKG-INFO` & `anemone_daisy_maker-1.56.1/anemone_daisy_maker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: anemone-daisy-maker
-Version: 1.56
+Version: 1.56.1
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
 Home-page: UNKNOWN
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
-License: UNKNOWN
+License: Apache 2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```
